# Comparing `tmp/fast-checkers-0.2.0.tar.gz` & `tmp/fast-checkers-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast-checkers-0.2.0.tar", last modified: Thu Jul  6 20:06:16 2023, max compression
+gzip compressed data, was "fast-checkers-0.3.0.tar", last modified: Tue Jul 11 09:05:46 2023, max compression
```

## Comparing `fast-checkers-0.2.0.tar` & `fast-checkers-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-07-06 20:06:16.818050 fast-checkers-0.2.0/
--rw-rw-rw-   0        0        0       18 2023-07-06 19:57:20.000000 fast-checkers-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5211 2023-07-06 20:06:16.817050 fast-checkers-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3834 2023-07-06 20:05:16.000000 fast-checkers-0.2.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-06 20:06:16.803058 fast-checkers-0.2.0/checkers/
--rw-rw-rw-   0        0        0      947 2023-07-06 19:56:06.000000 fast-checkers-0.2.0/checkers/__init__.py
--rw-rw-rw-   0        0        0     3780 2023-07-06 19:54:23.000000 fast-checkers-0.2.0/checkers/american.py
--rw-rw-rw-   0        0        0     6038 2023-07-06 19:55:03.000000 fast-checkers-0.2.0/checkers/base.py
--rw-rw-rw-   0        0        0     1441 2023-07-06 19:40:43.000000 fast-checkers-0.2.0/checkers/main.py
--rw-rw-rw-   0        0        0      674 2023-07-06 19:46:12.000000 fast-checkers-0.2.0/checkers/models.py
--rw-rw-rw-   0        0        0     4120 2023-07-06 18:18:47.000000 fast-checkers-0.2.0/checkers/move.py
--rw-rw-rw-   0        0        0       65 2023-06-18 11:52:25.000000 fast-checkers-0.2.0/checkers/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-06 20:06:16.812048 fast-checkers-0.2.0/fast_checkers.egg-info/
--rw-rw-rw-   0        0        0     5211 2023-07-06 20:06:16.000000 fast-checkers-0.2.0/fast_checkers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2023-07-06 20:06:16.000000 fast-checkers-0.2.0/fast_checkers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-06 20:06:16.000000 fast-checkers-0.2.0/fast_checkers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-06 20:06:16.000000 fast-checkers-0.2.0/fast_checkers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-06 20:06:16.818050 fast-checkers-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1723 2023-07-06 15:59:26.000000 fast-checkers-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-06 20:06:16.816048 fast-checkers-0.2.0/test/
--rw-rw-rw-   0        0        0     1123 2023-07-06 16:45:41.000000 fast-checkers-0.2.0/test/test_american_board.py
--rw-rw-rw-   0        0        0     2375 2023-07-06 15:09:38.000000 fast-checkers-0.2.0/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:05:46.965417 fast-checkers-0.3.0/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 08:33:07.000000 fast-checkers-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0       44 2023-07-11 08:55:47.000000 fast-checkers-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5712 2023-07-11 09:05:46.962423 fast-checkers-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4257 2023-07-11 08:33:07.000000 fast-checkers-0.3.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-11 09:05:46.911268 fast-checkers-0.3.0/checkers/
+-rw-rw-rw-   0        0        0      947 2023-07-11 09:05:03.000000 fast-checkers-0.3.0/checkers/__init__.py
+-rw-rw-rw-   0        0        0     3838 2023-07-10 08:43:08.000000 fast-checkers-0.3.0/checkers/american.py
+-rw-rw-rw-   0        0        0     7204 2023-07-11 08:33:07.000000 fast-checkers-0.3.0/checkers/base.py
+-rw-rw-rw-   0        0        0     1627 2023-07-10 08:43:08.000000 fast-checkers-0.3.0/checkers/main.py
+-rw-rw-rw-   0        0        0      674 2023-07-07 08:25:35.000000 fast-checkers-0.3.0/checkers/models.py
+-rw-rw-rw-   0        0        0     4120 2023-07-07 08:25:35.000000 fast-checkers-0.3.0/checkers/move.py
+-rw-rw-rw-   0        0        0     4363 2023-07-11 08:33:07.000000 fast-checkers-0.3.0/checkers/server.py
+-rw-rw-rw-   0        0        0     2340 2023-07-11 08:33:07.000000 fast-checkers-0.3.0/checkers/standard.py
+-rw-rw-rw-   0        0        0     1968 2023-07-11 08:33:07.000000 fast-checkers-0.3.0/checkers/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:05:46.939178 fast-checkers-0.3.0/fast_checkers.egg-info/
+-rw-rw-rw-   0        0        0     5712 2023-07-11 09:05:42.000000 fast-checkers-0.3.0/fast_checkers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      421 2023-07-11 09:05:45.000000 fast-checkers-0.3.0/fast_checkers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 09:05:42.000000 fast-checkers-0.3.0/fast_checkers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-11 09:05:42.000000 fast-checkers-0.3.0/fast_checkers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       27 2023-07-05 07:24:19.000000 fast-checkers-0.3.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 09:05:46.966437 fast-checkers-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2005 2023-07-11 08:55:38.000000 fast-checkers-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:05:46.955657 fast-checkers-0.3.0/test/
+-rw-rw-rw-   0        0        0     1123 2023-07-07 08:25:35.000000 fast-checkers-0.3.0/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2376 2023-07-11 08:33:07.000000 fast-checkers-0.3.0/test/test_board.py
```

### Comparing `fast-checkers-0.2.0/PKG-INFO` & `fast-checkers-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-checkers
-Version: 0.2.0
+Version: 0.3.0
 Summary: A checkers library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
 Home-page: https://github.com/michalskibinski109/checkers
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/checkers/index.html
 Keywords: checkers AI mini-max droughts,game,board
