# Comparing `tmp/mwxlib-0.86.0-py3-none-any.whl.zip` & `tmp/mwxlib-0.86.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 161647 bytes, number of entries: 22
+Zip file size: 164114 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat     2514 b- defN 23-Jun-23 06:26 mwx/__init__.py
--rw-rw-rw-  2.0 fat    45216 b- defN 23-Jul-05 09:18 mwx/controls.py
--rw-rw-rw-  2.0 fat    72768 b- defN 23-Jul-05 09:18 mwx/framework.py
+-rw-rw-rw-  2.0 fat    44804 b- defN 23-Jul-11 04:42 mwx/controls.py
+-rw-rw-rw-  2.0 fat    72902 b- defN 23-Jul-11 04:39 mwx/framework.py
 -rw-rw-rw-  2.0 fat    68688 b- defN 23-Jul-04 07:27 mwx/graphman.py
--rw-rw-rw-  2.0 fat    45726 b- defN 23-Jun-19 10:28 mwx/images.py
+-rw-rw-rw-  2.0 fat    49957 b- defN 23-Jul-11 09:28 mwx/images.py
 -rw-rw-rw-  2.0 fat    36005 b- defN 23-Jul-05 09:18 mwx/matplot2.py
 -rw-rw-rw-  2.0 fat    68253 b- defN 23-Jun-19 10:27 mwx/matplot2g.py
 -rw-rw-rw-  2.0 fat    27680 b- defN 23-Jul-04 05:48 mwx/matplot2lg.py
 -rw-rw-rw-  2.0 fat     6878 b- defN 23-Feb-21 08:50 mwx/mgplt.py
--rw-rw-rw-  2.0 fat   139007 b- defN 23-Jul-04 05:48 mwx/nutshell.py
--rw-rw-rw-  2.0 fat    37351 b- defN 23-Jul-03 08:45 mwx/utilus.py
+-rw-rw-rw-  2.0 fat   139236 b- defN 23-Jul-11 04:39 mwx/nutshell.py
+-rw-rw-rw-  2.0 fat    37660 b- defN 23-Jul-11 04:39 mwx/utilus.py
 -rw-rw-rw-  2.0 fat    11175 b- defN 23-Jun-20 08:11 mwx/wxmon.py
 -rw-rw-rw-  2.0 fat    19456 b- defN 23-Jun-19 10:43 mwx/wxpdb.py
 -rw-rw-rw-  2.0 fat     5372 b- defN 23-Jun-20 08:11 mwx/wxwil.py
 -rw-rw-rw-  2.0 fat     8314 b- defN 23-Jun-20 08:11 mwx/wxwit.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-23 14:06 mwx/py/__init__.py
 -rw-rw-rw-  2.0 fat    16794 b- defN 23-Jun-19 10:27 mwx/py/filling.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-05 09:19 mwxlib-0.86.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1893 b- defN 23-Jul-05 09:19 mwxlib-0.86.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-05 09:19 mwxlib-0.86.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-Jul-05 09:19 mwxlib-0.86.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1609 b- defN 23-Jul-05 09:19 mwxlib-0.86.0.dist-info/RECORD
-22 files, 615886 bytes uncompressed, 159145 bytes compressed:  74.2%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jul-11 09:30 mwxlib-0.86.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1893 b- defN 23-Jul-11 09:30 mwxlib-0.86.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 09:30 mwxlib-0.86.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-Jul-11 09:30 mwxlib-0.86.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1609 b- defN 23-Jul-11 09:30 mwxlib-0.86.2.dist-info/RECORD
+22 files, 620377 bytes uncompressed, 161612 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: mwx/py/__init__.py
 Comment: 
 
 Filename: mwx/py/filling.py
 Comment: 
 
-Filename: mwxlib-0.86.0.dist-info/LICENSE
+Filename: mwxlib-0.86.2.dist-info/LICENSE
 Comment: 
 
-Filename: mwxlib-0.86.0.dist-info/METADATA
+Filename: mwxlib-0.86.2.dist-info/METADATA
 Comment: 
 
-Filename: mwxlib-0.86.0.dist-info/WHEEL
+Filename: mwxlib-0.86.2.dist-info/WHEEL
 Comment: 
 
-Filename: mwxlib-0.86.0.dist-info/top_level.txt
+Filename: mwxlib-0.86.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mwxlib-0.86.0.dist-info/RECORD
+Filename: mwxlib-0.86.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mwx/controls.py

