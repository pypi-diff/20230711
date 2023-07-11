# Comparing `tmp/tianhutools-1.0.2.tar.gz` & `tmp/tianhutools-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tianhutools-1.0.2.tar", last modified: Sat Jun 24 05:38:40 2023, max compression
+gzip compressed data, was "tianhutools-1.0.3.tar", last modified: Tue Jul 11 04:52:09 2023, max compression
```

## Comparing `tianhutools-1.0.2.tar` & `tianhutools-1.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 05:38:40.025871 tianhutools-1.0.2/
--rw-rw-rw-   0        0        0       29 2023-06-03 09:16:20.000000 tianhutools-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4576 2023-06-24 05:38:40.023871 tianhutools-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4127 2023-06-24 05:33:28.000000 tianhutools-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-06-24 05:38:40.025871 tianhutools-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1134 2023-06-24 05:33:35.000000 tianhutools-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:38:40.000870 tianhutools-1.0.2/tianhutools/
--rw-rw-rw-   0        0        0        0 2023-05-25 09:22:46.000000 tianhutools-1.0.2/tianhutools/__init__.py
--rw-rw-rw-   0        0        0     2212 2023-05-27 05:03:59.000000 tianhutools-1.0.2/tianhutools/ip.py
--rw-rw-rw-   0        0        0     6929 2023-06-24 05:31:21.000000 tianhutools-1.0.2/tianhutools/jiami.py
--rw-rw-rw-   0        0        0     2313 2023-06-03 09:54:50.000000 tianhutools-1.0.2/tianhutools/text.py
-drwxrwxrwx   0        0        0        0 2023-06-24 05:38:40.018871 tianhutools-1.0.2/tianhutools.egg-info/
--rw-rw-rw-   0        0        0     4576 2023-06-24 05:38:39.000000 tianhutools-1.0.2/tianhutools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-06-24 05:38:39.000000 tianhutools-1.0.2/tianhutools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 05:38:39.000000 tianhutools-1.0.2/tianhutools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2023-06-24 05:38:39.000000 tianhutools-1.0.2/tianhutools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-24 05:38:39.000000 tianhutools-1.0.2/tianhutools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 04:52:09.294236 tianhutools-1.0.3/
+-rw-rw-rw-   0        0        0       29 2023-06-03 09:16:20.000000 tianhutools-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4666 2023-07-11 04:52:09.293236 tianhutools-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4217 2023-07-11 04:46:21.000000 tianhutools-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-11 04:52:09.298236 tianhutools-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1140 2023-07-11 04:52:03.000000 tianhutools-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 04:52:09.258234 tianhutools-1.0.3/tianhutools/
+-rw-rw-rw-   0        0        0        0 2023-05-25 09:22:46.000000 tianhutools-1.0.3/tianhutools/__init__.py
+-rw-rw-rw-   0        0        0     2212 2023-05-27 05:03:59.000000 tianhutools-1.0.3/tianhutools/ip.py
+-rw-rw-rw-   0        0        0     7745 2023-07-11 04:44:34.000000 tianhutools-1.0.3/tianhutools/jiami.py
+-rw-rw-rw-   0        0        0     2313 2023-06-03 09:54:50.000000 tianhutools-1.0.3/tianhutools/text.py
+drwxrwxrwx   0        0        0        0 2023-07-11 04:52:09.290236 tianhutools-1.0.3/tianhutools.egg-info/
+-rw-rw-rw-   0        0        0     4666 2023-07-11 04:52:08.000000 tianhutools-1.0.3/tianhutools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-07-11 04:52:09.000000 tianhutools-1.0.3/tianhutools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 04:52:08.000000 tianhutools-1.0.3/tianhutools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-07-11 04:52:08.000000 tianhutools-1.0.3/tianhutools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-11 04:52:08.000000 tianhutools-1.0.3/tianhutools.egg-info/top_level.txt
```

### Comparing `tianhutools-1.0.2/PKG-INFO` & `tianhutools-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tianhutools
-Version: 1.0.2
+Version: 1.0.3
 Summary: 由天狐宗开发的工具，方便开发时使用,已更名为tianhutools
 Home-page: https://github.com/tianhuzong/thztools
 Author: Sen
 Author-email: tianhuzong@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,14 +30,16 @@
 - - -
 >2023-6-3 +0800，正式更名为tianhutool，版本重置
 >并加入了文本缩短
 - - -
 >new 1.0.1版本中，将文本缩短修改为使用Python标准库re,math,和第三方库jieba
 - - -
 >1.0.2版本中，修复了上个版本未将jieba安装进setup，并将rsa密钥修改为pem格式，rsa的密文，明文，签名文本与aes的密文，明文都修改为base64
