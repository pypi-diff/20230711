# Comparing `tmp/lktbotfb-0.3.2.tar.gz` & `tmp/lktbotfb-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lktbotfb-0.3.2.tar", last modified: Tue Jul 11 17:50:05 2023, max compression
+gzip compressed data, was "lktbotfb-0.3.3.tar", last modified: Tue Jul 11 18:04:09 2023, max compression
```

## Comparing `lktbotfb-0.3.2.tar` & `lktbotfb-0.3.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 17:50:05.659112 lktbotfb-0.3.2/
--rw-rw-rw-   0        0        0     1093 2023-07-10 16:21:58.000000 lktbotfb-0.3.2/LICENSE
--rw-rw-rw-   0        0        0      885 2023-07-11 17:50:05.658057 lktbotfb-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      302 2023-07-10 16:19:54.000000 lktbotfb-0.3.2/README.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 17:50:05.660061 lktbotfb-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      764 2023-07-11 17:49:08.000000 lktbotfb-0.3.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:50:05.576061 lktbotfb-0.3.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 17:50:05.610058 lktbotfb-0.3.2/src/botfb/
--rw-rw-rw-   0        0        0       22 2023-07-10 14:52:18.000000 lktbotfb-0.3.2/src/botfb/__init__.py
--rw-rw-rw-   0        0        0     8436 2023-07-11 17:48:23.000000 lktbotfb-0.3.2/src/botfb/mylib.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:50:05.655074 lktbotfb-0.3.2/src/lktbotfb.egg-info/
--rw-rw-rw-   0        0        0      885 2023-07-11 17:50:05.000000 lktbotfb-0.3.2/src/lktbotfb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      247 2023-07-11 17:50:05.000000 lktbotfb-0.3.2/src/lktbotfb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 17:50:05.000000 lktbotfb-0.3.2/src/lktbotfb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-07-11 17:50:05.000000 lktbotfb-0.3.2/src/lktbotfb.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-07-11 17:50:05.000000 lktbotfb-0.3.2/src/lktbotfb.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 18:04:09.626093 lktbotfb-0.3.3/
+-rw-rw-rw-   0        0        0     1093 2023-07-10 16:21:58.000000 lktbotfb-0.3.3/LICENSE
+-rw-rw-rw-   0        0        0      885 2023-07-11 18:04:09.624093 lktbotfb-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2023-07-10 16:19:54.000000 lktbotfb-0.3.3/README.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 18:04:09.627095 lktbotfb-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      764 2023-07-11 18:03:20.000000 lktbotfb-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:04:09.568553 lktbotfb-0.3.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 18:04:09.582549 lktbotfb-0.3.3/src/botfb/
+-rw-rw-rw-   0        0        0       22 2023-07-10 14:52:18.000000 lktbotfb-0.3.3/src/botfb/__init__.py
+-rw-rw-rw-   0        0        0     8445 2023-07-11 18:02:49.000000 lktbotfb-0.3.3/src/botfb/mylib.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:04:09.622094 lktbotfb-0.3.3/src/lktbotfb.egg-info/
+-rw-rw-rw-   0        0        0      885 2023-07-11 18:04:09.000000 lktbotfb-0.3.3/src/lktbotfb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      247 2023-07-11 18:04:09.000000 lktbotfb-0.3.3/src/lktbotfb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 18:04:09.000000 lktbotfb-0.3.3/src/lktbotfb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-07-11 18:04:09.000000 lktbotfb-0.3.3/src/lktbotfb.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-07-11 18:04:09.000000 lktbotfb-0.3.3/src/lktbotfb.egg-info/top_level.txt
```

### Comparing `lktbotfb-0.3.2/LICENSE` & `lktbotfb-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lktbotfb-0.3.2/PKG-INFO` & `lktbotfb-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lktbotfb
-Version: 0.3.2
+Version: 0.3.3
 Summary: This makes it easy for you to create a chatbot for your Facebook page
 Home-page: https://github.com/AmirLouktaila/lktbotfb
 Author: Salah Louktaila
 Author-email: amir.Louktila@gmail.com
 License: MIT
 Keywords: chatbot
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `lktbotfb-0.3.2/setup.py` & `lktbotfb-0.3.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 10',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='lktbotfb',
-  version='0.3.2',
+  version='0.3.3',
   description='This makes it easy for you to create a chatbot for your Facebook page',
   long_description=open('README.txt').read(),
   url='https://github.com/AmirLouktaila/lktbotfb',  
   author='Salah Louktaila',
   author_email='amir.Louktila@gmail.com',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `lktbotfb-0.3.2/src/botfb/mylib.py` & `lktbotfb-0.3.3/src/botfb/mylib.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         startapp = str(namebot_ + "_")
         os.chdir(f"{namebot_}")
         creatbotapp = f"python manage.py startapp {startapp}"
         os.system(creatbotapp)
         startapp_edit="done create a app"   
         print(startapp_edit)
         time.sleep(2)
-        os.chdir(os.path.join(current_path, namebot_))
+        os.chdir(os.path.join(current_path, namebot_,namebot_))
         name_urls = "urls.py"
         with open(name_urls, 'w') as files:
             files.write(
 f'''
 # yomamabot/fb_yomamabot/urls.py
 from django.urls import re_path, include
 from .views import YoMamaBotView
```

### Comparing `lktbotfb-0.3.2/src/lktbotfb.egg-info/PKG-INFO` & `lktbotfb-0.3.3/src/lktbotfb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lktbotfb
-Version: 0.3.2
+Version: 0.3.3
 Summary: This makes it easy for you to create a chatbot for your Facebook page
 Home-page: https://github.com/AmirLouktaila/lktbotfb
 Author: Salah Louktaila
 Author-email: amir.Louktila@gmail.com
 License: MIT
 Keywords: chatbot
 Classifier: Development Status :: 5 - Production/Stable
```

