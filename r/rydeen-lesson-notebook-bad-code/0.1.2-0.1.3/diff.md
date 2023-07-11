# Comparing `tmp/rydeen-lesson-notebook-bad-code-0.1.2.tar.gz` & `tmp/rydeen-lesson-notebook-bad-code-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rydeen-lesson-notebook-bad-code-0.1.2.tar", last modified: Sat Jul  8 15:34:37 2023, max compression
+gzip compressed data, was "rydeen-lesson-notebook-bad-code-0.1.3.tar", last modified: Tue Jul 11 10:33:44 2023, max compression
```

## Comparing `rydeen-lesson-notebook-bad-code-0.1.2.tar` & `rydeen-lesson-notebook-bad-code-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 15:34:37.523267 rydeen-lesson-notebook-bad-code-0.1.2/
--rw-rw-rw-   0        0        0      263 2023-07-08 15:34:37.521271 rydeen-lesson-notebook-bad-code-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-08 15:34:37.501282 rydeen-lesson-notebook-bad-code-0.1.2/rydeen_lesson_notebook_bad_code.egg-info/
--rw-rw-rw-   0        0        0      263 2023-07-08 15:34:37.000000 rydeen-lesson-notebook-bad-code-0.1.2/rydeen_lesson_notebook_bad_code.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2023-07-08 15:34:37.000000 rydeen-lesson-notebook-bad-code-0.1.2/rydeen_lesson_notebook_bad_code.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 15:34:37.000000 rydeen-lesson-notebook-bad-code-0.1.2/rydeen_lesson_notebook_bad_code.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-07-08 15:34:37.000000 rydeen-lesson-notebook-bad-code-0.1.2/rydeen_lesson_notebook_bad_code.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 15:34:37.523267 rydeen-lesson-notebook-bad-code-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      378 2023-07-08 15:31:04.000000 rydeen-lesson-notebook-bad-code-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 15:34:37.517273 rydeen-lesson-notebook-bad-code-0.1.2/terminal_notebook_project/
--rw-rw-rw-   0        0        0     4577 2023-07-08 15:29:57.000000 rydeen-lesson-notebook-bad-code-0.1.2/terminal_notebook_project/file_models.py
--rw-rw-rw-   0        0        0     1033 2023-07-08 13:27:51.000000 rydeen-lesson-notebook-bad-code-0.1.2/terminal_notebook_project/models.py
--rw-rw-rw-   0        0        0     2129 2023-07-08 15:29:18.000000 rydeen-lesson-notebook-bad-code-0.1.2/terminal_notebook_project/presenter.py
--rw-rw-rw-   0        0        0      385 2023-07-08 14:15:42.000000 rydeen-lesson-notebook-bad-code-0.1.2/terminal_notebook_project/view.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:33:44.153894 rydeen-lesson-notebook-bad-code-0.1.3/
+-rw-rw-rw-   0        0        0      263 2023-07-11 10:33:44.152894 rydeen-lesson-notebook-bad-code-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-11 10:33:44.142903 rydeen-lesson-notebook-bad-code-0.1.3/rydeen_lesson_notebook_bad_code.egg-info/
+-rw-rw-rw-   0        0        0      263 2023-07-11 10:33:43.000000 rydeen-lesson-notebook-bad-code-0.1.3/rydeen_lesson_notebook_bad_code.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2023-07-11 10:33:43.000000 rydeen-lesson-notebook-bad-code-0.1.3/rydeen_lesson_notebook_bad_code.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 10:33:43.000000 rydeen-lesson-notebook-bad-code-0.1.3/rydeen_lesson_notebook_bad_code.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2023-07-11 10:33:43.000000 rydeen-lesson-notebook-bad-code-0.1.3/rydeen_lesson_notebook_bad_code.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-11 10:33:44.153894 rydeen-lesson-notebook-bad-code-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      378 2023-07-11 10:32:55.000000 rydeen-lesson-notebook-bad-code-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 10:33:44.150896 rydeen-lesson-notebook-bad-code-0.1.3/terminal_notebook_project/
+-rw-rw-rw-   0        0        0     4548 2023-07-10 18:01:40.000000 rydeen-lesson-notebook-bad-code-0.1.3/terminal_notebook_project/file_models.py
+-rw-rw-rw-   0        0        0      966 2023-07-11 09:40:24.000000 rydeen-lesson-notebook-bad-code-0.1.3/terminal_notebook_project/models.py
+-rw-rw-rw-   0        0        0      949 2023-07-11 09:26:21.000000 rydeen-lesson-notebook-bad-code-0.1.3/terminal_notebook_project/presenter.py
+-rw-rw-rw-   0        0        0     1217 2023-07-11 09:51:46.000000 rydeen-lesson-notebook-bad-code-0.1.3/terminal_notebook_project/view.py
```

### Comparing `rydeen-lesson-notebook-bad-code-0.1.2/terminal_notebook_project/file_models.py` & `rydeen-lesson-notebook-bad-code-0.1.3/terminal_notebook_project/file_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         :return: None
         :rtype: NoneType
         """
         with open(self.__filename, "w") as f:
             f.write(jsonpickle.encode(data))
 
 
-class DataBase:
+class Database:
     """
     This class works with the database
 
     :param filename: Get name of file to work
     :type: str
     :param mode: With what type of file mast work data base. Default = byte
     :type: str, optional
@@ -180,10 +180,7 @@
         """
         Show database
 
         :return: Return object selected class
         :rtype: object
         """
         return f"{self.data}"
-
-
-db = DataBase("db.txt")
```

### Comparing `rydeen-lesson-notebook-bad-code-0.1.2/terminal_notebook_project/models.py` & `rydeen-lesson-notebook-bad-code-0.1.3/terminal_notebook_project/models.py`

 * *Files 23% similar despite different names*

```diff
@@ -14,30 +14,31 @@
         """
         Constract method
         """
         self.title = title
         self.date = date
         self.text = text
 
-    @property
     def show(self):
         """
         This method shows the full information that is stored
-        in the Note object.  Contains the title of the note,
-        the creation date and the text of the note
+        in the Note object.
+        Contains:
+            Note title;
+            Date of creation:
+            Note text.
 
-        :return: Returns the contents of the Note object in f-string
-        :rtype: str
+        :return: None
+        :rtype: NoneType
         """
-        return f"""\nTitle: {self.text}
+        print(f"""\nTitle: {self.text}
 Date: {self.date}
-Text: {self.text}"""
+Text: {self.text}""")
 
-    @property
-    def show_title(self):
+    def __str__(self):
         """
-        This method return note title
+        Return title of class object
 
-        :return: Return Note object title
+        :return: Return objectvtitle
         :rtype: str
         """
         return self.title
```

