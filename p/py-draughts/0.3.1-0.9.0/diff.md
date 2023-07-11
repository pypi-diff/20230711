# Comparing `tmp/py-draughts-0.3.1.tar.gz` & `tmp/py-draughts-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-0.3.1.tar", last modified: Tue Jul 11 16:22:58 2023, max compression
+gzip compressed data, was "py-draughts-0.9.0.tar", last modified: Tue Jul 11 18:13:32 2023, max compression
```

## Comparing `py-draughts-0.3.1.tar` & `py-draughts-0.9.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 16:22:58.433276 py-draughts-0.3.1/
--rw-rw-rw-   0        0        0    35823 2023-07-11 12:53:30.000000 py-draughts-0.3.1/LICENSE
--rw-rw-rw-   0        0        0       44 2023-07-11 12:53:30.000000 py-draughts-0.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     5747 2023-07-11 16:22:58.432276 py-draughts-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     4294 2023-07-11 16:18:08.000000 py-draughts-0.3.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-11 16:22:58.414467 py-draughts-0.3.1/draughts/
--rw-rw-rw-   0        0        0      947 2023-07-11 12:53:30.000000 py-draughts-0.3.1/draughts/__init__.py
--rw-rw-rw-   0        0        0     3838 2023-07-11 16:12:53.000000 py-draughts-0.3.1/draughts/american.py
--rw-rw-rw-   0        0        0     7825 2023-07-11 16:12:53.000000 py-draughts-0.3.1/draughts/base.py
--rw-rw-rw-   0        0        0      674 2023-07-07 12:24:29.000000 py-draughts-0.3.1/draughts/models.py
--rw-rw-rw-   0        0        0     4120 2023-07-11 16:12:53.000000 py-draughts-0.3.1/draughts/move.py
--rw-rw-rw-   0        0        0     6086 2023-07-11 16:14:48.000000 py-draughts-0.3.1/draughts/server.py
--rw-rw-rw-   0        0        0     5632 2023-07-11 16:12:53.000000 py-draughts-0.3.1/draughts/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-11 16:22:58.391265 py-draughts-0.3.1/draughts/static/
-drwxrwxrwx   0        0        0        0 2023-07-11 16:22:58.415467 py-draughts-0.3.1/draughts/static/css/
--rw-rw-rw-   0        0        0     2814 2023-07-11 12:56:50.000000 py-draughts-0.3.1/draughts/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-07-11 16:22:58.417468 py-draughts-0.3.1/draughts/static/js/
--rw-rw-rw-   0        0        0     5824 2023-07-11 15:13:38.000000 py-draughts-0.3.1/draughts/static/js/script.js
-drwxrwxrwx   0        0        0        0 2023-07-11 16:22:58.420468 py-draughts-0.3.1/draughts/templates/
--rw-rw-rw-   0        0        0     1857 2023-07-10 15:34:15.000000 py-draughts-0.3.1/draughts/templates/base.html
--rw-rw-rw-   0        0        0     2500 2023-07-11 13:56:11.000000 py-draughts-0.3.1/draughts/templates/index.html
--rw-rw-rw-   0        0        0     1973 2023-07-11 13:47:51.000000 py-draughts-0.3.1/draughts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 16:22:58.427761 py-draughts-0.3.1/py_draughts.egg-info/
--rw-rw-rw-   0        0        0     5747 2023-07-11 16:22:58.000000 py-draughts-0.3.1/py_draughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      514 2023-07-11 16:22:58.000000 py-draughts-0.3.1/py_draughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 16:22:58.000000 py-draughts-0.3.1/py_draughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-11 16:22:58.000000 py-draughts-0.3.1/py_draughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       27 2023-07-04 21:57:35.000000 py-draughts-0.3.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 16:22:58.434276 py-draughts-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1894 2023-07-11 16:14:45.000000 py-draughts-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 16:22:58.431269 py-draughts-0.3.1/test/
--rw-rw-rw-   0        0        0     1123 2023-07-11 16:12:53.000000 py-draughts-0.3.1/test/test_american_board.py
--rw-rw-rw-   0        0        0     2376 2023-07-11 16:12:53.000000 py-draughts-0.3.1/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:13:32.796215 py-draughts-0.9.0/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 12:53:30.000000 py-draughts-0.9.0/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-11 18:05:22.000000 py-draughts-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5743 2023-07-11 18:13:32.795218 py-draughts-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4342 2023-07-11 18:11:30.000000 py-draughts-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 18:13:32.772208 py-draughts-0.9.0/draughts/
+-rw-rw-rw-   0        0        0      945 2023-07-11 18:13:19.000000 py-draughts-0.9.0/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3838 2023-07-11 16:12:53.000000 py-draughts-0.9.0/draughts/american.py
+-rw-rw-rw-   0        0        0     7825 2023-07-11 16:29:47.000000 py-draughts-0.9.0/draughts/base.py
+-rw-rw-rw-   0        0        0      674 2023-07-11 16:40:27.000000 py-draughts-0.9.0/draughts/models.py
+-rw-rw-rw-   0        0        0     4191 2023-07-11 17:16:02.000000 py-draughts-0.9.0/draughts/move.py
+-rw-rw-rw-   0        0        0     6490 2023-07-11 18:10:09.000000 py-draughts-0.9.0/draughts/server.py
+-rw-rw-rw-   0        0        0     5851 2023-07-11 17:24:52.000000 py-draughts-0.9.0/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:13:32.738914 py-draughts-0.9.0/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-11 18:13:32.774208 py-draughts-0.9.0/draughts/static/css/
+-rw-rw-rw-   0        0        0     2814 2023-07-11 12:56:50.000000 py-draughts-0.9.0/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-11 18:13:32.776208 py-draughts-0.9.0/draughts/static/js/
+-rw-rw-rw-   0        0        0     5824 2023-07-11 15:13:38.000000 py-draughts-0.9.0/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-11 18:13:32.778212 py-draughts-0.9.0/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-11 16:32:17.000000 py-draughts-0.9.0/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2500 2023-07-11 13:56:11.000000 py-draughts-0.9.0/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     1973 2023-07-11 13:47:51.000000 py-draughts-0.9.0/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:13:32.790230 py-draughts-0.9.0/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     5743 2023-07-11 18:13:32.000000 py-draughts-0.9.0/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-07-11 18:13:32.000000 py-draughts-0.9.0/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 18:13:32.000000 py-draughts-0.9.0/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-11 18:13:32.000000 py-draughts-0.9.0/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-11 18:13:32.000000 py-draughts-0.9.0/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 17:26:06.000000 py-draughts-0.9.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 18:13:32.796215 py-draughts-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1906 2023-07-11 17:45:47.000000 py-draughts-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:13:32.792215 py-draughts-0.9.0/test/
+-rw-rw-rw-   0        0        0     1123 2023-07-11 16:12:53.000000 py-draughts-0.9.0/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2376 2023-07-11 16:12:53.000000 py-draughts-0.9.0/test/test_board.py
```

### Comparing `py-draughts-0.3.1/LICENSE` & `py-draughts-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-0.3.1/PKG-INFO` & `py-draughts-0.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 0.3.1
-Summary: A checkers library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
+Version: 0.9.0
+Summary: A draughts library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,154 +19,149 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires: numpy
-Requires: easy_logs
-Requires: fastapi
 Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-py-draughts
