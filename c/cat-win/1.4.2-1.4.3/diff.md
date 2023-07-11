# Comparing `tmp/cat_win-1.4.2.tar.gz` & `tmp/cat_win-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cat_win-1.4.2.tar", last modified: Thu May 11 09:26:07 2023, max compression
+gzip compressed data, was "cat_win-1.4.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cat_win-1.4.2.tar` & `cat_win-1.4.3.tar`

### file list

```diff
@@ -1,61 +1,64 @@
--rw-r--r--   0        0        0     1090 2023-02-19 10:54:41.226281 cat_win-1.4.2/LICENSE
--rw-r--r--   0        0        0    13860 2023-05-05 17:29:17.289986 cat_win-1.4.2/README.md
--rw-r--r--   0        0        0       39 2023-02-26 11:57:46.261532 cat_win-1.4.2/cat_win/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2023-02-26 11:57:46.261532 cat_win-1.4.2/cat_win/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2023-02-26 11:57:46.261532 cat_win-1.4.2/cat_win/.pytest_cache/README.md
--rw-r--r--   0        0        0     5653 2023-02-26 11:57:52.638849 cat_win-1.4.2/cat_win/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2023-02-26 11:57:52.639848 cat_win-1.4.2/cat_win/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      289 2023-05-11 09:25:47.008420 cat_win-1.4.2/cat_win/__init__.py
--rw-r--r--   0        0        0      363 2023-05-01 18:46:04.882782 cat_win-1.4.2/cat_win/__main__.py
--rw-r--r--   0        0        0    35374 2023-05-10 15:30:06.562028 cat_win-1.4.2/cat_win/cat.py
--rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.4.2/cat_win/const/__init__.py
--rw-r--r--   0        0        0     4717 2023-05-03 09:19:54.039073 cat_win-1.4.2/cat_win/const/argconstants.py
--rw-r--r--   0        0        0     2492 2023-05-01 16:13:49.121661 cat_win-1.4.2/cat_win/const/colorconstants.py
--rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.4.2/cat_win/persistence/__init__.py
--rw-r--r--   0        0        0     8208 2023-05-04 20:42:15.378650 cat_win-1.4.2/cat_win/persistence/config.py
--rw-r--r--   0        0        0      319 2023-05-01 18:46:08.801676 cat_win-1.4.2/cat_win/shell.py
--rw-r--r--   0        0        0        0 2023-02-19 10:54:41.304282 cat_win-1.4.2/cat_win/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 10:00:24.210446 cat_win-1.4.2/cat_win/tests/mocks/__init__.py
--rw-r--r--   0        0        0     1443 2023-05-04 13:28:17.759035 cat_win-1.4.2/cat_win/tests/mocks/std.py
--rw-r--r--   0        0        0     1170 2023-05-01 15:49:21.685058 cat_win-1.4.2/cat_win/tests/test_argconstants.py
--rw-r--r--   0        0        0     8294 2023-05-02 08:59:10.289918 cat_win-1.4.2/cat_win/tests/test_argparser.py
--rw-r--r--   0        0        0     7492 2023-05-07 10:04:21.634459 cat_win-1.4.2/cat_win/tests/test_cat.py
--rw-r--r--   0        0        0     1131 2023-05-02 19:37:40.487184 cat_win-1.4.2/cat_win/tests/test_cbase64.py
--rw-r--r--   0        0        0     1569 2023-05-02 19:37:45.944459 cat_win-1.4.2/cat_win/tests/test_checksum.py
--rw-r--r--   0        0        0     1533 2023-05-04 13:57:20.651422 cat_win-1.4.2/cat_win/tests/test_config.py
--rw-r--r--   0        0        0     3613 2023-05-02 19:37:53.765103 cat_win-1.4.2/cat_win/tests/test_converter.py
--rw-r--r--   0        0        0      823 2023-05-02 19:38:00.930937 cat_win-1.4.2/cat_win/tests/test_file.py
--rw-r--r--   0        0        0     2021 2023-05-01 15:57:01.266856 cat_win-1.4.2/cat_win/tests/test_fileattributes.py
--rw-r--r--   0        0        0     6164 2023-05-07 09:54:17.443534 cat_win-1.4.2/cat_win/tests/test_full.py
--rw-r--r--   0        0        0     6922 2023-05-08 12:29:13.706678 cat_win-1.4.2/cat_win/tests/test_holder.py
--rw-r--r--   0        0        0     7408 2023-05-01 16:03:35.076827 cat_win-1.4.2/cat_win/tests/test_rawviewer.py
--rw-r--r--   0        0        0     4190 2023-05-07 09:56:25.443429 cat_win-1.4.2/cat_win/tests/test_shell.py
--rw-r--r--   0        0        0     1254 2023-05-04 13:29:46.034492 cat_win-1.4.2/cat_win/tests/test_stdinhelper.py
--rw-r--r--   0        0        0     3117 2023-05-02 09:42:04.478371 cat_win-1.4.2/cat_win/tests/test_stringfinder.py
--rw-r--r--   0        0        0     3951 2023-05-02 19:38:32.100152 cat_win-1.4.2/cat_win/tests/test_updatechecker.py
--rw-r--r--   0        0        0      170 2023-02-19 10:54:41.307281 cat_win-1.4.2/cat_win/tests/texts/full_test_result_B.txt
--rw-r--r--   0        0        0      196 2023-02-19 10:54:41.307281 cat_win-1.4.2/cat_win/tests/texts/full_test_result_C.txt
--rw-r--r--   0        0        0      139 2023-02-19 10:54:41.308281 cat_win-1.4.2/cat_win/tests/texts/full_test_result_D.txt
--rw-r--r--   0        0        0      189 2023-02-19 10:54:41.308281 cat_win-1.4.2/cat_win/tests/texts/test.txt
--rw-r--r--   0        0        0        0 2023-03-26 11:37:07.806578 cat_win-1.4.2/cat_win/tests/texts/test_empty.txt
--rw-r--r--   0        0        0       19 2023-02-19 10:54:41.308281 cat_win-1.4.2/cat_win/tests/texts/test_holderEdgeCase_1.txt
--rw-r--r--   0        0        0       21 2023-02-19 10:54:41.308281 cat_win-1.4.2/cat_win/tests/texts/test_holderEdgeCase_2.txt
--rw-r--r--   0        0        0       28 2023-03-26 12:18:11.309629 cat_win-1.4.2/cat_win/tests/texts/test_holderEdgeCase_3.txt
--rw-r--r--   0        0        0       10 2023-02-22 11:49:01.641263 cat_win-1.4.2/cat_win/tests/texts/test_holderEdgeCase_4.txt
--rw-r--r--   0        0        0       62 2023-03-26 12:18:56.747176 cat_win-1.4.2/cat_win/tests/texts/test_peek.txt
--rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.4.2/cat_win/util/__init__.py
--rw-r--r--   0        0        0     5959 2023-05-02 19:36:46.470436 cat_win-1.4.2/cat_win/util/argparser.py
--rw-r--r--   0        0        0     2765 2023-05-01 13:47:22.633145 cat_win-1.4.2/cat_win/util/cbase64.py
--rw-r--r--   0        0        0     1621 2023-05-01 16:15:32.374189 cat_win-1.4.2/cat_win/util/checksum.py
--rw-r--r--   0        0        0     3221 2023-05-01 14:51:45.585464 cat_win-1.4.2/cat_win/util/converter.py
--rw-r--r--   0        0        0      498 2023-05-05 19:13:34.870700 cat_win-1.4.2/cat_win/util/file.py
--rw-r--r--   0        0        0     3885 2023-05-08 17:38:04.295791 cat_win-1.4.2/cat_win/util/fileattributes.py
--rw-r--r--   0        0        0     7006 2023-05-07 19:58:27.528617 cat_win-1.4.2/cat_win/util/holder.py
--rw-r--r--   0        0        0     2793 2023-05-04 20:39:22.680079 cat_win-1.4.2/cat_win/util/rawviewer.py
--rw-r--r--   0        0        0     6620 2023-05-08 17:37:42.297614 cat_win-1.4.2/cat_win/util/stdinhelper.py
--rw-r--r--   0        0        0     3762 2023-05-01 16:20:02.002989 cat_win-1.4.2/cat_win/util/stringfinder.py
--rw-r--r--   0        0        0      386 2023-05-01 18:45:26.688828 cat_win-1.4.2/cat_win/util/tmpfilehelper.py
--rw-r--r--   0        0        0        0 2023-02-23 20:58:12.051941 cat_win-1.4.2/cat_win/web/__init__.py
--rw-r--r--   0        0        0     5851 2023-05-08 17:41:30.393772 cat_win-1.4.2/cat_win/web/updatechecker.py
--rw-r--r--   0        0        0     1552 2023-04-14 15:23:59.559474 cat_win-1.4.2/pyproject.toml
--rw-r--r--   0        0        0    14844 1970-01-01 00:00:00.000000 cat_win-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-02-19 10:54:41.226281 cat_win-1.4.3/LICENSE
+-rw-r--r--   0        0        0    14204 2023-07-09 18:57:52.251026 cat_win-1.4.3/README.md
+-rw-r--r--   0        0        0       39 2023-02-26 11:57:46.261532 cat_win-1.4.3/cat_win/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2023-02-26 11:57:46.261532 cat_win-1.4.3/cat_win/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2023-02-26 11:57:46.261532 cat_win-1.4.3/cat_win/.pytest_cache/README.md
+-rw-r--r--   0        0        0     5653 2023-02-26 11:57:52.638849 cat_win-1.4.3/cat_win/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2023-02-26 11:57:52.639848 cat_win-1.4.3/cat_win/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      289 2023-06-30 11:57:30.658406 cat_win-1.4.3/cat_win/__init__.py
+-rw-r--r--   0        0        0      363 2023-05-01 18:46:04.882782 cat_win-1.4.3/cat_win/__main__.py
+-rw-r--r--   0        0        0    37852 2023-07-09 10:28:00.405848 cat_win-1.4.3/cat_win/cat.py
+-rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.4.3/cat_win/const/__init__.py
+-rw-r--r--   0        0        0     5111 2023-07-08 12:02:02.596169 cat_win-1.4.3/cat_win/const/argconstants.py
+-rw-r--r--   0        0        0     2530 2023-06-25 11:16:34.728538 cat_win-1.4.3/cat_win/const/colorconstants.py
+-rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.4.3/cat_win/persistence/__init__.py
+-rw-r--r--   0        0        0     8739 2023-07-07 22:29:21.413769 cat_win-1.4.3/cat_win/persistence/config.py
+-rw-r--r--   0        0        0      319 2023-05-01 18:46:08.801676 cat_win-1.4.3/cat_win/shell.py
+-rw-r--r--   0        0        0        0 2023-02-19 10:54:41.304282 cat_win-1.4.3/cat_win/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-29 10:00:24.210446 cat_win-1.4.3/cat_win/tests/mocks/__init__.py
+-rw-r--r--   0        0        0     1443 2023-05-04 13:28:17.759035 cat_win-1.4.3/cat_win/tests/mocks/std.py
+-rw-r--r--   0        0        0     1170 2023-05-01 15:49:21.685058 cat_win-1.4.3/cat_win/tests/test_argconstants.py
+-rw-r--r--   0        0        0     8297 2023-07-05 11:38:10.806576 cat_win-1.4.3/cat_win/tests/test_argparser.py
+-rw-r--r--   0        0        0     7479 2023-07-07 22:06:49.315126 cat_win-1.4.3/cat_win/tests/test_cat.py
+-rw-r--r--   0        0        0     1131 2023-05-02 19:37:40.487184 cat_win-1.4.3/cat_win/tests/test_cbase64.py
+-rw-r--r--   0        0        0     1569 2023-05-02 19:37:45.944459 cat_win-1.4.3/cat_win/tests/test_checksum.py
+-rw-r--r--   0        0        0     1533 2023-05-04 13:57:20.651422 cat_win-1.4.3/cat_win/tests/test_config.py
+-rw-r--r--   0        0        0     3617 2023-06-26 15:01:49.825031 cat_win-1.4.3/cat_win/tests/test_converter.py
+-rw-r--r--   0        0        0      823 2023-05-02 19:38:00.930937 cat_win-1.4.3/cat_win/tests/test_file.py
+-rw-r--r--   0        0        0     2021 2023-05-01 15:57:01.266856 cat_win-1.4.3/cat_win/tests/test_fileattributes.py
+-rw-r--r--   0        0        0     7345 2023-07-05 11:37:17.148215 cat_win-1.4.3/cat_win/tests/test_full.py
+-rw-r--r--   0        0        0     7760 2023-07-08 17:18:22.308374 cat_win-1.4.3/cat_win/tests/test_holder.py
+-rw-r--r--   0        0        0     7408 2023-05-01 16:03:35.076827 cat_win-1.4.3/cat_win/tests/test_rawviewer.py
+-rw-r--r--   0        0        0     5508 2023-06-26 15:32:07.766622 cat_win-1.4.3/cat_win/tests/test_shell.py
+-rw-r--r--   0        0        0     1254 2023-05-04 13:29:46.034492 cat_win-1.4.3/cat_win/tests/test_stdinhelper.py
+-rw-r--r--   0        0        0     3117 2023-05-02 09:42:04.478371 cat_win-1.4.3/cat_win/tests/test_stringfinder.py
+-rw-r--r--   0        0        0     3951 2023-05-02 19:38:32.100152 cat_win-1.4.3/cat_win/tests/test_updatechecker.py
+-rw-r--r--   0        0        0     5393 2023-07-09 13:51:00.799550 cat_win-1.4.3/cat_win/tests/test_utility.py
+-rw-r--r--   0        0        0      170 2023-02-19 10:54:41.307281 cat_win-1.4.3/cat_win/tests/texts/full_test_result_B.txt
+-rw-r--r--   0        0        0      196 2023-02-19 10:54:41.307281 cat_win-1.4.3/cat_win/tests/texts/full_test_result_C.txt
+-rw-r--r--   0        0        0      139 2023-02-19 10:54:41.308281 cat_win-1.4.3/cat_win/tests/texts/full_test_result_D.txt
+-rw-r--r--   0        0        0      189 2023-02-19 10:54:41.308281 cat_win-1.4.3/cat_win/tests/texts/test.txt
+-rw-r--r--   0        0        0        0 2023-03-26 11:37:07.806578 cat_win-1.4.3/cat_win/tests/texts/test_empty.txt
+-rw-r--r--   0        0        0       19 2023-02-19 10:54:41.308281 cat_win-1.4.3/cat_win/tests/texts/test_holderEdgeCase_1.txt
+-rw-r--r--   0        0        0       21 2023-02-19 10:54:41.308281 cat_win-1.4.3/cat_win/tests/texts/test_holderEdgeCase_2.txt
+-rw-r--r--   0        0        0       28 2023-03-26 12:18:11.309629 cat_win-1.4.3/cat_win/tests/texts/test_holderEdgeCase_3.txt
+-rw-r--r--   0        0        0       10 2023-02-22 11:49:01.641263 cat_win-1.4.3/cat_win/tests/texts/test_holderEdgeCase_4.txt
+-rw-r--r--   0        0        0       62 2023-03-26 12:18:56.747176 cat_win-1.4.3/cat_win/tests/texts/test_peek.txt
+-rw-r--r--   0        0        0        0 2023-02-23 20:58:12.050939 cat_win-1.4.3/cat_win/util/__init__.py
+-rw-r--r--   0        0        0     6173 2023-07-08 17:00:15.447417 cat_win-1.4.3/cat_win/util/argparser.py
+-rw-r--r--   0        0        0     2765 2023-05-01 13:47:22.633145 cat_win-1.4.3/cat_win/util/cbase64.py
+-rw-r--r--   0        0        0     1621 2023-06-25 11:23:54.935989 cat_win-1.4.3/cat_win/util/checksum.py
+-rw-r--r--   0        0        0     7661 2023-07-07 16:24:02.692692 cat_win-1.4.3/cat_win/util/converter.py
+-rw-r--r--   0        0        0      498 2023-05-05 19:13:34.870700 cat_win-1.4.3/cat_win/util/file.py
+-rw-r--r--   0        0        0     3885 2023-05-08 17:38:04.295791 cat_win-1.4.3/cat_win/util/fileattributes.py
+-rw-r--r--   0        0        0     8276 2023-07-08 17:14:12.099770 cat_win-1.4.3/cat_win/util/holder.py
+-rw-r--r--   0        0        0     2793 2023-05-04 20:39:22.680079 cat_win-1.4.3/cat_win/util/rawviewer.py
+-rw-r--r--   0        0        0     6620 2023-05-08 17:37:42.297614 cat_win-1.4.3/cat_win/util/stdinhelper.py
+-rw-r--r--   0        0        0     4018 2023-07-06 12:13:13.574773 cat_win-1.4.3/cat_win/util/stringfinder.py
+-rw-r--r--   0        0        0      443 2023-07-07 16:41:26.573244 cat_win-1.4.3/cat_win/util/tmpfilehelper.py
+-rw-r--r--   0        0        0     2916 2023-07-09 10:31:54.415705 cat_win-1.4.3/cat_win/util/utility.py
+-rw-r--r--   0        0        0     3023 2023-07-09 10:32:58.454514 cat_win-1.4.3/cat_win/util/utilityold.py
+-rw-r--r--   0        0        0        0 2023-02-23 20:58:12.051941 cat_win-1.4.3/cat_win/web/__init__.py
+-rw-r--r--   0        0        0     5851 2023-05-08 17:41:30.393772 cat_win-1.4.3/cat_win/web/updatechecker.py
+-rw-r--r--   0        0        0     1552 2023-04-14 15:23:59.559474 cat_win-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0    15185 1970-01-01 00:00:00.000000 cat_win-1.4.3/PKG-INFO
```