@@ -19,30 +19,34 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
+Requires: numpy
+Requires: easy_logs
+Requires: fastapi
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 
 Fast Checkers
 =============
 
 .. image:: https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg
    :target: https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml
 
 .. image:: https://badge.fury.io/py/fast_checkers.svg
    :target: https://badge.fury.io/py/fast_checkers
 
 Checkers
 --------
 
-**Project still under active development. Usage may be different in future versions**
+*Project still under active developement. Still lacking some important functionality.*
 
 Efficient Modern and flexible implementation of checkers game with beautiful web interface. Supports multiple variants of the game and allows to play against AI.
 
 Documentation
 -------------
 
 `Documentation <https://michalskibinski109.github.io/checkers/>`_
@@ -128,25 +132,40 @@
     CUSTOM_POSITION = np.array([1] * 20 + [-1] * 12, dtype=np.int8)
     board = checkers.BaseBoard(starting_position=CUSTOM_POSITION)
     board.legal_moves = ... # create your own custom legal_moves method (property)
 
 UI
 --
 
-**for now UI is mostly used for debugging purpose**
+.. code-block:: python
+
+    from checkers.server import Server
+    Server().run()
+
+*It is as simple as that!*
+
+
+.. image:: https://github.com/michalskibinski109/checkers/assets/77834536/4ec36e49-38cc-45e8-a500-d0d24b21fce7
+   :width: 600
+
+.. image:: https://github.com/michalskibinski109/checkers/assets/77834536/b7e0bf73-1bc5-4769-8f82-a22cde3b7e90
+   :width: 600
+
+*pseudo legal moves for selected square* 
 
-.. image:: https://github.com/michalskibinski109/checkers/assets/77834536/acae0786-9cf3-4e30-9a04-abd7c018202b
-   :width: 400
+.. image:: https://github.com/michalskibinski109/checkers/assets/77834536/ef64179a-1e7d-46d4-991e-5a34fc803d7e
+   :width: 600
 
 Contributing
 ------------
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
 Bibliography
 ------------
 
 1. `notation <https://en.wikipedia.org/wiki/Portable_Draughts_Notation>`_
 2. `rules and variants <https://en.wikipedia.org/wiki/Checkers>`_
 3. `list of pdns <https://github.com/mig0/Games-Checkers/>`_
-4. `additional 1 (checkers online) <https://checkers.online/play>`_
-5. `additional 2 (chinook) <https://webdocs.cs.ualberta.ca/~chinook/play/notation.html>`_
+4. `droughts online  <https://lidraughts.org/>`_
+5. `additional 1 (checkers online) <https://checkers.online/play>`_
+6. `additional 2 (chinook) <https://webdocs.cs.ualberta.ca/~chinook/play/notation.html>`_
```

### Comparing `fast-checkers-0.2.0/README.rst` & `fast-checkers-0.3.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 .. image:: https://badge.fury.io/py/fast_checkers.svg
    :target: https://badge.fury.io/py/fast_checkers
 
 Checkers
 --------
 
