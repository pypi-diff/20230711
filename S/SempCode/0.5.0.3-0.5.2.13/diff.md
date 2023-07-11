# Comparing `tmp/SempCode-0.5.0.3-py3-none-any.whl.zip` & `tmp/SempCode-0.5.2.13-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5634 bytes, number of entries: 9
+Zip file size: 6394 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat     1808 b- defN 23-Jul-10 12:58 Semp/Command.py
 -rw-rw-rw-  2.0 fat     2390 b- defN 23-Jul-08 10:25 Semp/SempWrite.py
--rw-rw-rw-  2.0 fat     3938 b- defN 23-Jul-10 13:08 Semp/__init__.py
+-rw-rw-rw-  2.0 fat     5623 b- defN 23-Jul-11 09:52 Semp/__init__.py
 -rw-rw-rw-  2.0 fat      370 b- defN 23-Jul-08 11:54 Semp/about.py
--rw-rw-rw-  2.0 fat     2594 b- defN 23-Jul-10 13:24 Semp/EasyTkinter/__init__.py
--rw-rw-rw-  2.0 fat      842 b- defN 23-Jul-10 13:26 SempCode-0.5.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-10 13:26 SempCode-0.5.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-10 13:26 SempCode-0.5.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      681 b- defN 23-Jul-10 13:26 SempCode-0.5.0.3.dist-info/RECORD
-9 files, 12720 bytes uncompressed, 4470 bytes compressed:  64.9%
+-rw-rw-rw-  2.0 fat     2644 b- defN 23-Jul-11 09:21 Semp/EasyTkinter/__init__.py
+-rw-rw-rw-  2.0 fat     1118 b- defN 23-Jul-11 09:53 SempCode-0.5.2.13.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-11 09:53 SempCode-0.5.2.13.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 23-Jul-11 09:53 SempCode-0.5.2.13.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      686 b- defN 23-Jul-11 09:53 SempCode-0.5.2.13.dist-info/RECORD
+9 files, 14736 bytes uncompressed, 5222 bytes compressed:  64.6%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: Semp/about.py
 Comment: 
 
 Filename: Semp/EasyTkinter/__init__.py
 Comment: 
 
-Filename: SempCode-0.5.0.3.dist-info/METADATA
+Filename: SempCode-0.5.2.13.dist-info/METADATA
 Comment: 
 
-Filename: SempCode-0.5.0.3.dist-info/WHEEL
+Filename: SempCode-0.5.2.13.dist-info/WHEEL
 Comment: 
 
-Filename: SempCode-0.5.0.3.dist-info/top_level.txt
+Filename: SempCode-0.5.2.13.dist-info/top_level.txt
 Comment: 
 
-Filename: SempCode-0.5.0.3.dist-info/RECORD
+Filename: SempCode-0.5.2.13.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Semp/__init__.py