### Comparing `cat_win-1.4.2/LICENSE` & `cat_win-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/README.md` & `cat_win-1.4.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 [![Tests]](https://raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-tests.svg)
 <!-- [![Compile-and-Push]](https://github.com/SilenZcience/cat_win/actions/workflows/build_executable.yml/badge.svg) -->
 
 This project copies the fundamental framework of the cat command-line tool from Linux and translates its features to an OS Independent program using Python. </br> Over time the project evolved in subject areas of other tools like 'echo', 'grep', 'ls', 'base64'.
 
 Additionally it includes the feature to strip and reverse the content of any given file, make use of the standard-input, which enables cat piping into each other, generating the checksum of any file, converting decimal, hexadecimal and binary numbers within any text, and much <a href="#usage">more</a> ...
 
-Contrary to the name of the project it is of course possible to use cat_win on Linux or MacOS!
+It is of course possible to use cat_win on Linux or MacOS, aswell as Windows!
 
 ### Made With
 [![MadeWith-Python]](https://www.python.org/)
 [![Python][Python-Version]](https://www.python.org/)
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
@@ -139,30 +139,33 @@
 | *-l, --linelength*     | display the length of each line                           | ✔              |
 | *-e, --ends*           | display $ at the end of each line                         | ✔              |
 | *-t, --tabs*           | display TAB characters as ^I                              | ✔              |
 | *--eof, --eof*         | display EOF characters as ^EOF                            | ✔              |
 | *-u, --unique*         | suppress repeated output lines                            | ❌             |
 | *-b, --blank*          | hide empty lines                                          | ✔              |
 | *-r, --reverse*        | reverse output                                            | ❌             |
+| *--sort, --sort*       | sort all lines alphabetically                             | ❌             |
 | *-p, --peek*           | only print the first and last lines                       | ❌             |
 | *-s, --sum*            | show sum of lines                                         | ❌             |
 | *-S, --SUM*            | ONLY show sum of lines                                    | ❌             |
 | *-f, --files*          | list applied files                                        | ❌             |
 | *-F, --FILES*          | ONLY list applied files and file sizes                    | ❌             |
-| *-g, --grep*           | only show lines containing queried keywords               | ✔              |
+| *-g, --grep*           | only show lines containing queried keywords or patterns   | ✔              |
+| *-G, --GREP*           | only show found and matched substrings                    | ✔              |
 | *-i, --interactive*    | use stdin                                                 | ❌             |
-| *-o, --oneline*        | take only the first stdin-line                            | ❌             |
+| *-o, --oneline*        | take only the first stdin-line                            | ✔              |
 | *-E, --ECHO*           | handle every following parameter as stdin                 | ❌             |
 | *-c, --clip*           | copy output to clipboard                                  | ✔              |
 | *-m, --checksum*       | show the checksums of all files                           | ❌             |
 | *-a, --attributes*     | show meta-information about the files                     | ❌             |
 |                        |                                                           |                |
 | *--dec, --DEC*         | convert decimal numbers to hexadecimal and binary         | ✔              |
 | *--hex, --HEX*         | convert hexadecimal numbers to decimal and binary         | ✔              |
 | *--bin, --BIN*         | convert binary numbers to decimal and hexadecimal         | ✔              |
+| *--eval, --EVAL*       | evaluate simple mathematical equations                    | ✔              |
 | *--b64e, --b64e*       | encode the input to base64                                | ✔              |
 | *--b64d, --b64d*       | decode the input from base64                              | ✔              |
 |                        |                                                           |                |
 | *--hexview, --HEXVIEW* | display the raw byte representation in hexadecimal        | ❌             |
 | *--binview, --binview* | display the raw byte representation in binary             | ❌             |
 |                        |                                                           |                |
 | *--nc, --nocolor*      | disable colored output                                    | ✔              |
@@ -173,15 +176,15 @@
 | *-R, --R\<stream\>*    | reconfigure the std-stream(s) with the parsed encoding </br> \<stream\> = 'in'/'out'/'err' (default is stdin & stdout)| ✔ |
 |                        |                                                           |                |
 | *enc=X*                | set file enconding to X (default is utf-8)                | ✔              |
 | *find=X*               | find/query a substring X in the given files               | ✔              |
 | *match=X*              | find/query a pattern X in the given files                 | ✔              |
 | *trunc=X:Y*            | truncate file to lines X and Y (python-like)              | ❌             |
 |                        |                                                           |                |
-| *[a,b]*                | replace a with b in every line                            | ✔              |
+| *[a,b]*                | replace a with b in every line (escape chars with '\\')   | ✔              |
 | *[a:​b:c]*              | python-like string indexing syntax (line by line)         | ✔              |
 
 ### Examples
 
 <details open>
 	<summary><b>📂 Images 📂</b></summary>
 
@@ -205,25 +208,25 @@
    <p float="left">
       <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example7.png" width="49%"/>
       <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example8.png" width="49%"/>
    </p>
 
 </details>
 
-```c
+```py
 $ echo "Hello World :)" | catw -i [6:] | catw -i [::-1] -ln
 > 1) [8] ): dlroW
 ```
 
 - - - -
 
-```c
-$ cats --dec -nl
-> >>> 12345
-> 1) [53] 12345 {Hexadecimal: 0x3039; Binary: 0b11000000111001}
+```py
+$ cats --eval --dec -nl
+> >>> 0xF * 5
+> 1) [41] 75 {Hexadecimal: 0x4b; Binary: 0b1001011}
 > >>> ...
 ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Changelog
 
@@ -234,17 +237,17 @@
 This project is licensed under the MIT License - see the [LICENSE](https://github.com/SilenZcience/cat_win/blob/main/LICENSE) file for details
 
 ## Contact
 
 > **SilenZcience** <br/>
 [![GitHub-SilenZcience][GitHub-SilenZcience]](https://github.com/SilenZcience)
 
-[OS-Windows]: https://svgshare.com/i/ZhY.svg
-[OS-Linux]: https://svgshare.com/i/Zhy.svg
-[OS-MacOS]: https://svgshare.com/i/ZjP.svg
+[OS-Windows]: https://img.shields.io/badge/os-windows-green
+[OS-Linux]: https://img.shields.io/badge/os-linux-green
+[OS-MacOS]: https://img.shields.io/badge/os-macOS-green
 
 [Unittests]: https://github.com/SilenZcience/cat_win/actions/workflows/unit_test.yml/badge.svg
 [Build-and-Check]: https://github.com/SilenZcience/cat_win/actions/workflows/package_test.yml/badge.svg
 [Compile-and-Push]: https://github.com/SilenZcience/cat_win/actions/workflows/build_executable.yml/badge.svg
 
 [Coverage]: https://raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-coverage.svg
 [Tests]: https://raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-tests.svg
```

#### html2text {}

```diff
@@ -28,18 +28,18 @@
 cat_win/badges/.github/badges/badge-tests.svg)  This project copies the
 fundamental framework of the cat command-line tool from Linux and translates
 its features to an OS Independent program using Python.  Over time the project
 evolved in subject areas of other tools like 'echo', 'grep', 'ls', 'base64'.
 Additionally it includes the feature to strip and reverse the content of any
 given file, make use of the standard-input, which enables cat piping into each
 other, generating the checksum of any file, converting decimal, hexadecimal and
-binary numbers within any text, and much more ... Contrary to the name of the
-project it is of course possible to use cat_win on Linux or MacOS! ### Made
-With [![MadeWith-Python]](https://www.python.org/) [![Python][Python-Version]]
-(https://www.python.org/)
+binary numbers within any text, and much more ... It is of course possible to
+use cat_win on Linux or MacOS, aswell as Windows! ### Made With [![MadeWith-
+Python]](https://www.python.org/) [![Python][Python-Version]](https://
+www.python.org/)
                                                                   (back_to_top)
 ## Getting Started ### Prerequisites - Using cat_win as a Python-Package
 demands a Python-Interpreter (>= 3.7). - Using cat_win as an Executable
 (Windows only!) demands no prerequisites, hereby the stand-alone executables
 `catw.exe` (& `cats.exe`) are sufficient. ### Installation [![Version]
 [CurrentVersion]](https://pypi.org/project/cat-win/) Simply install the python
 package (via [PyPI-cat_win](https://pypi.org/project/cat-win/)): ```console
@@ -72,68 +72,71 @@
 â | | *-v, --version* | output version information | â | | *--debug, --
 debug* | show debug information | â | | | | | | *-n, --number* | number all
 output lines | â | | *-l, --linelength* | display the length of each line |
 â | | *-e, --ends* | display $ at the end of each line | â | | *-t, --tabs*
 | display TAB characters as ^I | â | | *--eof, --eof* | display EOF
 characters as ^EOF | â | | *-u, --unique* | suppress repeated output lines |
 â | | *-b, --blank* | hide empty lines | â | | *-r, --reverse* | reverse
-output | â | | *-p, --peek* | only print the first and last lines | â | |
-*-s, --sum* | show sum of lines | â | | *-S, --SUM* | ONLY show sum of lines
-| â | | *-f, --files* | list applied files | â | | *-F, --FILES* | ONLY
-list applied files and file sizes | â | | *-g, --grep* | only show lines
-containing queried keywords | â | | *-i, --interactive* | use stdin | â | |
-*-o, --oneline* | take only the first stdin-line | â | | *-E, --ECHO* |
-handle every following parameter as stdin | â | | *-c, --clip* | copy output
-to clipboard | â | | *-m, --checksum* | show the checksums of all files | â
-| | *-a, --attributes* | show meta-information about the files | â | | | | |
-| *--dec, --DEC* | convert decimal numbers to hexadecimal and binary | â | |
-*--hex, --HEX* | convert hexadecimal numbers to decimal and binary | â | | *-
--bin, --BIN* | convert binary numbers to decimal and hexadecimal | â | | *--
-b64e, --b64e* | encode the input to base64 | â | | *--b64d, --b64d* | decode
-the input from base64 | â | | | | | | *--hexview, --HEXVIEW* | display the
-raw byte representation in hexadecimal | â | | *--binview, --binview* |
-display the raw byte representation in binary | â | | | | | | *--nc, --
-nocolor* | disable colored output | â | | *--nb, --nobreak* | do not
-interrupt the output on queried keywords | â | | *--nk, --nokeyword* |
-inverse the grep output | â | | *--config, --config* | change color
-configuration | â | | | | | | *-R, --R\
+output | â | | *--sort, --sort* | sort all lines alphabetically | â | | *-
+p, --peek* | only print the first and last lines | â | | *-s, --sum* | show
+sum of lines | â | | *-S, --SUM* | ONLY show sum of lines | â | | *-f, --
+files* | list applied files | â | | *-F, --FILES* | ONLY list applied files
+and file sizes | â | | *-g, --grep* | only show lines containing queried
+keywords or patterns | â | | *-G, --GREP* | only show found and matched
+substrings | â | | *-i, --interactive* | use stdin | â | | *-o, --oneline*
+| take only the first stdin-line | â | | *-E, --ECHO* | handle every
+following parameter as stdin | â | | *-c, --clip* | copy output to clipboard
+| â | | *-m, --checksum* | show the checksums of all files | â | | *-a, --
+attributes* | show meta-information about the files | â | | | | | | *--dec, -
+-DEC* | convert decimal numbers to hexadecimal and binary | â | | *--hex, --
+HEX* | convert hexadecimal numbers to decimal and binary | â | | *--bin, --
+BIN* | convert binary numbers to decimal and hexadecimal | â | | *--eval, --
+EVAL* | evaluate simple mathematical equations | â | | *--b64e, --b64e* |
+encode the input to base64 | â | | *--b64d, --b64d* | decode the input from
+base64 | â | | | | | | *--hexview, --HEXVIEW* | display the raw byte
+representation in hexadecimal | â | | *--binview, --binview* | display the
+raw byte representation in binary | â | | | | | | *--nc, --nocolor* | disable
+colored output | â | | *--nb, --nobreak* | do not interrupt the output on
+queried keywords | â | | *--nk, --nokeyword* | inverse the grep output | â
+| | *--config, --config* | change color configuration | â | | | | | | *-R, --
+R\
 >* | reconfigure the std-stream(s) with the parsed encoding  \
 > = 'in'/'out'/'err' (default is stdin & stdout)| â | | | | | | *enc=X* | set
 file enconding to X (default is utf-8) | â | | *find=X* | find/query a
 substring X in the given files | â | | *match=X* | find/query a pattern X in
 the given files | â | | *trunc=X:Y* | truncate file to lines X and Y (python-
-like) | â | | | | | | *[a,b]* | replace a with b in every line | â | | *[a:
-âb:c]* | python-like string indexing syntax (line by line) | â | ###
-Examples  ð Images ð
+like) | â | | | | | | *[a,b]* | replace a with b in every line (escape chars
+with '\\') | â | | *[a:âb:c]* | python-like string indexing syntax (line by
+line) | â | ### Examples  ð Images ð
 [https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example1.png]
 [https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example2.png]
 [https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example3.png]
 [https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example4.png]
 [https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example5.png]
 [https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example6.png]
 - - - -
 [https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example7.png]
 [https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example8.png]
