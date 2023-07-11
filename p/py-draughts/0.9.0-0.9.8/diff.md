# Comparing `tmp/py-draughts-0.9.0.tar.gz` & `tmp/py-draughts-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-draughts-0.9.0.tar", last modified: Tue Jul 11 18:13:32 2023, max compression
+gzip compressed data, was "py-draughts-0.9.8.tar", last modified: Tue Jul 11 20:04:44 2023, max compression
```

## Comparing `py-draughts-0.9.0.tar` & `py-draughts-0.9.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 18:13:32.796215 py-draughts-0.9.0/
--rw-rw-rw-   0        0        0    35823 2023-07-11 12:53:30.000000 py-draughts-0.9.0/LICENSE
--rw-rw-rw-   0        0        0       43 2023-07-11 18:05:22.000000 py-draughts-0.9.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5743 2023-07-11 18:13:32.795218 py-draughts-0.9.0/PKG-INFO
--rw-rw-rw-   0        0        0     4342 2023-07-11 18:11:30.000000 py-draughts-0.9.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-11 18:13:32.772208 py-draughts-0.9.0/draughts/
--rw-rw-rw-   0        0        0      945 2023-07-11 18:13:19.000000 py-draughts-0.9.0/draughts/__init__.py
--rw-rw-rw-   0        0        0     3838 2023-07-11 16:12:53.000000 py-draughts-0.9.0/draughts/american.py
--rw-rw-rw-   0        0        0     7825 2023-07-11 16:29:47.000000 py-draughts-0.9.0/draughts/base.py
--rw-rw-rw-   0        0        0      674 2023-07-11 16:40:27.000000 py-draughts-0.9.0/draughts/models.py
--rw-rw-rw-   0        0        0     4191 2023-07-11 17:16:02.000000 py-draughts-0.9.0/draughts/move.py
--rw-rw-rw-   0        0        0     6490 2023-07-11 18:10:09.000000 py-draughts-0.9.0/draughts/server.py
--rw-rw-rw-   0        0        0     5851 2023-07-11 17:24:52.000000 py-draughts-0.9.0/draughts/standard.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:13:32.738914 py-draughts-0.9.0/draughts/static/
-drwxrwxrwx   0        0        0        0 2023-07-11 18:13:32.774208 py-draughts-0.9.0/draughts/static/css/
--rw-rw-rw-   0        0        0     2814 2023-07-11 12:56:50.000000 py-draughts-0.9.0/draughts/static/css/style.css
-drwxrwxrwx   0        0        0        0 2023-07-11 18:13:32.776208 py-draughts-0.9.0/draughts/static/js/
--rw-rw-rw-   0        0        0     5824 2023-07-11 15:13:38.000000 py-draughts-0.9.0/draughts/static/js/script.js
-drwxrwxrwx   0        0        0        0 2023-07-11 18:13:32.778212 py-draughts-0.9.0/draughts/templates/
--rw-rw-rw-   0        0        0     1860 2023-07-11 16:32:17.000000 py-draughts-0.9.0/draughts/templates/base.html
--rw-rw-rw-   0        0        0     2500 2023-07-11 13:56:11.000000 py-draughts-0.9.0/draughts/templates/index.html
--rw-rw-rw-   0        0        0     1973 2023-07-11 13:47:51.000000 py-draughts-0.9.0/draughts/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:13:32.790230 py-draughts-0.9.0/py_draughts.egg-info/
--rw-rw-rw-   0        0        0     5743 2023-07-11 18:13:32.000000 py-draughts-0.9.0/py_draughts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      547 2023-07-11 18:13:32.000000 py-draughts-0.9.0/py_draughts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 18:13:32.000000 py-draughts-0.9.0/py_draughts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-07-11 18:13:32.000000 py-draughts-0.9.0/py_draughts.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-11 18:13:32.000000 py-draughts-0.9.0/py_draughts.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 17:26:06.000000 py-draughts-0.9.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 18:13:32.796215 py-draughts-0.9.0/setup.cfg
--rw-rw-rw-   0        0        0     1906 2023-07-11 17:45:47.000000 py-draughts-0.9.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:13:32.792215 py-draughts-0.9.0/test/
--rw-rw-rw-   0        0        0     1123 2023-07-11 16:12:53.000000 py-draughts-0.9.0/test/test_american_board.py
--rw-rw-rw-   0        0        0     2376 2023-07-11 16:12:53.000000 py-draughts-0.9.0/test/test_board.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:04:44.241716 py-draughts-0.9.8/
+-rw-rw-rw-   0        0        0    35823 2023-07-11 18:56:31.000000 py-draughts-0.9.8/LICENSE
+-rw-rw-rw-   0        0        0       43 2023-07-11 18:56:31.000000 py-draughts-0.9.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     5460 2023-07-11 20:04:44.240737 py-draughts-0.9.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4059 2023-07-11 19:54:28.000000 py-draughts-0.9.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 20:04:44.206715 py-draughts-0.9.8/draughts/
+-rw-rw-rw-   0        0        0      945 2023-07-11 19:54:55.000000 py-draughts-0.9.8/draughts/__init__.py
+-rw-rw-rw-   0        0        0     3838 2023-07-11 18:56:31.000000 py-draughts-0.9.8/draughts/american.py
+-rw-rw-rw-   0        0        0     9140 2023-07-11 19:58:36.000000 py-draughts-0.9.8/draughts/base.py
+-rw-rw-rw-   0        0        0      674 2023-07-11 19:49:33.000000 py-draughts-0.9.8/draughts/models.py
+-rw-rw-rw-   0        0        0     4191 2023-07-11 18:56:31.000000 py-draughts-0.9.8/draughts/move.py
+-rw-rw-rw-   0        0        0     5098 2023-07-11 19:36:47.000000 py-draughts-0.9.8/draughts/server.py
+-rw-rw-rw-   0        0        0     5873 2023-07-11 19:34:13.000000 py-draughts-0.9.8/draughts/standard.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:04:44.139998 py-draughts-0.9.8/draughts/static/
+drwxrwxrwx   0        0        0        0 2023-07-11 20:04:44.208716 py-draughts-0.9.8/draughts/static/css/
+-rw-rw-rw-   0        0        0     2782 2023-07-11 19:06:37.000000 py-draughts-0.9.8/draughts/static/css/style.css
+drwxrwxrwx   0        0        0        0 2023-07-11 20:04:44.212720 py-draughts-0.9.8/draughts/static/js/
+-rw-rw-rw-   0        0        0     5824 2023-07-11 18:56:31.000000 py-draughts-0.9.8/draughts/static/js/script.js
+drwxrwxrwx   0        0        0        0 2023-07-11 20:04:44.219716 py-draughts-0.9.8/draughts/templates/
+-rw-rw-rw-   0        0        0     1860 2023-07-11 18:56:31.000000 py-draughts-0.9.8/draughts/templates/base.html
+-rw-rw-rw-   0        0        0     2500 2023-07-11 19:06:02.000000 py-draughts-0.9.8/draughts/templates/index.html
+-rw-rw-rw-   0        0        0     1973 2023-07-11 18:56:31.000000 py-draughts-0.9.8/draughts/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:04:44.233714 py-draughts-0.9.8/py_draughts.egg-info/
+-rw-rw-rw-   0        0        0     5460 2023-07-11 20:04:44.000000 py-draughts-0.9.8/py_draughts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      547 2023-07-11 20:04:44.000000 py-draughts-0.9.8/py_draughts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 20:04:44.000000 py-draughts-0.9.8/py_draughts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-07-11 20:04:44.000000 py-draughts-0.9.8/py_draughts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-11 20:04:44.000000 py-draughts-0.9.8/py_draughts.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 18:56:31.000000 py-draughts-0.9.8/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 20:04:44.241716 py-draughts-0.9.8/setup.cfg
+-rw-rw-rw-   0        0        0     1906 2023-07-11 18:56:31.000000 py-draughts-0.9.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 20:04:44.238715 py-draughts-0.9.8/test/
+-rw-rw-rw-   0        0        0     1123 2023-07-11 18:56:31.000000 py-draughts-0.9.8/test/test_american_board.py
+-rw-rw-rw-   0        0        0     2376 2023-07-11 18:56:31.000000 py-draughts-0.9.8/test/test_board.py
```

### Comparing `py-draughts-0.9.0/LICENSE` & `py-draughts-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.0/draughts/__init__.py` & `py-draughts-0.9.8/draughts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 """
 A draughts library for Python, with move generation and validation,
 PDN parsing and writing. Supprots multiple variants of game.
 """
 