```diff
@@ -82,35 +82,19 @@
     
     def __float__(self):
         return float(self.value)
     
     def __len__(self):
         return len(self.range)
     
-    def bind(self, f=None, target='control'):
-        la = self.callback[target]
-        if not f:
-            return lambda f: self.bind(f, target)
-        if not callable(f):
-            raise TypeError(f"{f!r} is not callable")
-        if f not in la:
-            la.append(f)
-        return f
-    
-    def unbind(self, f=None, target='control'):
-        la = self.callback[target]
-        if not f:
-            la[:] = [a for a in la if not callable(a)]
-            return True
-        if not callable(f):
-            raise TypeError(f"{f!r} is not callable")
-        if f in la:
-            la.remove(f)
-            return True
-        return False
+    def bind(self, action=None, target='control'):
+        return self.callback.bind(target, action)
+    
+    def unbind(self, action=None, target='control'):
+        return self.callback.unbind(target, action)
     
     def reset(self, v=None, backcall=True):
         """Reset value when indexed (by knobs) with callback."""
         if v is None or v == '':
             v = self.std_value
             if v is None:
                 return
@@ -892,15 +876,17 @@
     
     return wx.NullBitmap # The standard wx controls accept this,
 
 Icon.provided_arts = _provided_arts
 Icon.custom_images = _custom_images
 
 
-def Icon2(back, fore, size, subsize=0.5):
+def Icon2(back, fore, size=None, subsize=0.6):
+    if not size:
+        size = (16,16)
     if isinstance(subsize, float):
         subsize = wx.Size(size) * subsize
     back = Icon(back, size)
     fore = Icon(fore, subsize)
     x = size[0] - subsize[0]
     y = size[1] - subsize[1]
     dc = wx.MemoryDC(back)
```

## mwx/framework.py

```diff
@@ -1,14 +1,14 @@
 #! python3
 # -*- coding: utf-8 -*-
 """mwxlib framework
 
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 """
-__version__ = "0.86.0"
+__version__ = "0.86.2"
 __author__ = "Kazuya O'moto <komoto@jeol.co.jp>"
 
 from functools import wraps, partial
 from importlib import reload
 import traceback
 import builtins
 import datetime
@@ -244,34 +244,41 @@
         
         If no action, it invalidates the key and returns @decor(binder).
         The key must be in C-M-S order (ctrl + alt(meta) + shift).
         
         Note:
             kwargs `doc` and `alias` are reserved as kw-only-args.
         """
+        assert isinstance(keymap, str)
+        assert callable(action) or action is None
+        
         map, key, state = self._get_keymap_state(keymap)
         if map not in self.handler:
             self.make_keymap(map) # make new keymap
-        if action:
-            _f = _F(action, *args, **kwargs)
-            @wraps(_f)
-            def f(*v, **kw):
-                self.message(f.__name__)
-                return _f(*v, **kw)
-            if map != state:
-                self.handler.update({map: {key: [state, self.post_command_hook, f]}})
-            else:
-                self.handler.update({map: {key: [state, f]}})
-            return action
-        else:
+        
+        if action is None:
             self.handler.update({map: {key: [state]}})
             return lambda f: self.define_key(keymap, f, *args, **kwargs)
+        
+        _f = _F(action, *args, **kwargs)
+        @wraps(_f)
+        def f(*v, **kw):
+            self.message(f.__name__)
+            return _f(*v, **kw)
+        
+        if map != state:
+            self.handler.update({map: {key: [state, self.post_command_hook, f]}})
+        else:
+            self.handler.update({map: {key: [state, f]}})
+        return action
     
     def undefine_key(self, keymap):
         """Delete [map key (pressed)] context."""
+        assert isinstance(keymap, str)
+        
         map, key, state = self._get_keymap_state(keymap)
         try:
             del self.handler[map][key]
             return True
         except KeyError:
             return False
```

## mwx/images.py