- ```c $ echo "Hello World :)" | catw -i [6:] | catw -i [::-1] -ln > 1) [8] ):
-dlroW ``` - - - - ```c $ cats --dec -nl > >>> 12345 > 1) [53] 12345
-{Hexadecimal: 0x3039; Binary: 0b11000000111001} > >>> ... ```
+ ```py $ echo "Hello World :)" | catw -i [6:] | catw -i [::-1] -ln > 1) [8] ):
+dlroW ``` - - - - ```py $ cats --eval --dec -nl > >>> 0xF * 5 > 1) [41] 75
+{Hexadecimal: 0x4b; Binary: 0b1001011} > >>> ... ```
                                                                   (back_to_top)
 ## Changelog Take a look at the [Changelog](https://github.com/SilenZcience/
 cat_win/blob/main/CHANGELOG.md) file. ## License This project is licensed under
 the MIT License - see the [LICENSE](https://github.com/SilenZcience/cat_win/
 blob/main/LICENSE) file for details ## Contact > **SilenZcience**
 [![GitHub-SilenZcience][GitHub-SilenZcience]](https://github.com/SilenZcience)
-[OS-Windows]: https://svgshare.com/i/ZhY.svg [OS-Linux]: https://svgshare.com/
-i/Zhy.svg [OS-MacOS]: https://svgshare.com/i/ZjP.svg [Unittests]: https://
-github.com/SilenZcience/cat_win/actions/workflows/unit_test.yml/badge.svg
-[Build-and-Check]: https://github.com/SilenZcience/cat_win/actions/workflows/
-package_test.yml/badge.svg [Compile-and-Push]: https://github.com/SilenZcience/
-cat_win/actions/workflows/build_executable.yml/badge.svg [Coverage]: https://
+[OS-Windows]: https://img.shields.io/badge/os-windows-green [OS-Linux]: https:/
+/img.shields.io/badge/os-linux-green [OS-MacOS]: https://img.shields.io/badge/
+os-macOS-green [Unittests]: https://github.com/SilenZcience/cat_win/actions/
+workflows/unit_test.yml/badge.svg [Build-and-Check]: https://github.com/
+SilenZcience/cat_win/actions/workflows/package_test.yml/badge.svg [Compile-and-
+Push]: https://github.com/SilenZcience/cat_win/actions/workflows/
+build_executable.yml/badge.svg [Coverage]: https://raw.githubusercontent.com/
+SilenZcience/cat_win/badges/.github/badges/badge-coverage.svg [Tests]: https://
 raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-
-coverage.svg [Tests]: https://raw.githubusercontent.com/SilenZcience/cat_win/
-badges/.github/badges/badge-tests.svg [MadeWith-Python]: https://
-img.shields.io/badge/Made%20with-Python-brightgreen [Python-Version]: https://
-img.shields.io/badge/Python-
+tests.svg [MadeWith-Python]: https://img.shields.io/badge/Made%20with-Python-
+brightgreen [Python-Version]: https://img.shields.io/badge/Python-
 3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%20pypy--
 3.8%20%7C%20pypy--3.9-blue [CurrentVersion]: https://img.shields.io/pypi/v/
 cat_win.svg [GitHub-SilenZcience]: https://img.shields.io/badge/GitHub-
 SilenZcience-orange
```

### Comparing `cat_win-1.4.2/cat_win/.pytest_cache/v/cache/nodeids` & `cat_win-1.4.3/cat_win/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/cat_win/cat.py` & `cat_win-1.4.3/cat_win/cat.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,14 +13,18 @@
 from cat_win.const.argconstants import *
 from cat_win.const.colorconstants import CKW
 from cat_win.persistence.config import Config
 from cat_win.util.argparser import ArgParser
 from cat_win.util.cbase64 import decode_base64, encode_base64
 from cat_win.util.checksum import get_checksum_from_file
 from cat_win.util.converter import Converter
+try:
+    from cat_win.util.utility import comp_eval, comp_conv, split_replace
+except SyntaxError: # in case of Python 3.7
+    from cat_win.util.utilityold import comp_eval, comp_conv, split_replace
 from cat_win.util.fileattributes import get_file_meta_data, get_file_size, _convert_size
 from cat_win.util.holder import Holder
 from cat_win.util.rawviewer import get_raw_view_lines_gen
 from cat_win.util.stringfinder import StringFinder
 from cat_win.util.tmpfilehelper import TmpFileHelper
 from cat_win.util import stdinhelper
 from cat_win.web.updatechecker import print_update_information
@@ -81,15 +85,15 @@
     help_message += '\n'
     help_message += f"\t{'enc=X, enc:X'    : <25}set file encoding to X (default is utf-8)\n"
     help_message += f"\t{'find=X, find:X'  : <25}find/query a substring X in the given files\n"
     help_message += f"\t{'match=X, match:X': <25}find/query a pattern X in the given files\n"
     if not shell:
         help_message += f"\t{'trunc=X:Y, trunc:X:Y': <25}truncate file to lines x and y (python-like)\n"
     help_message += '\n'
-    help_message += f"\t{'[a,b]': <25}replace a with b in every line\n"
+    help_message += f"\t{'[a,b]': <25}replace a with b in every line (escape chars with '\\')\n"
     help_message += f"\t{'[a:b:c]': <25}python-like string indexing syntax (line by line)\n"
     help_message += '\n'
     help_message += 'Examples:\n'
     if shell:
         help_message += '\tcats --ln --dec\n'
         help_message += '\t> >>> 12345\n'
         help_message += '\t1) [53] 12345 {Hexadecimal: 0x3039; Binary: 0b11000000111001}\n'
@@ -124,15 +128,15 @@
 
 
 def _show_debug(args: list, unknown_args: list, known_files: list, unknown_files: list,
                 echo_args: list) -> None:
     """
     Print all neccassary debug information
     """
-    print('Debug Information:')
+    print('==================================== DEBUG ====================================')
     print('args: ', end='')
     print([(arg[0], arg[1], holder.args_id[arg[0]]) for arg in args])
     print('unknown_args: ', end='')
     print(unknown_args)
     print('known_files: ', end='')
     print(known_files)
     print('unknown_files: ', end='')
@@ -143,14 +147,15 @@
     print(arg_parser.file_encoding)
     print('search keyword(s): ', end='')
     print(arg_parser.file_search)
     print('search match(es): ', end='')
     print(arg_parser.file_match)
     print('truncate file: ', end='')
     print(arg_parser.file_truncate)
+    print('===============================================================================')
 
 
 def _show_count() -> None:
     """
     display the line sum of each file individually if
     ARGS_CCOUNT is specified.
     display the line sum of all files.
@@ -230,15 +235,15 @@
     """
     for file in holder.files:
         if show_meta:
             _print_meta(file.path)
         if show_checksum:
             _print_checksum(file.path)
 
-
+@lru_cache(maxsize=250)
 def remove_ansi_codes_from_line(line: str) -> str:
     """
     Parameters:
     line (str):
         the string to clean ANSI-Colorcodes from
         
     Returns:
@@ -367,14 +372,20 @@
     contains_queried = False
     string_finder = StringFinder(arg_parser.file_search, arg_parser.file_match)
 
     for line_prefix, line in content:
         cleaned_line = remove_ansi_codes_from_line(line)
         intervals, f_keywords, m_keywords = string_finder.find_keywords(cleaned_line)
 
+        if holder.args_id[ARGS_GREP_ONLY]:
+            if f_keywords or m_keywords:
+                fm_substrings = [line[pos[0]:pos[1]] for _, pos in f_keywords + m_keywords]
+                print(','.join(fm_substrings))
+            continue
+
         if len(f_keywords + m_keywords) == 0:
             if not holder.args_id[ARGS_GREP]:
                 print(line_prefix + line)
             continue
 
         contains_queried = True
         if holder.args_id[ARGS_NOKEYWORD]:
@@ -475,40 +486,41 @@
                                 for prefix, line in content]
                 except Exception:
                     print('Error at operation: ', param)
                     return
 
         for arg, param in holder.args:
             if arg == ARGS_ENDS:
-                content = [(prefix, line + color_dic[CKW.ENDS] + '$' + color_dic[CKW.RESET_ALL])
+                content = [(prefix, f"{line}{color_dic[CKW.ENDS]}${color_dic[CKW.RESET_ALL]}")
                            for prefix, line in content]
             elif arg == ARGS_TABS:
-                content = [(prefix, line.replace('\t', color_dic[CKW.TABS] + '^I' + color_dic[CKW.RESET_ALL]))
+                content = [(prefix, line.replace('\t', f"{color_dic[CKW.TABS]}^I{color_dic[CKW.RESET_ALL]}"))
                            for prefix, line in content]
             elif arg == ARGS_SQUEEZE:
                 content = [list(group)[0] for _, group in groupby(content, lambda x: x[1])]
             elif arg == ARGS_REVERSE:
                 content.reverse()
+            elif arg == ARGS_SORT:
+                content.sort(key = lambda l: l[1])
             elif arg == ARGS_BLANK:
                 content = [c for c in content if c[1]]
+            elif arg == ARGS_EVAL:
+                content = comp_eval(converter, content, param, remove_ansi_codes_from_line)
             elif arg == ARGS_DEC:
-                content = [(prefix, line + ' ' + color_dic[CKW.CONVERSION] + converter.c_from_dec(int(line), (param == param.lower())) +
-                            color_dic[CKW.RESET_ALL]) for prefix, line in content if converter.is_dec(line)]
+                content = comp_conv(converter, content, param, remove_ansi_codes_from_line)
             elif arg == ARGS_HEX:
-                content = [(prefix, line + ' ' + color_dic[CKW.CONVERSION] + converter.c_from_hex(line, (param == param.lower())) +
-                            color_dic[CKW.RESET_ALL]) for prefix, line in content if converter.is_hex(line)]
+                content = comp_conv(converter, content, param, remove_ansi_codes_from_line)
             elif arg == ARGS_BIN:
-                content = [(prefix, line + ' ' + color_dic[CKW.CONVERSION] + converter.c_from_bin(line, (param == param.lower())) +
-                            color_dic[CKW.RESET_ALL]) for prefix, line in content if converter.is_bin(line)]
+                content = comp_conv(converter, content, param, remove_ansi_codes_from_line)
             elif arg == ARGS_REPLACE:
-                replace_values = param[1:-1].split(",")
-                content = [(prefix, line.replace(replace_values[0], color_dic[CKW.REPLACE] + replace_values[1] + color_dic[CKW.RESET_ALL]))
+                replace_values = split_replace(param)
+                content = [(prefix, line.replace(replace_values[0], f"{color_dic[CKW.REPLACE]}{replace_values[1]}{color_dic[CKW.RESET_ALL]}"))
                            for prefix, line  in content]
             elif arg == ARGS_EOF:
-                content = [(prefix, line.replace(chr(26), color_dic[CKW.REPLACE] + '^EOF' + color_dic[CKW.RESET_ALL]))
+                content = [(prefix, line.replace(chr(26), f"{color_dic[CKW.REPLACE]}^EOF{color_dic[CKW.RESET_ALL]}"))
                            for prefix, line in content]
 
     if holder.args_id[ARGS_LLENGTH]:
         content = [(_get_line_length_prefix(c[0], c[1]), c[1]) for c in content]
     if holder.args_id[ARGS_B64E]:
         content = encode_base64(content, arg_parser.file_encoding)
 
@@ -571,61 +583,78 @@
             print('Operation failed! Try using the enc=X parameter.')
             return
 
     edit_content(content, show_bytecode, file_index)
 
 
 def _copy_to_clipboard(content: str, __dependency: int = 3,
-                       __clip_board_error: bool = False) -> None:
+                       __clip_board_error: bool = False) -> object:
     """
     copy a string to the clipboard, by recursively checking which module exists and could
     be used, this function should only be called by copy_to_clipboard()
     
     Parameters:
     content (str):
         the string to copy
     __dependency (int):
         do not change!
     __clip_board_error (bool):
         do not change!
+        
+    Returns:
+    (function):
+        the method used for copying to the clipboard
+        (in case we want to use this function again without another import)
     """
     if __dependency == 0:
         if __clip_board_error:
             error_msg = '\n'
             error_msg += "ClipBoardError: You can use either 'pyperclip3', 'pyperclip', or 'pyclip' in order to use the '--clip' parameter.\n"
             error_msg += "Try to install a different one using 'python -m pip install ...'"
         else:
             error_msg = '\n'
             error_msg += "ImportError: You need either 'pyperclip3', 'pyperclip', or 'pyclip' in order to use the '--clip' parameter.\n"
             error_msg += "Should you have any problem with either module, try to install a different one using 'python -m pip install ...'"
         print(error_msg)
-        return
+        return None
     try:
         if __dependency == 3:
             import pyperclip as pc
         elif __dependency == 2:
             import pyclip as pc
         elif __dependency == 1:
             import pyperclip3 as pc
         pc.copy(content)
+        return pc.copy
     except ImportError:
-        _copy_to_clipboard(content, __dependency-1, False or __clip_board_error)
+        return _copy_to_clipboard(content, __dependency-1, False or __clip_board_error)
     except Exception:
-        _copy_to_clipboard(content, __dependency-1, True or __clip_board_error)
+        return _copy_to_clipboard(content, __dependency-1, True or __clip_board_error)
 
 
-def copy_to_clipboard(content: str) -> None:
+def copy_to_clipboard(content: str, copy_function: object = None) -> object:
     """
     entry point to recursive function _copy_to_clipboard()
     
     Parameters:
     content (str):
         the string to copy
-    """
-    _copy_to_clipboard(content)
+    copy_function (function):
+        the method to use for copying to the clipboard
+        (in case such a method already exists we do not need to import any module (again))
+        
+    Returns:
+    (function):
+        the method used for copying to the clipboard
+        (in case we want to use this function again without another import)    
+    """
+    if copy_function is not None:
+        copy_function(content)
+        return copy_function
+    return _copy_to_clipboard(content)
 
 
 def print_raw_view(file_index: int = 0, mode: str = 'X') -> None:
     """
     print the raw byte representation of a file in hexadecimal or binary
     
     Parameters:
@@ -682,14 +711,17 @@
     # do not use colors if requested, or output will be piped anyways
     global color_dic
     if holder.args_id[ARGS_NOCOL] or (not sys.stdout.isatty() or sys.stdout.closed):
         color_dic = dict.fromkeys(color_dic, '')
     else:
         color_dic = default_color_dic.copy()
 
+    converter.set_params(holder.args_id[ARGS_DEBUG],
+                         [color_dic[CKW.EVALUATION], color_dic[CKW.CONVERSION], color_dic[CKW.RESET_ALL]])
+
 
 def init(shell: bool = False) -> tuple:
     """
     initiate the code by calling the argparser and handling the default
     parameters: -h, -v, -d, --config.
     
     Parameters:
@@ -788,34 +820,43 @@
         edit_files()  # print the cat-output
     except IOError: # catch broken-pipe error
         devnull = os.open(os.devnull, os.O_WRONLY)
         os.dup2(devnull, sys.stdout.fileno())
         sys.exit(1)  # Python exits with error code 1 on EPIPE
 
     # clean-up
+    if holder.args_id[ARGS_DEBUG] and tmp_file_helper.tmp_count:
+        print('==================================== DEBUG ====================================')
     for tmp_file in tmp_file_helper.get_generated_temp_files():
         if holder.args_id[ARGS_DEBUG]:
             print('Cleaning', tmp_file)
         try:
             os.remove(tmp_file)
         except FileNotFoundError:
             if holder.args_id[ARGS_DEBUG]:
                 print('FileNotFoundError', tmp_file)
+        except PermissionError:
+            if holder.args_id[ARGS_DEBUG]:
+                print('PermissionError', tmp_file)
+    if holder.args_id[ARGS_DEBUG] and tmp_file_helper.tmp_count:
+        print('===============================================================================')
 
 
 def shell_main():
     init(True)
 
     command_prefix = '!'
     shell_prefix = '>>> '
     eof_control_char = 'Z' if on_windows_os else 'D'
     oneline = holder.args_id[ARGS_ONELINE]
 
     class CmdExec:
-        exit_shell = False
+        def __init__(self) -> None:
+            self.exit_shell = False
+            self.last_cmd = ''
 
         def exec_colors(self) -> None:
             init_colors()
             _calculate_line_prefix_spacing.cache_clear()
             _calculate_line_length_prefix_spacing.cache_clear()
 
         def exec(self, cmd: str) -> bool:
@@ -831,52 +872,64 @@
             (bool):
                 indicates if a valid command has been found
                 and executed
             """
             if cmd[:1] != command_prefix:
                 return False
             line_split = cmd[1:].split(' ')
-            method = getattr(self, '_command_' + line_split[0], lambda _: False)
+            self.last_cmd = line_split[0]
+            method = getattr(self, '_command_' + self.last_cmd, self._command_unknown)
             method(line_split[1:])
             return True
 
+        def _command_unknown(self, _) -> None:
+            print("Command '!", self.last_cmd, "' is unknown.", sep='')
+            print("If you want to escape the command input, type: '\\!", self.last_cmd, "'.", sep='')
+
         def _command_cat(self, _) -> None:
             cat = " ,_     _\n |\\\\_,-~/\n / _  _ |    ,--.\n(  @  @ )   / ,-'\n \\  _T_/"
             cat += "-._( (\n /         `. \\\n|         _  \\ |\n \\ \\ ,  /      |\n  || |-_\\__   /\n ((_/`(____,-'\n"
             print('\n'.join(['\t\t\t' + c for c in cat.split('\n')]))
 
         def _command_help(self, _) -> None:
             print(f"Type ^{eof_control_char} (Ctrl + {eof_control_char}) or '!exit' to exit.")
-            print("Type '!add <OPTION>', '!del <OPTION>', '!see' to change/see the active parameters.")
+            print("Type '!add <OPTION>', '!del <OPTION>' to add/remove a specific parameter.")
+            print("Type '!see', '!clear' to see/remove all active parameters.")
+            print("Put a '\\' before a leading '!' to escape the command-input.")
 
         def _command_add(self, cmd: list) -> None:
             arg_parser.gen_arguments([''] + cmd)
-            holder.add_args(arg_parser.args)
+            holder.add_args(arg_parser._args)
             self.exec_colors()
-            print(f"successfully added {[arg for _, arg in arg_parser.args] if arg_parser.args else 'parameters'}.")
+            print(f"successfully added {[arg for _, arg in arg_parser._args] if arg_parser._args else 'parameters'}.")
 
         def _command_del(self, cmd: list) -> None:
             arg_parser.gen_arguments([''] + cmd, True)
-            holder.delete_args(arg_parser.args)
+            holder.delete_args(arg_parser._args)
             self.exec_colors()
-            print(f"successfully removed {[arg for _, arg in arg_parser.args] if arg_parser.args else 'parameters'}.")
+            print(f"successfully removed {[arg for _, arg in arg_parser._args] if arg_parser._args else 'parameters'}.")
+            
+        def _command_clear(self, _) -> None:
+            arg_parser.reset_values()
+            self._command_del([arg for _, arg in holder.args])
 
         def _command_see(self, _) -> None:
             print(f"{'Active Args:': <12} {[arg for _, arg in holder.args]}")
             if arg_parser.file_search:
                 print(f"{'Literals:':<12} {arg_parser.file_search}")
             if arg_parser.file_match:
                 print(f"{'Matches:': <12} {arg_parser.file_match}")
 
         def _command_exit(self, _) -> None:
             self.exit_shell = True
 
 
     cmd = CmdExec()
     command_count = 0
+    copy_function = None
 
     print(__project__, 'v' + __version__, 'shell', '(' + __url__ + ')', end=' - ')
     print("Use 'catw' to handle files.")
     print("Type '!help' for more information.")
 
     print(shell_prefix, end='', flush=True)
     for i, line in enumerate(stdinhelper.get_stdin_content(oneline)):
@@ -886,15 +939,15 @@
             if cmd.exit_shell:
                 break
         else:
             stripped_line = stripped_line[:1].replace('\\', '') + stripped_line[1:]
             if stripped_line:
                 edit_content([('', stripped_line)], False, -1, i-command_count)
                 if holder.args_id[ARGS_CLIP]:
-                    copy_to_clipboard(remove_ansi_codes_from_line(holder.clip_board))
+                    copy_function = copy_to_clipboard(remove_ansi_codes_from_line(holder.clip_board), copy_function)
                     holder.clip_board = ''
         if not oneline:
             print(shell_prefix, end='', flush=True)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `cat_win-1.4.2/cat_win/const/argconstants.py` & `cat_win-1.4.3/cat_win/const/argconstants.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,233 +63,258 @@
 000003e0: 0d0a 4152 4753 5f4e 4f4b 4559 574f 5244  ..ARGS_NOKEYWORD
 000003f0: 2c20 4152 4753 5f52 4543 4f4e 4649 4755  , ARGS_RECONFIGU
 00000400: 5245 2c20 4152 4753 5f52 4543 4f4e 4649  RE, ARGS_RECONFI
 00000410: 4755 5245 5f49 4e2c 2041 5247 535f 5245  GURE_IN, ARGS_RE
 00000420: 434f 4e46 4947 5552 455f 4f55 542c 2041  CONFIGURE_OUT, A
 00000430: 5247 535f 5245 434f 4e46 4947 5552 455f  RGS_RECONFIGURE_
 00000440: 4552 5220 3d20 7261 6e67 6528 3335 2c20  ERR = range(35, 
-00000450: 3430 290d 0a0d 0a41 4c4c 5f41 5247 5320  40)....ALL_ARGS 
-00000460: 3d20 5b0d 0a20 2020 2041 7267 436f 6e73  = [..    ArgCons
-00000470: 7461 6e74 2827 2d68 272c 2027 2d2d 6865  tant('-h', '--he
-00000480: 6c70 272c 2027 7368 6f77 2074 6869 7320  lp', 'show this 
-00000490: 6865 6c70 206d 6573 7361 6765 2061 6e64  help message and
-000004a0: 2065 7869 7427 2c20 4152 4753 5f48 454c   exit', ARGS_HEL
-000004b0: 5029 2c0d 0a20 2020 2041 7267 436f 6e73  P),..    ArgCons
-000004c0: 7461 6e74 2827 2d76 272c 2027 2d2d 7665  tant('-v', '--ve
-000004d0: 7273 696f 6e27 2c20 276f 7574 7075 7420  rsion', 'output 
-000004e0: 7665 7273 696f 6e20 696e 666f 726d 6174  version informat
-000004f0: 696f 6e20 616e 6420 6578 6974 272c 2041  ion and exit', A
-00000500: 5247 535f 5645 5253 494f 4e29 2c0d 0a20  RGS_VERSION),.. 
-00000510: 2020 2041 7267 436f 6e73 7461 6e74 2827     ArgConstant('
-00000520: 2d2d 6465 6275 6727 2c20 272d 2d64 6562  --debug', '--deb
-00000530: 7567 272c 2027 7368 6f77 2064 6562 7567  ug', 'show debug
-00000540: 2069 6e66 6f72 6d61 7469 6f6e 272c 2041   information', A
-00000550: 5247 535f 4445 4255 472c 2046 616c 7365  RGS_DEBUG, False
-00000560: 292c 0d0a 2020 2020 4172 6743 6f6e 7374  ),..    ArgConst
-00000570: 616e 7428 272d 6e27 2c20 272d 2d6e 756d  ant('-n', '--num
-00000580: 6265 7227 2c20 276e 756d 6265 7220 616c  ber', 'number al
-00000590: 6c20 6f75 7470 7574 206c 696e 6573 272c  l output lines',
-000005a0: 2041 5247 535f 4e55 4d42 4552 292c 0d0a   ARGS_NUMBER),..
-000005b0: 2020 2020 4172 6743 6f6e 7374 616e 7428      ArgConstant(
-000005c0: 272d 6c27 2c20 272d 2d6c 696e 656c 656e  '-l', '--linelen
-000005d0: 6774 6827 2c20 2764 6973 706c 6179 2074  gth', 'display t
-000005e0: 6865 206c 656e 6774 6820 6f66 2065 6163  he length of eac
-000005f0: 6820 6c69 6e65 272c 2041 5247 535f 4c4c  h line', ARGS_LL
-00000600: 454e 4754 4829 2c0d 0a20 2020 2041 7267  ENGTH),..    Arg
-00000610: 436f 6e73 7461 6e74 2827 2d65 272c 2027  Constant('-e', '
-00000620: 2d2d 656e 6473 272c 2027 6469 7370 6c61  --ends', 'displa
-00000630: 7920 2420 6174 2074 6865 2065 6e64 206f  y $ at the end o
-00000640: 6620 6561 6368 206c 696e 6527 2c20 4152  f each line', AR
-00000650: 4753 5f45 4e44 5329 2c0d 0a20 2020 2041  GS_ENDS),..    A
-00000660: 7267 436f 6e73 7461 6e74 2827 2d74 272c  rgConstant('-t',
-00000670: 2027 2d2d 7461 6273 272c 2027 6469 7370   '--tabs', 'disp
-00000680: 6c61 7920 5441 4220 6368 6172 6163 7465  lay TAB characte
-00000690: 7273 2061 7320 5e49 272c 2041 5247 535f  rs as ^I', ARGS_
-000006a0: 5441 4253 292c 0d0a 2020 2020 4172 6743  TABS),..    ArgC
-000006b0: 6f6e 7374 616e 7428 272d 2d65 6f66 272c  onstant('--eof',
-000006c0: 2027 2d2d 656f 6627 2c20 2764 6973 706c   '--eof', 'displ
-000006d0: 6179 2045 4f46 2063 6861 7261 6374 6572  ay EOF character
-000006e0: 7320 6173 205e 454f 4627 2c20 4152 4753  s as ^EOF', ARGS
-000006f0: 5f45 4f46 292c 0d0a 2020 2020 4172 6743  _EOF),..    ArgC
-00000700: 6f6e 7374 616e 7428 272d 7527 2c20 272d  onstant('-u', '-
-00000710: 2d75 6e69 7175 6527 2c20 2773 7570 7072  -unique', 'suppr
-00000720: 6573 7320 7265 7065 6174 6564 206f 7574  ess repeated out
-00000730: 7075 7420 6c69 6e65 7327 2c20 4152 4753  put lines', ARGS
-00000740: 5f53 5155 4545 5a45 2c20 5472 7565 2c20  _SQUEEZE, True, 
-00000750: 4661 6c73 6529 2c0d 0a20 2020 2041 7267  False),..    Arg
-00000760: 436f 6e73 7461 6e74 2827 2d62 272c 2027  Constant('-b', '
-00000770: 2d2d 626c 616e 6b27 2c20 2768 6964 6520  --blank', 'hide 
-00000780: 656d 7074 7920 6c69 6e65 7327 2c20 4152  empty lines', AR
-00000790: 4753 5f42 4c41 4e4b 292c 0d0a 2020 2020  GS_BLANK),..    
-000007a0: 4172 6743 6f6e 7374 616e 7428 272d 7227  ArgConstant('-r'
-000007b0: 2c20 272d 2d72 6576 6572 7365 272c 2027  , '--reverse', '
-000007c0: 7265 7665 7273 6520 6f75 7470 7574 272c  reverse output',
-000007d0: 2041 5247 535f 5245 5645 5253 452c 2054   ARGS_REVERSE, T
-000007e0: 7275 652c 2046 616c 7365 292c 0d0a 2020  rue, False),..  
-000007f0: 2020 4172 6743 6f6e 7374 616e 7428 272d    ArgConstant('-
-00000800: 7027 2c20 272d 2d70 6565 6b27 2c20 276f  p', '--peek', 'o
-00000810: 6e6c 7920 7072 696e 7420 7468 6520 6669  nly print the fi
-00000820: 7273 7420 616e 6420 6c61 7374 206c 696e  rst and last lin
-00000830: 6573 272c 2041 5247 535f 5045 454b 2c20  es', ARGS_PEEK, 
-00000840: 5472 7565 2c20 4661 6c73 6529 2c0d 0a20  True, False),.. 
-00000850: 2020 2041 7267 436f 6e73 7461 6e74 2827     ArgConstant('
-00000860: 2d73 272c 2027 2d2d 7375 6d27 2c20 2773  -s', '--sum', 's
-00000870: 686f 7720 7375 6d20 6f66 206c 696e 6573  how sum of lines
-00000880: 272c 2041 5247 535f 434f 554e 542c 2054  ', ARGS_COUNT, T
-00000890: 7275 652c 2046 616c 7365 292c 0d0a 2020  rue, False),..  
-000008a0: 2020 4172 6743 6f6e 7374 616e 7428 272d    ArgConstant('-
-000008b0: 5327 2c20 272d 2d53 554d 272c 2027 4f4e  S', '--SUM', 'ON
-000008c0: 4c59 2073 686f 7720 7375 6d20 6f66 206c  LY show sum of l
-000008d0: 696e 6573 272c 2041 5247 535f 4343 4f55  ines', ARGS_CCOU
-000008e0: 4e54 2c20 5472 7565 2c20 4661 6c73 6529  NT, True, False)
-000008f0: 2c0d 0a20 2020 2041 7267 436f 6e73 7461  ,..    ArgConsta
-00000900: 6e74 2827 2d66 272c 2027 2d2d 6669 6c65  nt('-f', '--file
-00000910: 7327 2c20 276c 6973 7420 6170 706c 6965  s', 'list applie
-00000920: 6420 6669 6c65 7327 2c20 4152 4753 5f46  d files', ARGS_F
-00000930: 494c 4553 2c20 5472 7565 2c20 4661 6c73  ILES, True, Fals
-00000940: 6529 2c0d 0a20 2020 2041 7267 436f 6e73  e),..    ArgCons
-00000950: 7461 6e74 2827 2d46 272c 2027 2d2d 4649  tant('-F', '--FI
-00000960: 4c45 5327 2c20 274f 4e4c 5920 6c69 7374  LES', 'ONLY list
-00000970: 2061 7070 6c69 6564 2066 696c 6573 2061   applied files a
-00000980: 6e64 2066 696c 6520 7369 7a65 7327 2c20  nd file sizes', 
-00000990: 4152 4753 5f46 4649 4c45 532c 2054 7275  ARGS_FFILES, Tru
-000009a0: 652c 2046 616c 7365 292c 0d0a 2020 2020  e, False),..    
-000009b0: 4172 6743 6f6e 7374 616e 7428 272d 6727  ArgConstant('-g'
-000009c0: 2c20 272d 2d67 7265 7027 2c20 276f 6e6c  , '--grep', 'onl
-000009d0: 7920 7368 6f77 206c 696e 6573 2063 6f6e  y show lines con
-000009e0: 7461 696e 696e 6720 7175 6572 6965 6420  taining queried 
-000009f0: 6b65 7977 6f72 6473 272c 2041 5247 535f  keywords', ARGS_
-00000a00: 4752 4550 292c 0d0a 2020 2020 4172 6743  GREP),..    ArgC
-00000a10: 6f6e 7374 616e 7428 272d 6927 2c20 272d  onstant('-i', '-
-00000a20: 2d69 6e74 6572 6163 7469 7665 272c 2027  -interactive', '
-00000a30: 7573 6520 7374 6469 6e27 2c20 4152 4753  use stdin', ARGS
-00000a40: 5f49 4e54 4552 4143 5449 5645 2c20 5472  _INTERACTIVE, Tr
-00000a50: 7565 2c20 4661 6c73 6529 2c0d 0a20 2020  ue, False),..   
-00000a60: 2041 7267 436f 6e73 7461 6e74 2827 2d6f   ArgConstant('-o
-00000a70: 272c 2027 2d2d 6f6e 656c 696e 6527 2c20  ', '--oneline', 
-00000a80: 2774 616b 6520 6f6e 6c79 2074 6865 2066  'take only the f
-00000a90: 6972 7374 2073 7464 696e 2d6c 696e 6527  irst stdin-line'
-00000aa0: 2c20 4152 4753 5f4f 4e45 4c49 4e45 2c20  , ARGS_ONELINE, 
-00000ab0: 5472 7565 2c20 4661 6c73 6529 2c0d 0a20  True, False),.. 
-00000ac0: 2020 2041 7267 436f 6e73 7461 6e74 2827     ArgConstant('
-00000ad0: 2d45 272c 2027 2d2d 4543 484f 272c 2027  -E', '--ECHO', '
-00000ae0: 6861 6e64 6c65 2065 7665 7279 2066 6f6c  handle every fol
-00000af0: 6c6f 7769 6e67 2070 6172 616d 6574 6572  lowing parameter
-00000b00: 2061 7320 7374 6469 6e27 2c20 4152 4753   as stdin', ARGS
-00000b10: 5f45 4348 4f2c 2054 7275 652c 2046 616c  _ECHO, True, Fal
-00000b20: 7365 292c 0d0a 2020 2020 4172 6743 6f6e  se),..    ArgCon
-00000b30: 7374 616e 7428 272d 6327 2c20 272d 2d63  stant('-c', '--c
-00000b40: 6c69 7027 2c20 2763 6f70 7920 6f75 7470  lip', 'copy outp
-00000b50: 7574 2074 6f20 636c 6970 626f 6172 6427  ut to clipboard'
-00000b60: 2c20 4152 4753 5f43 4c49 5029 2c0d 0a20  , ARGS_CLIP),.. 
-00000b70: 2020 2041 7267 436f 6e73 7461 6e74 2827     ArgConstant('
-00000b80: 2d6d 272c 2027 2d2d 6368 6563 6b73 756d  -m', '--checksum
-00000b90: 272c 2027 7368 6f77 2074 6865 2063 6865  ', 'show the che
-00000ba0: 636b 7375 6d73 206f 6620 616c 6c20 6669  cksums of all fi
-00000bb0: 6c65 7327 2c20 4152 4753 5f43 4845 434b  les', ARGS_CHECK
-00000bc0: 5355 4d2c 2054 7275 652c 2046 616c 7365  SUM, True, False
-00000bd0: 292c 0d0a 2020 2020 4172 6743 6f6e 7374  ),..    ArgConst
-00000be0: 616e 7428 272d 6127 2c20 272d 2d61 7474  ant('-a', '--att
-00000bf0: 7269 6275 7465 7327 2c20 2773 686f 7720  ributes', 'show 
-00000c00: 6d65 7461 2d69 6e66 6f72 6d61 7469 6f6e  meta-information
-00000c10: 2061 626f 7574 2074 6865 2066 696c 6573   about the files
-00000c20: 272c 2041 5247 535f 4441 5441 2c20 5472  ', ARGS_DATA, Tr
-00000c30: 7565 2c20 4661 6c73 6529 2c0d 0a20 2020  ue, False),..   
-00000c40: 2041 7267 436f 6e73 7461 6e74 2827 2d2d   ArgConstant('--
-00000c50: 6465 6327 2c20 272d 2d44 4543 272c 2027  dec', '--DEC', '
-00000c60: 636f 6e76 6572 7420 6465 6369 6d61 6c20  convert decimal 
-00000c70: 6e75 6d62 6572 7320 746f 2068 6578 6164  numbers to hexad
-00000c80: 6563 696d 616c 2061 6e64 2062 696e 6172  ecimal and binar
-00000c90: 7927 2c20 4152 4753 5f44 4543 292c 0d0a  y', ARGS_DEC),..
-00000ca0: 2020 2020 4172 6743 6f6e 7374 616e 7428      ArgConstant(
-00000cb0: 272d 2d68 6578 272c 2027 2d2d 4845 5827  '--hex', '--HEX'
-00000cc0: 2c20 2763 6f6e 7665 7274 2068 6578 6164  , 'convert hexad
-00000cd0: 6563 696d 616c 206e 756d 6265 7273 2074  ecimal numbers t
-00000ce0: 6f20 6465 6369 6d61 6c20 616e 6420 6269  o decimal and bi
-00000cf0: 6e61 7279 272c 2041 5247 535f 4845 5829  nary', ARGS_HEX)
+00000450: 3430 290d 0a41 5247 535f 4556 414c 2c20  40)..ARGS_EVAL, 
+00000460: 4152 4753 5f53 4f52 542c 2041 5247 535f  ARGS_SORT, ARGS_
+00000470: 4752 4550 5f4f 4e4c 5920 3d20 7261 6e67  GREP_ONLY = rang
+00000480: 6528 3430 2c20 3433 290d 0a0d 0a44 4946  e(40, 43)....DIF
+00000490: 4645 5245 4e54 4941 424c 455f 4152 4753  FERENTIABLE_ARGS
+000004a0: 203d 205b 4152 4753 5f43 5554 2c20 4152   = [ARGS_CUT, AR
+000004b0: 4753 5f52 4550 4c41 4345 5d0d 0a0d 0a41  GS_REPLACE]....A
+000004c0: 4c4c 5f41 5247 5320 3d20 5b0d 0a20 2020  LL_ARGS = [..   
+000004d0: 2041 7267 436f 6e73 7461 6e74 2827 2d68   ArgConstant('-h
+000004e0: 272c 2027 2d2d 6865 6c70 272c 2027 7368  ', '--help', 'sh
+000004f0: 6f77 2074 6869 7320 6865 6c70 206d 6573  ow this help mes
+00000500: 7361 6765 2061 6e64 2065 7869 7427 2c20  sage and exit', 
+00000510: 4152 4753 5f48 454c 5029 2c0d 0a20 2020  ARGS_HELP),..   
+00000520: 2041 7267 436f 6e73 7461 6e74 2827 2d76   ArgConstant('-v
+00000530: 272c 2027 2d2d 7665 7273 696f 6e27 2c20  ', '--version', 
+00000540: 276f 7574 7075 7420 7665 7273 696f 6e20  'output version 
+00000550: 696e 666f 726d 6174 696f 6e20 616e 6420  information and 
+00000560: 6578 6974 272c 2041 5247 535f 5645 5253  exit', ARGS_VERS
+00000570: 494f 4e29 2c0d 0a20 2020 2041 7267 436f  ION),..    ArgCo
+00000580: 6e73 7461 6e74 2827 2d2d 6465 6275 6727  nstant('--debug'
+00000590: 2c20 272d 2d64 6562 7567 272c 2027 7368  , '--debug', 'sh
+000005a0: 6f77 2064 6562 7567 2069 6e66 6f72 6d61  ow debug informa
+000005b0: 7469 6f6e 272c 2041 5247 535f 4445 4255  tion', ARGS_DEBU
+000005c0: 472c 2046 616c 7365 292c 0d0a 2020 2020  G, False),..    
+000005d0: 4172 6743 6f6e 7374 616e 7428 272d 6e27  ArgConstant('-n'
+000005e0: 2c20 272d 2d6e 756d 6265 7227 2c20 276e  , '--number', 'n
+000005f0: 756d 6265 7220 616c 6c20 6f75 7470 7574  umber all output
+00000600: 206c 696e 6573 272c 2041 5247 535f 4e55   lines', ARGS_NU
+00000610: 4d42 4552 292c 0d0a 2020 2020 4172 6743  MBER),..    ArgC
+00000620: 6f6e 7374 616e 7428 272d 6c27 2c20 272d  onstant('-l', '-
+00000630: 2d6c 696e 656c 656e 6774 6827 2c20 2764  -linelength', 'd
+00000640: 6973 706c 6179 2074 6865 206c 656e 6774  isplay the lengt
+00000650: 6820 6f66 2065 6163 6820 6c69 6e65 272c  h of each line',
+00000660: 2041 5247 535f 4c4c 454e 4754 4829 2c0d   ARGS_LLENGTH),.
+00000670: 0a20 2020 2041 7267 436f 6e73 7461 6e74  .    ArgConstant
+00000680: 2827 2d65 272c 2027 2d2d 656e 6473 272c  ('-e', '--ends',
+00000690: 2027 6469 7370 6c61 7920 2420 6174 2074   'display $ at t
+000006a0: 6865 2065 6e64 206f 6620 6561 6368 206c  he end of each l
+000006b0: 696e 6527 2c20 4152 4753 5f45 4e44 5329  ine', ARGS_ENDS)
+000006c0: 2c0d 0a20 2020 2041 7267 436f 6e73 7461  ,..    ArgConsta
+000006d0: 6e74 2827 2d74 272c 2027 2d2d 7461 6273  nt('-t', '--tabs
+000006e0: 272c 2027 6469 7370 6c61 7920 5441 4220  ', 'display TAB 
+000006f0: 6368 6172 6163 7465 7273 2061 7320 5e49  characters as ^I
+00000700: 272c 2041 5247 535f 5441 4253 292c 0d0a  ', ARGS_TABS),..
+00000710: 2020 2020 4172 6743 6f6e 7374 616e 7428      ArgConstant(
+00000720: 272d 2d65 6f66 272c 2027 2d2d 656f 6627  '--eof', '--eof'
+00000730: 2c20 2764 6973 706c 6179 2045 4f46 2063  , 'display EOF c
+00000740: 6861 7261 6374 6572 7320 6173 205e 454f  haracters as ^EO
+00000750: 4627 2c20 4152 4753 5f45 4f46 292c 0d0a  F', ARGS_EOF),..
+00000760: 2020 2020 4172 6743 6f6e 7374 616e 7428      ArgConstant(
+00000770: 272d 7527 2c20 272d 2d75 6e69 7175 6527  '-u', '--unique'
+00000780: 2c20 2773 7570 7072 6573 7320 7265 7065  , 'suppress repe
+00000790: 6174 6564 206f 7574 7075 7420 6c69 6e65  ated output line
+000007a0: 7327 2c20 4152 4753 5f53 5155 4545 5a45  s', ARGS_SQUEEZE
+000007b0: 2c20 5472 7565 2c20 4661 6c73 6529 2c0d  , True, False),.
+000007c0: 0a20 2020 2041 7267 436f 6e73 7461 6e74  .    ArgConstant
+000007d0: 2827 2d62 272c 2027 2d2d 626c 616e 6b27  ('-b', '--blank'
+000007e0: 2c20 2768 6964 6520 656d 7074 7920 6c69  , 'hide empty li
+000007f0: 6e65 7327 2c20 4152 4753 5f42 4c41 4e4b  nes', ARGS_BLANK
+00000800: 292c 0d0a 2020 2020 4172 6743 6f6e 7374  ),..    ArgConst
+00000810: 616e 7428 272d 7227 2c20 272d 2d72 6576  ant('-r', '--rev
+00000820: 6572 7365 272c 2027 7265 7665 7273 6520  erse', 'reverse 
+00000830: 6f75 7470 7574 272c 2041 5247 535f 5245  output', ARGS_RE
+00000840: 5645 5253 452c 2054 7275 652c 2046 616c  VERSE, True, Fal
+00000850: 7365 292c 0d0a 2020 2020 4172 6743 6f6e  se),..    ArgCon
+00000860: 7374 616e 7428 272d 2d73 6f72 7427 2c20  stant('--sort', 
+00000870: 272d 2d73 6f72 7427 2c20 2773 6f72 7420  '--sort', 'sort 
+00000880: 616c 6c20 6c69 6e65 7320 616c 7068 6162  all lines alphab
+00000890: 6574 6963 616c 6c79 272c 2041 5247 535f  etically', ARGS_
+000008a0: 534f 5254 2c20 5472 7565 2c20 4661 6c73  SORT, True, Fals
+000008b0: 6529 2c0d 0a20 2020 2041 7267 436f 6e73  e),..    ArgCons
+000008c0: 7461 6e74 2827 2d70 272c 2027 2d2d 7065  tant('-p', '--pe
+000008d0: 656b 272c 2027 6f6e 6c79 2070 7269 6e74  ek', 'only print
+000008e0: 2074 6865 2066 6972 7374 2061 6e64 206c   the first and l
+000008f0: 6173 7420 6c69 6e65 7327 2c20 4152 4753  ast lines', ARGS
+00000900: 5f50 4545 4b2c 2054 7275 652c 2046 616c  _PEEK, True, Fal
+00000910: 7365 292c 0d0a 2020 2020 4172 6743 6f6e  se),..    ArgCon
+00000920: 7374 616e 7428 272d 7327 2c20 272d 2d73  stant('-s', '--s
+00000930: 756d 272c 2027 7368 6f77 2073 756d 206f  um', 'show sum o
+00000940: 6620 6c69 6e65 7327 2c20 4152 4753 5f43  f lines', ARGS_C
+00000950: 4f55 4e54 2c20 5472 7565 2c20 4661 6c73  OUNT, True, Fals
+00000960: 6529 2c0d 0a20 2020 2041 7267 436f 6e73  e),..    ArgCons
+00000970: 7461 6e74 2827 2d53 272c 2027 2d2d 5355  tant('-S', '--SU
+00000980: 4d27 2c20 274f 4e4c 5920 7368 6f77 2073  M', 'ONLY show s
+00000990: 756d 206f 6620 6c69 6e65 7327 2c20 4152  um of lines', AR
+000009a0: 4753 5f43 434f 554e 542c 2054 7275 652c  GS_CCOUNT, True,
+000009b0: 2046 616c 7365 292c 0d0a 2020 2020 4172   False),..    Ar
+000009c0: 6743 6f6e 7374 616e 7428 272d 6627 2c20  gConstant('-f', 
+000009d0: 272d 2d66 696c 6573 272c 2027 6c69 7374  '--files', 'list
+000009e0: 2061 7070 6c69 6564 2066 696c 6573 272c   applied files',
+000009f0: 2041 5247 535f 4649 4c45 532c 2054 7275   ARGS_FILES, Tru
+00000a00: 652c 2046 616c 7365 292c 0d0a 2020 2020  e, False),..    
+00000a10: 4172 6743 6f6e 7374 616e 7428 272d 4627  ArgConstant('-F'
+00000a20: 2c20 272d 2d46 494c 4553 272c 2027 4f4e  , '--FILES', 'ON
+00000a30: 4c59 206c 6973 7420 6170 706c 6965 6420  LY list applied 
+00000a40: 6669 6c65 7320 616e 6420 6669 6c65 2073  files and file s
+00000a50: 697a 6573 272c 2041 5247 535f 4646 494c  izes', ARGS_FFIL
+00000a60: 4553 2c20 5472 7565 2c20 4661 6c73 6529  ES, True, False)
+00000a70: 2c0d 0a20 2020 2041 7267 436f 6e73 7461  ,..    ArgConsta
+00000a80: 6e74 2827 2d67 272c 2027 2d2d 6772 6570  nt('-g', '--grep
+00000a90: 272c 2027 6f6e 6c79 2073 686f 7720 6c69  ', 'only show li
+00000aa0: 6e65 7320 636f 6e74 6169 6e69 6e67 2071  nes containing q
+00000ab0: 7565 7269 6564 206b 6579 776f 7264 7320  ueried keywords 
+00000ac0: 6f72 2070 6174 7465 726e 7327 2c20 4152  or patterns', AR
+00000ad0: 4753 5f47 5245 5029 2c0d 0a20 2020 2041  GS_GREP),..    A
+00000ae0: 7267 436f 6e73 7461 6e74 2827 2d47 272c  rgConstant('-G',
+00000af0: 2027 2d2d 4752 4550 272c 2027 6f6e 6c79   '--GREP', 'only
+00000b00: 2073 686f 7720 666f 756e 6420 616e 6420   show found and 
+00000b10: 6d61 7463 6865 6420 7375 6273 7472 696e  matched substrin
+00000b20: 6773 272c 2041 5247 535f 4752 4550 5f4f  gs', ARGS_GREP_O
+00000b30: 4e4c 5929 2c0d 0a20 2020 2041 7267 436f  NLY),..    ArgCo
+00000b40: 6e73 7461 6e74 2827 2d69 272c 2027 2d2d  nstant('-i', '--
+00000b50: 696e 7465 7261 6374 6976 6527 2c20 2775  interactive', 'u
+00000b60: 7365 2073 7464 696e 272c 2041 5247 535f  se stdin', ARGS_
+00000b70: 494e 5445 5241 4354 4956 452c 2054 7275  INTERACTIVE, Tru
+00000b80: 652c 2046 616c 7365 292c 0d0a 2020 2020  e, False),..    
+00000b90: 4172 6743 6f6e 7374 616e 7428 272d 6f27  ArgConstant('-o'
+00000ba0: 2c20 272d 2d6f 6e65 6c69 6e65 272c 2027  , '--oneline', '
+00000bb0: 7461 6b65 206f 6e6c 7920 7468 6520 6669  take only the fi
+00000bc0: 7273 7420 7374 6469 6e2d 6c69 6e65 272c  rst stdin-line',
+00000bd0: 2041 5247 535f 4f4e 454c 494e 452c 2054   ARGS_ONELINE, T
+00000be0: 7275 652c 2046 616c 7365 292c 0d0a 2020  rue, False),..  
+00000bf0: 2020 4172 6743 6f6e 7374 616e 7428 272d    ArgConstant('-
+00000c00: 4527 2c20 272d 2d45 4348 4f27 2c20 2768  E', '--ECHO', 'h
+00000c10: 616e 646c 6520 6576 6572 7920 666f 6c6c  andle every foll
+00000c20: 6f77 696e 6720 7061 7261 6d65 7465 7220  owing parameter 
+00000c30: 6173 2073 7464 696e 272c 2041 5247 535f  as stdin', ARGS_
+00000c40: 4543 484f 2c20 5472 7565 2c20 4661 6c73  ECHO, True, Fals
+00000c50: 6529 2c0d 0a20 2020 2041 7267 436f 6e73  e),..    ArgCons
+00000c60: 7461 6e74 2827 2d63 272c 2027 2d2d 636c  tant('-c', '--cl
+00000c70: 6970 272c 2027 636f 7079 206f 7574 7075  ip', 'copy outpu
+00000c80: 7420 746f 2063 6c69 7062 6f61 7264 272c  t to clipboard',
+00000c90: 2041 5247 535f 434c 4950 292c 0d0a 2020   ARGS_CLIP),..  
+00000ca0: 2020 4172 6743 6f6e 7374 616e 7428 272d    ArgConstant('-
+00000cb0: 6d27 2c20 272d 2d63 6865 636b 7375 6d27  m', '--checksum'
+00000cc0: 2c20 2773 686f 7720 7468 6520 6368 6563  , 'show the chec
+00000cd0: 6b73 756d 7320 6f66 2061 6c6c 2066 696c  ksums of all fil
+00000ce0: 6573 272c 2041 5247 535f 4348 4543 4b53  es', ARGS_CHECKS
+00000cf0: 554d 2c20 5472 7565 2c20 4661 6c73 6529  UM, True, False)
 00000d00: 2c0d 0a20 2020 2041 7267 436f 6e73 7461  ,..    ArgConsta
-00000d10: 6e74 2827 2d2d 6269 6e27 2c20 272d 2d42  nt('--bin', '--B
-00000d20: 494e 272c 2027 636f 6e76 6572 7420 6269  IN', 'convert bi
-00000d30: 6e61 7279 206e 756d 6265 7273 2074 6f20  nary numbers to 
-00000d40: 6465 6369 6d61 6c20 616e 6420 6865 7861  decimal and hexa
-00000d50: 6465 6369 6d61 6c27 2c20 4152 4753 5f42  decimal', ARGS_B
-00000d60: 494e 292c 0d0a 2020 2020 4172 6743 6f6e  IN),..    ArgCon
-00000d70: 7374 616e 7428 272d 2d62 3634 6527 2c20  stant('--b64e', 
-00000d80: 272d 2d62 3634 6527 2c20 2765 6e63 6f64  '--b64e', 'encod
-00000d90: 6520 7468 6520 696e 7075 7420 746f 2062  e the input to b
-00000da0: 6173 6536 3427 2c20 4152 4753 5f42 3634  ase64', ARGS_B64
-00000db0: 4529 2c0d 0a20 2020 2041 7267 436f 6e73  E),..    ArgCons
-00000dc0: 7461 6e74 2827 2d2d 6236 3464 272c 2027  tant('--b64d', '
-00000dd0: 2d2d 6236 3464 272c 2027 6465 636f 6465  --b64d', 'decode
-00000de0: 2074 6865 2069 6e70 7574 2066 726f 6d20   the input from 
-00000df0: 6261 7365 3634 272c 2041 5247 535f 4236  base64', ARGS_B6
-00000e00: 3444 292c 0d0a 2020 2020 4172 6743 6f6e  4D),..    ArgCon
-00000e10: 7374 616e 7428 272d 2d68 6578 7669 6577  stant('--hexview
-00000e20: 272c 2027 2d2d 4845 5856 4945 5727 2c20  ', '--HEXVIEW', 
-00000e30: 2764 6973 706c 6179 2074 6865 2072 6177  'display the raw
-00000e40: 2062 7974 6520 7265 7072 6573 656e 7461   byte representa
-00000e50: 7469 6f6e 2069 6e20 6865 7861 6465 6369  tion in hexadeci
-00000e60: 6d61 6c27 2c20 4152 4753 5f48 4558 5649  mal', ARGS_HEXVI
-00000e70: 4557 2c20 5472 7565 2c20 4661 6c73 6529  EW, True, False)
-00000e80: 2c0d 0a20 2020 2041 7267 436f 6e73 7461  ,..    ArgConsta
-00000e90: 6e74 2827 2d2d 6269 6e76 6965 7727 2c20  nt('--binview', 
-00000ea0: 272d 2d62 696e 7669 6577 272c 2027 6469  '--binview', 'di
-00000eb0: 7370 6c61 7920 7468 6520 7261 7720 6279  splay the raw by
-00000ec0: 7465 2072 6570 7265 7365 6e74 6174 696f  te representatio
-00000ed0: 6e20 696e 2062 696e 6172 7927 2c20 4152  n in binary', AR
-00000ee0: 4753 5f42 494e 5649 4557 2c20 5472 7565  GS_BINVIEW, True
-00000ef0: 2c20 4661 6c73 6529 2c0d 0a20 2020 2041  , False),..    A
-00000f00: 7267 436f 6e73 7461 6e74 2827 2d2d 6e63  rgConstant('--nc
-00000f10: 272c 2027 2d2d 6e6f 636f 6c6f 7227 2c20  ', '--nocolor', 
-00000f20: 2764 6973 6162 6c65 2063 6f6c 6f72 6564  'disable colored
-00000f30: 206f 7574 7075 7427 2c20 4152 4753 5f4e   output', ARGS_N
-00000f40: 4f43 4f4c 292c 0d0a 2020 2020 4172 6743  OCOL),..    ArgC
-00000f50: 6f6e 7374 616e 7428 272d 2d6e 6227 2c20  onstant('--nb', 
-00000f60: 272d 2d6e 6f62 7265 616b 272c 2027 646f  '--nobreak', 'do
-00000f70: 206e 6f74 2069 6e74 6572 7275 7074 2074   not interrupt t
-00000f80: 6865 206f 7574 7075 7420 6f6e 2071 7565  he output on que
-00000f90: 7269 6564 206b 6579 776f 7264 7327 2c20  ried keywords', 
-00000fa0: 4152 4753 5f4e 4f42 5245 414b 292c 0d0a  ARGS_NOBREAK),..
-00000fb0: 2020 2020 4172 6743 6f6e 7374 616e 7428      ArgConstant(
-00000fc0: 272d 2d6e 6b27 2c20 272d 2d6e 6f6b 6579  '--nk', '--nokey
-00000fd0: 776f 7264 272c 2027 696e 7665 7273 6520  word', 'inverse 
-00000fe0: 7468 6520 6772 6570 206f 7574 7075 7427  the grep output'
-00000ff0: 2c20 4152 4753 5f4e 4f4b 4559 574f 5244  , ARGS_NOKEYWORD
-00001000: 292c 0d0a 2020 2020 4172 6743 6f6e 7374  ),..    ArgConst
-00001010: 616e 7428 272d 2d63 6f6e 6669 6727 2c20  ant('--config', 
-00001020: 272d 2d63 6f6e 6669 6727 2c20 2763 6861  '--config', 'cha
-00001030: 6e67 6520 636f 6c6f 7220 636f 6e66 6967  nge color config
-00001040: 7572 6174 696f 6e27 2c20 4152 4753 5f43  uration', ARGS_C
-00001050: 4f4e 4649 4729 2c0d 0a20 2020 2041 7267  ONFIG),..    Arg
-00001060: 436f 6e73 7461 6e74 2827 2d52 272c 2027  Constant('-R', '
-00001070: 2d2d 5227 2c20 2772 6563 6f6e 6669 6775  --R', 'reconfigu
-00001080: 7265 2074 6865 2073 7464 696e 2061 6e64  re the stdin and
-00001090: 2073 7464 6f75 7420 7769 7468 2074 6865   stdout with the
-000010a0: 2070 6172 7365 6420 656e 636f 6469 6e67   parsed encoding
-000010b0: 272c 2041 5247 535f 5245 434f 4e46 4947  ', ARGS_RECONFIG
-000010c0: 5552 452c 2046 616c 7365 292c 0d0a 2020  URE, False),..  
-000010d0: 2020 4172 6743 6f6e 7374 616e 7428 272d    ArgConstant('-
-000010e0: 2d52 696e 272c 2027 2d2d 5269 6e27 2c20  -Rin', '--Rin', 
-000010f0: 2772 6563 6f6e 6669 6775 7265 2074 6865  'reconfigure the
-00001100: 2073 7464 696e 2077 6974 6820 7468 6520   stdin with the 
-00001110: 7061 7273 6564 2065 6e63 6f64 696e 6727  parsed encoding'
-00001120: 2c20 4152 4753 5f52 4543 4f4e 4649 4755  , ARGS_RECONFIGU
-00001130: 5245 5f49 4e2c 2046 616c 7365 292c 0d0a  RE_IN, False),..
-00001140: 2020 2020 4172 6743 6f6e 7374 616e 7428      ArgConstant(
-00001150: 272d 2d52 6f75 7427 2c20 272d 2d52 6f75  '--Rout', '--Rou
-00001160: 7427 2c20 2772 6563 6f6e 6669 6775 7265  t', 'reconfigure
-00001170: 2074 6865 2073 7464 6f75 7420 7769 7468   the stdout with
-00001180: 2074 6865 2070 6172 7365 6420 656e 636f   the parsed enco
-00001190: 6469 6e67 272c 2041 5247 535f 5245 434f  ding', ARGS_RECO
-000011a0: 4e46 4947 5552 455f 4f55 542c 2046 616c  NFIGURE_OUT, Fal
-000011b0: 7365 292c 0d0a 2020 2020 4172 6743 6f6e  se),..    ArgCon
-000011c0: 7374 616e 7428 272d 2d52 6572 7227 2c20  stant('--Rerr', 
-000011d0: 272d 2d52 6572 7227 2c20 2772 6563 6f6e  '--Rerr', 'recon
-000011e0: 6669 6775 7265 2074 6865 2073 7464 6572  figure the stder
-000011f0: 7220 7769 7468 2074 6865 2070 6172 7365  r with the parse
-00001200: 6420 656e 636f 6469 6e67 272c 2041 5247  d encoding', ARG
-00001210: 535f 5245 434f 4e46 4947 5552 455f 4552  S_RECONFIGURE_ER
-00001220: 522c 2046 616c 7365 292c 0d0a 2020 2020  R, False),..    
-00001230: 5d0d 0a0d 0a48 4947 4845 5354 5f41 5247  ]....HIGHEST_ARG
-00001240: 5f49 4420 3d20 6d61 7828 5b61 7267 2e61  _ID = max([arg.a
-00001250: 7267 5f69 6420 666f 7220 6172 6720 696e  rg_id for arg in
-00001260: 2041 4c4c 5f41 5247 535d 290d 0a          ALL_ARGS])..
+00000d10: 6e74 2827 2d61 272c 2027 2d2d 6174 7472  nt('-a', '--attr
+00000d20: 6962 7574 6573 272c 2027 7368 6f77 206d  ibutes', 'show m
+00000d30: 6574 612d 696e 666f 726d 6174 696f 6e20  eta-information 
+00000d40: 6162 6f75 7420 7468 6520 6669 6c65 7327  about the files'
+00000d50: 2c20 4152 4753 5f44 4154 412c 2054 7275  , ARGS_DATA, Tru
+00000d60: 652c 2046 616c 7365 292c 0d0a 2020 2020  e, False),..    
+00000d70: 4172 6743 6f6e 7374 616e 7428 272d 2d64  ArgConstant('--d
+00000d80: 6563 272c 2027 2d2d 4445 4327 2c20 2763  ec', '--DEC', 'c
+00000d90: 6f6e 7665 7274 2064 6563 696d 616c 206e  onvert decimal n
+00000da0: 756d 6265 7273 2074 6f20 6865 7861 6465  umbers to hexade
+00000db0: 6369 6d61 6c20 616e 6420 6269 6e61 7279  cimal and binary
+00000dc0: 272c 2041 5247 535f 4445 4329 2c0d 0a20  ', ARGS_DEC),.. 
+00000dd0: 2020 2041 7267 436f 6e73 7461 6e74 2827     ArgConstant('
+00000de0: 2d2d 6865 7827 2c20 272d 2d48 4558 272c  --hex', '--HEX',
+00000df0: 2027 636f 6e76 6572 7420 6865 7861 6465   'convert hexade
+00000e00: 6369 6d61 6c20 6e75 6d62 6572 7320 746f  cimal numbers to
+00000e10: 2064 6563 696d 616c 2061 6e64 2062 696e   decimal and bin
+00000e20: 6172 7927 2c20 4152 4753 5f48 4558 292c  ary', ARGS_HEX),
+00000e30: 0d0a 2020 2020 4172 6743 6f6e 7374 616e  ..    ArgConstan
+00000e40: 7428 272d 2d62 696e 272c 2027 2d2d 4249  t('--bin', '--BI
+00000e50: 4e27 2c20 2763 6f6e 7665 7274 2062 696e  N', 'convert bin
+00000e60: 6172 7920 6e75 6d62 6572 7320 746f 2064  ary numbers to d
+00000e70: 6563 696d 616c 2061 6e64 2068 6578 6164  ecimal and hexad
+00000e80: 6563 696d 616c 272c 2041 5247 535f 4249  ecimal', ARGS_BI
+00000e90: 4e29 2c0d 0a20 2020 2041 7267 436f 6e73  N),..    ArgCons
+00000ea0: 7461 6e74 2827 2d2d 6576 616c 272c 2027  tant('--eval', '
+00000eb0: 2d2d 4556 414c 272c 2027 6576 616c 7561  --EVAL', 'evalua
+00000ec0: 7465 2073 696d 706c 6520 6d61 7468 656d  te simple mathem
+00000ed0: 6174 6963 616c 2065 7175 6174 696f 6e73  atical equations
+00000ee0: 272c 2041 5247 535f 4556 414c 292c 0d0a  ', ARGS_EVAL),..
+00000ef0: 2020 2020 4172 6743 6f6e 7374 616e 7428      ArgConstant(
+00000f00: 272d 2d62 3634 6527 2c20 272d 2d62 3634  '--b64e', '--b64
+00000f10: 6527 2c20 2765 6e63 6f64 6520 7468 6520  e', 'encode the 
+00000f20: 696e 7075 7420 746f 2062 6173 6536 3427  input to base64'
+00000f30: 2c20 4152 4753 5f42 3634 4529 2c0d 0a20  , ARGS_B64E),.. 
+00000f40: 2020 2041 7267 436f 6e73 7461 6e74 2827     ArgConstant('
+00000f50: 2d2d 6236 3464 272c 2027 2d2d 6236 3464  --b64d', '--b64d
+00000f60: 272c 2027 6465 636f 6465 2074 6865 2069  ', 'decode the i
+00000f70: 6e70 7574 2066 726f 6d20 6261 7365 3634  nput from base64
+00000f80: 272c 2041 5247 535f 4236 3444 292c 0d0a  ', ARGS_B64D),..
+00000f90: 2020 2020 4172 6743 6f6e 7374 616e 7428      ArgConstant(
+00000fa0: 272d 2d68 6578 7669 6577 272c 2027 2d2d  '--hexview', '--
+00000fb0: 4845 5856 4945 5727 2c20 2764 6973 706c  HEXVIEW', 'displ
+00000fc0: 6179 2074 6865 2072 6177 2062 7974 6520  ay the raw byte 
+00000fd0: 7265 7072 6573 656e 7461 7469 6f6e 2069  representation i
+00000fe0: 6e20 6865 7861 6465 6369 6d61 6c27 2c20  n hexadecimal', 
+00000ff0: 4152 4753 5f48 4558 5649 4557 2c20 5472  ARGS_HEXVIEW, Tr
+00001000: 7565 2c20 4661 6c73 6529 2c0d 0a20 2020  ue, False),..   
+00001010: 2041 7267 436f 6e73 7461 6e74 2827 2d2d   ArgConstant('--
+00001020: 6269 6e76 6965 7727 2c20 272d 2d62 696e  binview', '--bin
+00001030: 7669 6577 272c 2027 6469 7370 6c61 7920  view', 'display 
+00001040: 7468 6520 7261 7720 6279 7465 2072 6570  the raw byte rep
+00001050: 7265 7365 6e74 6174 696f 6e20 696e 2062  resentation in b
+00001060: 696e 6172 7927 2c20 4152 4753 5f42 494e  inary', ARGS_BIN
+00001070: 5649 4557 2c20 5472 7565 2c20 4661 6c73  VIEW, True, Fals
+00001080: 6529 2c0d 0a20 2020 2041 7267 436f 6e73  e),..    ArgCons
+00001090: 7461 6e74 2827 2d2d 6e63 272c 2027 2d2d  tant('--nc', '--
+000010a0: 6e6f 636f 6c6f 7227 2c20 2764 6973 6162  nocolor', 'disab
+000010b0: 6c65 2063 6f6c 6f72 6564 206f 7574 7075  le colored outpu
+000010c0: 7427 2c20 4152 4753 5f4e 4f43 4f4c 292c  t', ARGS_NOCOL),
+000010d0: 0d0a 2020 2020 4172 6743 6f6e 7374 616e  ..    ArgConstan
+000010e0: 7428 272d 2d6e 6227 2c20 272d 2d6e 6f62  t('--nb', '--nob
+000010f0: 7265 616b 272c 2027 646f 206e 6f74 2069  reak', 'do not i
+00001100: 6e74 6572 7275 7074 2074 6865 206f 7574  nterrupt the out
+00001110: 7075 7420 6f6e 2071 7565 7269 6564 206b  put on queried k
+00001120: 6579 776f 7264 7327 2c20 4152 4753 5f4e  eywords', ARGS_N
+00001130: 4f42 5245 414b 292c 0d0a 2020 2020 4172  OBREAK),..    Ar
+00001140: 6743 6f6e 7374 616e 7428 272d 2d6e 6b27  gConstant('--nk'
+00001150: 2c20 272d 2d6e 6f6b 6579 776f 7264 272c  , '--nokeyword',
+00001160: 2027 696e 7665 7273 6520 7468 6520 6772   'inverse the gr
+00001170: 6570 206f 7574 7075 7427 2c20 4152 4753  ep output', ARGS
+00001180: 5f4e 4f4b 4559 574f 5244 292c 0d0a 2020  _NOKEYWORD),..  
+00001190: 2020 4172 6743 6f6e 7374 616e 7428 272d    ArgConstant('-
+000011a0: 2d63 6f6e 6669 6727 2c20 272d 2d63 6f6e  -config', '--con
+000011b0: 6669 6727 2c20 2763 6861 6e67 6520 636f  fig', 'change co
+000011c0: 6c6f 7220 636f 6e66 6967 7572 6174 696f  lor configuratio
+000011d0: 6e27 2c20 4152 4753 5f43 4f4e 4649 4729  n', ARGS_CONFIG)
+000011e0: 2c0d 0a20 2020 2041 7267 436f 6e73 7461  ,..    ArgConsta
+000011f0: 6e74 2827 2d52 272c 2027 2d2d 5227 2c20  nt('-R', '--R', 
+00001200: 2772 6563 6f6e 6669 6775 7265 2074 6865  'reconfigure the
+00001210: 2073 7464 696e 2061 6e64 2073 7464 6f75   stdin and stdou
+00001220: 7420 7769 7468 2074 6865 2070 6172 7365  t with the parse
+00001230: 6420 656e 636f 6469 6e67 272c 2041 5247  d encoding', ARG
+00001240: 535f 5245 434f 4e46 4947 5552 452c 2046  S_RECONFIGURE, F
+00001250: 616c 7365 292c 0d0a 2020 2020 4172 6743  alse),..    ArgC
+00001260: 6f6e 7374 616e 7428 272d 2d52 696e 272c  onstant('--Rin',
+00001270: 2027 2d2d 5269 6e27 2c20 2772 6563 6f6e   '--Rin', 'recon
+00001280: 6669 6775 7265 2074 6865 2073 7464 696e  figure the stdin
+00001290: 2077 6974 6820 7468 6520 7061 7273 6564   with the parsed
+000012a0: 2065 6e63 6f64 696e 6727 2c20 4152 4753   encoding', ARGS
+000012b0: 5f52 4543 4f4e 4649 4755 5245 5f49 4e2c  _RECONFIGURE_IN,
+000012c0: 2046 616c 7365 292c 0d0a 2020 2020 4172   False),..    Ar
+000012d0: 6743 6f6e 7374 616e 7428 272d 2d52 6f75  gConstant('--Rou
+000012e0: 7427 2c20 272d 2d52 6f75 7427 2c20 2772  t', '--Rout', 'r
+000012f0: 6563 6f6e 6669 6775 7265 2074 6865 2073  econfigure the s
+00001300: 7464 6f75 7420 7769 7468 2074 6865 2070  tdout with the p
+00001310: 6172 7365 6420 656e 636f 6469 6e67 272c  arsed encoding',
+00001320: 2041 5247 535f 5245 434f 4e46 4947 5552   ARGS_RECONFIGUR
+00001330: 455f 4f55 542c 2046 616c 7365 292c 0d0a  E_OUT, False),..
+00001340: 2020 2020 4172 6743 6f6e 7374 616e 7428      ArgConstant(
+00001350: 272d 2d52 6572 7227 2c20 272d 2d52 6572  '--Rerr', '--Rer
+00001360: 7227 2c20 2772 6563 6f6e 6669 6775 7265  r', 'reconfigure
+00001370: 2074 6865 2073 7464 6572 7220 7769 7468   the stderr with
+00001380: 2074 6865 2070 6172 7365 6420 656e 636f   the parsed enco
+00001390: 6469 6e67 272c 2041 5247 535f 5245 434f  ding', ARGS_RECO
+000013a0: 4e46 4947 5552 455f 4552 522c 2046 616c  NFIGURE_ERR, Fal
+000013b0: 7365 292c 0d0a 2020 2020 5d0d 0a0d 0a48  se),..    ]....H
+000013c0: 4947 4845 5354 5f41 5247 5f49 4420 3d20  IGHEST_ARG_ID = 
+000013d0: 6d61 7828 5b61 7267 2e61 7267 5f69 6420  max([arg.arg_id 
+000013e0: 666f 7220 6172 6720 696e 2041 4c4c 5f41  for arg in ALL_A
+000013f0: 5247 535d 290d 0a                        RGS])..
```

### Comparing `cat_win-1.4.2/cat_win/const/colorconstants.py` & `cat_win-1.4.3/cat_win/const/colorconstants.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     RESET_MATCHED = 'reset_matched'
 
     NUMBER = 'line_numbers'
     LINE_LENGTH = 'line_length'
     ENDS = 'line_ends'
     TABS = 'tab_characters'
     CONVERSION = 'number_conversion'
+    EVALUATION = 'number_evaluation'
     REPLACE = 'substring_replacement'
     FOUND = 'found_keyword'
     FOUND_MESSAGE = 'found_keyword_message'
     MATCHED = 'matched_pattern'
     MATCHED_MESSAGE = 'matched_pattern_message'
     CHECKSUM = 'checksum_message'
     COUNT_AND_FILES = 'processed_message'
```

### Comparing `cat_win-1.4.2/cat_win/persistence/config.py` & `cat_win-1.4.3/cat_win/persistence/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     allows for reading and writing the config file.
     """
     default_dic = {CKW.NUMBER: ColorOptions.Fore['GREEN'],
                    CKW.LINE_LENGTH: ColorOptions.Fore['LIGHTBLUE'],
                    CKW.ENDS: ColorOptions.Back['YELLOW'],
                    CKW.TABS: ColorOptions.Back['YELLOW'],
                    CKW.CONVERSION: ColorOptions.Fore['CYAN'],
+                   CKW.EVALUATION: ColorOptions.Fore['BLUE'],
                    CKW.REPLACE: ColorOptions.Fore['YELLOW'],
                    CKW.FOUND: ColorOptions.Fore['RED'],
                    CKW.FOUND_MESSAGE: ColorOptions.Fore['MAGENTA'],
                    CKW.MATCHED: ColorOptions.Back['CYAN'],
                    CKW.MATCHED_MESSAGE: ColorOptions.Fore['LIGHTCYAN'],
                    CKW.CHECKSUM: ColorOptions.Fore['CYAN'],
                    CKW.COUNT_AND_FILES: ColorOptions.Fore['CYAN'],
@@ -148,38 +149,47 @@
         the method load_config() was already called.
         """
         self._print_all_available_elements()
         keyword = ''
         while keyword not in self.elements:
             if keyword != '':
                 print(f"Something went wrong. Unknown keyword '{keyword}'")
-            keyword = input('Input name of keyword to change: ')
+            try:
+                keyword = input('Input name of keyword to change: ')
+            except EOFError:
+                print('\nAborting due to End-of-File character...')
+                return
             if keyword.isdigit():
                 keyword = self.elements[int(keyword)-1] if (
                     0 < int(keyword) <= len(self.elements)) else keyword
-        print(f"Successfully selected element '{keyword}'.")
+        print(f"Successfully selected element '{self.color_dic[keyword]}{keyword}{ColorOptions.Style['RESET']}'.")
 
         color_options = self._print_get_all_available_colors()
         color = ''
         while color not in color_options:
             if color != '':
                 print(f"Something went wrong. Unknown option '{color}'.")
-            color = input('Input color: ')
+            try:
+                color = input('Input color: ')
+            except EOFError:
+                print('\nAborting due to End-of-File character...')
+                return
             if color.isdigit():
                 color = color_options[int(color)-1] if (
                     0 < int(color) <= len(color_options)) else color
 
         if keyword in self.exclusive_definitions['Fore'] and color.startswith('Back'):
             print(f"An Error occured: '{keyword}' can only be of style 'Fore'")
             return
         if keyword in self.exclusive_definitions['Back'] and color.startswith('Fore'):
             print(f"An Error occured: '{keyword}' can only be of style 'Back'")
             return
 
-        print(f"Successfully selected element '{color}'.")
+        color_split = color.split('.')
+        print(f"Successfully selected element '{getattr(ColorOptions, color_split[0])[color_split[1]]}{color}{ColorOptions.Style['RESET']}'.")
 
         self.config_parser['COLORS'][keyword] = color
         try:
             with open(self.config_file, 'w', encoding='utf-8') as conf:
                 self.config_parser.write(conf)
             print(f"Successfully updated config file:\n\t{self.config_file}")
         except OSError:
```

### Comparing `cat_win-1.4.2/cat_win/tests/mocks/std.py` & `cat_win-1.4.3/cat_win/tests/mocks/std.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/cat_win/tests/test_argconstants.py` & `cat_win-1.4.3/cat_win/tests/test_argconstants.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/cat_win/tests/test_argparser.py` & `cat_win-1.4.3/cat_win/tests/test_argparser.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,30 +84,30 @@
         self.assertCountEqual(arg_parser.file_search, set(['Test123']))
 
     def test_get_arguments_trunc(self):
         arg_parser = ArgParser()
         arg_parser.get_arguments(['CAT', 'trunc=0:'])
         self.assertListEqual(arg_parser.file_truncate, [0, None, None])
         arg_parser.get_arguments(['CAT', 'trunc:1:'])
-        self.assertListEqual(arg_parser.file_truncate, [0, None, None])
-        arg_parser.get_arguments(['CAT', 'trunc:2:'])
         self.assertListEqual(arg_parser.file_truncate, [1, None, None])
+        arg_parser.get_arguments(['CAT', 'trunc:2:'])
+        self.assertListEqual(arg_parser.file_truncate, [2, None, None])
         arg_parser.get_arguments(['CAT', 'trunc:::-1'])
         self.assertListEqual(arg_parser.file_truncate, [None, None, -1])
         arg_parser.get_arguments(['CAT', 'trunc:4::-5'])
-        self.assertListEqual(arg_parser.file_truncate, [3, None, -5])
+        self.assertListEqual(arg_parser.file_truncate, [4, None, -5])
         arg_parser.get_arguments(['CAT', 'trunc:4:6:-5'])
-        self.assertListEqual(arg_parser.file_truncate, [3, 6, -5])
+        self.assertListEqual(arg_parser.file_truncate, [4, 6, -5])
         arg_parser.get_arguments(['CAT', 'trunc=:2*4-3:'])
         self.assertListEqual(arg_parser.file_truncate, [None, 5, None])
 
     def test_get_arguments_cut(self):
         arg_parser = ArgParser()
         arg_parser.gen_arguments(['CAT', '[2*5:20]'])
-        self.assertCountEqual(arg_parser.args, [(ARGS_CUT, '[2*5:20]')])
+        self.assertCountEqual(arg_parser._args, [(ARGS_CUT, '[2*5:20]')])
 
     def test_get_arguments_replace(self):
         arg_parser = ArgParser()
         args, _, _, _, _ = arg_parser.get_arguments(['CAT', '[test,404]'])
         self.assertCountEqual(args, [(ARGS_REPLACE, '[test,404]')])
 
     def test_get_arguments_dir(self):
@@ -135,30 +135,30 @@
         self.assertEqual(len(unknown_files), 2)
         self.assertIn('testTesttest', ''.join(unknown_files))
         self.assertIn('test-file.txt', ''.join(unknown_files))
 
     def test_get_arguments_unknown_args(self):
         arg_parser = ArgParser()
         arg_parser.gen_arguments(['CAT', '--test-file.txt'])
-        self.assertCountEqual(arg_parser.unknown_args, ['--test-file.txt'])
+        self.assertCountEqual(arg_parser._unknown_args, ['--test-file.txt'])
 
     def test_get_arguments_echo_args(self):
         arg_parser = ArgParser()
         args, unknown_args, known_files, unknown_files, echo_args = arg_parser.get_arguments(['CAT', '-n', '-E', '-n', 'random', test_file_dir])
         args = list(map(lambda x: x[1], args))
         self.assertCountEqual(args, ['-n', '-E'])
         self.assertCountEqual(unknown_args, [])
         self.assertCountEqual(known_files, [])
         self.assertCountEqual(unknown_files, [])
         self.assertCountEqual(echo_args, ['-n', 'random', test_file_dir])
 
     def test_get_arguments_echo_args_recursive(self):
         arg_parser = ArgParser()
         echo = arg_parser._add_argument('-nEn')
-        args = list(map(lambda x: x[1], arg_parser.args))
+        args = list(map(lambda x: x[1], arg_parser._args))
         self.assertCountEqual(args, ['-n', '-E'])
         self.assertEqual(echo, True)
 
     def test_delete_queried(self):
         arg_parser = ArgParser()
         arg_parser._add_argument('find=hello')
         arg_parser._add_argument('find=world')
```

### Comparing `cat_win-1.4.2/cat_win/tests/test_cat.py` & `cat_win-1.4.3/cat_win/tests/test_cat.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,13 +163,13 @@
             self.assertIn('Author', fake_out.getvalue())
 
     @patch('cat_win.cat.arg_parser.file_search', new=set(['hello', 'world']))
     def test__show_debug(self):
         with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat._show_debug([], ['test'], [], [], [])
             self.assertIn('test', fake_out.getvalue())
-            self.assertIn('Debug Information:', fake_out.getvalue())
+            self.assertIn('DEBUG', fake_out.getvalue())
             self.assertIn('hello', fake_out.getvalue())
             self.assertIn('world', fake_out.getvalue())
 
 
 # python -m unittest discover -s cat_win.tests -p test*.py
```

### Comparing `cat_win-1.4.2/cat_win/tests/test_cbase64.py` & `cat_win-1.4.3/cat_win/tests/test_cbase64.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/cat_win/tests/test_checksum.py` & `cat_win-1.4.3/cat_win/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/cat_win/tests/test_config.py` & `cat_win-1.4.3/cat_win/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/cat_win/tests/test_converter.py` & `cat_win-1.4.3/cat_win/tests/test_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 
 converter = Converter()
 
 
 class TestConverter(TestCase):
     def test_converter_dec(self):
         expected_output = '{Hexadecimal: 0x3039; Binary: 0b11000000111001}'
-        self.assertEqual(converter.c_from_dec(12345, True), expected_output)
+        self.assertEqual(converter.c_from_dec('12345', True), expected_output)
 
         expected_output = '{Hexadecimal: 3039; Binary: 11000000111001}'
-        self.assertEqual(converter.c_from_dec(12345, False), expected_output)
+        self.assertEqual(converter.c_from_dec('12345', False), expected_output)
 
     def test_converter_hex(self):
         expected_output = '{Decimal: 12345; Binary: 0b11000000111001}'
         self.assertEqual(converter.c_from_hex('0x3039', True), expected_output)
 
         expected_output = '{Decimal: 12345; Binary: 11000000111001}'
         self.assertEqual(converter.c_from_hex('0x3039', False), expected_output)
```

### Comparing `cat_win-1.4.2/cat_win/tests/test_file.py` & `cat_win-1.4.3/cat_win/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/cat_win/tests/test_fileattributes.py` & `cat_win-1.4.3/cat_win/tests/test_fileattributes.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/cat_win/tests/test_full.py` & `cat_win-1.4.3/cat_win/tests/test_full.py`

 * *Files 25% similar despite different names*

```diff
@@ -26,40 +26,40 @@
     def tearDown(self):
         cat._calculate_line_prefix_spacing.cache_clear()
         cat._calculate_line_length_prefix_spacing.cache_clear()
         cat.arg_parser = ArgParser()
         cat.holder = Holder()
 
     # no files parsed
-    @patch('cat_win.cat.sys.argv', ['<CAT>', '-ln', '--nc', '[::-2]', 'enc=utf8'])
+    @patch('cat_win.cat.sys.argv', ['<CAT>', '-ln', '[::-2]', 'enc=utf8'])
     def test_cat_output_full_a(self):
         expected_output = ''
         with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
 
-    @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, '-ln', '--nc', '[::-2]', 'enc=utf8'])
+    @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, '-ln', '[::-2]', 'enc=utf8'])
     def test_cat_output_full_b(self):
         expected_output = ''
         with open(test_result_B, 'r', encoding='utf-8') as output:
             expected_output = output.read()
         with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
 
-    @patch('cat_win.cat.sys.argv', ['<CAT>', 'enc:UTF-8', test_file_path, '-ub', '[Sample,TEST]', '--nc', '-le'])
+    @patch('cat_win.cat.sys.argv', ['<CAT>', 'enc:UTF-8', test_file_path, '-ub', '[Sample,TEST]', '-le'])
     def test_cat_output_full_c(self):
         expected_output = ''
         with open(test_result_C, 'r', encoding='utf-8') as output:
             expected_output = output.read()
         with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
 
-    @patch('cat_win.cat.sys.argv', ['<CAT>', 'enc=utf-8', test_file_path, 'trunc=2:6', '-n', '--reverse', '--nc', '-t'])
+    @patch('cat_win.cat.sys.argv', ['<CAT>', 'enc=utf-8', test_file_path, 'trunc=1:6', '-n', '--reverse', '-t'])
     def test_cat_output_full_d(self):
         expected_output = ''
         with open(test_result_D, 'r', encoding='utf-8') as output:
             expected_output = output.read()
         with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
@@ -67,54 +67,54 @@
     @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'trunc=0:0',])
     def test_cat_output_full_empty(self):
         expected_output = ''
         with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
 
-    @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=cp1252', '--nc'])
+    @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=cp1252'])
     def test_cat_output_full_cp1252(self):
         expected_output = ''
         with open(test_file_path, 'r', encoding='cp1252') as output:
             expected_output = output.read() + '\n'
         with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
 
-    @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=latin_1', '--nc'])
+    @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=latin_1'])
     def test_cat_output_full_latin1(self):
         expected_output = ''
         with open(test_file_path, 'r', encoding='latin_1') as output:
             expected_output = output.read() + '\n'
         with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
 
-    @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=utf-8', 'trunc=0:1', 'find=ple ', 'match=:', '--nc'])
+    @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=utf-8', 'trunc=0:1', 'find=ple ', 'match=:'])
     def test_cat_output_full_find_found(self):
         expected_output = "Sample Text:\n--------------- Found [('ple ', [3, 7])] ---------------\n--------------- Matched [(':', [11, 12])] ---------------\n"
         with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
 
-    @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=utf-8', 'trunc=0:1', 'find=NOTINLINE', '--nc'])
+    @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=utf-8', 'trunc=0:1', 'find=NOTINLINE'])
     def test_cat_output_full_find_not_found(self):
         expected_output = 'Sample Text:\n'
         with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
 
-    @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=utf-8', 'trunc=0:1', 'find=Text', '--nc', '--nk'])
+    @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=utf-8', 'trunc=0:1', 'find=Text', '--nk'])
     def test_cat_output_full_find_found_nokeyword(self):
         expected_output = ''
         with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
 
-    @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=utf-8', 'find=Text', '--nc', '--grep'])
+    @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, 'enc=utf-8', 'find=Text', '--grep'])
     def test_cat_output_full_find_found_grep(self):
         expected_output = 'Sample Text:\n'
         with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
 
     @patch('cat_win.cat.sys.argv', ['<CAT>', test_peek, 'enc=utf-8', '--peek'])
@@ -133,8 +133,31 @@
 9
 10
 """
         with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.main()
             self.assertEqual(fake_out.getvalue(), expected_output)
 
+    @patch('cat_win.cat.sys.argv', ['<CAT>', 'enc=utf-8', '--eval', '--dec', '-E', '5 + 5 * 5 // 2 - 3'])
+    def test_cat_output_full_eval(self):
+        expected_output = '14 {Hexadecimal: 0xe; Binary: 0b1110}\n'
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
+            cat.main()
+            self.assertEqual(fake_out.getvalue(), expected_output)
+
+    @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, test_empty_path, test_peek, '-F'])
+    def test_cat_output_full_show_files(self):
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
+            cat.main()
+            self.assertIn(test_file_path, fake_out.getvalue())
+            self.assertIn(test_empty_path, fake_out.getvalue())
+            self.assertIn(test_peek, fake_out.getvalue())
+
+    @patch('cat_win.cat.sys.argv', ['<CAT>', test_file_path, test_empty_path, test_peek, '-S'])
+    def test_cat_output_full_show_count(self):
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
+            cat.main()
+            self.assertIn(test_file_path, fake_out.getvalue())
+            self.assertIn(test_empty_path, fake_out.getvalue())
+            self.assertIn(test_peek, fake_out.getvalue())
+
 # python -m unittest discover -s cat_win.tests -p test*.py
