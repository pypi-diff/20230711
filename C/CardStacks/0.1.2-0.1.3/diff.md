# Comparing `tmp/CardStacks-0.1.2.tar.gz` & `tmp/CardStacks-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CardStacks-0.1.2.tar", last modified: Tue Jul 11 09:47:57 2023, max compression
+gzip compressed data, was "CardStacks-0.1.3.tar", last modified: Tue Jul 11 15:41:58 2023, max compression
```

## Comparing `CardStacks-0.1.2.tar` & `CardStacks-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 09:47:57.042029 CardStacks-0.1.2/
-drwxrwxrwx   0        0        0        0 2023-07-11 09:47:57.019523 CardStacks-0.1.2/CardStacks/
--rw-rw-rw-   0        0        0     7807 2023-07-10 19:05:10.000000 CardStacks-0.1.2/CardStacks/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 09:47:57.039029 CardStacks-0.1.2/CardStacks.egg-info/
--rw-rw-rw-   0        0        0     1645 2023-07-11 09:47:56.000000 CardStacks-0.1.2/CardStacks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      185 2023-07-11 09:47:56.000000 CardStacks-0.1.2/CardStacks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 09:47:56.000000 CardStacks-0.1.2/CardStacks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-07-11 09:47:56.000000 CardStacks-0.1.2/CardStacks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    35821 2023-07-08 19:08:55.000000 CardStacks-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1645 2023-07-11 09:47:57.041029 CardStacks-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      791 2023-07-10 20:26:35.000000 CardStacks-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-11 09:47:57.042029 CardStacks-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1161 2023-07-10 20:27:47.000000 CardStacks-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 15:41:58.104271 CardStacks-0.1.3/
+drwxrwxrwx   0        0        0        0 2023-07-11 15:41:58.065313 CardStacks-0.1.3/CardStacks/
+-rw-rw-rw-   0        0        0     7784 2023-07-11 12:38:01.000000 CardStacks-0.1.3/CardStacks/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 15:41:58.101079 CardStacks-0.1.3/CardStacks.egg-info/
+-rw-rw-rw-   0        0        0     1645 2023-07-11 15:41:57.000000 CardStacks-0.1.3/CardStacks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2023-07-11 15:41:57.000000 CardStacks-0.1.3/CardStacks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 15:41:57.000000 CardStacks-0.1.3/CardStacks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-07-11 15:41:57.000000 CardStacks-0.1.3/CardStacks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    35821 2023-07-08 19:08:55.000000 CardStacks-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1645 2023-07-11 15:41:58.103119 CardStacks-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      791 2023-07-10 20:26:35.000000 CardStacks-0.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-11 15:41:58.104271 CardStacks-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1161 2023-07-11 15:39:12.000000 CardStacks-0.1.3/setup.py
```

### Comparing `CardStacks-0.1.2/CardStacks/__init__.py` & `CardStacks-0.1.3/CardStacks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import random
 
-__version__ = "0.4.0"
+__version__ = "0.1.3"
 __author__ = "SpeedyGo55"
 
+
 class CardStack:
     def __init__(self, suits=None, ranks=None):
         if suits is None:
             self.cards_on_stack = {
                 "Spades": ["2", "3", "4", "5", "6", "7", "8", "9", "10", "Jack", "Queen", "King", "Ace"],
                 "Hearts": ["2", "3", "4", "5", "6", "7", "8", "9", "10", "Jack", "Queen", "King", "Ace"],
                 "Clubs": ["2", "3", "4", "5", "6", "7", "8", "9", "10", "Jack", "Queen", "King", "Ace"],
@@ -83,15 +84,14 @@
         output = {}
         if size > len(self) or size < 0:
             raise ValueError("Stack is not big enough")
         for suit in self.cards_on_stack:
             output[suit] = []
         for i in range(size):
             suit = random.choice(list(self.cards_on_stack.keys()))
-            print(suit)
             while True:
                 if len(self.cards_on_stack[suit]) == 0:
                     suit = random.choice(list(self.cards_on_stack.keys()))
                 else:
                     break
             card = random.choice(self.cards_on_stack[suit])
             self.cards_in_play[suit].append(card)
```

### Comparing `CardStacks-0.1.2/CardStacks.egg-info/PKG-INFO` & `CardStacks-0.1.3/CardStacks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CardStacks
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple library for creating and manipulating stacks of cards.
 Home-page: https://github.com/SpeedyGo55/CardStacks
 Author: SpeedyGo55
 Author-email: SpeedyGo55@outlook.com
 License: GPLv3
 Project-URL: Bug Reports, https://github.com/SpeedyGo55/CardStacks/issues
 Project-URL: Source, https://github.com/SpeedyGo55/CardStacks
```

### Comparing `CardStacks-0.1.2/LICENSE` & `CardStacks-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `CardStacks-0.1.2/PKG-INFO` & `CardStacks-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CardStacks
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple library for creating and manipulating stacks of cards.
 Home-page: https://github.com/SpeedyGo55/CardStacks
 Author: SpeedyGo55
 Author-email: SpeedyGo55@outlook.com
 License: GPLv3
 Project-URL: Bug Reports, https://github.com/SpeedyGo55/CardStacks/issues
 Project-URL: Source, https://github.com/SpeedyGo55/CardStacks
```

### Comparing `CardStacks-0.1.2/README.md` & `CardStacks-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `CardStacks-0.1.2/setup.py` & `CardStacks-0.1.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="CardStacks",
-    version="0.1.2",
+    version="0.1.3",
     description="A simple library for creating and manipulating stacks of cards.",
     url="https://github.com/SpeedyGo55/CardStacks",
     author="SpeedyGo55",
     author_email="SpeedyGo55@outlook.com",
     license="GPLv3",
     packages=["CardStacks"],
     classifiers=[
```

