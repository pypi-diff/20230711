# Comparing `tmp/cgpmgr-1.5.tar.gz` & `tmp/cgpmgr-1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgpmgr-1.5.tar", last modified: Tue Jun 27 14:41:01 2023, max compression
+gzip compressed data, was "cgpmgr-1.6.tar", last modified: Tue Jul  4 05:28:33 2023, max compression
```

## Comparing `cgpmgr-1.5.tar` & `cgpmgr-1.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-27 14:41:01.235649 cgpmgr-1.5/
--rw-r--r--   0 pi        (1000) pi        (1000)    11342 2021-09-04 14:18:09.000000 cgpmgr-1.5/LICENSE
--rw-r--r--   0 pi        (1000) pi        (1000)      307 2023-06-27 14:41:01.235649 cgpmgr-1.5/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     2812 2023-06-05 04:58:21.000000 cgpmgr-1.5/README.md
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-27 14:41:01.225649 cgpmgr-1.5/cgpmgr/
--rwxr-xr-x   0 pi        (1000) pi        (1000)       19 2021-09-05 05:17:17.000000 cgpmgr-1.5/cgpmgr/__init__.py
--rwxr-xr-x   0 pi        (1000) pi        (1000)    30617 2023-06-27 14:40:06.000000 cgpmgr-1.5/cgpmgr/cli.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-06-27 14:41:01.235649 cgpmgr-1.5/cgpmgr.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)      307 2023-06-27 14:41:01.000000 cgpmgr-1.5/cgpmgr.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      241 2023-06-27 14:41:01.000000 cgpmgr-1.5/cgpmgr.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-06-27 14:41:01.000000 cgpmgr-1.5/cgpmgr.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-27 14:41:01.000000 cgpmgr-1.5/cgpmgr.egg-info/entry_points.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       14 2023-06-27 14:41:01.000000 cgpmgr-1.5/cgpmgr.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        7 2023-06-27 14:41:01.000000 cgpmgr-1.5/cgpmgr.egg-info/top_level.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-06-27 14:41:01.235649 cgpmgr-1.5/setup.cfg
--rwxr-xr-x   0 pi        (1000) pi        (1000)      478 2023-06-27 14:40:06.000000 cgpmgr-1.5/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-04 05:28:33.150441 cgpmgr-1.6/
+-rw-r--r--   0 pi        (1000) pi        (1000)    11342 2021-09-04 14:18:09.000000 cgpmgr-1.6/LICENSE
+-rw-r--r--   0 pi        (1000) pi        (1000)      307 2023-07-04 05:28:33.140440 cgpmgr-1.6/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     2812 2023-06-05 04:58:21.000000 cgpmgr-1.6/README.md
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-04 05:28:33.120440 cgpmgr-1.6/cgpmgr/
+-rwxr-xr-x   0 pi        (1000) pi        (1000)       19 2021-09-05 05:17:17.000000 cgpmgr-1.6/cgpmgr/__init__.py
+-rwxr-xr-x   0 pi        (1000) pi        (1000)    31122 2023-07-04 05:26:27.000000 cgpmgr-1.6/cgpmgr/cli.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-04 05:28:33.140440 cgpmgr-1.6/cgpmgr.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)      307 2023-07-04 05:28:32.000000 cgpmgr-1.6/cgpmgr.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      241 2023-07-04 05:28:33.000000 cgpmgr-1.6/cgpmgr.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-07-04 05:28:32.000000 cgpmgr-1.6/cgpmgr.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-07-04 05:28:32.000000 cgpmgr-1.6/cgpmgr.egg-info/entry_points.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       14 2023-07-04 05:28:32.000000 cgpmgr-1.6/cgpmgr.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        7 2023-07-04 05:28:32.000000 cgpmgr-1.6/cgpmgr.egg-info/top_level.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       38 2023-07-04 05:28:33.150441 cgpmgr-1.6/setup.cfg
+-rwxr-xr-x   0 pi        (1000) pi        (1000)      478 2023-07-04 05:26:27.000000 cgpmgr-1.6/setup.py
```

### Comparing `cgpmgr-1.5/LICENSE` & `cgpmgr-1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cgpmgr-1.5/README.md` & `cgpmgr-1.6/README.md`

 * *Files identical despite different names*

### Comparing `cgpmgr-1.5/cgpmgr/cli.py` & `cgpmgr-1.6/cgpmgr/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Raspberry Pi/Jetson Nano電源管理 拡張基板 RPZ-PowerMGR用コントロールツール
 Indoor Corgi, https://www.indoorcorgielec.com
 GitHub: https://github.com/IndoorCorgi/cgpmgr