```diff
@@ -210,14 +210,27 @@
     b'ecZ5ngcrEa3YnJ/7fHehY6Kqqiq+eedgP7cH4zZ6dxZmnamKoiqGnpjTXcxj2tSVq/4qGkXR'
     b'GOlrfDcvK7TJ0qypoiiKob5G9cWsukSHoCiqamQgiiqKoE12p2YUxVBf0aiK6ybs0qbu/HJZ'
     b'MTRQFEWjuOFU3aFNnn06vLCnr1EURbHq1PF+ntIKXiz/+fDTFV/90HHNTWdOTO69fU8rYH0t'
     b'r7rzc2YUF8aOx3m0NYJWAPe76VmttzK1bzsbW0dAKwAAAID/tYu/URIDsoEAAAAASUVORK5C'
     b'YII=')
 
 #----------------------------------------------------------------------
+copy = PyEmbeddedImage(
+    b'iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABmJLR0QAAAAAAAD5Q7t/AAAA'
+    b'CXBIWXMAAAsTAAALEwEAmpwYAAAAB3RJTUUH1QoaFAgvgxQ0mwAAAX9JREFUOMuVk0tLAlEY'
+    b'ht8jM2PagP0KzwjdFv2PCFq2iKB1F/BCtrBFkXbbREREG7E2Bf4EMbM2gWUwo7+gmjAFN83t'
+    b'tGl0Rkexb/Wdw3kf3vfjO+ToJDOv6/osRijBz71trsXvnHecYRjT8ejWKHqkD/YmAbgBdtNq'
+    b'NcEY6xMRQgAAodCEJ5RzHmq1Gl6rlYXGd2NmkIv9zG7K7nmev3UBJElCsVSY+kekRRdAUZRO'
+    b'jFarOVRsR3IBKKUolgqdsyzLnuJIJNI/A8YYZFl2DdL5cFC5AJRSlMrFoQ56oZwttiwGRRnN'
+    b'QTA4jna73QXoug7GGMJhivJTaagDSiWYpoHKS6UL0LQfBAJjsCw21O7l1QUeHu/dEQSer56d'
+    b'n7oWhzHL07YoilhZXoVlmVC/VOSus+A21qN5AHnHcmwbhuHrFTtLVVXkbrIA8OzzGpKm6fD7'
+    b'/RAEAaIoghCCer0OgODj890WpxKx5BzpFR8ep7OmaS55fay/KgAoJGLJHQD4BUJZpgMViPfY'
+    b'AAAAAElFTkSuQmCC')
+
+#----------------------------------------------------------------------
 core = PyEmbeddedImage(
     b'iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAACXBIWXMAAAsTAAALEwEAmpwY'
     b'AAAABGdBTUEAALGOfPtRkwAAACBjSFJNAAB6JQAAgIMAAPn/AACA6QAAdTAAAOpgAAA6mAAA'
     b'F2+SX8VGAAACnUlEQVR42mJcsWLFfwYKAEAAmubYBmAYBIDgR2IBJLcszEJmJxo30MSSrRRp'
     b'rj35GGOQmagqIkJEMOeku1lrUVWc8z8Pe7+YGe7OFYDDMbgBGAaBmNmAldh/DyagEqgRNPRl'
     b'2fc52QdmRkTc4dDdZCZV9fty24zwHph+rguqirvzCSCwC8TExMAYGYBsBGFGRkagS34w/Pvz'
     b'hoGH+RoDw59vDH95QsAuXblyJQNAALGg++nTp08M7969A9v+/v17hocPHzKcPnOBwUSHi8FA'
@@ -243,14 +256,34 @@
     b'qImPpH13qZge9LUrmLEB1FU7sZd9jJw5MljNthYk/KLnxdFqeAjzdz9Z/z3Ck2fRE36qx9pa'
     b'kAjME1y4Lbb9GTMyTD52GUXsZO3ZadTkL6umrSD4ZZrAezvLH54Q915EjwywtXSH8FQf+t+I'
     b'9V12FLwe6wE1SmjyAi77Qb6Kt3rGe9H+hKzwrgLH9eMUPE4K3gm8jpPMjRwlHfNTLBbr7Cjo'
     b'7znA2NVOXA/PsThzi2wyah1pI+0E/9rNQQsqMtM4CyfE36fLhb2ERa0mB7BR0CElexjnGnL0'
     b'O2T2PyFunSz8jchwAAAAAElFTkSuQmCC')
 
 #----------------------------------------------------------------------
+erase = PyEmbeddedImage(
+    b'iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABGdBTUEAAK/INwWK6QAAABl0'
+    b'RVh0U29mdHdhcmUAQWRvYmUgSW1hZ2VSZWFkeXHJZTwAAAMOSURBVHjaYjx66tobAT4e9n//'
+    b'/zPAwD8g88ePnwy/f/1mePPuI9Of3//ef/78xYOZheUKExMTw+1bNxkaqjPAagECiIWdjY1b'
+    b'U02GgwEJ/Aca9uPXP4a/fxgY7t5/zMDDzcl198Hz/U+evQxlZ2c/gKwWIICYGLAARkZGBqBF'
+    b'DIxM/xiYmJkYJCRFGBysdUXUVeV3srKwhPxDOJYBIIBYsBkAkmcEYjY2Fob7Dx4zvHr5koGL'
+    b'm4Phz++/bJ8+flj979+/IqB0P0gtQABhdQHYFUxAVwBNERURYvj1j5Hh5YuPDHfuPmZg42Bj'
+    b'+PLlQxtMHUAAYXUByHYmoDf+/P7DoGugwfDrBzAwP/9kePf8OQMrKxvDqRNH4WoBAgjhgn9/'
+    b'GRiun2JguHmW4R+Q+wfojz+srAxf7t1jYOoqYmDdu46BlYsb6C1WBmZmZrg2gABCuODJLQaG'
+    b'4zsYGL5+YPj/6B7DV5sQhv8PbzIITqpiYN+7g4FT7hjDb20zBiYxaWAgI1wLEEAIAySVGRjk'
+    b'1RkY9qxjYL45n4H7zFEGpjt3GFgPH2T4LaXE8D6nkYFZRJyBlfEf1JMQABBALDD2DyYg0y6E'
+    b'gfHbTwbWFTMY2K9uZmB49Z7ht5YBw7u6qQy/FTUYmL98YQAmJnA0wwBAALHAAuEPMAgYWZkZ'
+    b'WJg4GBifvmJgePaageHzDwaGp28ZGIGxwAjyO1AfMyMsoiEAIICY/sFC/vcvBrbFkxnYOysY'
+    b'GF5/ZPhrZMHwj1uYgfXsDQZhH1cG9m1AF3FyQW1HuAAggOCxwHJkBwPr1A4GhhdvGH5FJjN8'
+    b'XriT4WvvLIb/fPwMzK9eMQgU5zIwvXrB8B8YjcgAIIAQXjBzYmB08mP4L6PC8CulEJwffvv6'
+    b'MnxYvZGBq6yA4Wt6FsM/XqBhwLSB7AWAAGKBpWtuQT4GhvbpYClWIP77F5SpgLSLHcOv8+eA'
+    b'XvzPwP31FwMLCytKIAIEEMvHT5++tnVO/sPExALNB/+APmQCav4HNuA/NGf8B3P+AzUzMXz5'
+    b'BEyWUAAQYABehgBuH0rveAAAAABJRU5ErkJggg==')
+
+#----------------------------------------------------------------------
 exit = PyEmbeddedImage(
     b'iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAABGdBTUEAAK/INwWK6QAAABl0'
     b'RVh0U29mdHdhcmUAQWRvYmUgSW1hZ2VSZWFkeXHJZTwAAAN1SURBVHjaYvz//z8DJQAggFhA'
     b'xEpGRgaQMX+B+A8DgwYLM1M+r4K8P4+8vMi/P38Y3j18+O7Fs+fbvv7+0w9Uc/kHVG070HKA'
     b'AGJBNg0omC5jZtynnpfHJeHkzPDmxQuGf6/eMIj+/yP+9MD+xFPrN8Reu3W3Gqi0D2IXAwNA'
     b'AIEN+A/hpWuEBMwwmj6TgUVEjOHTo0cM9y9dZfj76ycDCysrg4K5FYMUvyAL7+pVnYfOXwJp'
     b'6wIRAAHECAqDJYyMWpLmpmftN2/mYBEVZ3h38SLD9wcPGP6LioIN/7Z+PQM3UB3vv/8MXB/f'
@@ -401,14 +434,42 @@
     b'WgyM/2bLqEpZWHiaMumYyQLzMhPD1x8MDOzfvzCsnbQFWPj9/sUETJZfv//5//zV1y//f/3d'
     b'xcDBlsXAzPgB5MP/Z9LA5gEEEGrksTJdA2Y96yd3XritmbRl2hUjBeWwWFMGCzMxhs/AoLn1'
     b'6PPX3x9+eADD5g0w7BiAmegRAzPzN2x1BUAAMWFURSAfsLPsAiYrlRtn7+U1l6x9t3zyEYb/'
     b'n78wcHADSx8ulhsMHEDMzAiK1m+4qiaAAEINij9/GcAuAcUWKHYYwRmFC1g1tQmIcGd8/f33'
     b'ye/ff7WAEr/AsQjLoWAnQipdWFAABBgAhGIfg4WD5MwAAAAASUVORK5CYII=')
 
 #----------------------------------------------------------------------
+memo = PyEmbeddedImage(
+    b'iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAACEElEQVR4AY2TA5BbUQBFs5mO'
+    b'2kFt2xrVtm2bw9pGWNu2ubZt24y+cZtX//X9xjnPKhK9UbNOZzhrOaM5iaoO+z9Z9msvVWXR'
+    b'6s9YC4sKIMsyqoqjoyOuXb/KntWeWmJcrFYrBKQEAtsoK8yWMpSZS1FaVozi0iIUlRSgoCgP'
+    b'3t5eCAsLw6M9G/gXzRvIjxqqI+80d6j3V0BCBBaruVLJh4/vkR74DW/at0b28ePwGDYYdzo4'
+    b'fFIIKNqG0LBQUt0Kx2XtTrzTTEPyzYPwnz8bHm3b4mFdlaQQMAxNJP/VxARSk6QIF3zQTkOB'
+    b'2xFIrmvhOq4VHtVR4WZ3h3UKAcuxCAsPU5T84ekVvDs7BfmuhyF+X4iY871xfX1D6LcvBWEV'
+    b'Ap7nQCQMS2pCISPeF+81dtjlIETHRYgwdMf1DY1QlBkFwlQQCKKA8PDwXyU/v443pyYi12k/'
+    b'gRGs6YJrGxojIyEIgFy5QJIkIgHPcXh9fDRyHPcRGP6nO+P21lbISY+EyWwCgMoFZC5ERETg'
+    b'7X0NnC7Mgei8Ep7HOuDaxhb4/O4pomOiYbZWLfibA5sn4u6ugbi9sSGe7h2A0sIM0AwFG2WD'
+    b'1WapXsBSJsyf2BOanbORmxQIXuDB/exYhkhAUbaaBGUQWOpvn4ii+FfC2iUsx5CmKgX2lWg1'
+    b'mUyoTQhcVFwIrf6slbC1Xc6Kg/xLGML+APJWxIkWy8dWAAAAAElFTkSuQmCC')
+
+#----------------------------------------------------------------------
+paste = PyEmbeddedImage(
+    b'iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAAACXBIWXMAAAsTAAALEwEAmpwY'
+    b'AAAAB3RJTUUH1QoOABwVr+LxGAAAAdBJREFUOMuVk7FrU1EUxn/3vTSCJDGN1JQMhSIGXFy0'
+    b'amIE0RJwdtAhOBRFbR3ExUGXgjgIjvoPNIO7m6hL1S66OCmRUqjRSEJeb2zQRu85DqExL20g'
+    b'ftv9zj0/zvngGAZUKpWM73vPnZPZft/3vRfOSbFcLmu/bwBuzporBh4qjCsedvISudwRPM8A'
+    b'IKKsrHxgX+0pBgFoquqtxy9ZMvNnifieCS6cORj70snwLsjStB2mp6cwZhsgrK2tk0xEOZr8'
+    b'zKS/zrPXq1ZUUxEg5nlmLBrxeV/Psnj/EUEQUKlUQqvNzR0ilUpx7+5tLma+IaoxIBrp/9Te'
+    b'gkQigaowM3NsMB7i8Thbf8Cp6Xk9gGooG5bfvA29C/kcuynCEJ0+lecfXBBxwwG6S2F7AlVF'
+    b'RcidPP5/ExTyOUQEEUFVsNYyMZEeDdDfKNJtbv1ojT6BiOtBql+rNBr1HSGHAQM157qAVsvS'
+    b'qNcpFs8P2xRv2ATWblD7XkNEev71+atcnloevsLeMaUZNEmnM6TTGbLZw1i7gapwY+Far9k3'
+    b'GgJsiujv9i+350TyIw8W7/DT7YymsP8Tq+0DACS1ijFmU1U7BmDhXPcaMYwzglS71/jkFUt/'
+    b'AU/m4Zh4acTaAAAAAElFTkSuQmCC')
+
+#----------------------------------------------------------------------
 pen = PyEmbeddedImage(
     b'iVBORw0KGgoAAAANSUhEUgAAABYAAAAWCAIAAABL1vtsAAAABnRSTlMAAAAAAABupgeRAAAA'
     b'CXBIWXMAAA7EAAAOxAGVKw4bAAAFzUlEQVR42gHCBT36AAAAAAAAAAAAAAAAAAAAAAAAAAAA'
     b'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAEAAAAAAAAA'
     b'AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACVHjwKAgQAAAAAAABh4MAAAAAAAAAA'
     b'AAAAAAAEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAMDAwRkZGESQnGMjcIRhI'
     b'INzaPQwYSNu33PnxAAAAAAAAAwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAEpKSoiI'
```

