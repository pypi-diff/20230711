# Comparing `tmp/python-lemming-0.5.1.tar.gz` & `tmp/python-lemming-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-lemming-0.5.1.tar", last modified: Fri Jun 23 13:15:56 2023, max compression
+gzip compressed data, was "python-lemming-0.6.0.tar", last modified: Tue Jul 11 13:00:24 2023, max compression
```

## Comparing `python-lemming-0.5.1.tar` & `python-lemming-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-23 13:15:56.623979 python-lemming-0.5.1/
--rw-rw-rw-   0        0        0    33094 2022-11-26 12:00:55.000000 python-lemming-0.5.1/LICENSE
--rw-rw-rw-   0        0        0     6305 2023-06-23 13:15:56.624979 python-lemming-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     5341 2023-06-11 12:10:56.000000 python-lemming-0.5.1/README.md
--rw-rw-rw-   0        0        0     1625 2023-06-12 17:12:49.000000 python-lemming-0.5.1/pyproject.toml
--rw-rw-rw-   0        0        0     1456 2023-06-23 13:15:56.629979 python-lemming-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0       94 2022-12-17 14:25:46.000000 python-lemming-0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-23 13:15:56.575980 python-lemming-0.5.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-23 13:15:56.602980 python-lemming-0.5.1/src/lemming/
--rw-rw-rw-   0        0        0      922 2023-06-23 12:58:00.000000 python-lemming-0.5.1/src/lemming/__init__.py
--rw-rw-rw-   0        0        0     9713 2023-06-23 12:58:11.000000 python-lemming-0.5.1/src/lemming/__main__.py
--rw-rw-rw-   0        0        0    11284 2023-06-23 13:00:24.000000 python-lemming-0.5.1/src/lemming/config.py
--rw-rw-rw-   0        0        0        0 2022-11-26 11:55:00.000000 python-lemming-0.5.1/src/lemming/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-23 13:15:56.622979 python-lemming-0.5.1/src/python_lemming.egg-info/
--rw-rw-rw-   0        0        0     6305 2023-06-23 13:15:56.000000 python-lemming-0.5.1/src/python_lemming.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      437 2023-06-23 13:15:56.000000 python-lemming-0.5.1/src/python_lemming.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-23 13:15:56.000000 python-lemming-0.5.1/src/python_lemming.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-23 13:15:56.000000 python-lemming-0.5.1/src/python_lemming.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-12-17 14:43:45.000000 python-lemming-0.5.1/src/python_lemming.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       91 2023-06-23 13:15:56.000000 python-lemming-0.5.1/src/python_lemming.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-23 13:15:56.000000 python-lemming-0.5.1/src/python_lemming.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 13:00:24.747348 python-lemming-0.6.0/
+-rw-rw-rw-   0        0        0    33094 2022-11-26 12:00:55.000000 python-lemming-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0    15930 2023-07-11 13:00:24.747348 python-lemming-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0    14865 2023-07-11 12:59:00.000000 python-lemming-0.6.0/README.md
+-rw-rw-rw-   0        0        0     1633 2023-07-11 12:59:00.000000 python-lemming-0.6.0/pyproject.toml
+-rw-rw-rw-   0        0        0     1550 2023-07-11 13:00:24.758347 python-lemming-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0       94 2022-12-17 14:25:46.000000 python-lemming-0.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 13:00:24.686347 python-lemming-0.6.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 13:00:24.704349 python-lemming-0.6.0/src/lemming/
+-rw-rw-rw-   0        0        0      922 2023-07-11 12:59:29.000000 python-lemming-0.6.0/src/lemming/__init__.py
+-rw-rw-rw-   0        0        0    17696 2023-07-11 12:59:00.000000 python-lemming-0.6.0/src/lemming/__main__.py
+-rw-rw-rw-   0        0        0    13842 2023-07-11 12:59:00.000000 python-lemming-0.6.0/src/lemming/config.py
+-rw-rw-rw-   0        0        0        0 2022-11-26 11:55:00.000000 python-lemming-0.6.0/src/lemming/py.typed
+drwxrwxrwx   0        0        0        0 2023-07-11 13:00:24.745348 python-lemming-0.6.0/src/python_lemming.egg-info/
+-rw-rw-rw-   0        0        0    15930 2023-07-11 13:00:24.000000 python-lemming-0.6.0/src/python_lemming.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2023-07-11 13:00:24.000000 python-lemming-0.6.0/src/python_lemming.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 13:00:24.000000 python-lemming-0.6.0/src/python_lemming.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-07-11 13:00:24.000000 python-lemming-0.6.0/src/python_lemming.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-12-17 14:43:45.000000 python-lemming-0.6.0/src/python_lemming.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      106 2023-07-11 13:00:24.000000 python-lemming-0.6.0/src/python_lemming.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-11 13:00:24.000000 python-lemming-0.6.0/src/python_lemming.egg-info/top_level.txt
```

### Comparing `python-lemming-0.5.1/LICENSE` & `python-lemming-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-lemming-0.5.1/pyproject.toml` & `python-lemming-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 profile = "black"
 
 [tool.ruff]
 select = ["ALL"]
 ignore = [
     "ANN101",
     "ANN102",
+    "ANN401",
     "COM",
     "D",
     "EM102",
     "FBT",
     "T",
     "TRY003",
     "PLR0913",
@@ -64,19 +65,18 @@
 
 [[tool.lemming.formatters]]
 packages = ["setup_cfg_fmt"]
 format_command = "{pyexe} -m setup_cfg_fmt --include-version-classifiers"
 # no check
 
 [[tool.lemming.formatters]]
-packages = ["isort"]
-format_command = "{pyexe} -m isort --profile black {path}"
-check_command = "{pyexe} -m isort --profile black -c {path}"
-
-[[tool.lemming.formatters]]
 packages = ["ruff"]
-format_command = "{pyexe} -m ruff check . --show-source --fix -n"
-check_command = "{pyexe} -m ruff check . --show-source --show-fixes -n"
+format_command = "{pyexe} -m ruff check --show-source --fix -n {path}"
+check_command = "{pyexe} -m ruff check --show-source --show-fixes -n {path}"
 
 [[tool.lemming.linters]]
 packages = ["pyroma"]
 command = "{pyexe} -m pyroma {path}"
+
+[[tool.lemming.linters]]
+packages = ["vermin"]
+command = "vermin --target=3.7 --eval-annotations --backport typing --backport typing_extensions -vv src"
```

### Comparing `python-lemming-0.5.1/setup.cfg` & `python-lemming-0.6.0/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -34,58 +34,64 @@
 00000210: 610d 0a09 5072 6f67 7261 6d6d 696e 6720  a...Programming 
 00000220: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
 00000230: 6f6e 203a 3a20 330d 0a09 5072 6f67 7261  on :: 3...Progra
 00000240: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
 00000250: 3a20 5079 7468 6f6e 203a 3a20 3320 3a3a  : Python :: 3 ::
 00000260: 204f 6e6c 790d 0a09 5072 6f67 7261 6d6d   Only...Programm
 00000270: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-00000280: 5079 7468 6f6e 203a 3a20 332e 380d 0a09  Python :: 3.8...
+00000280: 5079 7468 6f6e 203a 3a20 332e 360d 0a09  Python :: 3.6...
 00000290: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
 000002a0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000002b0: 3a20 332e 390d 0a09 5072 6f67 7261 6d6d  : 3.9...Programm
+000002b0: 3a20 332e 370d 0a09 5072 6f67 7261 6d6d  : 3.7...Programm
 000002c0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
-000002d0: 5079 7468 6f6e 203a 3a20 332e 3130 0d0a  Python :: 3.10..
-000002e0: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-000002f0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
-00000300: 3a3a 2033 2e31 310d 0a09 5072 6f67 7261  :: 3.11...Progra
-00000310: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-00000320: 3a20 5079 7468 6f6e 203a 3a20 332e 3132  : Python :: 3.12
-00000330: 0d0a 6b65 7977 6f72 6473 203d 206c 656d  ..keywords = lem
-00000340: 6d69 6e67 2c20 666f 726d 6174 2c20 666f  ming, format, fo
-00000350: 726d 6174 7465 722c 206c 696e 742c 206c  rmatter, lint, l
-00000360: 696e 7469 6e67 2c20 6c69 6e74 6572 0d0a  inting, linter..
-00000370: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 6163  ..[options]..pac
-00000380: 6b61 6765 7320 3d20 0d0a 096c 656d 6d69  kages = ...lemmi
-00000390: 6e67 0d0a 696e 7374 616c 6c5f 7265 7175  ng..install_requ
-000003a0: 6972 6573 203d 200d 0a09 746f 6d6c 693b  ires = ...tomli;
-000003b0: 2070 7974 686f 6e5f 7665 7273 696f 6e3c   python_version<
-000003c0: 2733 2e31 3127 0d0a 0970 7974 686f 6e2d  '3.11'...python-
-000003d0: 6d79 6c6f 673e 3d30 2e37 2e30 0d0a 0963  mylog>=0.7.0...c
-000003e0: 6f6e 667a 0d0a 0974 7970 696e 672d 6578  onfz...typing-ex
-000003f0: 7465 6e73 696f 6e73 3e3d 342e 342e 300d  tensions>=4.4.0.
-00000400: 0a09 7479 7065 720d 0a70 7974 686f 6e5f  ..typer..python_
-00000410: 7265 7175 6972 6573 203d 203e 3d33 2e31  requires = >=3.1
-00000420: 310d 0a70 6163 6b61 6765 5f64 6972 203d  1..package_dir =
-00000430: 200d 0a09 3d73 7263 0d0a 7a69 705f 7361   ...=src..zip_sa
-00000440: 6665 203d 206e 6f0d 0a0d 0a5b 6f70 7469  fe = no....[opti
-00000450: 6f6e 732e 7061 636b 6167 655f 6461 7461  ons.package_data
-00000460: 5d0d 0a6c 656d 6d69 6e67 203d 2070 792e  ]..lemming = py.
-00000470: 7479 7065 640d 0a0d 0a5b 6f70 7469 6f6e  typed....[option
-00000480: 732e 656e 7472 795f 706f 696e 7473 5d0d  s.entry_points].
-00000490: 0a63 6f6e 736f 6c65 5f73 6372 6970 7473  .console_scripts
-000004a0: 203d 200d 0a09 6c65 6d6d 696e 6720 3d20   = ...lemming = 
-000004b0: 6c65 6d6d 696e 672e 5f5f 6d61 696e 5f5f  lemming.__main__
-000004c0: 3a6d 6169 6e0d 0a0d 0a5b 7079 636f 6465  :main....[pycode
-000004d0: 7374 796c 655d 0d0a 6967 6e6f 7265 203d  style]..ignore =
-000004e0: 2045 3230 330d 0a0d 0a5b 7079 6c61 6d61   E203....[pylama
-000004f0: 5d0d 0a69 676e 6f72 6520 3d20 5735 3033  ]..ignore = W503
-00000500: 0d0a 0d0a 5b66 6c61 6b65 385d 0d0a 6578  ....[flake8]..ex
-00000510: 7465 6e64 2d69 676e 6f72 6520 3d20 5735  tend-ignore = W5
-00000520: 3033 0d0a 6578 7465 6e64 2d65 7863 6c75  03..extend-exclu
-00000530: 6465 203d 2076 656e 762c 2a63 6163 6865  de = venv,*cache
-00000540: 2a0d 0a70 6572 2d66 696c 652d 6967 6e6f  *..per-file-igno
-00000550: 7265 7320 3d20 0d0a 0974 6573 7473 2f2a  res = ...tests/*
-00000560: 3a20 5331 3031 0d0a 0d0a 5b69 736f 7274  : S101....[isort
-00000570: 5d0d 0a70 726f 6669 6c65 203d 2062 6c61  ]..profile = bla
-00000580: 636b 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d  ck....[egg_info]
-00000590: 0d0a 7461 675f 6275 696c 6420 3d20 0d0a  ..tag_build = ..
-000005a0: 7461 675f 6461 7465 203d 2030 0d0a 0d0a  tag_date = 0....
+000002d0: 5079 7468 6f6e 203a 3a20 332e 380d 0a09  Python :: 3.8...
+000002e0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+000002f0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000300: 3a20 332e 390d 0a09 5072 6f67 7261 6d6d  : 3.9...Programm
+00000310: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000320: 5079 7468 6f6e 203a 3a20 332e 3130 0d0a  Python :: 3.10..
+00000330: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+00000340: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+00000350: 3a3a 2033 2e31 310d 0a09 5072 6f67 7261  :: 3.11...Progra
+00000360: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
+00000370: 3a20 5079 7468 6f6e 203a 3a20 332e 3132  : Python :: 3.12
+00000380: 0d0a 6b65 7977 6f72 6473 203d 206c 656d  ..keywords = lem
+00000390: 6d69 6e67 2c20 666f 726d 6174 2c20 666f  ming, format, fo
+000003a0: 726d 6174 7465 722c 206c 696e 742c 206c  rmatter, lint, l
+000003b0: 696e 7469 6e67 2c20 6c69 6e74 6572 0d0a  inting, linter..
+000003c0: 0d0a 5b6f 7074 696f 6e73 5d0d 0a70 6163  ..[options]..pac
+000003d0: 6b61 6765 7320 3d20 0d0a 096c 656d 6d69  kages = ...lemmi
+000003e0: 6e67 0d0a 696e 7374 616c 6c5f 7265 7175  ng..install_requ
+000003f0: 6972 6573 203d 200d 0a09 746f 6d6c 693b  ires = ...tomli;
+00000400: 2070 7974 686f 6e5f 7665 7273 696f 6e3c   python_version<
+00000410: 2733 2e31 3127 0d0a 0970 7974 686f 6e2d  '3.11'...python-
+00000420: 6d79 6c6f 673e 3d30 2e38 2e30 2d62 6574  mylog>=0.8.0-bet
+00000430: 612e 320d 0a09 7479 7069 6e67 2d65 7874  a.2...typing-ext
+00000440: 656e 7369 6f6e 733e 3d34 2e34 2e30 0d0a  ensions>=4.4.0..
+00000450: 0974 7970 6572 0d0a 0970 7964 616e 7469  .typer...pydanti
+00000460: 633e 3d31 2e35 0d0a 7079 7468 6f6e 5f72  c>=1.5..python_r
+00000470: 6571 7569 7265 7320 3d20 3e3d 332e 370d  equires = >=3.7.
+00000480: 0a70 6163 6b61 6765 5f64 6972 203d 200d  .package_dir = .
+00000490: 0a09 3d73 7263 0d0a 7a69 705f 7361 6665  ..=src..zip_safe
+000004a0: 203d 206e 6f0d 0a0d 0a5b 6f70 7469 6f6e   = no....[option
+000004b0: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
+000004c0: 0a6c 656d 6d69 6e67 203d 2070 792e 7479  .lemming = py.ty
+000004d0: 7065 640d 0a0d 0a5b 6f70 7469 6f6e 732e  ped....[options.
+000004e0: 656e 7472 795f 706f 696e 7473 5d0d 0a63  entry_points]..c
+000004f0: 6f6e 736f 6c65 5f73 6372 6970 7473 203d  onsole_scripts =
+00000500: 200d 0a09 6c65 6d6d 696e 6720 3d20 6c65   ...lemming = le
+00000510: 6d6d 696e 672e 5f5f 6d61 696e 5f5f 3a6d  mming.__main__:m
+00000520: 6169 6e0d 0a0d 0a5b 7079 636f 6465 7374  ain....[pycodest
+00000530: 796c 655d 0d0a 6967 6e6f 7265 203d 2045  yle]..ignore = E
+00000540: 3230 330d 0a0d 0a5b 7079 6c61 6d61 5d0d  203....[pylama].
+00000550: 0a69 676e 6f72 6520 3d20 5735 3033 0d0a  .ignore = W503..
+00000560: 0d0a 5b66 6c61 6b65 385d 0d0a 6578 7465  ..[flake8]..exte
+00000570: 6e64 2d69 676e 6f72 6520 3d20 5735 3033  nd-ignore = W503
+00000580: 0d0a 6578 7465 6e64 2d65 7863 6c75 6465  ..extend-exclude
+00000590: 203d 2076 656e 762c 2a63 6163 6865 2a0d   = venv,*cache*.
+000005a0: 0a70 6572 2d66 696c 652d 6967 6e6f 7265  .per-file-ignore
+000005b0: 7320 3d20 0d0a 0974 6573 7473 2f2a 3a20  s = ...tests/*: 
+000005c0: 5331 3031 0d0a 0d0a 5b69 736f 7274 5d0d  S101....[isort].
+000005d0: 0a70 726f 6669 6c65 203d 2062 6c61 636b  .profile = black
+000005e0: 0d0a 0d0a 5b65 6767 5f69 6e66 6f5d 0d0a  ....[egg_info]..
+000005f0: 7461 675f 6275 696c 6420 3d20 0d0a 7461  tag_build = ..ta
+00000600: 675f 6461 7465 203d 2030 0d0a 0d0a       g_date = 0....
```

### Comparing `python-lemming-0.5.1/src/lemming/__init__.py` & `python-lemming-0.6.0/src/lemming/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,12 +14,12 @@
 GNU General Public License for more details.
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # SPDX-License-Identifier: GPL-3.0-or-later
 __all__ = ["__version__", "logger"]
-__version__ = "0.5.1"
+__version__ = "0.6.0"
 import mylog
 
 logger = mylog.root.get_child("lemming")
 logger.threshold = mylog.Level.info
```

### Comparing `python-lemming-0.5.1/src/lemming/config.py` & `python-lemming-0.6.0/src/lemming/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,21 +15,28 @@
 
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 # SPDX-License-Identifier: GPL-3.0-or-later
 import os
 import pathlib
+import secrets
 import shlex
 import subprocess
 import sys
-from typing import Iterable, List, Mapping, MutableSequence, Optional, Union
+from typing import (
+    Any,
+    Iterable,
+    List,
+    Optional,
+    Union,
+    cast,
+)
 
-from confz import ConfZ, ConfZFileSource
-from confz.exceptions import ConfZFileException
+import pydantic
 from typing_extensions import NamedTuple, Self, TypeVar
 
 from . import logger
 
 try:
     import tomllib  # novermin
 except Exception:  # noqa: BLE001
@@ -49,54 +56,43 @@
 
 
 class WhatToQuiet(NamedTuple):
     commands: bool
     pip: bool
 
 
-def assert_dict_keys(
-    dictionary: Iterable[T], keys: MutableSequence[T]
-) -> None:
-    """
-    Assert that `dictionary`'s keys are in `keys`
-
-    Args:
-        dictionary (Iterable[Any, Any]): The dictionary to check.
-        keys (MutableSequence[Any]): The keys that are allowed.
-
-    Raises:
-        ValueError: If a key is found within `dictionary` but not within
-        `keys`.
-    """
-    logger.debug(f"Making sure that dict {dictionary!r} only has key {keys!r}")
-    with logger.ctxmgr:
-        for key in dictionary:
-            if key not in keys:
-                logger.error(
-                    f"Key {key!r} cannot be found within {keys}. Invalid"
-                    " config!"
-                )
-                raise ValueError(
-                    f"config {dictionary!r} cannot have key {key!r}"
-                )
-            keys.remove(key)
-
-
-class FormatterOrLinter(ConfZ):
+class FormatterOrLinter(pydantic.BaseModel):
     """
     An ABC for formatters and linters.
 
     Args:
-        packages (List[str]): The packages' name (optionally versions
+        name (str, optional): The name of the formatter/linter. Only used to
+        specify which formatter/linter to run. Defaults to packages[0].
+        packages (List[str]): The packages' names (optionally versions
         with "==x.y.z") to install with pip.
     """
 
-    # it's actually Iterable, but that introduces some bugs
+    name: str = ""
     packages: List[str]
 
+    @pydantic.model_validator(mode="after")
+    def _validate_name(self, _: Any) -> Self:
+        if self.name == "":
+            try:
+                self.name = self.packages[0]
+            except IndexError:
+                name = secrets.token_hex(2)
+                logger.warning(
+                    "A formatter or linter does not have packages nor a name!"
+                    " Please provide a name for it! Its name will be set to"
+                    f" {name!r} for this run."
+                )
+                self.name = name
+        return self
+
     def replace_command(
         self,
         command: str,
         paths_to_check: Iterable[pathlib.Path],
     ) -> str:
         r"""
         Return the command with {pyexe}, {path}, and {packages} being replaced.
@@ -127,36 +123,40 @@
         self,
         command: str,
         paths_to_check: Iterable[pathlib.Path],
         quiet: bool,
     ) -> bool:
         """
         Run command `command`.
-        Also replaces these:
-        - `{pyexe}` -> `sys.executable`
-
-        In `self.args` `{path}` be replaced by `paths_to_check`.
 
         Args:
             command (str): The command to run.
             paths_to_check (Iterable[pathlib.Path]): The paths to check.
             quiet (bool): Don't let the command write to stdout and stderr
 
         Returns:
             bool: `exit_status == 0`
         """
         command = self.replace_command(command, paths_to_check)
 
         splitted = shlex.split(command, posix=os.name != "nt")
         logger.debug(f"Running command {splitted!r}")
-        completed_process = subprocess.run(
-            splitted,
-            check=False,
-            capture_output=quiet,
-            shell=False,  # noqa: S603
+        quiet_kwargs = (
+            {"stdout": subprocess.DEVNULL, "stderr": subprocess.DEVNULL}
+            if quiet
+            else {}
+        )
+        completed_process = cast(
+            subprocess.CompletedProcess[str],
+            subprocess.run(
+                splitted,
+                check=False,
+                shell=False,  # noqa: S603
+                **quiet_kwargs,
+            ),
         )
         exit_status = completed_process.returncode
         if exit_status == 0:
             logger.info(f"Successfully ran command {command!r}")
             return True
         logger.error(
             f"Command {command!r} returned non-zero exit status {exit_status}"
@@ -177,56 +177,90 @@
         with logger.ctxmgr:
             return self.run_command(
                 "{pyexe} -m pip install -U {packages}", [], quiet
             )
 
 
 class Formatter(FormatterOrLinter):
+    """
+    A formatter.
+
+    Args:
+        packages (List[str]): The packages' names (optionally versions
+        with "==x.y.z") to install with pip.
+        format_command (str): The command to use to format the code (with the
+        `format` subcommand)
+        check_command (Optional[str], optional): The command to use to check
+        the code (with the `check` subcommand). Defaults to None.
+        allow_nonzero_on_format (bool, optional): Whether or not to allow the
+        formatter to return a non-zero exit status when formatting. Defaults
+        to False.
+    """
+
     format_command: str
     check_command: Optional[str] = None
     allow_nonzero_on_format: bool = False
 
     def run_format(
         self,
         paths_to_check: Iterable[pathlib.Path],
         what_to_quiet: WhatToQuiet,
     ) -> bool:
+        """
+        Format the code.
+
+        Args:
+            paths_to_check (Iterable[pathlib.Path]): The paths to format.
+            what_to_quiet (WhatToQuiet): What to quiet.
+
+        Returns:
+            bool: `exit_status == 0`
+        """
         install_success = self.install(what_to_quiet.pip)
         if not install_success:
             logger.error(
                 f"Could not install the packages {self.packages}! See"
                 " pip's output for more information."
             )
             return False
 
         success = self.run_command(
             self.format_command, paths_to_check, what_to_quiet.commands
         )
         if success or self.allow_nonzero_on_format:
-            logger.info(
-                f"Successfully ran (format) formatter {self.packages}!"
-            )
+            logger.info(f"Successfully ran (format) formatter {self.name}!")
         else:
             logger.error(
-                f"Could not run (format) formatter ({self.packages};"
-                f" {self.format_command!r})! (NOTE: The format_command command"
-                " is expected to modify/format the code and return zero. This"
-                " is DIFFERENT from check_command. If you still want to allow"
-                " this, set allow_nonzero_on_format=true for this formatter.)"
+                f"Could not run (format) formatter {self.name};"
+                f" ({self.format_command!r})! (NOTE: The format_command"
+                " command is expected to modify/format the code and return"
+                " zero. This is DIFFERENT from check_command. If you still"
+                " want to allow this, set allow_nonzero_on_format=true for"
+                " this formatter.)"
             )
         return success
 
     def run_check(
         self,
         paths_to_check: Iterable[pathlib.Path],
         what_to_quiet: WhatToQuiet,
     ) -> bool:
+        """
+        Check the code.
+
+        Args:
+            paths_to_check (Iterable[pathlib.Path]): Paths to check.
+            what_to_quiet (WhatToQuiet): What to quiet.
+
+        Returns:
+            bool: `exit_status == 0`
+        """
         if not self.check_command:
             logger.warning(
-                f"The formatter {self.packages} does NOT have a check_command!"
+                f"The formatter {self.name} does NOT have a check_command!"
                 " Skipping..."
             )
             return True
 
         install_success = self.install(what_to_quiet.pip)
         if not install_success:
             logger.error(
@@ -235,111 +269,169 @@
             )
             return False
 
         success = self.run_command(
             self.check_command, paths_to_check, what_to_quiet.commands
         )
         if success:
-            logger.info(f"Successfully ran (check) formatter {self.packages}!")
+            logger.info(f"Successfully ran (check) formatter {self.name}!")
         else:
             logger.error(
-                f"Could not run (check) formatter ({self.packages};"
-                f" {self.format_command!r})! (NOTE: The check_command command"
+                f"Could not run (check) formatter {self.name}"
+                f" ({self.check_command!r})! (NOTE: The check_command command"
                 " is expected to CHECK that the code is up to standards. If"
                 " the code is ok, the command should return 0; otherwise it"
                 " should return non-zero.)"
             )
         return success
 
-    @classmethod
-    def from_dict(cls, dict_: Mapping[str, Union[str, bool]]) -> Self:
-        assert_dict_keys(
-            dict_,
-            [
-                "packages",
-                "format_command",
-                "check_command",
-                "allow_nonzero_on_format",
-            ],
-        )
-        return cls(**dict_)
-
 
 class Linter(FormatterOrLinter):
+    """
+    A linter.
+
+    Args:
+        packages (List[str]): The packages' names (optionally versions
+        with "==x.y.z") to install with pip.
+        command (str): The command to use to lint the code
+        run_first (bool, optional): Whether or not to run this linter before
+        all other linters and formatters.
+    """
+
     command: str
     run_first: bool = False
 
     def run(
         self,
         paths_to_check: Iterable[pathlib.Path],
         what_to_quiet: WhatToQuiet,
     ) -> bool:
+        """
+        Lint the code.
+
+        Args:
+            paths_to_check (Iterable[pathlib.Path]): Paths to lint.
+            what_to_quiet (WhatToQuiet): What to quiet.
+
+        Returns:
+            bool: `exit_status == 0`
+        """
         install_success = self.install(what_to_quiet.pip)
         if not install_success:
             logger.error(
-                f"Could not install linter {self.packages}! See"
+                f"Could not install packages {self.packages}! See"
                 " pip's output for more information."
             )
+            return False
 
         success = self.run_command(
             self.command, paths_to_check, what_to_quiet.commands
         )
         if success:
-            logger.info(f"Successfully ran linter {self.packages}!")
+            logger.info(f"Successfully ran linter {self.name}!")
         else:
             logger.error(
-                "Linting failed! See the linter's output for more"
+                f"Linter {self.name} failed! See the linter's output for more"
                 " information!"
             )
         return success
 
-    @classmethod
-    def from_dict(cls, dict_: Mapping[str, Union[str, bool]]) -> Self:
-        assert_dict_keys(
-            dict_,
-            ["packages", "command", "run_first"],
-        )
-        return cls(**dict_)
 
+class Config(pydantic.BaseModel):
+    """
+    The configuration.
+
+    Args:
+        formatters (List[Formatter], optional): The formatters. Default
+        factory is list.
+        linters (List[Linter], optional): The linters. Default factory is list.
+        fail_fast (bool, optional): Whether or not to immediately quit when a
+        formatter or linter fails.
+    """
 
-class Config(ConfZ):
-    # we should be safe with mutable default arguments
-    formatters: List[Formatter] = []  # noqa: RUF012
-    linters: List[Linter] = []  # noqa: RUF012
-    # ^ also modify within read_config_file()
+    formatters: List[Formatter] = pydantic.Field(default_factory=list)
+    linters: List[Linter] = pydantic.Field(default_factory=list)
     fail_fast: bool = True
 
     def get_first_linters(self) -> List[Linter]:
+        """
+        Get the first linters.
+
+        Returns:
+            List[Linter]: Get linters, where `linter.run_first is True`
+        """
         return [linter for linter in self.linters if linter.run_first]
 
     def get_other_linters(self) -> List[Linter]:
+        """
+        Get the other linters.
+
+        Returns:
+            List[Linter]: Get linters, where `linter.run_first is False`
+        """
         return [linter for linter in self.linters if not linter.run_first]
 
 
-def get_config_dot_lemming(folder: pathlib.Path) -> Config:
-    return Config(ConfZFileSource(file=".lemming.toml", folder=folder))
+def get_config_dot_lemming(file: pathlib.Path) -> Config:
+    """
+    Get the config from `file`.
+
+    Args:
+        file (pathlib.Path): The config file to read from. Must use
+        the `.lemming.toml` syntax (not the `pyproject.toml` syntax).
+
+    Returns:
+        Config: The configuration.
+    """
+    return Config.model_validate(
+        tomllib.loads(file.read_text(encoding="utf-8"))
+    )
 
 
 def get_config_pyproject(pyproject: pathlib.Path) -> Config:
+    """
+    Get the config from `pyproject`.
+
+    Args:
+        pyproject (pathlib.Path): The config file to read from. Must use the
+        `pyproject.toml` syntax (not the `.lemming.toml` syntax).
+
+    Raises:
+        ValueError: If the config file does not contain a `tool.lemming` key.
+
+    Returns:
+        Config: The configuration.
+    """
     config_text = pyproject.read_text(encoding="utf-8")
     pyproject_config = tomllib.loads(config_text)
     try:
         lemming_config = pyproject_config["tool"]["lemming"]
     except KeyError as exception:
         raise CONFIG_HAS_NO_LEMMING_STUFF from exception
-    return Config(**lemming_config)
+    return Config.model_validate(lemming_config)
 
 
 def get_config(_folder: Union[os.PathLike[str], str]) -> Config:
+    """
+    Get the configuration from `_folder` or a parent folder recursively.
+
+    Args:
+        _folder (Union[os.PathLike[str], str]): The folder to use.
+
+    Raises:
+        FileNotFoundError: If no `pyproject.toml` nor `.lemming.toml` file was
+        found in `_folder` and its parents.
+
+    Returns:
+        Config: The configuration.
+    """
     folder = pathlib.Path(_folder)
-    try:
-        # try .lemming.toml
-        return get_config_dot_lemming(folder)
-    except ConfZFileException:
-        # try pyproject.toml
-        pyproject = folder / "pyproject.toml"
-        if not pyproject.exists():
-            # recursion... recursion recursion...
-            if folder.parent == folder:
-                raise CONFIG_FILE_NOT_FOUND_EXC from None
-            return get_config(folder.parent)
+    config_file = folder / CONFIG_FILE_NAME
+    if config_file.exists():
+        return get_config_dot_lemming(config_file)
+    pyproject = folder / "pyproject.toml"
+    if pyproject.exists():
         return get_config_pyproject(pyproject)
+    # recursion... recursion recursion...
+    if folder.parent == folder:
+        raise CONFIG_FILE_NOT_FOUND_EXC from None
+    return get_config(folder.parent)
```