-**Project still under active development. Usage may be different in future versions**
+*Project still under active developement. Still lacking some important functionality.*
 
 Efficient Modern and flexible implementation of checkers game with beautiful web interface. Supports multiple variants of the game and allows to play against AI.
 
 Documentation
 -------------
 
 `Documentation <https://michalskibinski109.github.io/checkers/>`_
@@ -100,25 +100,40 @@
     CUSTOM_POSITION = np.array([1] * 20 + [-1] * 12, dtype=np.int8)
     board = checkers.BaseBoard(starting_position=CUSTOM_POSITION)
     board.legal_moves = ... # create your own custom legal_moves method (property)
 
 UI
 --
 
-**for now UI is mostly used for debugging purpose**
+.. code-block:: python
+
+    from checkers.server import Server
+    Server().run()
+
+*It is as simple as that!*
+
+
+.. image:: https://github.com/michalskibinski109/checkers/assets/77834536/4ec36e49-38cc-45e8-a500-d0d24b21fce7
+   :width: 600
+
+.. image:: https://github.com/michalskibinski109/checkers/assets/77834536/b7e0bf73-1bc5-4769-8f82-a22cde3b7e90
+   :width: 600
+
+*pseudo legal moves for selected square* 
 
-.. image:: https://github.com/michalskibinski109/checkers/assets/77834536/acae0786-9cf3-4e30-9a04-abd7c018202b
-   :width: 400
+.. image:: https://github.com/michalskibinski109/checkers/assets/77834536/ef64179a-1e7d-46d4-991e-5a34fc803d7e
+   :width: 600
 
 Contributing
 ------------
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
 Bibliography
 ------------
 
 1. `notation <https://en.wikipedia.org/wiki/Portable_Draughts_Notation>`_
 2. `rules and variants <https://en.wikipedia.org/wiki/Checkers>`_
 3. `list of pdns <https://github.com/mig0/Games-Checkers/>`_
-4. `additional 1 (checkers online) <https://checkers.online/play>`_
-5. `additional 2 (chinook) <https://webdocs.cs.ualberta.ca/~chinook/play/notation.html>`_
+4. `droughts online  <https://lidraughts.org/>`_
+5. `additional 1 (checkers online) <https://checkers.online/play>`_
+6. `additional 2 (chinook) <https://webdocs.cs.ualberta.ca/~chinook/play/notation.html>`_
```

### Comparing `fast-checkers-0.2.0/checkers/__init__.py` & `fast-checkers-0.3.0/checkers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """
 A checkers library for Python, with move generation and validation,
 PDN parsing and writing. Supprots multiple variants of game.
 """
 
-__version__ = "0.2.0"
+__version__ = "0.3.0"
 __author__ = "Michał Skibiński"
```

### Comparing `fast-checkers-0.2.0/checkers/american.py` & `fast-checkers-0.3.0/checkers/american.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from __future__ import annotations
 
 from typing import Generator
 
 import numpy as np
-
 from checkers.base import BaseBoard
 from checkers.models import Color, Entity
 from checkers.move import Move
 from checkers.utils import logger
 
 
 # fmt: off