## mwx/nutshell.py

```diff
@@ -2195,23 +2195,28 @@
         
         t, v, tb = sys.exc_info()
         try:
             self.parent.handler('interp_error', v)
         except AttributeError:
             pass
     
-    def getCallTip(self, *args, **kwargs):
+    def getCallTip(self, command='', *args, **kwargs):
         """Return call tip text for a command.
         
         (override) Ignore DeprecationWarning: for function,
                    `formatargspec` is deprecated since Python 3.5.
+        (override) Ignore ValueError: no signature found for builtin
+                   if the unwrapped function is a builtin function.
         """
         with warnings.catch_warnings():
             warnings.simplefilter('ignore', DeprecationWarning)
-            return interpreter.Interpreter.getCallTip(self, *args, **kwargs)
+            try:
+                return interpreter.Interpreter.getCallTip(self, command, *args, **kwargs)
+            except ValueError:
+                return interpreter.Interpreter.getCallTip(self) # dummy
 
 
 class Nautilus(Shell, EditorInterface):
     """Nautilus in the Shell.
     
     Objects in the process can be accessed using,
     
@@ -2467,15 +2472,14 @@
            '*backspace pressed' : (0, self.OnBackspace),
                 'enter pressed' : (0, self.OnEnter),
               'C-enter pressed' : (0, _F(self.insertLineBreak)),
             'C-S-enter pressed' : (0, _F(self.insertLineBreak)),
               'M-enter pressed' : (0, _F(self.duplicate_command)),
                '*enter pressed' : (0, ), # -> OnShowCompHistory 無効
                  'left pressed' : (0, self.OnBackspace),
-               'C-left pressed' : (0, self.OnBackspace),
                   'C-[ pressed' : (0, _F(self.goto_previous_mark_arrow)),
                 'C-S-[ pressed' : (0, _F(self.goto_previous_mark_arrow, selection=1)),
                   'C-] pressed' : (0, _F(self.goto_next_mark_arrow)),
                 'C-S-] pressed' : (0, _F(self.goto_next_mark_arrow, selection=1)),
                  'M-up pressed' : (0, _F(self.goto_previous_white_arrow)),
                'M-down pressed' : (0, _F(self.goto_next_white_arrow)),
                 'C-S-c pressed' : (0, skip),
```