-Version 1.5
+Version 1.6
 
 必要環境:
 1) Raspberry Pi OS / Jetson Linux, Python3
 2) I2Cインターフェース
   Raspberry PiでI2Cを有効にする方法
   https://www.indoorcorgielec.com/resources/raspberry-pi/raspberry-pi-i2c/
 3) 電源管理 拡張基板 RPZ-PowerMGR
@@ -44,15 +44,15 @@
   -D <date>  登録するスケジュールの月/日を指定. *か**で全てに一致. 
              日はSun, Mon, Tue, Wed, Thu, Fri, Satで曜日も指定可能. 例)5/10, , 9/Sun, */15. 
   <time>     登録するスケジュールの時:分を指定. *か**で全てに一致. 
              分は*指定不可. 例)21:30, *:45
   on         電源をONするスケジュールを登録する. 
   off        電源をOFFするスケジュールを登録する. 
   -l <min>   現在からmin分後にスケジュールを登録. 秒は切り上げになる. 0-999の範囲で指定. 
-             0を指定すると1分単位で可能な限り早いスケジュールになる. 
+             0を指定すると可能な限り早いスケジュールになる. 
              このオプションで登録するとOneTime(1回のみ)になる. 
   -R <num>   指定すると登録済みスケジュールから指定番号のものを削除. 255を指定すると全て削除. 
   -i         スケジュールをcsvファイルから読み出して追加する. 
              省略すると登録済みスケジュールをcsvファイルに保存する.
 
   me         Raspberry Pi/Jetson Nanoの消費電流測定, 結果ログを行うサブコマンド. 
              オプションを指定しないと直近の電流測定値を表示. 
@@ -77,32 +77,34 @@
 import struct
 import subprocess
 import hashlib
 import smbus2
 import RPi.GPIO as GPIO
 
 i2c_adr = 0x20
-compatible_fw = {1: 5, 2: 2}
+compatible_fw = {1: 6, 2: 3}
 sig2gpio = [0, 16, 17, 26, 27]  # SIG番号とGPIO番号の対応
 dow2str = ['Sun', 'Mon', 'Tue', 'Wed', 'Thu', 'Fri', 'Sat']  # スケジュールデータは日曜が1, 土曜が7
 gpio_rst = 7
 gpio_boot = 25
 fw_ver = []
 
 # ファームウェアハッシュ値
 known_hash = [
     'cf0d1818ade696bc5b7af150ff4a085266fdc829f196f26ed2ed127b7ba12eb3',  # Ver1.0
     '1a6fdf815b5b23a6e39c79d6b734bfd3bd51ddf59b803912425bfc07504f0d1b',  # Ver1.1
     '5764c3cc8442930997fefcc048e35a8242df9bdcdf5f302ed4fb43f1a4fd8c24',  # Ver1.2
     'a37fe6f36a4e99bab07e3106cb99306d13f88d4c72c68b309a4fd9eb8e4c44e8',  # Ver1.3
     '36313403baab9d50183f17d0f9cea991455baf7b1b0478e1ef8773cee0ea91cc',  # Ver1.4
     'c3f465e5c8e2e004b23d85a6f5846931e106fd8a06715d48e54750c875cfe882',  # Ver1.5
+    '6aff47c6ceb831cf48662a71dcc0090b437a6129aa8b29d5bcebb5e0cd46e98b',  # Ver1.6
     '0bdb41e819fcd8380a9bf1f551a6a7692bd22bcdb3734580413e4401fa613490',  # Ver2.0
     'f5aa9ab42affd8004238bf1f747d93095b5138602473660eb7965a24d03b167b',  # Ver2.1
     'a49c1fa3c1f540fcbb77d69be4d599791d3a5a88508e7519aaab2c5426f0fb0c',  # Ver2.2
+    'c39cc7100644abafd3f69bc0b61304093b4a535097fd637282837ed8fe007821',  # Ver2.3
 ]
 
 
 def cli():
   """
   コマンドラインツールを実行
   """
@@ -304,14 +306,22 @@
 
     if args['-o']:
       sch[0] |= 0x80
 
     if args['-l'] != None:
       if not check_digit('-l', args['-l'], 0, 999):
         return
+
+      # -l 0 offかつファームウェアが対応している場合, すぐにシャットダウンリクエスト
+      if 0 == int(args['-l']):
+        if (fw_ver[1] == 1 and fw_ver[0] >= 6) or (fw_ver[1] == 2 and fw_ver[0] >= 3):
+          print('シャットダウン要求を開始します')
+          i2c_write(0x40, [0xFF])
+          return
+
       dtrtc = read_rtc()
       delay = int(args['-l'])
       if delay == 0:
         dt = dtrtc + datetime.timedelta(seconds=75)  # 通信, 計算マージン15秒 + 桁繰り上げ用60秒
       else:
         dt = dtrtc + datetime.timedelta(minutes=1 + delay)
       sch[0] |= dt.minute | 0x80
```

