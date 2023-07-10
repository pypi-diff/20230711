# Comparing `tmp/doFolder-0.1.0.tar.gz` & `tmp/doFolder-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doFolder-0.1.0.tar", last modified: Tue Jun 13 12:28:09 2023, max compression
+gzip compressed data, was "doFolder-1.0.0.tar", last modified: Mon Jul 10 23:40:07 2023, max compression
```

## Comparing `doFolder-0.1.0.tar` & `doFolder-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 12:28:09.030596 doFolder-0.1.0/
--rw-rw-rw-   0        0        0     3157 2023-06-13 12:28:09.030596 doFolder-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2430 2023-06-13 12:27:21.000000 doFolder-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-13 12:28:09.012596 doFolder-0.1.0/doFolder/
--rw-rw-rw-   0        0        0      569 2023-05-31 14:24:09.000000 doFolder-0.1.0/doFolder/__init__.py
--rw-rw-rw-   0        0        0    10940 2023-06-13 12:20:24.000000 doFolder-0.1.0/doFolder/compare.py
--rw-rw-rw-   0        0        0    27772 2023-06-13 12:22:36.000000 doFolder-0.1.0/doFolder/main.py
--rw-rw-rw-   0        0        0    13847 2023-05-31 14:13:25.000000 doFolder-0.1.0/doFolder/terminal.py
-drwxrwxrwx   0        0        0        0 2023-06-13 12:28:09.028595 doFolder-0.1.0/doFolder.egg-info/
--rw-rw-rw-   0        0        0     3157 2023-06-13 12:28:08.000000 doFolder-0.1.0/doFolder.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      292 2023-06-13 12:28:08.000000 doFolder-0.1.0/doFolder.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 12:28:08.000000 doFolder-0.1.0/doFolder.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-06-13 12:28:08.000000 doFolder-0.1.0/doFolder.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       25 2023-06-13 12:28:08.000000 doFolder-0.1.0/doFolder.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-13 12:28:08.000000 doFolder-0.1.0/doFolder.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 12:28:09.030596 doFolder-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1220 2023-06-13 12:23:11.000000 doFolder-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-10 23:40:07.248440 doFolder-1.0.0/
+-rw-rw-rw-   0        0        0     3157 2023-07-10 23:40:07.247440 doFolder-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2430 2023-06-13 12:27:21.000000 doFolder-1.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-10 23:40:07.242441 doFolder-1.0.0/doFolder/
+-rw-rw-rw-   0        0        0      548 2023-07-10 23:34:32.000000 doFolder-1.0.0/doFolder/__init__.py
+-rw-rw-rw-   0        0        0    10940 2023-06-13 12:20:24.000000 doFolder-1.0.0/doFolder/compare.py
+-rw-rw-rw-   0        0        0    28896 2023-07-10 23:35:29.000000 doFolder-1.0.0/doFolder/main.py
+-rw-rw-rw-   0        0        0    13847 2023-05-31 14:13:25.000000 doFolder-1.0.0/doFolder/terminal.py
+drwxrwxrwx   0        0        0        0 2023-07-10 23:40:07.246441 doFolder-1.0.0/doFolder.egg-info/
+-rw-rw-rw-   0        0        0     3157 2023-07-10 23:40:07.000000 doFolder-1.0.0/doFolder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      292 2023-07-10 23:40:07.000000 doFolder-1.0.0/doFolder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-10 23:40:07.000000 doFolder-1.0.0/doFolder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-10 23:40:07.000000 doFolder-1.0.0/doFolder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       25 2023-07-10 23:40:07.000000 doFolder-1.0.0/doFolder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-10 23:40:07.000000 doFolder-1.0.0/doFolder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-10 23:40:07.248440 doFolder-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     1220 2023-07-10 23:32:45.000000 doFolder-1.0.0/setup.py
```

### Comparing `doFolder-0.1.0/PKG-INFO` & `doFolder-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.1.0
+Version: 1.0.0
 Summary: Manage files more easily
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
```

### Comparing `doFolder-0.1.0/README.rst` & `doFolder-1.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `doFolder-0.1.0/doFolder/__init__.py` & `doFolder-1.0.0/doFolder/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,9 +5,9 @@
 You may obtain a copy of Mulan PSL v2 at:
          http://license.coscl.org.cn/MulanPSL2
 THIS SOFTWARE IS PROVIDED ON AN "AS IS" BASIS, WITHOUT WARRANTIES OF ANY KIND,
 EITHER EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO NON-INFRINGEMENT,
 MERCHANTABILITY OR FIT FOR A PARTICULAR PURPOSE.
 See the Mulan PSL v2 for more details.
 """
-from doFolder.main import *
-import doFolder.compare as compare
+from .main import *
+from . import compare
```