```

### Comparing `cat_win-1.4.2/cat_win/tests/test_holder.py` & `cat_win-1.4.3/cat_win/tests/test_holder.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from unittest import TestCase
 import os
 
-from cat_win.const.argconstants import ARGS_B64E, ARGS_NOCOL, ARGS_LLENGTH, ARGS_NUMBER, ARGS_TABS, ARGS_ENDS
-from cat_win.util.holder import Holder, reduce_list
+from cat_win.const.argconstants import ARGS_B64E, ARGS_NOCOL, ARGS_LLENGTH, ARGS_NUMBER, ARGS_TABS, ARGS_ENDS, ARGS_REPLACE
+from cat_win.util.holder import Holder, reduce_list, diff_list
 # import sys
 # sys.path.append('../cat_win')
 
 
 test_file_dir = os.path.join(os.path.dirname(__file__), 'texts')
 test_file_path        = os.path.join(test_file_dir, 'test.txt')
 test_file_edge_case_1 = os.path.join(test_file_dir, 'test_holderEdgeCase_1.txt')
@@ -125,26 +125,40 @@
         self.assertListEqual(holder.args, [(ARGS_NUMBER, 'a'), (ARGS_LLENGTH, 'b'), (ARGS_TABS, 'c')])
         self.assertEqual(holder.args_id.count(True), 3)
 
     def test_delete_args(self):
         holder = Holder()
         holder.set_args([(ARGS_NUMBER, 'a'), (ARGS_LLENGTH, 'b')])
         holder.delete_args([(ARGS_ENDS, 'a'), (ARGS_NUMBER, 'x')])
