# Comparing `tmp/XME-3.0.tar.gz` & `tmp/XME-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "XME-3.0.tar", last modified: Sat Jul  8 16:12:17 2023, max compression
+gzip compressed data, was "XME-3.1.tar", last modified: Tue Jul 11 09:20:31 2023, max compression
```

## Comparing `XME-3.0.tar` & `XME-3.1.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 16:12:17.468396 XME-3.0/
--rw-rw-rw-   0        0        0     1527 2023-07-08 14:55:51.000000 XME-3.0/LICENSE.txt
--rw-rw-rw-   0        0        0     3529 2023-07-08 16:12:17.467396 XME-3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2957 2023-07-08 15:49:27.000000 XME-3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 16:12:17.447391 XME-3.0/XME/
--rw-rw-rw-   0        0        0     2280 2023-07-08 14:44:16.000000 XME-3.0/XME/XME.py
-drwxrwxrwx   0        0        0        0 2023-07-08 16:12:17.465395 XME-3.0/XME/XMElib/
--rw-rw-rw-   0        0        0     1661 2023-07-08 10:05:12.000000 XME-3.0/XME/XMElib/ArrayOperator.py
--rw-rw-rw-   0        0        0     3640 2023-07-04 02:14:30.000000 XME-3.0/XME/XMElib/Executor.py
--rw-rw-rw-   0        0        0     1959 2023-07-08 15:36:18.000000 XME-3.0/XME/XMElib/Logputter.py
--rw-rw-rw-   0        0        0        0 2023-01-27 18:19:50.000000 XME-3.0/XME/XMElib/__init__.py
--rw-rw-rw-   0        0        0       73 2023-07-03 19:15:18.000000 XME-3.0/XME/XMElib/version_info.py
--rw-rw-rw-   0        0        0        0 2023-07-08 14:44:19.000000 XME-3.0/XME/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-08 16:12:17.455393 XME-3.0/XME.egg-info/
--rw-rw-rw-   0        0        0     3529 2023-07-08 16:12:17.000000 XME-3.0/XME.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      290 2023-07-08 16:12:17.000000 XME-3.0/XME.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 16:12:17.000000 XME-3.0/XME.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-07-08 16:12:17.000000 XME-3.0/XME.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 16:12:17.468396 XME-3.0/setup.cfg
--rw-rw-rw-   0        0        0      814 2023-07-08 14:57:14.000000 XME-3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:20:31.511501 XME-3.1/
+-rw-rw-rw-   0        0        0     1527 2023-07-08 14:55:51.000000 XME-3.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     3545 2023-07-11 09:20:31.511501 XME-3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2973 2023-07-11 09:16:04.000000 XME-3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-07-11 09:20:31.492497 XME-3.1/XME/
+drwxrwxrwx   0        0        0        0 2023-07-11 09:20:31.509501 XME-3.1/XME/XMElib/
+-rw-rw-rw-   0        0        0     1661 2023-07-08 10:05:12.000000 XME-3.1/XME/XMElib/ArrayOperator.py
+-rw-rw-rw-   0        0        0     3640 2023-07-04 02:14:30.000000 XME-3.1/XME/XMElib/Executor.py
+-rw-rw-rw-   0        0        0     1959 2023-07-08 15:35:32.000000 XME-3.1/XME/XMElib/Logputter.py
+-rw-rw-rw-   0        0        0        0 2023-01-27 18:19:50.000000 XME-3.1/XME/XMElib/__init__.py
+-rw-rw-rw-   0        0        0       73 2023-07-11 09:04:54.000000 XME-3.1/XME/XMElib/version_info.py
+-rw-rw-rw-   0        0        0     2341 2023-07-11 09:04:31.000000 XME-3.1/XME/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-11 09:20:31.499498 XME-3.1/XME.egg-info/
+-rw-rw-rw-   0        0        0     3545 2023-07-11 09:20:31.000000 XME-3.1/XME.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-11 09:20:31.000000 XME-3.1/XME.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 09:20:31.000000 XME-3.1/XME.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-07-11 09:20:31.000000 XME-3.1/XME.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 09:20:31.512501 XME-3.1/setup.cfg
+-rw-rw-rw-   0        0        0      814 2023-07-11 09:13:01.000000 XME-3.1/setup.py
```

### Comparing `XME-3.0/LICENSE.txt` & `XME-3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `XME-3.0/PKG-INFO` & `XME-3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: XME
-Version: 3.0
+Version: 3.1
 Summary: This is a Python interface for process pool establishment, and result collection based on the Multiprocessing module.
 Home-page: https://github.com/wacmkxiaoyi/Xenon-Multiprocessing-Engine
 Author: Junxiang Huang & Weihui Li
 Author-email: huangjunxiang@mail.ynu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Xenon-Multiprocessing-Engine
 Xenon-Multiprocessing-Engine (**XME** thereafter) is a Python interface for process pool establishment, and result collection based on the Multiprocessing module.
 
-Version 3.0
-Update: 2023-07-08
+Version 3.1
+Update: 2023-07-11
 
 Author: Junxiang H. & Weihui L. <br>
 Suggestion to: huangjunxiang@mail.ynu.edu.cn
 Website: wacmk.cn/com
 
 A multiprocessing interface for python.
-You can download the package at **"Releases"** in your right hand.
+You can download the **outdate** package at **"Releases"** in your right hand.
 
 # Install
 
 ```shell
 pip3 install XME
 ```
 
@@ -45,15 +45,16 @@
   z=targetfun(x,y)
   print(z)
 ```
 
 You should update your main function and call **XME**
 
 ```python
-from XME.XME import XME
+from XME import XME
+#import XME.XME as XME 
 if __name__=="__main__":
   xme=XME(targetfun,pnum=3) #where targetfun is target function, pnum is how many cores you would like to do in this function (default - all cores callable of your computer)
   x=50
   y=np.array(100)
   z=xme.fun(x,xme.Array(y)) # xme.Array class indicates the array y will be detached into pnum parts, and run targetfun eachself
   #For example:
   #core 0, y=: 0 3 6 9 12 ....
@@ -61,32 +62,31 @@
   #core 2: 2 5 8 11....
 #result: <tuple>
 #>>>(50,51,52,53....,147,148,149)
 ```
 
 # Logger Output
 