-__version__ = "0.9.0"
+__version__ = "0.9.8"
 __author__ = "Michał Skibiński"
```

### Comparing `py-draughts-0.9.0/draughts/american.py` & `py-draughts-0.9.8/draughts/american.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.0/draughts/base.py` & `py-draughts-0.9.8/draughts/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -178,60 +178,99 @@
             move = Move.from_string(str_move, self.legal_moves)
         except ValueError as e:
             logger.error(f"{e} \n {str(self)}")
             raise e
         self.push(move)
 
     @property
+    def fen(self):
+        """
+        Returns a FEN string of the board position.
+
+        ``[FEN "[Turn]:[Color 1][K][Square number][,]...]:[Color 2][K][Square number][,]...]"]``
+
+        Fen examples:
+
+        - ``[FEN "B:W18,24,27,28,K10,K15:B12,16,20,K22,K25,K29"]``
+        - ``[FEN "B:W18,19,21,23,24,26,29,30,31,32:B1,2,3,4,6,7,9,10,11,12"]``
+        """
+        COLORS_REPR = {Color.WHITE: "W", Color.BLACK: "B"}
+        fen_components = [
+            f'[FEN "{COLORS_REPR[self.turn]}:W',
+            ",".join(
+                "K" * bool(self._pos[sq] < -1) + str(sq + 1)
+                for sq in np.where(self.position < 0)[0]
+            ),
+            ":B",
+            ",".join(
+                "K" * bool(self._pos[sq] > 1) + str(sq + 1)
+                for sq in np.where(self.position > 0)[0]
+            ),
+            '"]',
+        ]
+        return "".join(fen_components)
+
+    @classmethod
+    def from_fen(cls, fen: str) -> BaseBoard:
+        # [FEN "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32"]
+        # remove everthing before W or B
+        raise NotImplementedError("Not implemented yet")
+
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
+    @property
     def friendly_form(self) -> np.ndarray:
         """
-        Really tricky method. It is used to print board in a friendly way.
-        Designed so it can be used with any board size.
+        Returns a board position in a friendly form.
+        *Makes board with size n x n from a board with size n x n/2*
         """
         new_pos = [0]
         for idx, sq in enumerate(self.position):
             new_pos.extend([0] * (idx % (self.shape[0] // 2) != 0))
             new_pos.extend([0, 0] * (idx % self.shape[0] == 0 and idx != 0))
             new_pos.append(sq)
         new_pos.append(0)
         return np.array(new_pos)
 
     def __repr__(self) -> str:
         board = ""
         position = self.friendly_form
         for i in range(self.shape[0]):
-            board += f"{'-' * (self.shape[0]*4 + 1) }\n|"
+            # board += f"{'-' * (self.shape[0]*4 + 1) }\n|"
             for j in range(self.shape[0]):
-                board += f" {ENTITY_REPR[position[i*self.shape[0] + j]]} |"
+                board += f" {ENTITY_REPR[position[i*self.shape[0] + j]]}"
             board += "\n"
         return board
 
     def __iter__(self) -> Generator[Entity, None, None]:
         for sq in self.position:
             yield sq
 
     def __getitem__(self, key: SquareT) -> Entity:
         return self.position[key]
 
-    @classmethod
-    @property
-    def info(cls) -> str:
-        board_size = int(np.sqrt(cls.STARTING_POSITION.shape[0]))
-        data = (
-            f'[GameType "{cls.GAME_TYPE}"]\n'
-            f'[Variant "{cls.VARIANT_NAME}"]\n'
-            f'[BoardSize "{board_size} X {board_size}"]\n'
-            f'[StartingColor "{cls.STARTING_COLOR}"]\n'
-        )
-        return data
 
+if __name__ == "__main__":
+    board = BaseBoard(BaseBoard.STARTING_POSITION)
+    print(board)
+    # BaseBoard.from_fen(
+    #     '[FEN "W:W4,11,28,31,K33,K34,38,40,K41,43,K44,45,K46,47:BK3,21,27,32"]'
+    # )
 
-# if __name__ == "__main__":
-#     board = BaseBoard(STARTING_POSITION)
-#     print(board.info)
+# print(board.info)
 #     m1 = Move([C3, B4])
 #     board.push(m1)
 
 #     m2 = Move([B6, A5])
 #     board.push(m2)
 
 #     m3 = Move([G3, H4])
```

### Comparing `py-draughts-0.9.0/draughts/models.py` & `py-draughts-0.9.8/draughts/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,11 +23,11 @@
     MAN = 1
     EMPTY = 0
 
 
 ENTITY_REPR = {
     Entity.BLACK_MAN: "b",
     Entity.WHITE_MAN: "w",
-    Entity.EMPTY: " ",
+    Entity.EMPTY: ".",
     Entity.BLACK_KING: "B",
     Entity.WHITE_KING: "W",
 }
```

### Comparing `py-draughts-0.9.0/draughts/move.py` & `py-draughts-0.9.8/draughts/move.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.0/draughts/standard.py` & `py-draughts-0.9.8/draughts/standard.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,7 +148,8 @@
 
 if __name__ == "__main__":
     board = Board()
     from pprint import pprint
 
     pprint(board)
     pprint(list(board.legal_moves))
+    print(board.fen)
```

### Comparing `py-draughts-0.9.0/draughts/static/css/style.css` & `py-draughts-0.9.8/draughts/static/css/style.css`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,17 @@
     overflow: hidden;
 }
 
 .board {
     display: grid;
     grid-template-columns: repeat(10, 1fr);
     grid-template-rows: repeat(10, 1fr);
-    /* grid-gap: 5px; */
-    border: 3px;
+    grid-gap: 1px;
+    border: 2px;
     height: 95%;
-    /* height: 56rem; */
 
     margin: 20px auto;
     background-color: var(--secondary);
     padding: 10px;
     border-radius: 10px;
     color: var(--light);
```

### Comparing `py-draughts-0.9.0/draughts/static/js/script.js` & `py-draughts-0.9.8/draughts/static/js/script.js`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.0/draughts/templates/base.html` & `py-draughts-0.9.8/draughts/templates/base.html`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.0/draughts/templates/index.html` & `py-draughts-0.9.8/draughts/templates/index.html`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.0/draughts/utils.py` & `py-draughts-0.9.8/draughts/utils.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.0/py_draughts.egg-info/SOURCES.txt` & `py-draughts-0.9.8/py_draughts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.0/setup.py` & `py-draughts-0.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.0/test/test_american_board.py` & `py-draughts-0.9.8/test/test_american_board.py`

 * *Files identical despite different names*

### Comparing `py-draughts-0.9.0/test/test_board.py` & `py-draughts-0.9.8/test/test_board.py`

 * *Files identical despite different names*