-=============
+# py-draughts
 
-.. image:: https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg
-   :target: https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml
+[![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
+[![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
 
-.. image:: https://badge.fury.io/py/fast_checkers.svg
-   :target: https://badge.fury.io/py/fast_checkers
 
-Draughts
---------
+Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
+Supports multiple variants of the game and allows playing against AI.
 
-*Project still under active developement. Still lacking some important functionality.*
 
-Efficient Modern and flexible implementation of draughts game with beautiful web interface. Supports multiple variants of the game and allows to play against AI.
 
+## Installation
 
+```bash
+pip install py-draughts
+```
 
+## [Documentation](https://michalskibinski109.github.io/py-draughts/)
 
-`Documentation <https://michalskibinski109.github.io/draughts/>`_
------------------------------------------------------------------
+## Usage
 
-Installation
-------------
 
-.. code-block:: bash
 
-    python -m pip install py-draughts
+#### Initialize board
 
-Usage
------
+```python
+>>> from draughts.standard import Board
+>>> board = Board()
+Board initialized with shape (10, 10). (base.py:108)
+```
 
-simple
-*******
+#### Make and undo moves
 
-.. code-block:: python
+```python
+>>> board.push_from_str("37-32")
+>>> board.push_from_str("14-19")
+>>> board.push_from_str("32-28")
+>>> board.push_from_str("19-23")
+>>> board.pop() # undo last move
+>>> board.push_from_str("19-23")
+>>> board.push_from_str("28x19")
+```
 
-    >>> import draughts.american as draughts
+#### Shows simple ascii board
 
-    >>> board = draughts.Board()
-    ---------------------------------
-    |   | x |   | x |   | x |   | x |
-    ---------------------------------
-    | x |   | x |   | x |   | x |   |
-    ---------------------------------
-    |   | x |   | x |   | x |   | x |
-    ---------------------------------
-    |   |   |   |   |   |   |   |   |
-    ---------------------------------
-    |   |   |   |   |   |   |   |   |
-    ---------------------------------
-    | o |   | o |   | o |   | o |   |
-    ---------------------------------
-    |   | o |   | o |   | o |   | o |
-    ---------------------------------
-    | o |   | o |   | o |   | o |   |
+```python
+>>> print(board)
+-----------------------------------------
+|   | b |   | b |   | b |   | b |   | b |
+-----------------------------------------
+| b |   | b |   | b |   | b |   | b |   |
+-----------------------------------------
+|   | b |   | b |   | b |   |   |   | b |
+-----------------------------------------
+|   |   |   |   |   |   | w |   |   |   |
+-----------------------------------------
+|   |   |   |   |   |   |   |   |   |   |
+-----------------------------------------
+|   |   |   |   |   |   |   |   |   |   |
+-----------------------------------------
+|   |   |   |   |   |   |   |   |   |   |
+-----------------------------------------
+| w |   |   |   | w |   | w |   | w |   |
+-----------------------------------------
+|   | w |   | w |   | w |   | w |   | w |
+-----------------------------------------
+| w |   | w |   | w |   | w |   | w |   |
+```
 
+### American checkers
 
-Moving pieces
-*************
+```python
+>>> from draughts.american import Board
+>>> board = Board()
+Board initialized with shape (8, 8). (base.py:108)
+>>> print(board)
+---------------------------------
+|   | b |   | b |   | b |   | b |
+---------------------------------
+| b |   | b |   | b |   | b |   |
+---------------------------------
+|   | b |   | b |   | b |   | b |
+---------------------------------
+|   |   |   |   |   |   |   |   |
+---------------------------------
+|   |   |   |   |   |   |   |   |
+---------------------------------
+| w |   | w |   | w |   | w |   |
+---------------------------------
+|   | w |   | w |   | w |   | w |
+---------------------------------
+| w |   | w |   | w |   | w |   |
+```
 
-.. code-block:: python
 
-    >>> board.push_from_str("24-19")
-    >>> board.push_from_str("12-16")
-    >>> board.push_from_str("23-18")
-    >>> board.push_from_str("16x23")
-    >>> board.push_from_str("26x19")
-    >>> board.pop()
-    >>> print(board)
-    ---------------------------------
-    |   | x |   | x |   | x |   | x |
-    ---------------------------------
-    | x |   | x |   | x |   | x |   |
-    ---------------------------------
-    |   | x |   | x |   | x |   |   |
-    ---------------------------------
-    |   |   |   |   |   |   |   |   |
-    ---------------------------------
-    |   |   |   | o |   |   |   |   |
-    ---------------------------------
-    | o |   | o |   | x |   |   |   |
-    ---------------------------------
-    |   | o |   | o |   | o |   | o |
-    ---------------------------------
-    | o |   | o |   | o |   | o |   |
+## UI
 
+```python
+from draughts.server import Server
+Server().run()
+```
 
-.. code-block:: python
+### Use for testing your engine.
 
-    >>> print(list(board.legal_moves))
-    [Move: 21->17, Move: 22->18, Move: 22->17, Move: 23->19, Move: 23->18, Move: 24->20, Move: 24->19]
+_Example with simplest possible engine._
 
-Creating custom board
-*********************
+```python
+>>> server = Server(get_best_move_method=lambda board: np.random.choice([board.legal_moves]))
+>>> server.run()
+INFO:     Started server process [1617]
+INFO:     Waiting for application startup.
+INFO:     Application startup complete.
+INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
+```
 
-.. code-block:: python
+_It is as simple as that!_
 
-    import draughts.base as draughts
-    import numpy as np
-    CUSTOM_POSITION = np.array([1] * 20 + [-1] * 12, dtype=np.int8)
-    board = draughts.BaseBoard(starting_position=CUSTOM_POSITION)
-    board.legal_moves = ... # create your own custom legal_moves method (property)
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/a5e2ca89-28e1-4dcc-96ae-b18fc602c9bc" width="600" />
 
-UI
---
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/b14523ea-4bc4-45e1-b5c0-5deea3ed5328" width="600" />
 
-.. code-block:: python
+*Legal moves for selected square (on image "16")*
 
-    from draughts.server import Server
-    Server().run()
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/c8245cbc-06ec-4623-81ab-c9aaa9302627" width="600" />
 
-*It is as simple as that!*
 
-
-.. image:: https://github.com/michalskibinski109/draughts/assets/77834536/4ec36e49-38cc-45e8-a500-d0d24b21fce7
-   :width: 600
-
-.. image:: https://github.com/michalskibinski109/draughts/assets/77834536/b7e0bf73-1bc5-4769-8f82-a22cde3b7e90
-   :width: 600
-
-*pseudo legal moves for selected square* 
-
-.. image:: https://github.com/michalskibinski109/draughts/assets/77834536/ef64179a-1e7d-46d4-991e-5a34fc803d7e
-   :width: 600
-
-Contributing
-------------
+## Contributing
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
-Bibliography
-------------
+## Bibliography
 
-1. `notation <https://en.wikipedia.org/wiki/Portable_Draughts_Notation>`_
-2. `rules and variants <https://en.wikipedia.org/wiki/Checkers>`_
-3. `list of pdns <https://github.com/mig0/Games-Checkers/>`_
-4. `droughts online  <https://lidraughts.org/>`_
-5. `additional 1 (checkers online) <https://checkers.online/play>`_
-6. `additional 2 (chinook) <https://webdocs.cs.ualberta.ca/~chinook/play/notation.html>`_
+1. [Notation](https://en.wikipedia.org/wiki/Portable_Draughts_Notation)
+2. [Rules and variants](https://en.wikipedia.org/wiki/Checkers)
+3. [List of PDNs](https://github.com/mig0/Games-Checkers/)
+4. [Draughts online](https://lidraughts.org/)
+5. [Additional 1 (Checkers online)](https://checkers.online/play)
+6. [Additional 2 (Chinook)](https://webdocs.cs.ualberta.ca/~chinook/play/notation.html)
```

### Comparing `py-draughts-0.3.1/README.rst` & `py-draughts-0.9.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,140 +1,138 @@
-py-draughts
-=============
+# py-draughts
 
-.. image:: https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg
-   :target: https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml
+[![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
+[![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
 
-.. image:: https://badge.fury.io/py/fast_checkers.svg
-   :target: https://badge.fury.io/py/fast_checkers
 
-Draughts
---------
+Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
+Supports multiple variants of the game and allows playing against AI.
 
-*Project still under active developement. Still lacking some important functionality.*
 
-Efficient Modern and flexible implementation of draughts game with beautiful web interface. Supports multiple variants of the game and allows to play against AI.
 
+## Installation
 
+```bash
+pip install py-draughts
+```
 
+## [Documentation](https://michalskibinski109.github.io/py-draughts/)
 
-`Documentation <https://michalskibinski109.github.io/draughts/>`_
------------------------------------------------------------------
+## Usage
 
-Installation
-------------
 
-.. code-block:: bash
 
-    python -m pip install py-draughts
+#### Initialize board
 
-Usage
------
+```python
+>>> from draughts.standard import Board
+>>> board = Board()
+Board initialized with shape (10, 10). (base.py:108)
+```
 
-simple
-*******
+#### Make and undo moves
 
-.. code-block:: python
+```python
+>>> board.push_from_str("37-32")
+>>> board.push_from_str("14-19")
+>>> board.push_from_str("32-28")
+>>> board.push_from_str("19-23")
+>>> board.pop() # undo last move
+>>> board.push_from_str("19-23")
+>>> board.push_from_str("28x19")
+```
 
-    >>> import draughts.american as draughts
+#### Shows simple ascii board
 
-    >>> board = draughts.Board()
-    ---------------------------------
-    |   | x |   | x |   | x |   | x |
-    ---------------------------------
-    | x |   | x |   | x |   | x |   |
-    ---------------------------------
-    |   | x |   | x |   | x |   | x |
-    ---------------------------------
-    |   |   |   |   |   |   |   |   |
-    ---------------------------------
-    |   |   |   |   |   |   |   |   |
-    ---------------------------------
-    | o |   | o |   | o |   | o |   |
-    ---------------------------------
-    |   | o |   | o |   | o |   | o |
-    ---------------------------------
-    | o |   | o |   | o |   | o |   |
+```python
+>>> print(board)
+-----------------------------------------
+|   | b |   | b |   | b |   | b |   | b |
+-----------------------------------------
+| b |   | b |   | b |   | b |   | b |   |
+-----------------------------------------
+|   | b |   | b |   | b |   |   |   | b |
+-----------------------------------------
+|   |   |   |   |   |   | w |   |   |   |
+-----------------------------------------
+|   |   |   |   |   |   |   |   |   |   |
+-----------------------------------------
+|   |   |   |   |   |   |   |   |   |   |
+-----------------------------------------
+|   |   |   |   |   |   |   |   |   |   |
+-----------------------------------------
+| w |   |   |   | w |   | w |   | w |   |
+-----------------------------------------
+|   | w |   | w |   | w |   | w |   | w |
+-----------------------------------------
+| w |   | w |   | w |   | w |   | w |   |
+```
 
+### American checkers
 
-Moving pieces
-*************
+```python
+>>> from draughts.american import Board
+>>> board = Board()
+Board initialized with shape (8, 8). (base.py:108)
+>>> print(board)
+---------------------------------
+|   | b |   | b |   | b |   | b |
+---------------------------------
+| b |   | b |   | b |   | b |   |
+---------------------------------
+|   | b |   | b |   | b |   | b |
+---------------------------------
+|   |   |   |   |   |   |   |   |
+---------------------------------
+|   |   |   |   |   |   |   |   |
+---------------------------------
+| w |   | w |   | w |   | w |   |
+---------------------------------
+|   | w |   | w |   | w |   | w |
+---------------------------------
+| w |   | w |   | w |   | w |   |
+```
 
-.. code-block:: python
 
-    >>> board.push_from_str("24-19")
-    >>> board.push_from_str("12-16")
-    >>> board.push_from_str("23-18")
-    >>> board.push_from_str("16x23")
-    >>> board.push_from_str("26x19")
-    >>> board.pop()
-    >>> print(board)
-    ---------------------------------
-    |   | x |   | x |   | x |   | x |
-    ---------------------------------
-    | x |   | x |   | x |   | x |   |
-    ---------------------------------
-    |   | x |   | x |   | x |   |   |
-    ---------------------------------
-    |   |   |   |   |   |   |   |   |
-    ---------------------------------
-    |   |   |   | o |   |   |   |   |
-    ---------------------------------
-    | o |   | o |   | x |   |   |   |
-    ---------------------------------
-    |   | o |   | o |   | o |   | o |
-    ---------------------------------
-    | o |   | o |   | o |   | o |   |
+## UI
 
+```python
+from draughts.server import Server
+Server().run()
+```
 
-.. code-block:: python
+### Use for testing your engine.
 
-    >>> print(list(board.legal_moves))
-    [Move: 21->17, Move: 22->18, Move: 22->17, Move: 23->19, Move: 23->18, Move: 24->20, Move: 24->19]
+_Example with simplest possible engine._
 
-Creating custom board
-*********************
+```python
+>>> server = Server(get_best_move_method=lambda board: np.random.choice([board.legal_moves]))
+>>> server.run()
+INFO:     Started server process [1617]
+INFO:     Waiting for application startup.
+INFO:     Application startup complete.
+INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
+```
 
-.. code-block:: python
+_It is as simple as that!_
 
-    import draughts.base as draughts
-    import numpy as np
-    CUSTOM_POSITION = np.array([1] * 20 + [-1] * 12, dtype=np.int8)
-    board = draughts.BaseBoard(starting_position=CUSTOM_POSITION)
-    board.legal_moves = ... # create your own custom legal_moves method (property)
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/a5e2ca89-28e1-4dcc-96ae-b18fc602c9bc" width="600" />
 
-UI
---
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/b14523ea-4bc4-45e1-b5c0-5deea3ed5328" width="600" />
 
-.. code-block:: python
+*Legal moves for selected square (on image "16")*
 
-    from draughts.server import Server
-    Server().run()
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/c8245cbc-06ec-4623-81ab-c9aaa9302627" width="600" />
 
-*It is as simple as that!*
 
-
-.. image:: https://github.com/michalskibinski109/draughts/assets/77834536/4ec36e49-38cc-45e8-a500-d0d24b21fce7
-   :width: 600
-
-.. image:: https://github.com/michalskibinski109/draughts/assets/77834536/b7e0bf73-1bc5-4769-8f82-a22cde3b7e90
-   :width: 600
-
-*pseudo legal moves for selected square* 
-
-.. image:: https://github.com/michalskibinski109/draughts/assets/77834536/ef64179a-1e7d-46d4-991e-5a34fc803d7e
-   :width: 600
-
-Contributing
-------------
+## Contributing
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
-Bibliography
-------------
+## Bibliography
 
-1. `notation <https://en.wikipedia.org/wiki/Portable_Draughts_Notation>`_
-2. `rules and variants <https://en.wikipedia.org/wiki/Checkers>`_
-3. `list of pdns <https://github.com/mig0/Games-Checkers/>`_
-4. `droughts online  <https://lidraughts.org/>`_
-5. `additional 1 (checkers online) <https://checkers.online/play>`_
-6. `additional 2 (chinook) <https://webdocs.cs.ualberta.ca/~chinook/play/notation.html>`_
+1. [Notation](https://en.wikipedia.org/wiki/Portable_Draughts_Notation)
+2. [Rules and variants](https://en.wikipedia.org/wiki/Checkers)
+3. [List of PDNs](https://github.com/mig0/Games-Checkers/)
+4. [Draughts online](https://lidraughts.org/)
+5. [Additional 1 (Checkers online)](https://checkers.online/play)
+6. [Additional 2 (Chinook)](https://webdocs.cs.ualberta.ca/~chinook/play/notation.html)
```

### Comparing `py-draughts-0.3.1/draughts/__init__.py` & `py-draughts-0.9.0/draughts/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file is part of the fast-checkers library.
+# This file is part of the py-draughts library.
 # Copyright (C) 2023-2023 Michał Skibiński
 #
 # This program is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
@@ -11,13 +11,13 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """
-A checkers library for Python, with move generation and validation,
+A draughts library for Python, with move generation and validation,
 PDN parsing and writing. Supprots multiple variants of game.
 """
 
-__version__ = "0.3.1"
+__version__ = "0.9.0"
 __author__ = "Michał Skibiński"
```

### Comparing `py-draughts-0.3.1/draughts/american.py` & `py-draughts-0.9.0/draughts/american.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.3.1/draughts/base.py` & `py-draughts-0.9.0/draughts/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,20 +33,20 @@
 class BaseBoard(ABC):
     """
     Abstact class for all draughts variants.
 
     .. important::
         All boards contain all methods from this class.
 
-    Class is designed to support checkers boards of any size.
+    Class is designed to support draughts boards of any size.
     By specifying the starting position, the user can create a board of any size.
 
 
 
-    To create new variants of checkers, inherit from this class and:
+    To create new variants of draughts, inherit from this class and:
 
     - override the ``legal_moves`` property
     - override the ``SQUARES`` list to match the new board size
     - override the ``STARTING_POSITION`` to specify the starting position
 
     Constraints:
     - There are only two colors:
```

### Comparing `py-draughts-0.3.1/draughts/models.py` & `py-draughts-0.9.0/draughts/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,13 +21,13 @@
     WHITE_MAN = Color.WHITE.value
     KING = 10
     MAN = 1
     EMPTY = 0
 
 
 ENTITY_REPR = {
-    Entity.BLACK_MAN: "x",
-    Entity.WHITE_MAN: "o",
+    Entity.BLACK_MAN: "b",
+    Entity.WHITE_MAN: "w",
     Entity.EMPTY: " ",
-    Entity.BLACK_KING: "X",
-    Entity.WHITE_KING: "O",
+    Entity.BLACK_KING: "B",
+    Entity.WHITE_KING: "W",
 }
```

### Comparing `py-draughts-0.3.1/draughts/move.py` & `py-draughts-0.9.0/draughts/move.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,14 +62,17 @@
                 else other.square_list
             )
 
             return all(square in longer for square in shorter)
 
         return False
 
+    def __len__(self) -> int:
+        return len(self.square_list)
+
     def __add__(self, other: Move) -> Move:
         """Append moves"""
         if self.square_list[-1] != other.square_list[0]:
             raise ValueError(
                 f"Cannot append moves {self} and {other}. Last square of first move should be equal to first square of second move."
             )
         return Move(
```

### Comparing `py-draughts-0.3.1/draughts/server.py` & `py-draughts-0.9.0/draughts/server.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,35 +5,42 @@
 import json
 from fastapi.staticfiles import StaticFiles
 from fastapi.templating import Jinja2Templates
 from draughts import __version__
 from draughts.standard import Board
 from typing import Literal
 from collections import defaultdict
+from pathlib import Path
 
 
 class Server:
     def __init__(
         self,
         board=Board(),
+        get_best_move_method: callable = None,
         draw_board=True,
         populate_board=True,
         show_pseudo_legal_moves=True,
     ):
         self.app = FastAPI(title="py-draughts", version=__version__)
-        self.app.mount(
-            "/static", StaticFiles(directory="draughts/static"), name="static"
-        )
-        self.templates = Jinja2Templates(directory="draughts/templates/")
+        static_dir = Path(__file__).parent / "static"
+        templates_dir = Path(__file__).parent / "templates"
+        self.app.mount("/static", StaticFiles(directory=static_dir), name="static")
+        self.get_best_move_method = get_best_move_method
+        if not get_best_move_method:
+            self.get_best_move_method = lambda board: np.random.choice(
+                list(board.legal_moves)
+            )
+        self.templates = Jinja2Templates(directory=templates_dir)
         self.board = board
         self.router = APIRouter()
         self.router.add_api_route("/", self.index)
         self.router.add_api_route("/set_board/{board_type}", self.set_board)
         self.router.add_api_route("/set_random_position", self.set_random_position)
-        self.router.add_api_route("/random_move", self.random_move)
+        self.router.add_api_route("/random_move", self.get_best_move)
         self.router.add_api_route("/get_board_info", self.get_board_info)
         self.router.add_api_route("/get_legal_moves", self.get_legal_moves)
         self.app.include_router(self.router)
         self.draw_board = draw_board
         self.populate_board = populate_board
         self.show_pseudo_legal_moves = show_pseudo_legal_moves
 
@@ -51,16 +58,16 @@
 
     def get_legal_moves(self):
         legal_moves = list(self.board.legal_moves)
         from pprint import pprint
 
         pprint(legal_moves)
         moves_dict = defaultdict(list)
-        for move in legal_moves:
-            moves_dict[int(move.square_list[0])].extend(move.square_list[1:])
+        for move in list(legal_moves):
+            moves_dict[int(move.square_list[0])].extend(map(int, move.square_list[1:]))
         print(moves_dict)
         return {
             "legal_moves": json.dumps(moves_dict),
         }
 
     def get_board_info(self, request: Request):
         return (
@@ -84,19 +91,19 @@
             size=len(self.board.STARTING_POSITION),
             replace=True,
             p=[0.1, 0.6, 0.1, 0.1, 0.1],
         )
         self.board._pos = STARTING_POSITION
         return RedirectResponse(url="/")
 
-    def random_move(self, request: Request):
+    def get_best_move(self, request: Request):
         legal_moves = list(self.board.legal_moves)
         # print longest capture chain
         print(max(legal_moves, key=lambda x: len(x.captured_list)))
-        move = np.random.choice(legal_moves)
+        move = self.get_best_move_method(self.board)
         print(move)
         self.board.push(move)
         return {"position": self.board.friendly_form.tolist()}
 
     def index(self, request: Request):
         return self.templates.TemplateResponse(
             "index.html",
```

### Comparing `py-draughts-0.3.1/draughts/standard.py` & `py-draughts-0.9.0/draughts/standard.py`

 * *Files 10% similar despite different names*

```diff
@@ -117,15 +117,18 @@
                             [square, direction[i]], [target], [self._pos[target]]
                         )
                         moves.append(move)
                         self.push(move, False)
                         moves += [
                             move + m for m in self._legal_moves_from(direction[i], True)
                         ]
+                        # if one move is longer then others return only this one
                         self.pop(False)
+                        max_len = max([len(m) for m in moves])
+                        moves = [m for m in moves if len(m) == max_len]
                         i += 1
                     break
                 if (
                     self._pos[target] == Entity.EMPTY.value and not is_capture_mandatory
                 ):  # casual move
                     moves.append(Move([square, target]))
                 else:
```

### Comparing `py-draughts-0.3.1/draughts/static/css/style.css` & `py-draughts-0.9.0/draughts/static/css/style.css`

 * *Files identical despite different names*

### Comparing `py-draughts-0.3.1/draughts/static/js/script.js` & `py-draughts-0.9.0/draughts/static/js/script.js`

 * *Files identical despite different names*

### Comparing `py-draughts-0.3.1/draughts/templates/base.html` & `py-draughts-0.9.0/draughts/templates/base.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html lang="en">
   <head>
     <meta charset="UTF-8" />
     <meta http-equiv="X-UA-Compatible" content="IE=edge" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-    <title>Checkers</title>
+    <title>py-draughts</title>
 
     <script
       src="https://code.jquery.com/jquery-3.4.1.slim.min.js"
       integrity="sha384-J6qa4849blE2+poT4WnyKhv5vZF5SrPo0iEjwBvKU7imGFAV0wwj1yYfoRSJoZ+n"
       crossorigin="anonymous"
     ></script>
     <script
```

### Comparing `py-draughts-0.3.1/draughts/templates/index.html` & `py-draughts-0.9.0/draughts/templates/index.html`

 * *Files identical despite different names*

### Comparing `py-draughts-0.3.1/draughts/utils.py` & `py-draughts-0.9.0/draughts/utils.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.3.1/py_draughts.egg-info/PKG-INFO` & `py-draughts-0.9.0/py_draughts.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: py-draughts
-Version: 0.3.1
-Summary: A checkers library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
+Version: 0.9.0
+Summary: A draughts library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
 Home-page: https://github.com/michalskibinski109/draughts
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/draughts/index.html
 Keywords: draughts,checkers,AI mini-max,game,board
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,154 +19,149 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
-Requires: numpy
-Requires: easy_logs
-Requires: fastapi
 Requires-Python: >=3.10
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
-py-draughts
-=============
+# py-draughts
 
-.. image:: https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg
-   :target: https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml
+[![GitHub Actions](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg)](https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml)
+[![PyPI version](https://badge.fury.io/py/py-draughts.svg)](https://badge.fury.io/py/py-draughts)
 
-.. image:: https://badge.fury.io/py/fast_checkers.svg
-   :target: https://badge.fury.io/py/fast_checkers
 
-Draughts
---------
+Efficient modern and flexible implementation of the draughts game with a beautiful web interface. 
+Supports multiple variants of the game and allows playing against AI.
 
-*Project still under active developement. Still lacking some important functionality.*
 
-Efficient Modern and flexible implementation of draughts game with beautiful web interface. Supports multiple variants of the game and allows to play against AI.
 
+## Installation
 
+```bash
+pip install py-draughts
+```
 
+## [Documentation](https://michalskibinski109.github.io/py-draughts/)
 
-`Documentation <https://michalskibinski109.github.io/draughts/>`_
------------------------------------------------------------------
+## Usage
 
-Installation
-------------
 
-.. code-block:: bash
 
-    python -m pip install py-draughts
+#### Initialize board
 
-Usage
------
+```python
+>>> from draughts.standard import Board
+>>> board = Board()
+Board initialized with shape (10, 10). (base.py:108)
+```
 
-simple
-*******
+#### Make and undo moves
 
-.. code-block:: python
+```python
+>>> board.push_from_str("37-32")
+>>> board.push_from_str("14-19")
+>>> board.push_from_str("32-28")
+>>> board.push_from_str("19-23")
+>>> board.pop() # undo last move
+>>> board.push_from_str("19-23")
+>>> board.push_from_str("28x19")
+```
 
-    >>> import draughts.american as draughts
+#### Shows simple ascii board
 
-    >>> board = draughts.Board()
-    ---------------------------------
-    |   | x |   | x |   | x |   | x |
-    ---------------------------------
-    | x |   | x |   | x |   | x |   |
-    ---------------------------------
-    |   | x |   | x |   | x |   | x |
-    ---------------------------------
-    |   |   |   |   |   |   |   |   |
-    ---------------------------------
-    |   |   |   |   |   |   |   |   |
-    ---------------------------------
-    | o |   | o |   | o |   | o |   |
-    ---------------------------------
-    |   | o |   | o |   | o |   | o |
-    ---------------------------------
-    | o |   | o |   | o |   | o |   |
+```python
+>>> print(board)
+-----------------------------------------
+|   | b |   | b |   | b |   | b |   | b |
+-----------------------------------------
+| b |   | b |   | b |   | b |   | b |   |
+-----------------------------------------
+|   | b |   | b |   | b |   |   |   | b |
+-----------------------------------------
+|   |   |   |   |   |   | w |   |   |   |
+-----------------------------------------
+|   |   |   |   |   |   |   |   |   |   |
+-----------------------------------------
+|   |   |   |   |   |   |   |   |   |   |
+-----------------------------------------
+|   |   |   |   |   |   |   |   |   |   |
+-----------------------------------------
+| w |   |   |   | w |   | w |   | w |   |
+-----------------------------------------
+|   | w |   | w |   | w |   | w |   | w |
+-----------------------------------------
+| w |   | w |   | w |   | w |   | w |   |
+```
 
+### American checkers
 
-Moving pieces
-*************
+```python
+>>> from draughts.american import Board
+>>> board = Board()
+Board initialized with shape (8, 8). (base.py:108)
+>>> print(board)
+---------------------------------
+|   | b |   | b |   | b |   | b |
+---------------------------------
+| b |   | b |   | b |   | b |   |
+---------------------------------
+|   | b |   | b |   | b |   | b |
+---------------------------------
+|   |   |   |   |   |   |   |   |
+---------------------------------
+|   |   |   |   |   |   |   |   |
+---------------------------------
+| w |   | w |   | w |   | w |   |
+---------------------------------
+|   | w |   | w |   | w |   | w |
+---------------------------------
+| w |   | w |   | w |   | w |   |
+```
 
-.. code-block:: python
 
-    >>> board.push_from_str("24-19")
-    >>> board.push_from_str("12-16")
-    >>> board.push_from_str("23-18")
-    >>> board.push_from_str("16x23")
-    >>> board.push_from_str("26x19")
-    >>> board.pop()
-    >>> print(board)
-    ---------------------------------
-    |   | x |   | x |   | x |   | x |
-    ---------------------------------
-    | x |   | x |   | x |   | x |   |
-    ---------------------------------
-    |   | x |   | x |   | x |   |   |
-    ---------------------------------
-    |   |   |   |   |   |   |   |   |
-    ---------------------------------
-    |   |   |   | o |   |   |   |   |
-    ---------------------------------
-    | o |   | o |   | x |   |   |   |
-    ---------------------------------
-    |   | o |   | o |   | o |   | o |
-    ---------------------------------
-    | o |   | o |   | o |   | o |   |
+## UI
 
+```python
+from draughts.server import Server
+Server().run()
+```
 
-.. code-block:: python
+### Use for testing your engine.
 
-    >>> print(list(board.legal_moves))
-    [Move: 21->17, Move: 22->18, Move: 22->17, Move: 23->19, Move: 23->18, Move: 24->20, Move: 24->19]
+_Example with simplest possible engine._
 
-Creating custom board
-*********************
+```python
+>>> server = Server(get_best_move_method=lambda board: np.random.choice([board.legal_moves]))
+>>> server.run()
+INFO:     Started server process [1617]
+INFO:     Waiting for application startup.
+INFO:     Application startup complete.
+INFO:     Uvicorn running on http://127.0.0.1:8000 (Press CTRL+C to quit)
+```
 
-.. code-block:: python
+_It is as simple as that!_
 
-    import draughts.base as draughts
-    import numpy as np
-    CUSTOM_POSITION = np.array([1] * 20 + [-1] * 12, dtype=np.int8)
-    board = draughts.BaseBoard(starting_position=CUSTOM_POSITION)
-    board.legal_moves = ... # create your own custom legal_moves method (property)
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/a5e2ca89-28e1-4dcc-96ae-b18fc602c9bc" width="600" />
 
-UI
---
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/b14523ea-4bc4-45e1-b5c0-5deea3ed5328" width="600" />
 
-.. code-block:: python
+*Legal moves for selected square (on image "16")*
 
-    from draughts.server import Server
-    Server().run()
+<img src="https://github.com/michalskibinski109/py-draughts/assets/77834536/c8245cbc-06ec-4623-81ab-c9aaa9302627" width="600" />
 
-*It is as simple as that!*
 
-
-.. image:: https://github.com/michalskibinski109/draughts/assets/77834536/4ec36e49-38cc-45e8-a500-d0d24b21fce7
-   :width: 600
-
-.. image:: https://github.com/michalskibinski109/draughts/assets/77834536/b7e0bf73-1bc5-4769-8f82-a22cde3b7e90
-   :width: 600
-
-*pseudo legal moves for selected square* 
-
-.. image:: https://github.com/michalskibinski109/draughts/assets/77834536/ef64179a-1e7d-46d4-991e-5a34fc803d7e
-   :width: 600
-
-Contributing
-------------
+## Contributing
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
-Bibliography
-------------
+## Bibliography
 
-1. `notation <https://en.wikipedia.org/wiki/Portable_Draughts_Notation>`_
-2. `rules and variants <https://en.wikipedia.org/wiki/Checkers>`_
-3. `list of pdns <https://github.com/mig0/Games-Checkers/>`_
-4. `droughts online  <https://lidraughts.org/>`_
-5. `additional 1 (checkers online) <https://checkers.online/play>`_
-6. `additional 2 (chinook) <https://webdocs.cs.ualberta.ca/~chinook/play/notation.html>`_
+1. [Notation](https://en.wikipedia.org/wiki/Portable_Draughts_Notation)
+2. [Rules and variants](https://en.wikipedia.org/wiki/Checkers)
+3. [List of PDNs](https://github.com/mig0/Games-Checkers/)
+4. [Draughts online](https://lidraughts.org/)
+5. [Additional 1 (Checkers online)](https://checkers.online/play)
+6. [Additional 2 (Chinook)](https://webdocs.cs.ualberta.ca/~chinook/play/notation.html)
```

### Comparing `py-draughts-0.3.1/py_draughts.egg-info/SOURCES.txt` & `py-draughts-0.9.0/py_draughts.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 LICENSE
 MANIFEST.in
-README.rst
+README.md
 requirements.txt
 setup.py
 draughts/__init__.py
 draughts/american.py
 draughts/base.py
 draughts/models.py
 draughts/move.py
@@ -14,10 +14,11 @@
 draughts/static/css/style.css
 draughts/static/js/script.js
 draughts/templates/base.html
 draughts/templates/index.html
 py_draughts.egg-info/PKG-INFO
 py_draughts.egg-info/SOURCES.txt
 py_draughts.egg-info/dependency_links.txt
+py_draughts.egg-info/requires.txt
 py_draughts.egg-info/top_level.txt
 test/test_american_board.py
 test/test_board.py
```

### Comparing `py-draughts-0.3.1/setup.py` & `py-draughts-0.9.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 from pathlib import Path
 
 import setuptools
 
 from draughts.__init__ import __doc__, __version__
 
 this_directory = Path(__file__).parent
-long_description = (this_directory / "readme.rst").read_text()
+long_description = (this_directory / "readme.md").read_text()
 
 with open(this_directory / "requirements.txt") as f:
     requirements = f.read().splitlines()
 
+
 setuptools.setup(
     name="py-draughts",
     version=__version__,
     author="Michał Skibiński",
     author_email="mskibinski109@gmail.com",
     description=__doc__.replace("\n", " ").strip(),
     long_description=long_description,
     # rst
-    long_description_content_type="text/x-rst",
+    long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     package_data={"draughts": ["static/js/*", "static/css/*", "templates/*"]},
-    requires=requirements,
+    install_requires=requirements,
     license="GPL-3.0+",
     keywords=" draughts, checkers, AI mini-max, game, board",
     url="https://github.com/michalskibinski109/draughts",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
```

### Comparing `py-draughts-0.3.1/test/test_american_board.py` & `py-draughts-0.9.0/test/test_american_board.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.3.1/test/test_board.py` & `py-draughts-0.9.0/test/test_board.py`

 * *Files identical despite different names*