@@ -29,15 +28,17 @@
 
      - Board size: 8x8
      - Short moves only
      - Only the king can capture backwards
      - Capture - choose any
     """
 
+    GAME_TYPE = 23
     STARTING_POSITION = np.array([1] * 12 + [0] * 8 + [-1] * 12, dtype=np.int8)
+    VARIANT_NAME = "American checkers"
     size = int(np.sqrt(len(STARTING_POSITION) * 2))
     row_idx = {val: val // 4 for val in range(len(STARTING_POSITION))}
     col_idx = {val: val % 8 for val in range(len(STARTING_POSITION))}
 
     def __init__(self, starting_position=STARTING_POSITION) -> None:
         super().__init__(starting_position)
 
@@ -57,15 +58,15 @@
     ) -> Generator[Move, None, None]:
         row = self.row_idx[square]
         moves = []
         odd = bool(row % 2 != 0 and self.turn == Color.BLACK) or (
             row % 2 == 0 and self.turn == Color.WHITE
         )
         is_king = bool(self[square] == self.turn.value * Entity.KING)
-        # is_king = False  # DEBUF
+        # is_king = False  # DEBUG
         for mv_offset, cap_offset, dir in [
             (4 - odd, 7, self.turn.value),
             (5 - odd, 9, self.turn.value),
         ] + is_king * [
             (4 - (not odd), 7, -self.turn.value),
             (5 - (not odd), 9, -self.turn.value),
         ]:
```

### Comparing `fast-checkers-0.2.0/checkers/base.py` & `fast-checkers-0.3.0/checkers/base.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,20 +3,24 @@
 
 """
 
 from __future__ import annotations
 
 from abc import ABC
 from typing import Generator
-
+from collections import defaultdict
 import numpy as np
 
-from checkers.models import ENTITY_REPR, STARTING_POSITION, Color, Entity, SquareT
+from checkers.models import ENTITY_REPR, Color, Entity, SquareT
 from checkers.move import Move