-        self.assertListEqual(holder.args, [(ARGS_NUMBER, 'a'), (ARGS_LLENGTH, 'b')])
-        self.assertEqual(holder.args_id.count(True), 2)
+        self.assertListEqual(holder.args, [(ARGS_LLENGTH, 'b')])
+        self.assertEqual(holder.args_id.count(True), 1)
 
         holder.delete_args([(ARGS_NUMBER, 'x'), (ARGS_LLENGTH, 'b')])
-        self.assertListEqual(holder.args, [(ARGS_NUMBER, 'a')])
-        self.assertEqual(holder.args_id.count(True), 1)
+        self.assertListEqual(holder.args, [])
+        self.assertEqual(holder.args_id.count(True), 0)
 
     def test_reduce_list(self):
         test_list = [(ARGS_NUMBER, 'a'), (ARGS_LLENGTH, 'b')]
         reduced_list = reduce_list(test_list)
         self.assertListEqual(reduced_list, [(ARGS_NUMBER, 'a'), (ARGS_LLENGTH, 'b')])
-        
+
         test_list += [(ARGS_NUMBER, 'c'), (ARGS_ENDS, 'd')]
         reduced_list = reduce_list(test_list)
         self.assertListEqual(reduced_list, [(ARGS_NUMBER, 'a'), (ARGS_LLENGTH, 'b'), (ARGS_ENDS, 'd')])