## mwx/utilus.py

```diff
@@ -475,31 +475,33 @@
                     return typename(a, docp=1, qualp=0)
                 return repr(a)
             return ', '.join(_name(a) for a in v)
         return '\n'.join("{:>32} : {}".format(str(k), lstr(v)) for k, v in self.items())
     
     def bind(self, event, action=None):
         """Append a transaction to the context."""
+        assert callable(action) or action is None
+        if event not in self:
+            self[event] = []
         transaction = self[event]
         if action is None:
             return lambda f: self.bind(event, f)
-        if not callable(action):
-            raise TypeError("{!r} is not callable".format(action))
         if action not in transaction:
             transaction.append(action)
         return action
     
     def unbind(self, event, action=None):
         """Remove a transaction from the context."""
+        assert callable(action) or action is None
+        if event not in self:
+            return None
         transaction = self[event]
         if action is None:
-            del self[event]
+            transaction.clear()
             return True
-        if not callable(action):
-            raise TypeError("{!r} is not callable".format(action))
         if action in transaction:
             transaction.remove(action)
             return True
         return False
 
 
 class FSM(dict):
@@ -797,14 +799,15 @@
         
         equiv. self[state] += {event : [state2, action]}
         
         The transaction is expected to be a list (not a tuple).
         If no action, it creates only the transition and returns @decor(binder).
         """
         assert isinstance(event, str)
+        assert callable(action) or action is None
         warn = self.log
         
         if state not in self:
             warn("- FSM:warning: [{!r}] context newly created.".format(state))
             self[state] = SSM() # new context
         
         context = self[state]
@@ -826,15 +829,14 @@
             ##     pass
             context[event] = [state2] # new event:transaction
         
         transaction = context[event]
         if action is None:
             return lambda f: self.bind(event, f, state, state2)
         
-        assert callable(action), "{!r} is not callable".format(action)
         if action not in transaction:
             try:
                 transaction.append(action)
             except AttributeError:
                 warn("- FSM:warning: appending action to context ({!r} : {!r})\n"
                      "  The transaction must be a list, not a tuple".format(state, event))
         return action
@@ -843,14 +845,15 @@
         """Remove a transaction from the context.
         
         equiv. self[state] -= {event : [?, action]}
         
         The transaction is expected to be a list (not a tuple).
         If no action, it will remove the transaction from the context.
         """
+        assert callable(action) or action is None
         warn = self.log
         
         if state not in self:
             warn("- FSM:warning: [{!r}] context does not exist.".format(state))
             return
         
         context = self[state]
@@ -860,15 +863,14 @@
         
         transaction = context[event]
         if action is None:
             for act in transaction[1:]:
                 self.unbind(event, act, state)
             return True
         
-        assert callable(action), "{!r} is not callable".format(action)
         if action in transaction:
             try:
                 transaction.remove(action)
                 return True
             except AttributeError:
                 warn("- FSM:warning: removing action from context ({!r} : {!r})\n"
                      "  The transaction must be a list, not a tuple".format(state, event))
@@ -978,90 +980,100 @@
     def delf(self, ls, key):
         if '/' in key:
             p, key = key.rsplit('/', 1)
             ls = self.getf(ls, p)
         ls.remove(next(x for x in ls if x and x[0] == key))
 
 
+def get_fullargspec(f):
+    argv = []
+    defaults = {}
+    varargs = None
+    varkwargs = None
+    kwonlyargs = []
+    kwonlydefaults = {}
+    try:
+        sig = inspect.signature(f)
+        for k, v in sig.parameters.items():
+            if v.kind <= 1: # POSITIONAL_ONLY / POSITIONAL_OR_KEYWORD
+                argv.append(k)
+                if v.default != v.empty:
+                    defaults[k] = v.default
+            elif v.kind == 2: # VAR_POSITIONAL (*args)
+                varargs = k
+            elif v.kind == 3: # KEYWORD_ONLY
+                kwonlyargs.append(k)
+                if v.default != v.empty:
+                    kwonlydefaults[k] = v.default
+            elif v.kind == 4: # VAR_KEYWORD (**kwargs)
+                varkwargs = k
+    except ValueError:
+        ## Builtin functions don't have an argspec that we can get.
+        ## Try alalyzing the doc:str to get argspec info.
+        ## 
+        ## Wx builtin method doc is written in the following style:
+        ## ```name(argspec) -> retval
+        ## 
+        ## ...(details)...
+        ## ```
+        docs = [ln for ln in inspect.getdoc(f).splitlines() if ln]
+        m = re.search(r"(\w+)\((.*)\)", docs[0])
+        if m:
+            name, argspec = m.groups()
+            argv = [x for x in argspec.strip().split(',') if x]
+            defaults = dict(re.findall(r"(\w+)\s*=\s*([\w' ]+)", argspec))
+        else:
+            return None
+    return (argv, varargs, varkwargs,
+            defaults, kwonlyargs, kwonlydefaults)
+
+
 def funcall(f, *args, doc=None, alias=None, **kwargs):
     """Decorator of event handler
     
-    Check if the event argument can be omitted
-    and required arguments are given by args and kwargs.
+    Check if the event argument can be omitted and if any other
+    required arguments are specified in args and kwargs.
     
     Returns:
         lambda: Decorated function f as `alias<doc>`
         
         >>> Act1 = lambda *v,**kw: f(*(v+args), **(kwargs|kw))
         >>> Act2 = lambda *v,**kw: f(*args, **(kwargs|kw))
         
-        Act1 that accepts event arguments if there are any 
-        remaining arguments that must be explicitly specified in f.
-        Otherwise, Act2 that ignores event arguments.
+        Returns Act1 (accepts event arguments) if event arguments
+        cannot be omitted or if there are any remaining arguments
+        that must be explicitly specified.
+        Otherwise, returns Act2 (ignores event arguments).
     """
     assert callable(f)
     assert isinstance(doc, (str, type(None)))
     assert isinstance(alias, (str, type(None)))
     
     @wraps(f)
     def _Act(*v, **kw):
         kwargs.update(kw)