### Comparing `doFolder-0.1.0/doFolder/compare.py` & `doFolder-1.0.0/doFolder/compare.py`

 * *Files identical despite different names*

### Comparing `doFolder-0.1.0/doFolder/main.py` & `doFolder-1.0.0/doFolder/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,22 +20,32 @@
 import logging
 from concurrent.futures import ThreadPoolExecutor
 from specialStr import Path
 import base64
 import json
 from concurrent.futures import ThreadPoolExecutor,_base
 import time
+
 __all__=["File","Folder","Path"]
 
 
 SearchCondition=Union[str,re.Pattern,Callable[[Union["File","Folder"]],bool]]
 FormatedMatching=Tuple[Callable[[Union["File","Folder"]],bool],int,Union[int,None]]
 UnformattedMatching=Union[SearchCondition,Tuple[SearchCondition,int,Union[int,None]]]
 _T=TypeVar("_T",bound="_HasName")
 _U=TypeVar("_U")
+class RuntimeError(Exception):
+    def __init__(self, error:BaseException) -> None:
+        super().__init__(str(error))
+        self.error=error
+def tryRun(fn:Callable[...,_U])->Union[_U,RuntimeError]:
+    try:
+        return fn()
+    except BaseException as e:
+        return RuntimeError(e)
 class _HasName(Generic[_T]):
     name: str
 
 class _FolderUpdateHeader (FileSystemEventHandler):
     def __init__(self,target:"Folder"):
         self.target=target
     def on_moved(self, event:FileSystemMovedEvent):
@@ -123,21 +133,38 @@
         except AttributeError:
             for i in self.values:
                 if i.name == key:
                     return i
             raise AttributeError(f"name {key} is neither attribute or name of values")
     def __iter__(self):
         return self.values.__iter__()
+    def getSubAttribute(self,key:str)->List:
+        retsult=[]
+        for i in self:
+            if type(tryRun(lambda:i.__getattribute__(key)))==RuntimeError:
+                raise AttributeError(f"Not all attributes named \"{key}\" of the list are existent")
+            retsult.append(i.__getattribute__(key))
+        return retsult
+    def callSubAttribute(self,fn:str,*args,**kw)->Any:
+        li=self.getSubAttribute(fn)
+        for i in li:
+            if not callable(i):
+                raise AttributeError(f"Not all attributes named \"{fn}\" of the list are callable")
+        return [tryRun(lambda:i(*args,**kw)) for i in li]
 
 class SearchResult(_ObjectListIndexedByName[Union["File","Folder"]]):
     def __init__(self,var:Iterable[Union["File","Folder"]]=[],match:Union[FormatedMatching,None]=None):
         super().__init__(var)
         self.match=match
     def __add__(self,var:"SearchResult"):
         return SearchResult(self.values+var.values,match=self.match)
+    def remove(self) -> None:
+        self.callSubAttribute("remove")
+    def copy(self,path:Union[str,Path]) -> None:
+        self.callSubAttribute("copy",path)
 class FileList(_ObjectListIndexedByName["File"]):
     def __init__(self,var:Iterable["File"]=[]):
         super().__init__(var)
     def __add__(self,var:"FileList"):
         return FileList(self.values+var.values)
 class FolderList(_ObjectListIndexedByName["Folder"]):
     def __init__(self,var:Iterable["Folder"]=[]):
```

### Comparing `doFolder-0.1.0/doFolder/terminal.py` & `doFolder-1.0.0/doFolder/terminal.py`

 * *Files identical despite different names*

### Comparing `doFolder-0.1.0/doFolder.egg-info/PKG-INFO` & `doFolder-1.0.0/doFolder.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: doFolder
-Version: 0.1.0
+Version: 1.0.0
 Summary: Manage files more easily
 Home-page: https://kuankuan2007.gitee.io/docs/do-folder/
 Author: kuankuan
 Author-email: 2163826131@qq.com
 License: Mulan PSL v2
 Keywords: file,foler,path,filesystem
 Platform: windows
```

### Comparing `doFolder-0.1.0/setup.py` & `doFolder-1.0.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 from distutils.core import setup
 setup(
     name = 'doFolder',
-    version = '0.1.0',
+    version = '1.0.0',
     keywords = ['file',"foler","path","filesystem"],
     description = 'Manage files more easily',
     long_description = open("README.rst","r",encoding="utf-8").read(),
     author = 'kuankuan',
     author_email = '2163826131@qq.com',
     url="https://kuankuan2007.gitee.io/docs/do-folder/",
     install_requires = [
```