-        
+
         test_list += [(ARGS_NUMBER, 'a'), (ARGS_LLENGTH, 'b'), (ARGS_NUMBER, 'c'), (ARGS_ENDS, 'd')]
         reduced_list = reduce_list(test_list)
         self.assertListEqual(reduced_list, [(ARGS_NUMBER, 'a'), (ARGS_LLENGTH, 'b'), (ARGS_ENDS, 'd')])
+
+    def test_diff_list(self):
+        test_list = [(ARGS_NUMBER, 'a'), (ARGS_LLENGTH, 'b')]
+        reduced_list = diff_list(test_list, [(ARGS_ENDS, 'a'), (ARGS_LLENGTH, 'c')])
+        self.assertListEqual(reduced_list, [(ARGS_NUMBER, 'a')])
+
+    def test_diff_list_differentiable(self):
+        test_list = [(ARGS_REPLACE, '[a,b]'), (ARGS_REPLACE, '[c,a]'), (ARGS_REPLACE, '[a,b]')]
+        reduced_list = diff_list(test_list, [(ARGS_REPLACE, '[a,b]'), (ARGS_REPLACE, '[l,l]')])
+        self.assertListEqual(reduced_list, [(ARGS_REPLACE, '[c,a]'), (ARGS_REPLACE, '[a,b]')])
+
+        test_list = [(ARGS_REPLACE, '[a,b]'), (ARGS_REPLACE, '[c,a]'), (ARGS_REPLACE, '[a,b]')]
+        reduced_list = diff_list(test_list, [(ARGS_REPLACE, '[a,b]'), (ARGS_REPLACE, '[a,b]')])
+        self.assertListEqual(reduced_list, [(ARGS_REPLACE, '[c,a]')])
```

### Comparing `cat_win-1.4.2/cat_win/tests/test_rawviewer.py` & `cat_win-1.4.3/cat_win/tests/test_rawviewer.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/cat_win/tests/test_shell.py` & `cat_win-1.4.3/cat_win/tests/test_shell.py`

 * *Files 15% similar despite different names*

```diff
@@ -31,14 +31,29 @@
         stdinhelpermock.set_content('test1\n!add -n\n!help\ntest2')
         expected_output = ['2) test2']
         with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.shell_main()
             fake_output = [line.lstrip('>>> ') for line in fake_out.getvalue().splitlines()[-2:-1]]
             self.assertListEqual(fake_output, expected_output)
 