-        return f(*(v + args), **kwargs) # function with event args
+        return f(*v, *args, **kwargs) # function with event args
     
     @wraps(f)
     def _Act2(*v, **kw):
         kwargs.update(kw)
         return f(*args, **kwargs) # function with no explicit args
     
     action = _Act
-    
-    def _explicit_args(argv, defaults):
-        """The rest of argv that must be given explicitly in f."""
+    try:
+        (argv, varargs, varkwargs, defaults,
+            kwonlyargs, kwonlydefaults) = get_fullargspec(f)
+    except Exception:
+        return f
+    if not varargs:
         N = len(argv)
-        j = len(defaults)
         i = len(args)
-        return set(argv[i:N-j]) - set(kwargs)
-    
-    if not inspect.isbuiltin(f):
-        sig = inspect.signature(f)
-        argv = []
-        defaults = []
-        varargs = None
-        varkwargs = None
-        for k, v in sig.parameters.items():
-            if v.kind <= 1: # POSITIONAL_ONLY, POSITIONAL_OR_KEYWORD
-                argv.append(k)
-                if v.default != v.empty:
-                    defaults.append(v.default)
-            elif v.kind == 2: # VAR_POSITIONAL (*args)
-                varargs = k
-            elif v.kind == 4: # VAR_KEYWORD (**kwargs)
-                varkwargs = k
-        if varargs:
-            action = _Act
-        elif not _explicit_args(argv, defaults):
+        assert i <= N, "too many args"
+        ## remaining arguments that need to be specified explicitly.
+        rest = set(argv[i:]) - set(defaults) - set(kwargs)
+        if not rest:
             action = _Act2