-from checkers.utils import logger
+from checkers.utils import (
+    logger,
+    get_king_pseudo_legal_moves,
+    get_man_pseudo_legal_moves,
+)
 
 # fmt: off
 SQUARES = [_, B8, D8, F8, H8,
         A7, C7, E7, G7,
         B6, D6, F6, H6,
         A5, C5, E5, G5,
         B4, D4, F4, H4,
@@ -41,14 +45,21 @@
 
     Constraints:
     - There are only two colors: ``Color.WHITE`` and ``Color.BLACK``
     - There are only two types of pieces: ``PieceType.MAN`` and ``PieceType.KING``
     - Board should always be square.
     """
 
+    GAME_TYPE = -1
+    VARIANT_NAME = "Abstract variant"
+    STARTING_POSITION = np.array([1] * 12 + [0] * 8 + [-1] * 12, dtype=np.int8)
+    STARTING_COLOR = Color.WHITE
+    PSEUDO_LEGAL_KING_MOVES = get_king_pseudo_legal_moves(len(STARTING_POSITION))
+    PSEUDO_LEGAL_MAN_MOVES = get_man_pseudo_legal_moves(len(STARTING_POSITION))
+
     def __init__(self, starting_position: np.ndarray) -> None:
         """
         Initializes the board with a starting position.
         The starting position must be a numpy array of length n * n/2,
         where n is the size of the board.
 
         """
@@ -72,21 +83,25 @@
         pass
 
     @property
     def position(self) -> np.ndarray:
         """Returns board position."""
         return self._pos
 
+    @property
+    def is_game_over(self) -> bool:
+        """Returns ``True`` if the game is over."""
+        return not bool(list(self.legal_moves))
+
     def push(self, move: Move, is_finished: bool = True) -> None:
         """Pushes a move to the board.
         Automatically promotes a piece if it reaches the last row.
 
         If ``is_finished`` is set to ``True``, the turn is switched. This parameter is used only
         for generating legal moves.
-
         """
         src, tg = (
             move.square_list[0],
             move.square_list[-1],
         )
         self._pos[src], self._pos[tg] = self._pos[tg], self._pos[src]
         # is promotion
@@ -163,24 +178,50 @@
     def __iter__(self) -> Generator[Entity, None, None]:
         for sq in self.position:
             yield sq
 
     def __getitem__(self, key: SquareT) -> Entity:
         return self.position[key]
 
+    @classmethod
+    @property
+    def info(cls) -> str:
+        board_size = int(np.sqrt(cls.STARTING_POSITION.shape[0]))
+        data = (
+            f'[GameType "{cls.GAME_TYPE}"]\n'
+            f'[Variant "{cls.VARIANT_NAME}"]\n'
+            f'[BoardSize "{board_size} X {board_size}"]\n'
+            f'[StartingColor "{cls.STARTING_COLOR}"]\n'
+        )
+        return data
+
+
+# if __name__ == "__main__":
+#     board = BaseBoard(STARTING_POSITION)
+#     print(board.info)
+#     m1 = Move([C3, B4])
+#     board.push(m1)
+
+#     m2 = Move([B6, A5])
+#     board.push(m2)
+
+#     m3 = Move([G3, H4])
+#     board.push(m3)
+#     print(board)
+
+#     m4 = Move([A5, C3], captured_list=[B4])
+#     board.push(m4)
+#     print(board)
+
+
+def foo(a):
+    return a * 2
 
-if __name__ == "__main__":
-    board = BaseBoard(STARTING_POSITION)
 
-    m1 = Move([C3, B4])
-    board.push(m1)
+class A:
+    B = [1, 2, 3]
+    C = B * 2
+    for a in range(len(B)):
+        print(a)
 
-    m2 = Move([B6, A5])
-    board.push(m2)
 
-    m3 = Move([G3, H4])
-    board.push(m3)
-    print(board)
-
-    m4 = Move([A5, C3], captured_list=[B4])
-    board.push(m4)
-    print(board)
+A()
```

### Comparing `fast-checkers-0.2.0/checkers/main.py` & `fast-checkers-0.3.0/checkers/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 import numpy as np
 import uvicorn
 from fastapi import FastAPI, Request
+import json
 from fastapi.staticfiles import StaticFiles
 from fastapi.templating import Jinja2Templates
-
-from checkers.american import Board
+from pprint import pprint
+from checkers.standard import Board
 
 templates = Jinja2Templates(directory="checkers/templates/")
 
 app = FastAPI()
 # STARTING_POSITION = np.array([0] * 8 + [10] * 8 + [-10] * 8 + [0] * 8, dtype=np.int8)
 
 # board = Board(STARTING_POSITION)
 board = Board()
 app.mount("/static", StaticFiles(directory="checkers/static"), name="static")
 
 
 @app.get("/")
 def index(request: Request):
+    pprint(board.PSEUDO_LEGAL_KING_MOVES)
     return templates.TemplateResponse(
         "index.html",
-        {"request": request, "board": board.friendly_form.reshape(8, 8).tolist()},
+        {
+            "request": request,
+            "board": board.friendly_form.reshape(10, 10).tolist(),
+            "debug": json.dumps(board.PSEUDO_LEGAL_KING_MOVES),
+        },
     )
 
 
 @app.get("/random_move")
 def random_move(request: Request):
     moves = list(board.legal_moves)
     # get move wiht longest capture chain
```

### Comparing `fast-checkers-0.2.0/checkers/models.py` & `fast-checkers-0.3.0/checkers/models.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.2.0/checkers/move.py` & `fast-checkers-0.3.0/checkers/move.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.2.0/fast_checkers.egg-info/PKG-INFO` & `fast-checkers-0.3.0/fast_checkers.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-checkers
-Version: 0.2.0
+Version: 0.3.0
 Summary: A checkers library for Python, with move generation and validation, PDN parsing and writing. Supprots multiple variants of game.
 Home-page: https://github.com/michalskibinski109/checkers
 Author: Michał Skibiński
 Author-email: mskibinski109@gmail.com
 License: GPL-3.0+
 Project-URL: Documentation, https://michalskibinski109.github.io/checkers/index.html
 Keywords: checkers AI mini-max droughts,game,board
@@ -19,30 +19,34 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Games/Entertainment :: Board Games
 Classifier: Topic :: Games/Entertainment :: Turn Based Strategy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
+Requires: numpy
+Requires: easy_logs
+Requires: fastapi
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
+License-File: LICENSE
 
 Fast Checkers
 =============
 
 .. image:: https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml/badge.svg
    :target: https://github.com/michalskibinski109/checkers/actions/workflows/python-app.yml
 
 .. image:: https://badge.fury.io/py/fast_checkers.svg
    :target: https://badge.fury.io/py/fast_checkers
 
 Checkers
 --------
 
-**Project still under active development. Usage may be different in future versions**
+*Project still under active developement. Still lacking some important functionality.*
 
 Efficient Modern and flexible implementation of checkers game with beautiful web interface. Supports multiple variants of the game and allows to play against AI.
 
 Documentation
 -------------
 
 `Documentation <https://michalskibinski109.github.io/checkers/>`_
@@ -128,25 +132,40 @@
     CUSTOM_POSITION = np.array([1] * 20 + [-1] * 12, dtype=np.int8)
     board = checkers.BaseBoard(starting_position=CUSTOM_POSITION)
     board.legal_moves = ... # create your own custom legal_moves method (property)
 
 UI
 --
 
-**for now UI is mostly used for debugging purpose**
+.. code-block:: python
+
+    from checkers.server import Server
+    Server().run()
+
+*It is as simple as that!*
+
+
+.. image:: https://github.com/michalskibinski109/checkers/assets/77834536/4ec36e49-38cc-45e8-a500-d0d24b21fce7
+   :width: 600
+
+.. image:: https://github.com/michalskibinski109/checkers/assets/77834536/b7e0bf73-1bc5-4769-8f82-a22cde3b7e90
+   :width: 600
+
+*pseudo legal moves for selected square* 
 
-.. image:: https://github.com/michalskibinski109/checkers/assets/77834536/acae0786-9cf3-4e30-9a04-abd7c018202b
-   :width: 400
+.. image:: https://github.com/michalskibinski109/checkers/assets/77834536/ef64179a-1e7d-46d4-991e-5a34fc803d7e
+   :width: 600
 
 Contributing
 ------------
 
 Contributions to this project are welcome. If you encounter any issues or have suggestions for improvements, please open an issue or submit a pull request on the project repository.
 
 Bibliography
 ------------
 
 1. `notation <https://en.wikipedia.org/wiki/Portable_Draughts_Notation>`_
 2. `rules and variants <https://en.wikipedia.org/wiki/Checkers>`_
 3. `list of pdns <https://github.com/mig0/Games-Checkers/>`_
-4. `additional 1 (checkers online) <https://checkers.online/play>`_
-5. `additional 2 (chinook) <https://webdocs.cs.ualberta.ca/~chinook/play/notation.html>`_
+4. `droughts online  <https://lidraughts.org/>`_
+5. `additional 1 (checkers online) <https://checkers.online/play>`_
+6. `additional 2 (chinook) <https://webdocs.cs.ualberta.ca/~chinook/play/notation.html>`_
```

### Comparing `fast-checkers-0.2.0/setup.py` & `fast-checkers-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,25 +3,36 @@
 import setuptools
 
 from checkers.__init__ import __doc__, __version__
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "readme.rst").read_text()
 
+with open(this_directory /'requirements.txt') as f:
+    requirements = f.read().splitlines()
+
 setuptools.setup(
     name="fast-checkers",
     version=__version__,
     author="Michał Skibiński",
     author_email="mskibinski109@gmail.com",
     files_to_include=["checkers"],
     description=__doc__.replace("\n", " ").strip(),
     long_description=long_description,
     # rst
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(),
+    package_data={
+        'checkers': [
+        "checkers/static/js/*",
+        "checkers/static/css/*",
+        "checkers/templates/*"
+    ]
+    },
+    requires=requirements,
     license="GPL-3.0+",
     keywords="checkers AI mini-max droughts, game, board",
     url="https://github.com/michalskibinski109/checkers",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
```

### Comparing `fast-checkers-0.2.0/test/test_american_board.py` & `fast-checkers-0.3.0/test/test_american_board.py`

 * *Files identical despite different names*

### Comparing `fast-checkers-0.2.0/test/test_board.py` & `fast-checkers-0.3.0/test/test_board.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import numpy as np
 import pytest
 
 import checkers.base as checkers
-from checkers.base import STARTING_POSITION, BaseBoard, Color, Entity, Move
+from checkers.base import BaseBoard, Color, Entity, Move
 
 
 class TestBoard:
     @pytest.fixture(autouse=True)
     def setup(self):
-        self.board = BaseBoard(STARTING_POSITION)
+        self.board = BaseBoard(BaseBoard.STARTING_POSITION)
         yield
         del self.board
 
     def test_init(self):
         assert self.board.turn == Color.WHITE
-        assert np.array_equal(self.board.position, STARTING_POSITION)
+        assert np.array_equal(self.board.position, BaseBoard.STARTING_POSITION)
 
     def test_move(self):
         m = Move([checkers.A3, checkers.B4])
         self.board.push(m)
         assert self.board.turn == Color.BLACK
         assert self.board[checkers.A3] == Entity.EMPTY
         assert self.board[checkers.B4] == Entity.WHITE_MAN
```