+    def test_cat_shell_unknown_param(self):
+        wrong_cmd = '!xyz'
+        stdinhelpermock.set_content(wrong_cmd)
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
+            cat.shell_main()
+            self.assertIn(wrong_cmd, fake_out.getvalue())
+
+    def test_cat_shell_help_param(self):
+        stdinhelpermock.set_content('!help')
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
+            cat.shell_main()
+            self.assertIn('!add', fake_out.getvalue())
+            self.assertIn('!del', fake_out.getvalue())
+            self.assertIn('!see', fake_out.getvalue())
+
     def test_cat_shell_add_param(self):
         stdinhelpermock.set_content('abc\n!add -ln\nabc')
         expected_output = ['abc', "successfully added ['-l', '-n'].", '2) [3] abc']
         with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.shell_main()
             fake_output = [line.lstrip('>>> ') for line in fake_out.getvalue().splitlines()[2:-1]]
             self.assertListEqual(fake_output, expected_output)
@@ -56,14 +71,24 @@
         expected_output = ["successfully added ['-l', '-n'].", "Active Args: ['-l', '-n']",
                            "Literals:    {'test'}", "Matches:     {'[0-9]'}"]
         with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.shell_main()
             fake_output = [line.lstrip('>>> ') for line in fake_out.getvalue().splitlines()[2:-1]]
             self.assertListEqual(fake_output, expected_output)
 
+    def test_cat_shell_clear_param(self):
+        stdinhelpermock.set_content('!add -ln find=test match=[0-9]\n!see\n!clear\n!see')
+        expected_output = ["successfully added ['-l', '-n'].", "Active Args: ['-l', '-n']",
+                           "Literals:    {'test'}", "Matches:     {'[0-9]'}",
+                           "successfully removed ['-l', '-n'].", 'Active Args: []']
+        with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
+            cat.shell_main()
+            fake_output = [line.lstrip('>>> ') for line in fake_out.getvalue().splitlines()[2:-1]]
+            self.assertListEqual(fake_output, expected_output)
+
     def test_cat_shell_exit(self):
         stdinhelpermock.set_content('abc\n!exit\nabc')
         expected_output = ['abc']
         with patch('cat_win.cat.sys.stdout', new=StdOutMock()) as fake_out:
             cat.shell_main()
             fake_output = [line.lstrip('>>> ') for line in fake_out.getvalue().splitlines()[2:-1]]
             self.assertListEqual(fake_output, expected_output)
```

### Comparing `cat_win-1.4.2/cat_win/tests/test_stdinhelper.py` & `cat_win-1.4.3/cat_win/tests/test_stdinhelper.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/cat_win/tests/test_stringfinder.py` & `cat_win-1.4.3/cat_win/tests/test_stringfinder.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/cat_win/tests/test_updatechecker.py` & `cat_win-1.4.3/cat_win/tests/test_updatechecker.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/cat_win/util/argparser.py` & `cat_win-1.4.3/cat_win/util/argparser.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 from glob import iglob
 from os.path import isfile, realpath, isdir
-from re import match
+from re import match, IGNORECASE
 
 from cat_win.const.argconstants import ALL_ARGS, ARGS_CUT, ARGS_REPLACE, ARGS_ECHO
 
 
 DEFAULT_FILE_ENCODING = 'utf-8'
 
 
 class ArgParser:
     def __init__(self) -> None:
+        self._args = []
+        self._unknown_args = []
+        self._known_files = []
+        self._unknown_files = []
+        self._echo_args = []
+        
+        self.reset_values()
+        
+    def reset_values(self) -> None:
+        """
+        The here defined variables may be accessed from the outside.
+        """
         self.file_encoding: str = DEFAULT_FILE_ENCODING
         self.file_search = set()
         self.file_match = set()
         self.file_truncate = [None, None, None]
-        self.args = []
-        self.unknown_args = []
-        self.known_files = []
-        self.unknown_files = []
-        self.echo_args = []
 
     def get_arguments(self, argv: list, delete: bool = False) -> tuple:
         """
         Read all args to either a valid parameter, an invalid parameter,
         a known file, an unknown file, or an echo parameter to print out.
         
         Parameters:
@@ -33,15 +40,15 @@
             the shell when changing file_search, file_match
         
         Returns:
         (args, unknown_args, known_files, unknown_files, echo_args) (tuple):
             contains the paramater in a sorted manner
         """
         self.gen_arguments(argv, delete)
-        return (self.args, self.unknown_args, self.known_files, self.unknown_files, self.echo_args)
+        return (self._args, self._unknown_args, self._known_files, self._unknown_files, self._echo_args)
 
     def _add_argument(self, param: str, delete: bool = False) -> bool:
         """
         sorts an argument to either list option, by appending to it.
         
         Parameters:
         param (str):
@@ -52,75 +59,75 @@
             
         Returns:
         (bool):
             True if -E has been called, meaning every following parameter
             should simply be printed to stdout.
         """
         # 'enc' + ('=' or ':') + file_encoding
-        if match(r"\Aenc[\=\:].+\Z", param):
+        if match(r"\Aenc[\=\:].+\Z", param, IGNORECASE):
             self.file_encoding = param[4:]
             return False
         # 'match' + ('=' or ':') + file_match
-        if match(r"\Amatch[\=\:].+\Z", param):
+        if match(r"\Amatch[\=\:].+\Z", param, IGNORECASE):
             if delete:
                 self.file_match.discard(param[6:])
                 return False
             self.file_match.add(fr'{param[6:]}')
             return False
         # 'find' + ('=' or ':') + file_search
-        if match(r"\Afind[\=\:].+\Z", param):
+        if match(r"\Afind[\=\:].+\Z", param, IGNORECASE):
             if delete:
                 self.file_search.discard(param[5:])
                 return False
             self.file_search.add(param[5:])
             return False
         # 'trunc' + ('=' or ':') + file_truncate[0] + ':' + file_truncate[1] [+ ':' + file_truncate[2]]
-        if match(r"\Atrunc[\=\:][0-9()+\-*\/]*\:[0-9()+\-*\/]*\:?[0-9()+\-*\/]*\Z", param):
-            param_split = param[6:].split(':')
-            self.file_truncate[0] = None if param_split[0] == '' else max(0, int(eval(param_split[0]))-1)
-            self.file_truncate[1] = None if param_split[1] == '' else int(eval(param_split[1]))
-            if len(param_split) == 3:
-                self.file_truncate[2] = None if param_split[2] == '' else int(eval(param_split[2]))
+        if match(r"\Atrunc[\=\:][0-9\(\)\+\-\*\/]*\:[0-9\(\)\+\-\*\/]*\:?[0-9\(\)\+\-\*\/]*\Z", param, IGNORECASE):
+            for i, p_split in enumerate(param[6:].split(':')):
+                try:
+                    self.file_truncate[i] = int(eval(p_split))
+                except:
+                    self.file_truncate[i] = None
             return False
         # '[' + ARGS_CUT + ']'
-        if match(r"\A\[[0-9()+\-*\/]*\:[0-9()+\-*\/]*\:?[0-9()+\-*\/]*\]\Z", param):
-            self.args.append((ARGS_CUT, param))
+        if match(r"\A\[[0-9\(\)\+\-\*\/]*\:[0-9\(\)\+\-\*\/]*\:?[0-9\(\)\+\-\*\/]*\]\Z", param):
+            self._args.append((ARGS_CUT, param))
             return False
-        # '[' + ARGS_REPLACE + ']'
-        if match(r"\A\[.+\,.+\]\Z", param):
-            self.args.append((ARGS_REPLACE, param))
+        # '[' + ARGS_REPLACE_THIS + ',' + ARGS_REPLACE_WITH + ']' (escape chars with '\')
+        if match(r"\A\[(?:.*[^\\])?(?:\\\\)*,(?:.*[^\\])?(?:\\\\)*\]\Z", param):
+            self._args.append((ARGS_REPLACE, param))
             return False
 
         # default parameters
         for arg in ALL_ARGS:
             if param in (arg.short_form, arg.long_form):
-                self.args.append((arg.arg_id, param))
+                self._args.append((arg.arg_id, param))
                 if arg.arg_id == ARGS_ECHO:
                     return True
                 return False
 
         possible_path = realpath(param)
         if match(r".*\*+.*", param):
             for filename in iglob(param, recursive=True):
                 if isfile(filename):
-                    self.known_files.append(realpath(filename))
+                    self._known_files.append(realpath(filename))
         elif isdir(possible_path):
             for filename in iglob(possible_path + '**/**', recursive=True):
                 if isfile(filename):
-                    self.known_files.append(realpath(filename))
+                    self._known_files.append(realpath(filename))
         elif isfile(possible_path):
-            self.known_files.append(possible_path)
+            self._known_files.append(possible_path)
         elif len(param) > 2 and param[0] == '-' and param[1] != '-':
             for i in range(1, len(param)):
                 if self._add_argument('-' + param[i], delete):
                     return True
-        elif match(r"\A[^-]+.*\Z", param):
-            self.unknown_files.append(realpath(param))
+        elif match(r"\A[^-].*\Z", param):
+            self._unknown_files.append(realpath(param))
         else:
-            self.unknown_args.append(param)
+            self._unknown_args.append(param)
         return False
 
 
     def gen_arguments(self, argv: list, delete: bool = False) -> None:
         """
         Read all args to either a valid parameter, an invalid parameter,
         a known file, an unknown file, or an echo parameter to print out.
@@ -133,20 +140,20 @@
             the shell when changing file_search, file_match
         
         Returns:
         (args, unknown_args, known_files, unknown_files, echo_args) (tuple):
             contains the paramater in a sorted manner
         """
         input_args = argv[1:]
-        self.args = []
-        self.unknown_args = []
-        self.known_files = []
-        self.unknown_files = []
-        self.echo_args = []
+        self._args = []
+        self._unknown_args = []
+        self._known_files = []
+        self._unknown_files = []
+        self._echo_args = []
 
         echo_call = False
 
         for arg in input_args:
             if echo_call:
-                self.echo_args.append(arg)
+                self._echo_args.append(arg)
                 continue
             echo_call = self._add_argument(arg, delete)
```

### Comparing `cat_win-1.4.2/cat_win/util/cbase64.py` & `cat_win-1.4.3/cat_win/util/cbase64.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/cat_win/util/checksum.py` & `cat_win-1.4.3/cat_win/util/checksum.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/cat_win/util/fileattributes.py` & `cat_win-1.4.3/cat_win/util/fileattributes.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/cat_win/util/holder.py` & `cat_win-1.4.3/cat_win/util/holder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,77 @@
 from functools import lru_cache
 from heapq import nlargest
 
 from cat_win.const.argconstants import HIGHEST_ARG_ID, ARGS_NOCOL, ARGS_LLENGTH, ARGS_NUMBER, \
-    ARGS_REVERSE, ARGS_B64D, ARGS_B64E, ARGS_COUNT, ARGS_CCOUNT
+    ARGS_REVERSE, ARGS_B64D, ARGS_B64E, ARGS_COUNT, ARGS_CCOUNT, DIFFERENTIABLE_ARGS
 from cat_win.util.cbase64 import _decode_base64
 from cat_win.util.file import File
 
 
 def reduce_list(args: list) -> list:
     """
     remove duplicate args regardless if shortform or
-    longform has been used.
+    longform has been used, an exception exists for those
+    args that contain different information per parameter.
     
     Parameters:
     args (list):
         the entire list of args, containing possible duplicates
         
     Returns:
     new_args (list):
         the args-list without duplicates
     """
     new_args = []
     temp_args_id = []
-    
+
     for arg in args:
         id, _ = arg
-        if id not in temp_args_id:
+        # it can make sense to have the exact same parameter twice, even if it does
+        # the same information, therefor we do not test for the param here.
+        if id in DIFFERENTIABLE_ARGS:
+            new_args.append(arg)
+        elif id not in temp_args_id:
             temp_args_id.append(id)
             new_args.append(arg)
+
     return new_args
 
+def diff_list(args: list, to_remove: list) -> list:
+    """
+    subtract args in to_remove from args in args regardless
+    if shortform or longform has been used, an exception exists for those
+    args that contain different information per parameter.
+    
+    Parameters:
+    args (list):
+        the entire list of args
+    to_remove (list):
+        the list of args to subtract from the args list
+        
+    Returns:
+    new_args (list):
+        the args-list without duplicates
+    """
+    new_args = []
+    temp_args_id = [id for id, _ in to_remove]
+    temp_args = [arg for arg in to_remove if arg[0] in DIFFERENTIABLE_ARGS]
+
+    for arg in args:
+        id, _ = arg
+        if id not in temp_args_id or id in DIFFERENTIABLE_ARGS:
+            new_args.append(arg)
+
+    for arg in temp_args:
+        try:
+            new_args.remove(arg)
+        except ValueError:
+            pass
+
+    return new_args
 
 class Holder():
     def __init__(self) -> None:
         self.files: list = []  # all files, including tmp-file from stdin
         self._inner_files: list = []
         self.args: list = []  # list of all used parameters: format [[id, param]]
         self.args_id: list = [False] * (HIGHEST_ARG_ID + 1)