+- - -
+>1.0.3版本中，修改了AES加密使用的lib，修复了RSA加密出的错误
 ##使用方法：
 - - -
 ####安装模块
 ```bash
 pip install tianhutools
 ```
 安装完模块之后接下来就是引用了
```

### Comparing `tianhutools-1.0.2/README.md` & `tianhutools-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 - - -
 >2023-6-3 +0800，正式更名为tianhutool，版本重置
 >并加入了文本缩短
 - - -
 >new 1.0.1版本中，将文本缩短修改为使用Python标准库re,math,和第三方库jieba
 - - -
 >1.0.2版本中，修复了上个版本未将jieba安装进setup，并将rsa密钥修改为pem格式，rsa的密文，明文，签名文本与aes的密文，明文都修改为base64
+- - -
+>1.0.3版本中，修改了AES加密使用的lib，修复了RSA加密出的错误
 ##使用方法：
 - - -
 ####安装模块
 ```bash
 pip install tianhutools
 ```
 安装完模块之后接下来就是引用了
```

### Comparing `tianhutools-1.0.2/setup.py` & `tianhutools-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup
 with open("./README.md",mode='r',encoding='utf-8') as f:
     des = f.read()
 setup(
     name="tianhutools",      # 包名，用于安装和调用该包
-    version="1.0.2",               # 版本号
+    version="1.0.3",               # 版本号
     author="Sen",
     description="由天狐宗开发的工具，方便开发时使用,已更名为tianhutools",
     long_description=des,
     long_description_content_type='text/markdown',
     author_email="tianhuzong@qq.com",
     url="https://github.com/tianhuzong/thztools",
     license="MIT",
     packages=["tianhutools"],     # 需要打包的包，可以是单个或多个包
     package_data={"tianhutools": ["*.py"]},  # 包需要包含的数据文件（可选）
     install_requires=[           # 安装依赖，可以是单个或多个依赖项
         "rsa",
-        "Crypto",
+        "cryptography",
         "2ip",
         "sumy",
         "jieba"
     ],
     classifiers=[                # 分类标签（可选），使用 PyPI 标准分类
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
```

### Comparing `tianhutools-1.0.2/tianhutools/ip.py` & `tianhutools-1.0.3/tianhutools/ip.py`

 * *Files identical despite different names*

### Comparing `tianhutools-1.0.2/tianhutools/jiami.py` & `tianhutools-1.0.3/tianhutools/jiami.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-from Crypto.Cipher import AES as AESclass
-from Crypto.Random import get_random_bytes
+from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
+from cryptography.hazmat.primitives import padding
+from cryptography.hazmat.backends import default_backend
+from cryptography.hazmat.primitives import hashes
 import rsa
 import base64
-
+import os
 def __bytes_to_b64(bytes_var : bytes) -> str:
     return base64.b64decode(bytes_var)
 def __b64_to_bytes(b64str : str) -> bytes:
     return base64.b64encode(b64str)
 class KaiSa:
     def jiami(self,plaintext, shift):
         """
@@ -40,108 +42,133 @@
                 if char.isupper():  # 大写字母
                     num = (num - 65 - shift) % 26 + 65
                 else:  # 小写字母
                     num = (num - 97 - shift) % 26 + 97
                 char = chr(num)
             plaintext += char
         return plaintext
+import base64
+import rsa
+
 class RSA:
-    def newkeys(self,length : int = 1024):
+    def newkeys(self, length: int = 1024):
         """
         生成一个rsa密钥对，默认为1024位
         :param length : int,长度，默认为1024
         :return 公钥,私钥
         """
-        (gongyao,siyao) = rsa.newkeys(length)
+        (gongyao, siyao) = rsa.newkeys(length)
         gongyao_save = gongyao.save_pkcs1().decode()
         siyao_save = siyao.save_pkcs1().decode()
-        return gongyao_save,siyao_save
-    def jiami(self,gongyao,text) -> str:
+        return gongyao_save, siyao_save
+
+    def jiami(self, gongyao, text) -> str:
         """
         使用rsa算法进行加密
         Args:
             gongyao : rsa 公钥pem格式
             text : 欲加密文本
         Return:
             返回密文(base64)
         """
         message = text.encode()
         gongyao_obj = rsa.PublicKey.load_pkcs1(gongyao.encode())
-        miwen = base64.b64decode( rsa.encrypt(message, gongyao_obj) ).decode()
+        miwen = base64.b64encode(rsa.encrypt(message, gongyao_obj)).decode()
         return miwen
-    def jiemi(self,siyao,miwen:str):
+
+    def jiemi(self, siyao, miwen: str):
         """
         使用rsa算法进行解密
         Args:
             siyao : rsa私钥,pem格式
             miwen : 密文（base64）
         Return:
             明文
         """
-        return rsa.decrypt(base64.b64encode(miwen), siyao).decode()
-    def sign(self,siyao,text):
+        siyao_obj = rsa.PrivateKey.load_pkcs1(siyao)
+        plaintext = rsa.decrypt(base64.b64decode(miwen), siyao_obj).decode()
+        return plaintext
+
+    def sign(self, siyao, text):
         """
         使用rsa算法进行数字签名
         :param siyao:rsa私钥,pem格式
         :param text:欲签名文本
         :return 返回签名文本
         """
         siyao_obj = rsa.PrivateKey.load_pkcs1(siyao)
-        qianminwenben = base64.b64decode( rsa.sign(text.encode(),siyao_obj,'SHA-1') ).decode()
+        qianminwenben = base64.b64encode(rsa.sign(text.encode(), siyao_obj, 'SHA-1')).decode()
         return qianminwenben
-    def qmyz(self,text,qmwb,gongyao):
+
+    def qmyz(self, text, qmwb, gongyao):
         """
         签名验证
         :param text:被验证的文本
         :param qmwb:签名文本，sign()函数的返回值
         :param gongyao:rsa公钥,pem格式
         :return 成功返回True，失败返回False
         """
-        res = rsa.verify(text.encode(),base64.b64encode(qmwb),rsa.PublicKey.load_pkcs1(gongyao))
+        res = rsa.verify(text.encode(), base64.b64decode(qmwb), rsa.PublicKey.load_pkcs1(gongyao))
         if res:
             return True
         else:
             return False
+
+
 class AES:
     def newkey(self):
         """
         自动生成32位（256位）AES秘钥
-        :return key，base64编码的key
+        :return: key，base64编码的key
         """
-        key = get_random_bytes(32)
-        return base64.b64decode(key).decode()
+        key = os.urandom(32)
+        return base64.b64encode(key).decode()
 
-    def jiami(self,plaintext, key):
+    def jiami(self, plaintext, key):
         """
         AES加密算法
         plaintext: 明文
-        key: 秘钥,base64
+        key: 秘钥, base64编码的字符串
         Returns:
-            密文,随机数，验证标签，均为str类型的base64编码
+            密文, 随机数，验证标签，均为str类型的base64编码
         """
-        # 用秘钥创建一个AES对象
-        cipher = AESclass.new(base64.b64encode(key), AESclass.MODE_EAX)
-        # 加密明文
-        ciphertext, tag = cipher.encrypt_and_digest(plaintext.encode('utf-8'))
-        # 返回加密后的密文和必要的参数
-        return __bytes_to_b64(ciphertext), __bytes_to_b64(cipher.nonce), __bytes_to_b64(tag)
+        key_bytes = base64.b64decode(key)
+        iv = os.urandom(12)  # 生成12字节的随机向量
+        cipher = Cipher(algorithms.AES(key_bytes), modes.GCM(iv), backend=default_backend())
+        encryptor = cipher.encryptor()
+
+        padder = padding.PKCS7(algorithms.AES.block_size).padder()
+        padded_data = padder.update(plaintext.encode('utf-8')) + padder.finalize()
+
+        ciphertext = encryptor.update(padded_data) + encryptor.finalize()
 
-    def jiemi(self,ciphertext, key, nonce, tag):
+        return base64.b64encode(ciphertext).decode(), base64.b64encode(iv).decode(), base64.b64encode(
+            encryptor.tag).decode()
+
+    def jiemi(self, ciphertext, key, iv, tag):
         """
         AES解密算法
         ciphertext: 密文
         key: 秘钥
-        nonce: 加密时生成的随机数
+        iv: 加密时生成的随机向量
         tag: 加密时生成的验证标签
         """
-        # 用密钥和随机数创建一个AES对象
-        cipher = AESclass.new(__b64_to_bytes(key), AESclass.MODE_EAX, nonce=__b64_to_bytes(nonce))
+        key_bytes = base64.b64decode(key)
+        iv_bytes = base64.b64decode(iv)
+        tag_bytes = base64.b64decode(tag)
+
+        cipher = Cipher(algorithms.AES(key_bytes), modes.GCM(iv_bytes, tag_bytes), backend=default_backend())
+        decryptor = cipher.decryptor()
+
         try:
-            # 解密密文
-            plaintext = cipher.decrypt_and_verify(__b64_to_bytes(ciphertext), __b64_to_bytes(tag))
+            padded_data = decryptor.update(base64.b64decode(ciphertext)) + decryptor.finalize()
+
+            unpadder = padding.PKCS7(algorithms.AES.block_size).unpadder()
+            plaintext = unpadder.update(padded_data) + unpadder.finalize()
+
             return plaintext.decode('utf-8')
         except:
             return None
 class Weijiniya:
     def jiami(self,plaintext, key):
         """
         使用维吉尼亚密码加密明文字符串
```

### Comparing `tianhutools-1.0.2/tianhutools/text.py` & `tianhutools-1.0.3/tianhutools/text.py`

 * *Files identical despite different names*

### Comparing `tianhutools-1.0.2/tianhutools.egg-info/PKG-INFO` & `tianhutools-1.0.3/tianhutools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tianhutools
-Version: 1.0.2
+Version: 1.0.3
 Summary: 由天狐宗开发的工具，方便开发时使用,已更名为tianhutools
 Home-page: https://github.com/tianhuzong/thztools
 Author: Sen
 Author-email: tianhuzong@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -30,14 +30,16 @@
 - - -
 >2023-6-3 +0800，正式更名为tianhutool，版本重置
 >并加入了文本缩短
 - - -
 >new 1.0.1版本中，将文本缩短修改为使用Python标准库re,math,和第三方库jieba
 - - -
 >1.0.2版本中，修复了上个版本未将jieba安装进setup，并将rsa密钥修改为pem格式，rsa的密文，明文，签名文本与aes的密文，明文都修改为base64
+- - -
+>1.0.3版本中，修改了AES加密使用的lib，修复了RSA加密出的错误
 ##使用方法：
 - - -
 ####安装模块
 ```bash
 pip install tianhutools
 ```
 安装完模块之后接下来就是引用了
```