```diff
@@ -1,31 +1,39 @@
 """
     Semp Python Tool by Win12Home
-    Version:0.5.0.3 Beta
+    Version:0.5.2.13 Beta
     
 """
 from PIL import Image,ImageTk
 from requests import *
 from sys import set_int_max_str_digits as max
 from subprocess import Popen
+from random import randint
+from datetime import datetime
 
 
 max(0)
 BINARY_TRUE="BTRUE"
 BINARY_FALSE="BFALSE"
 
+AUTO="AutoEnter"
+NONE="NoEnter"
+
 class NumberError(Exception):
     def __init__(self, *args, **kwargs):
         pass
 
 class BoolError(Exception):
     def __init__(self, *args, **kwargs):
         pass
 
- 
+class ArgumentError(Exception):
+    def __init__(self, *args, **kwargs):
+        pass
+
 def PhotoTk(file: str = ...):
     photo=Image.open(file)
     #Open Photo
     tkphoto=ImageTk.PhotoImage(image=photo)
     #Save Photo
     return tkphoto
 
@@ -39,15 +47,26 @@
         try:
             for x in range(b_from, to + 1,passnum):
                 a.append(x)
             return a
         except:
             raise NumberError("Name error.")
 
- 
+def CreatePassword(length: int = ...):
+    sslist=["0","1","2","3","4","5","6","7","8","9","^","%","a","A","B","c","C","d","E","f","D","F","g","H","i","j","K","l","M","N","o","P","q","Q","r","s"
+          ,"t","U","V","v","T","w","W","x","Y","z","!"]
+    password=""
+    temps=""
+    for __count in range(length):
+        for __count in range(5):
+            temps=sslist[randint(0,len(sslist)-1)]
+        password+=temps
+    return password
+
+
 class request_simplifies:
     def Download(website: str = ...,name: str = ...,binary: bool = ...):
         r = get(website)
         if binary == True or binary == BINARY_TRUE:
             with open(name, "wb") as f:
                 for chunk in r.iter_content(chunk_size=512):
                     f.write(chunk)
@@ -112,14 +131,42 @@
  
 def CmdPrompt():
     Popen(
         "cmd.exe",
         shell=True
     )
 
+def CreateMarkdown(title: str = ...,text: list[str] = ...,name: str = ...,auto: str = AUTO):
+    markdown=""
+    markdown+=f"---\n{title}\n---\n"
+    if auto == AUTO:
+        for word in text:
+            markdown+=f"{word}<br/>"
+            with open(name, "w") as f:
+                f.write(markdown)
+    elif auto == NONE:
+        for word in text:
+            markdown+=word
+        with open(name,"w") as f:
+            f.write(markdown)
+    else:
+        raise ArgumentError("Not in AUTO or NONE")
+
+def GetTime(format:str = "%Y.%m.%d %H:%M:%S"):
+    return datetime.now().strftime(format)
+
+def NowDate():
+    return datetime.now()
+
+def Date(year:int = ...,month:int = ...,day: int = ...):
+    return datetime(year,month,day)
+
+def DateWeekday(datevar):
+    weekday={1:"Monday",2:"Tuesday",3:"Wednesday",4:"Thursday",5:"Friday",6:"Saturday",7:"Sunday"}
+    return weekday[int(datevar.isoweekday())]
 """
 Here are some examples.
 Response(variable):
     response=Requester("https://1.1.1.1/")
     response.ResponseGet()
 Response(code):
     request_simplifies.ResponseGet("https://1.1.1.1/")
@@ -133,8 +180,10 @@
     from tkinter import *
     root=Tk()
     root.title("Test")
     img=PhotoTk("C:/test.jpg")
     a=Label(self,image=img)
     a.pack()
     root.mainloop()
+Markdown Creator:
+    CreateMarkdown("Hello World!",["They are some example","They are some example"],"README.md")
 """
```

## Semp/EasyTkinter/__init__.py

```diff
@@ -30,14 +30,15 @@
         self.text=Text(self,bd=0,font=(font,8))
         self.text.pack()
         self.text.insert(END, text)
         self.text.configure(state=DISABLED)
 
         self.exit=Button(self,text="Exit",command=lambda:self.quit())
         self.exit.pack()
+        self.mainloop()
 
 class CommandWindow(ThemedTk):
     def __init__(self,theme:str = DEFAULT_THEME,font:str = DEFAULT_FONT):
         super().__init__(theme=theme)
         self.configure(bg="white")
         self.wm_title("Command Prompt")
         self.wm_state("zoomed")
@@ -56,14 +57,15 @@
         self.ppppppp.geometry("600x200")
         self.entry=Entry(self.ppppppp)
         self.entry.pack(fill=X)
         self.ppppppp.configure(bg="white")
 
         self.button=Button(self.ppppppp,text="Done",command=lambda:self.to_use(command=self.entry.get()))
         self.button.pack()
+        self.mainloop()
     def to_use(self,command:str = ...):
         self.ppppppp.destroy()
         self.Use(command=command)
     def Use(self,command:str = ...):
         self.runner=Popen(command,shell=True,stdout=PIPE,stderr=STDOUT,encoding="gb2312")
         self.text["state"]=NORMAL
         self.ms=self.runner.communicate()[0]
```