-XME has a built-in log output module. You can add the **logobj** into targetfun's **parameters' list**, and replace **print** (optional)
+XME has a built-in log output module. You can add the **print** into targetfun's **parameters' list**, and replace **print** (optional)
 
 ```python
-def target(x,y,logobj):
-  print=logobj.write_log
+def target(x,y,print=print):
   print("x=",x,"y=",y,"x+y",x+y) #useage like built-in function print
 ```
 
 The default output takes the pid, time and the user-def output in **print**
 
 ## Advanced usage of logobj
 
 You can define the **logobj**'s parameters when create a XME object
 
 ```python
 if __name__=="__main__":
   xme=XME(targetfun,
-    do_with_log=True, #if set to False, the logger will be close (general switch), default True
+    do_with_log=True, #if set to False, the logger will be shutdowned (general switch), default True
     print_in_screen=True, #if set to False, the log will not show in your screen (or a terminal)
     logfile=None, #if set to a file (e.g., ***.log), the log will save into this file
     show_version_info=True #if set to False, the version info of XME will be hiden
   )
 ```
 
 # Unavailabe cases
```

### Comparing `XME-3.0/README.md` & `XME-3.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Xenon-Multiprocessing-Engine
 Xenon-Multiprocessing-Engine (**XME** thereafter) is a Python interface for process pool establishment, and result collection based on the Multiprocessing module.
 
-Version 3.0
-Update: 2023-07-08
+Version 3.1
+Update: 2023-07-11
 
 Author: Junxiang H. & Weihui L. <br>
 Suggestion to: huangjunxiang@mail.ynu.edu.cn
 Website: wacmk.cn/com
 
 A multiprocessing interface for python.