-    else:
-        ## Builtin functions don't have an argspec that we can get.
-        ## Try alalyzing the doc:str to get argspec info.
-        ## 
-        ## Wx builtin method doc is written in the following style:
-        ## ```name(argspec) -> retval
-        ## 
-        ## ...(details)...
-        ## ```
-        docs = [ln for ln in inspect.getdoc(f).splitlines() if ln]
-        m = re.search(r"(\w+)\((.*)\)", docs[0])
-        if m:
-            name, argspec = m.groups()
-            argv = [x for x in argspec.strip().split(',') if x]
-            defaults = re.findall(r"\w+\s*=(\w+)", argspec)
-            if not _explicit_args(argv, defaults):
-                action = _Act2
-                if len(docs) > 1:
-                    action.__doc__ = '\n'.join(docs[1:])
-    
     if alias:
         action.__name__ = str(alias)
     if doc:
         action.__doc__ = doc
     return action
```

## Comparing `mwxlib-0.86.0.dist-info/LICENSE` & `mwxlib-0.86.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mwxlib-0.86.0.dist-info/METADATA` & `mwxlib-0.86.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwxlib
-Version: 0.86.0
+Version: 0.86.2
 Summary: A wrapper of matplotlib and wxPython (phoenix)
 Home-page: https://github.com/komoto48g/mwxlib
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 Author-email: komoto@jeol.co.jp
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `mwxlib-0.86.0.dist-info/RECORD` & `mwxlib-0.86.2.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 mwx/__init__.py,sha256=6vaRq60B9cLrnsiaoytM9JAIheZvDs2R1Kqv3I9rf3g,2514
-mwx/controls.py,sha256=_SKdIlBzyzbw5KSKwEYVD5XEW1tnQxVl-6YImy9FksA,45216
-mwx/framework.py,sha256=nplBanRBFgTr_TppgFdCkHROaYnz6bP2ngkKukW5UUI,72768
+mwx/controls.py,sha256=6rFO7hlAml5NTqH4mvP2seYRfBmFe7u9HuoKSf9OEZA,44804
+mwx/framework.py,sha256=AfGZzS4j8UcNcl7MHB8hpH7jxVG5kqkFRxpfdLlSjCU,72902
 mwx/graphman.py,sha256=b2q0YNTq9MT6fZy3lRYSxxNE2o7w9fLHrtNBdbZ3XLo,68688
-mwx/images.py,sha256=Xyvsq9m_R8JYERHA4Z3YznnUXbXkR7eUG7Cia1v1k2c,45726
+mwx/images.py,sha256=mrnUYH12I3XLVSZcEXlpVltX0XMxufbl2yRvDIQJZqc,49957
 mwx/matplot2.py,sha256=j35ObyXYInuxJAOyTiF1LFPynVAloCZUy98aIc1B2Qw,36005
 mwx/matplot2g.py,sha256=cBuLMnQt3XSKQL9io0XJb_v8Lv0pO9hm0IMjVIERtu4,68253
 mwx/matplot2lg.py,sha256=uF2jbsANhBqTX1Rpffrqc9DIYw6n2G1KeLsBb8l-U1M,27680
 mwx/mgplt.py,sha256=49_wpFZUEKErQmtobqrlNKDjWlAsdLft-izlqSyGPD0,6878
-mwx/nutshell.py,sha256=wkeHYRasJJNHm-5cZKSI9sZzaZJdTN6lntAPyr3pTYc,139007
-mwx/utilus.py,sha256=rz39wmKMGwXtP_6Zx7ykgij0hFjP7gKrPaHHssmCXLY,37351
+mwx/nutshell.py,sha256=nSDffOa_DlTNOY6ElDa1ZLlJ363Sx8e_fCA9ZulAdMA,139236
+mwx/utilus.py,sha256=PfT8LyMEVy0SfW1-5BfOUGP5rjP4DpSMSnRA3nb4-po,37660
 mwx/wxmon.py,sha256=JQ4sv-QDvMyqIXDektJZvvWD5ED0T30duAXLLcnO4cg,11175
 mwx/wxpdb.py,sha256=BKr8HVJQx8uC-yPS6am3ifD_sl89Ar-xEBi5scf7vm8,19456
 mwx/wxwil.py,sha256=_kyqGfKd6zRDKriHQehSkhQhv09dXizGqW3MkKA5MZ0,5372
 mwx/wxwit.py,sha256=G_86UM-99fPq7s8aiYoTXS1TiEWiFV9PbtgUfbrEmT4,8314
 mwx/py/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 mwx/py/filling.py,sha256=f6KMBcBv7gwrl6qmJYLTL-O0Z47bWNAdTCZtUZIo8vM,16794
-mwxlib-0.86.0.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
-mwxlib-0.86.0.dist-info/METADATA,sha256=oeV0mjU18hBMLEhhaXmVfLPgQfDwrbvORe20TFtLwb4,1893
-mwxlib-0.86.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-mwxlib-0.86.0.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
-mwxlib-0.86.0.dist-info/RECORD,,
+mwxlib-0.86.2.dist-info/LICENSE,sha256=PGtRKCaTkmUDlBQwpptJAxJtdqxIUtAmdBsaT9nUVkA,1091
+mwxlib-0.86.2.dist-info/METADATA,sha256=PozGRa9O3VsfxA-HWqFNEwvJuX59wIlmiKljQ8LMaD0,1893
+mwxlib-0.86.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+mwxlib-0.86.2.dist-info/top_level.txt,sha256=SI1Mh118AstnUFGPNq5aMNKiAnVNmZk1S9Ij-OwAEpY,4
+mwxlib-0.86.2.dist-info/RECORD,,
```