@@ -91,15 +129,15 @@
 
     def add_args(self, args: list) -> None:
         self.args_id = [False] * (HIGHEST_ARG_ID + 1)
         self.set_args(self.args + args)
 
     def delete_args(self, args: list) -> None:
         self.args_id = [False] * (HIGHEST_ARG_ID + 1)
-        self.set_args([arg for arg in self.args if arg not in args])
+        self.set_args(diff_list(self.args, args))
 
     def set_temp_file_stdin(self, file: str) -> None:
         self.temp_file_stdin = file
 
     def set_temp_file_echo(self, file: str) -> None:
         self.temp_file_echo = file
```

### Comparing `cat_win-1.4.2/cat_win/util/rawviewer.py` & `cat_win-1.4.3/cat_win/util/rawviewer.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/cat_win/util/stdinhelper.py` & `cat_win-1.4.3/cat_win/util/stdinhelper.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/cat_win/util/stringfinder.py` & `cat_win-1.4.3/cat_win/util/stringfinder.py`

 * *Files 13% similar despite different names*

```diff
@@ -105,14 +105,18 @@
         matched_list = []
         matched_position = []
 
         for keyword in self.kw_literals:
             for _f in self._findliterals(keyword, line):
                 found_position.append(_f[:])
                 found_list.append((keyword, _f))
-
+        # sort by start position (necessary for a deterministic output)
+        found_list.sort(key = lambda x: x[1][0])
+        
         for keyword in self.kw_regex:
             for _m in self._findregex(keyword, line):
                 matched_position.append(_m[:])
                 matched_list.append((keyword, _m))
+        # sort by start position (necessary for a deterministic output)
+        matched_list.sort(key = lambda x: x[1][0])
 
         return (self._merge_keyword_intervals(found_position, matched_position), found_list, matched_list)
```

### Comparing `cat_win-1.4.2/cat_win/web/updatechecker.py` & `cat_win-1.4.3/cat_win/web/updatechecker.py`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/pyproject.toml` & `cat_win-1.4.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cat_win-1.4.2/PKG-INFO` & `cat_win-1.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cat_win
-Version: 1.4.2
+Version: 1.4.3
 Summary: Simple OS Independent 'cat' Command-line Tool made in Python.
 Keywords: cat,cli,console,crossplatform,python,terminal
 Author-email: "Silas A. Kraume" <silas.kraume1552@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -97,15 +97,15 @@
 [![Tests]](https://raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-tests.svg)
 <!-- [![Compile-and-Push]](https://github.com/SilenZcience/cat_win/actions/workflows/build_executable.yml/badge.svg) -->
 
 This project copies the fundamental framework of the cat command-line tool from Linux and translates its features to an OS Independent program using Python. </br> Over time the project evolved in subject areas of other tools like 'echo', 'grep', 'ls', 'base64'.
 
 Additionally it includes the feature to strip and reverse the content of any given file, make use of the standard-input, which enables cat piping into each other, generating the checksum of any file, converting decimal, hexadecimal and binary numbers within any text, and much <a href="#usage">more</a> ...
 
-Contrary to the name of the project it is of course possible to use cat_win on Linux or MacOS!
+It is of course possible to use cat_win on Linux or MacOS, aswell as Windows!
 
 ### Made With
 [![MadeWith-Python]](https://www.python.org/)
 [![Python][Python-Version]](https://www.python.org/)
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
@@ -167,30 +167,33 @@
 | *-l, --linelength*     | display the length of each line                           | ✔              |
 | *-e, --ends*           | display $ at the end of each line                         | ✔              |
 | *-t, --tabs*           | display TAB characters as ^I                              | ✔              |
 | *--eof, --eof*         | display EOF characters as ^EOF                            | ✔              |
 | *-u, --unique*         | suppress repeated output lines                            | ❌             |
 | *-b, --blank*          | hide empty lines                                          | ✔              |
 | *-r, --reverse*        | reverse output                                            | ❌             |
+| *--sort, --sort*       | sort all lines alphabetically                             | ❌             |
 | *-p, --peek*           | only print the first and last lines                       | ❌             |
 | *-s, --sum*            | show sum of lines                                         | ❌             |
 | *-S, --SUM*            | ONLY show sum of lines                                    | ❌             |
 | *-f, --files*          | list applied files                                        | ❌             |
 | *-F, --FILES*          | ONLY list applied files and file sizes                    | ❌             |
-| *-g, --grep*           | only show lines containing queried keywords               | ✔              |
+| *-g, --grep*           | only show lines containing queried keywords or patterns   | ✔              |
+| *-G, --GREP*           | only show found and matched substrings                    | ✔              |
 | *-i, --interactive*    | use stdin                                                 | ❌             |
-| *-o, --oneline*        | take only the first stdin-line                            | ❌             |
+| *-o, --oneline*        | take only the first stdin-line                            | ✔              |
 | *-E, --ECHO*           | handle every following parameter as stdin                 | ❌             |
 | *-c, --clip*           | copy output to clipboard                                  | ✔              |
 | *-m, --checksum*       | show the checksums of all files                           | ❌             |
 | *-a, --attributes*     | show meta-information about the files                     | ❌             |
 |                        |                                                           |                |
 | *--dec, --DEC*         | convert decimal numbers to hexadecimal and binary         | ✔              |
 | *--hex, --HEX*         | convert hexadecimal numbers to decimal and binary         | ✔              |
 | *--bin, --BIN*         | convert binary numbers to decimal and hexadecimal         | ✔              |
+| *--eval, --EVAL*       | evaluate simple mathematical equations                    | ✔              |
 | *--b64e, --b64e*       | encode the input to base64                                | ✔              |
 | *--b64d, --b64d*       | decode the input from base64                              | ✔              |
 |                        |                                                           |                |
 | *--hexview, --HEXVIEW* | display the raw byte representation in hexadecimal        | ❌             |
 | *--binview, --binview* | display the raw byte representation in binary             | ❌             |
 |                        |                                                           |                |
 | *--nc, --nocolor*      | disable colored output                                    | ✔              |
@@ -201,15 +204,15 @@
 | *-R, --R\<stream\>*    | reconfigure the std-stream(s) with the parsed encoding </br> \<stream\> = 'in'/'out'/'err' (default is stdin & stdout)| ✔ |
 |                        |                                                           |                |
 | *enc=X*                | set file enconding to X (default is utf-8)                | ✔              |
 | *find=X*               | find/query a substring X in the given files               | ✔              |
 | *match=X*              | find/query a pattern X in the given files                 | ✔              |
 | *trunc=X:Y*            | truncate file to lines X and Y (python-like)              | ❌             |
 |                        |                                                           |                |
-| *[a,b]*                | replace a with b in every line                            | ✔              |
+| *[a,b]*                | replace a with b in every line (escape chars with '\\')   | ✔              |
 | *[a:​b:c]*              | python-like string indexing syntax (line by line)         | ✔              |
 
 ### Examples
 
 <details open>
 	<summary><b>📂 Images 📂</b></summary>
 
@@ -233,25 +236,25 @@
    <p float="left">
       <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example7.png" width="49%"/>
       <img src="https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example8.png" width="49%"/>
    </p>
 
 </details>
 
-```c
+```py
 $ echo "Hello World :)" | catw -i [6:] | catw -i [::-1] -ln
 > 1) [8] ): dlroW
 ```
 
 - - - -
 
-```c
-$ cats --dec -nl
-> >>> 12345
-> 1) [53] 12345 {Hexadecimal: 0x3039; Binary: 0b11000000111001}
+```py
+$ cats --eval --dec -nl
+> >>> 0xF * 5
+> 1) [41] 75 {Hexadecimal: 0x4b; Binary: 0b1001011}
 > >>> ...
 ```
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Changelog
 
@@ -262,17 +265,17 @@
 This project is licensed under the MIT License - see the [LICENSE](https://github.com/SilenZcience/cat_win/blob/main/LICENSE) file for details
 
 ## Contact
 
 > **SilenZcience** <br/>
 [![GitHub-SilenZcience][GitHub-SilenZcience]](https://github.com/SilenZcience)
 
-[OS-Windows]: https://svgshare.com/i/ZhY.svg
-[OS-Linux]: https://svgshare.com/i/Zhy.svg
-[OS-MacOS]: https://svgshare.com/i/ZjP.svg
+[OS-Windows]: https://img.shields.io/badge/os-windows-green
+[OS-Linux]: https://img.shields.io/badge/os-linux-green
+[OS-MacOS]: https://img.shields.io/badge/os-macOS-green
 
 [Unittests]: https://github.com/SilenZcience/cat_win/actions/workflows/unit_test.yml/badge.svg
 [Build-and-Check]: https://github.com/SilenZcience/cat_win/actions/workflows/package_test.yml/badge.svg
 [Compile-and-Push]: https://github.com/SilenZcience/cat_win/actions/workflows/build_executable.yml/badge.svg
 
 [Coverage]: https://raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-coverage.svg
 [Tests]: https://raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-tests.svg
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cat_win Version: 1.4.2 Summary: Simple OS
+Metadata-Version: 2.1 Name: cat_win Version: 1.4.3 Summary: Simple OS
 Independent 'cat' Command-line Tool made in Python. Keywords:
 cat,cli,console,crossplatform,python,terminal Author-email: "Silas A. Kraume"
 kraume1552@gmail.com> Requires-Python: >=3.7 Description-Content-Type: text/
 markdown Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
@@ -45,18 +45,18 @@
 cat_win/badges/.github/badges/badge-tests.svg)  This project copies the
 fundamental framework of the cat command-line tool from Linux and translates
 its features to an OS Independent program using Python.  Over time the project
 evolved in subject areas of other tools like 'echo', 'grep', 'ls', 'base64'.
 Additionally it includes the feature to strip and reverse the content of any
 given file, make use of the standard-input, which enables cat piping into each
 other, generating the checksum of any file, converting decimal, hexadecimal and
-binary numbers within any text, and much more ... Contrary to the name of the
-project it is of course possible to use cat_win on Linux or MacOS! ### Made
-With [![MadeWith-Python]](https://www.python.org/) [![Python][Python-Version]]
-(https://www.python.org/)
+binary numbers within any text, and much more ... It is of course possible to
+use cat_win on Linux or MacOS, aswell as Windows! ### Made With [![MadeWith-
+Python]](https://www.python.org/) [![Python][Python-Version]](https://
+www.python.org/)
                                                                   (back_to_top)
 ## Getting Started ### Prerequisites - Using cat_win as a Python-Package
 demands a Python-Interpreter (>= 3.7). - Using cat_win as an Executable
 (Windows only!) demands no prerequisites, hereby the stand-alone executables
 `catw.exe` (& `cats.exe`) are sufficient. ### Installation [![Version]
 [CurrentVersion]](https://pypi.org/project/cat-win/) Simply install the python
 package (via [PyPI-cat_win](https://pypi.org/project/cat-win/)): ```console
@@ -89,68 +89,71 @@
 â | | *-v, --version* | output version information | â | | *--debug, --
 debug* | show debug information | â | | | | | | *-n, --number* | number all
 output lines | â | | *-l, --linelength* | display the length of each line |
 â | | *-e, --ends* | display $ at the end of each line | â | | *-t, --tabs*
 | display TAB characters as ^I | â | | *--eof, --eof* | display EOF
 characters as ^EOF | â | | *-u, --unique* | suppress repeated output lines |
 â | | *-b, --blank* | hide empty lines | â | | *-r, --reverse* | reverse
-output | â | | *-p, --peek* | only print the first and last lines | â | |
-*-s, --sum* | show sum of lines | â | | *-S, --SUM* | ONLY show sum of lines
-| â | | *-f, --files* | list applied files | â | | *-F, --FILES* | ONLY
-list applied files and file sizes | â | | *-g, --grep* | only show lines
-containing queried keywords | â | | *-i, --interactive* | use stdin | â | |
-*-o, --oneline* | take only the first stdin-line | â | | *-E, --ECHO* |
-handle every following parameter as stdin | â | | *-c, --clip* | copy output
-to clipboard | â | | *-m, --checksum* | show the checksums of all files | â
-| | *-a, --attributes* | show meta-information about the files | â | | | | |
-| *--dec, --DEC* | convert decimal numbers to hexadecimal and binary | â | |
-*--hex, --HEX* | convert hexadecimal numbers to decimal and binary | â | | *-
--bin, --BIN* | convert binary numbers to decimal and hexadecimal | â | | *--
-b64e, --b64e* | encode the input to base64 | â | | *--b64d, --b64d* | decode
-the input from base64 | â | | | | | | *--hexview, --HEXVIEW* | display the
-raw byte representation in hexadecimal | â | | *--binview, --binview* |
-display the raw byte representation in binary | â | | | | | | *--nc, --
-nocolor* | disable colored output | â | | *--nb, --nobreak* | do not
-interrupt the output on queried keywords | â | | *--nk, --nokeyword* |
-inverse the grep output | â | | *--config, --config* | change color
-configuration | â | | | | | | *-R, --R\
+output | â | | *--sort, --sort* | sort all lines alphabetically | â | | *-
+p, --peek* | only print the first and last lines | â | | *-s, --sum* | show
+sum of lines | â | | *-S, --SUM* | ONLY show sum of lines | â | | *-f, --
+files* | list applied files | â | | *-F, --FILES* | ONLY list applied files
+and file sizes | â | | *-g, --grep* | only show lines containing queried
+keywords or patterns | â | | *-G, --GREP* | only show found and matched
+substrings | â | | *-i, --interactive* | use stdin | â | | *-o, --oneline*
+| take only the first stdin-line | â | | *-E, --ECHO* | handle every
+following parameter as stdin | â | | *-c, --clip* | copy output to clipboard
+| â | | *-m, --checksum* | show the checksums of all files | â | | *-a, --
+attributes* | show meta-information about the files | â | | | | | | *--dec, -
+-DEC* | convert decimal numbers to hexadecimal and binary | â | | *--hex, --
+HEX* | convert hexadecimal numbers to decimal and binary | â | | *--bin, --
+BIN* | convert binary numbers to decimal and hexadecimal | â | | *--eval, --
+EVAL* | evaluate simple mathematical equations | â | | *--b64e, --b64e* |
+encode the input to base64 | â | | *--b64d, --b64d* | decode the input from
+base64 | â | | | | | | *--hexview, --HEXVIEW* | display the raw byte
+representation in hexadecimal | â | | *--binview, --binview* | display the
+raw byte representation in binary | â | | | | | | *--nc, --nocolor* | disable
+colored output | â | | *--nb, --nobreak* | do not interrupt the output on
+queried keywords | â | | *--nk, --nokeyword* | inverse the grep output | â
+| | *--config, --config* | change color configuration | â | | | | | | *-R, --
+R\
 >* | reconfigure the std-stream(s) with the parsed encoding  \
 > = 'in'/'out'/'err' (default is stdin & stdout)| â | | | | | | *enc=X* | set
 file enconding to X (default is utf-8) | â | | *find=X* | find/query a
 substring X in the given files | â | | *match=X* | find/query a pattern X in
 the given files | â | | *trunc=X:Y* | truncate file to lines X and Y (python-
-like) | â | | | | | | *[a,b]* | replace a with b in every line | â | | *[a:
-âb:c]* | python-like string indexing syntax (line by line) | â | ###
-Examples  ð Images ð
+like) | â | | | | | | *[a,b]* | replace a with b in every line (escape chars
+with '\\') | â | | *[a:âb:c]* | python-like string indexing syntax (line by
+line) | â | ### Examples  ð Images ð
 [https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example1.png]
 [https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example2.png]
 [https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example3.png]
 [https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example4.png]
 [https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example5.png]
 [https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example6.png]
 - - - -
 [https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example7.png]
 [https://raw.githubusercontent.com/SilenZcience/cat_win/main/img/example8.png]
- ```c $ echo "Hello World :)" | catw -i [6:] | catw -i [::-1] -ln > 1) [8] ):
-dlroW ``` - - - - ```c $ cats --dec -nl > >>> 12345 > 1) [53] 12345
-{Hexadecimal: 0x3039; Binary: 0b11000000111001} > >>> ... ```
+ ```py $ echo "Hello World :)" | catw -i [6:] | catw -i [::-1] -ln > 1) [8] ):
+dlroW ``` - - - - ```py $ cats --eval --dec -nl > >>> 0xF * 5 > 1) [41] 75
+{Hexadecimal: 0x4b; Binary: 0b1001011} > >>> ... ```
                                                                   (back_to_top)
 ## Changelog Take a look at the [Changelog](https://github.com/SilenZcience/
 cat_win/blob/main/CHANGELOG.md) file. ## License This project is licensed under
 the MIT License - see the [LICENSE](https://github.com/SilenZcience/cat_win/
 blob/main/LICENSE) file for details ## Contact > **SilenZcience**
 [![GitHub-SilenZcience][GitHub-SilenZcience]](https://github.com/SilenZcience)
-[OS-Windows]: https://svgshare.com/i/ZhY.svg [OS-Linux]: https://svgshare.com/
-i/Zhy.svg [OS-MacOS]: https://svgshare.com/i/ZjP.svg [Unittests]: https://
-github.com/SilenZcience/cat_win/actions/workflows/unit_test.yml/badge.svg
-[Build-and-Check]: https://github.com/SilenZcience/cat_win/actions/workflows/
-package_test.yml/badge.svg [Compile-and-Push]: https://github.com/SilenZcience/
-cat_win/actions/workflows/build_executable.yml/badge.svg [Coverage]: https://
+[OS-Windows]: https://img.shields.io/badge/os-windows-green [OS-Linux]: https:/
+/img.shields.io/badge/os-linux-green [OS-MacOS]: https://img.shields.io/badge/
+os-macOS-green [Unittests]: https://github.com/SilenZcience/cat_win/actions/
+workflows/unit_test.yml/badge.svg [Build-and-Check]: https://github.com/
+SilenZcience/cat_win/actions/workflows/package_test.yml/badge.svg [Compile-and-
+Push]: https://github.com/SilenZcience/cat_win/actions/workflows/
+build_executable.yml/badge.svg [Coverage]: https://raw.githubusercontent.com/
+SilenZcience/cat_win/badges/.github/badges/badge-coverage.svg [Tests]: https://
 raw.githubusercontent.com/SilenZcience/cat_win/badges/.github/badges/badge-
-coverage.svg [Tests]: https://raw.githubusercontent.com/SilenZcience/cat_win/
-badges/.github/badges/badge-tests.svg [MadeWith-Python]: https://
-img.shields.io/badge/Made%20with-Python-brightgreen [Python-Version]: https://
-img.shields.io/badge/Python-
+tests.svg [MadeWith-Python]: https://img.shields.io/badge/Made%20with-Python-
+brightgreen [Python-Version]: https://img.shields.io/badge/Python-
 3.7%20%7C%203.8%20%7C%203.9%20%7C%203.10%20%7C%203.11%20%7C%20pypy--
 3.8%20%7C%20pypy--3.9-blue [CurrentVersion]: https://img.shields.io/pypi/v/
 cat_win.svg [GitHub-SilenZcience]: https://img.shields.io/badge/GitHub-
 SilenZcience-orange
```