-You can download the package at **"Releases"** in your right hand.
+You can download the **outdate** package at **"Releases"** in your right hand.
 
 # Install
 
 ```shell
 pip3 install XME
 ```
 
@@ -31,15 +31,16 @@
   z=targetfun(x,y)
   print(z)
 ```
 
 You should update your main function and call **XME**
 
 ```python
-from XME.XME import XME
+from XME import XME
+#import XME.XME as XME 
 if __name__=="__main__":
   xme=XME(targetfun,pnum=3) #where targetfun is target function, pnum is how many cores you would like to do in this function (default - all cores callable of your computer)
   x=50
   y=np.array(100)
   z=xme.fun(x,xme.Array(y)) # xme.Array class indicates the array y will be detached into pnum parts, and run targetfun eachself
   #For example:
   #core 0, y=: 0 3 6 9 12 ....
@@ -47,32 +48,31 @@
   #core 2: 2 5 8 11....
 #result: <tuple>
 #>>>(50,51,52,53....,147,148,149)
 ```
 
 # Logger Output
 
-XME has a built-in log output module. You can add the **logobj** into targetfun's **parameters' list**, and replace **print** (optional)
+XME has a built-in log output module. You can add the **print** into targetfun's **parameters' list**, and replace **print** (optional)
 
 ```python
-def target(x,y,logobj):
-  print=logobj.write_log
+def target(x,y,print=print):
   print("x=",x,"y=",y,"x+y",x+y) #useage like built-in function print
 ```
 
 The default output takes the pid, time and the user-def output in **print**
 
 ## Advanced usage of logobj
 
 You can define the **logobj**'s parameters when create a XME object
 
 ```python
 if __name__=="__main__":
   xme=XME(targetfun,
-    do_with_log=True, #if set to False, the logger will be close (general switch), default True
+    do_with_log=True, #if set to False, the logger will be shutdowned (general switch), default True
     print_in_screen=True, #if set to False, the log will not show in your screen (or a terminal)
     logfile=None, #if set to a file (e.g., ***.log), the log will save into this file
     show_version_info=True #if set to False, the version info of XME will be hiden
   )
 ```
 
 # Unavailabe cases
```

### Comparing `XME-3.0/XME/XME.py` & `XME-3.1/XME/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from multiprocessing import cpu_count
-from XME.XMElib.ArrayOperator import ArrayOperator
-from XME.XMElib.Executor import Executor
-from XME.XMElib.Logputter import Logputter
-from XME.XMElib.version_info import XME_Version_info
+from XMElib.ArrayOperator import ArrayOperator
+from XMElib.Executor import Executor
+from XMElib.Logputter import Logputter
+from XMElib.version_info import XME_Version_info
 def get_par(args,name,default=None):
 	try:
 		return args[name]
 	except:
 		return default
 class XME:
 	aoobj_array=[]
@@ -15,21 +15,23 @@
 		def __init__(self,array):
 			self.array=array
 			self.length=len(array)
 	def __init__(self,*fun,**args):
 		self.pnum=get_par(args,"pnum",cpu_count())
 		self.funs=[]
 		if get_par(args,"do_with_log",True):
-			self.logobj=Logputter(get_par(args,"logfile"),XME_Version_info,get_par(args,"show_version_info",False))
+			self.logobj=Logputter(get_par(args,"logfile"),XME_Version_info,get_par(args,"show_version_info",True))
 			self.logobj.print_in_screen=get_par(args,"print_in_screen",True)
 		else:
 			self.logobj=None
 		for fu in fun:
 			def func(*targ,**args):
 				args.update({"logobj":self.logobj})
+				if self.logobj!=None:
+					args.update({"print":self.logobj.write_log})
 				calnum=get_par(args,"calnum",0)
 				if calnum==0:
 					for i in targ:
 						if type(i)==self.Array:
 							calnum=max(calnum,i.length)
 					for i in args.keys():
 						if type(args[i])==self.Array:
```

### Comparing `XME-3.0/XME/XMElib/ArrayOperator.py` & `XME-3.1/XME/XMElib/ArrayOperator.py`

 * *Files identical despite different names*

### Comparing `XME-3.0/XME/XMElib/Executor.py` & `XME-3.1/XME/XMElib/Executor.py`

 * *Files identical despite different names*

### Comparing `XME-3.0/XME/XMElib/Logputter.py` & `XME-3.1/XME/XMElib/Logputter.py`

 * *Files identical despite different names*

### Comparing `XME-3.0/XME.egg-info/PKG-INFO` & `XME-3.1/XME.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Metadata-Version: 2.1
 Name: XME
-Version: 3.0
+Version: 3.1
 Summary: This is a Python interface for process pool establishment, and result collection based on the Multiprocessing module.
 Home-page: https://github.com/wacmkxiaoyi/Xenon-Multiprocessing-Engine
 Author: Junxiang Huang & Weihui Li
 Author-email: huangjunxiang@mail.ynu.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # Xenon-Multiprocessing-Engine
 Xenon-Multiprocessing-Engine (**XME** thereafter) is a Python interface for process pool establishment, and result collection based on the Multiprocessing module.
 
-Version 3.0
-Update: 2023-07-08
+Version 3.1
+Update: 2023-07-11
 
 Author: Junxiang H. & Weihui L. <br>
 Suggestion to: huangjunxiang@mail.ynu.edu.cn
 Website: wacmk.cn/com
 
 A multiprocessing interface for python.
-You can download the package at **"Releases"** in your right hand.
+You can download the **outdate** package at **"Releases"** in your right hand.
 
 # Install
 
 ```shell
 pip3 install XME
 ```
 
@@ -45,15 +45,16 @@
   z=targetfun(x,y)
   print(z)
 ```
 
 You should update your main function and call **XME**
 
 ```python
-from XME.XME import XME
+from XME import XME
+#import XME.XME as XME 
 if __name__=="__main__":
   xme=XME(targetfun,pnum=3) #where targetfun is target function, pnum is how many cores you would like to do in this function (default - all cores callable of your computer)
   x=50
   y=np.array(100)
   z=xme.fun(x,xme.Array(y)) # xme.Array class indicates the array y will be detached into pnum parts, and run targetfun eachself
   #For example:
   #core 0, y=: 0 3 6 9 12 ....
@@ -61,32 +62,31 @@
   #core 2: 2 5 8 11....
 #result: <tuple>
 #>>>(50,51,52,53....,147,148,149)
 ```
 
 # Logger Output
 
-XME has a built-in log output module. You can add the **logobj** into targetfun's **parameters' list**, and replace **print** (optional)
+XME has a built-in log output module. You can add the **print** into targetfun's **parameters' list**, and replace **print** (optional)
 
 ```python
-def target(x,y,logobj):
-  print=logobj.write_log
+def target(x,y,print=print):
   print("x=",x,"y=",y,"x+y",x+y) #useage like built-in function print
 ```
 
 The default output takes the pid, time and the user-def output in **print**
 
 ## Advanced usage of logobj
 
 You can define the **logobj**'s parameters when create a XME object
 
 ```python
 if __name__=="__main__":
   xme=XME(targetfun,
-    do_with_log=True, #if set to False, the logger will be close (general switch), default True
+    do_with_log=True, #if set to False, the logger will be shutdowned (general switch), default True
     print_in_screen=True, #if set to False, the log will not show in your screen (or a terminal)
     logfile=None, #if set to a file (e.g., ***.log), the log will save into this file
     show_version_info=True #if set to False, the version info of XME will be hiden
   )
 ```
 
 # Unavailabe cases
```

### Comparing `XME-3.0/setup.py` & `XME-3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="XME",
-    version="3.0",
+    version="3.1",
     author="Junxiang Huang & Weihui Li",
     author_email="huangjunxiang@mail.ynu.edu.cn",
     description="This is a Python interface for process pool establishment, and result collection based on the Multiprocessing module.",
     long_description=long_description, 
     long_description_content_type="text/markdown",
     url="https://github.com/wacmkxiaoyi/Xenon-Multiprocessing-Engine", 
     packages=setuptools.find_packages(),
```

