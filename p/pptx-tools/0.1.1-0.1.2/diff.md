# Comparing `tmp/pptx-tools-0.1.1.tar.gz` & `tmp/pptx-tools-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pptx-tools-0.1.1.tar", last modified: Fri May 27 09:39:50 2022, max compression
+gzip compressed data, was "pptx-tools-0.1.2.tar", last modified: Tue Jul 11 05:23:47 2023, max compression
```

## Comparing `pptx-tools-0.1.1.tar` & `pptx-tools-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 09:39:50.830516 pptx-tools-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1058 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-05-27 09:39:50.830516 pptx-tools-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      256 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 09:39:50.822517 pptx-tools-0.1.1/pptx_tools/
--rw-r--r--   0 runner    (1001) docker     (121)      131 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/pptx_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 09:39:50.826516 pptx-tools-0.1.1/pptx_tools/apps/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/pptx_tools/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1853 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/pptx_tools/apps/slide_add_voice.py
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/pptx_tools/audio_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 09:39:50.826516 pptx-tools-0.1.1/pptx_tools/data/
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/pptx_tools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    38382 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/pptx_tools/data/hello.pptx
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/pptx_tools/data/transparent.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 09:39:50.826516 pptx-tools-0.1.1/pptx_tools/tts/
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/pptx_tools/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2287 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/pptx_tools/tts/azure_tts.py
--rw-r--r--   0 runner    (1001) docker     (121)    17546 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/pptx_tools/tts/azure_tts_voice.py
--rw-r--r--   0 runner    (1001) docker     (121)     2369 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/pptx_tools/tts/google_tts.py
--rw-r--r--   0 runner    (1001) docker     (121)    18411 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/pptx_tools/tts/google_tts_voice.py
--rw-r--r--   0 runner    (1001) docker     (121)     3293 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/pptx_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 09:39:50.826516 pptx-tools-0.1.1/pptx_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-05-27 09:39:50.000000 pptx-tools-0.1.1/pptx_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      764 2022-05-27 09:39:50.000000 pptx-tools-0.1.1/pptx_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-27 09:39:50.000000 pptx-tools-0.1.1/pptx_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-05-27 09:39:50.000000 pptx-tools-0.1.1/pptx_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-27 09:39:50.000000 pptx-tools-0.1.1/pptx_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-05-27 09:39:50.000000 pptx-tools-0.1.1/pptx_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-05-27 09:39:50.000000 pptx-tools-0.1.1/pptx_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-05-27 09:39:50.830516 pptx-tools-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2093 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 09:39:50.826516 pptx-tools-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-27 09:39:50.830516 pptx-tools-0.1.1/tests/pptx_tools/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/tests/pptx_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      648 2022-05-27 09:39:41.000000 pptx-tools-0.1.1/tests/pptx_tools/test_slide_add_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/pptx_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/pptx_tools/apps/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/apps/slide_add_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/audio_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/pptx_tools/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42073 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/data/hello.pptx
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/data/transparent.png
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/pptx_tools/tts/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/tts/azure_tts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17546 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/tts/azure_tts_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3357 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/tts/google_tts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18411 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/tts/google_tts_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/pptx_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-07-11 05:23:47.000000 pptx-tools-0.1.2/pptx_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-07-11 05:23:47.000000 pptx-tools-0.1.2/pptx_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 05:23:47.000000 pptx-tools-0.1.2/pptx_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-11 05:23:47.000000 pptx-tools-0.1.2/pptx_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 05:23:47.000000 pptx-tools-0.1.2/pptx_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      186 2023-07-11 05:23:47.000000 pptx-tools-0.1.2/pptx_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-11 05:23:47.000000 pptx-tools-0.1.2/pptx_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/tests/pptx_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/tests/pptx_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      712 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/tests/pptx_tools/test_slide_add_voice.py
```

### Comparing `pptx-tools-0.1.1/LICENSE` & `pptx-tools-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.1/pptx_tools/apps/slide_add_voice.py` & `pptx-tools-0.1.2/pptx_tools/apps/slide_add_voice.py`

 * *Files 20% similar despite different names*

```diff
@@ -26,21 +26,21 @@
                         default='google',
                         help='select the text-to-speech engine. '
                         'You can choose {}.'.format(tts_engines))
     args = parser.parse_args()
     if args.voice_name is not None:
         if args.tts == 'google' and args.voice_name not in google_voice:
             print('Invalid voice_name. Avaliable voices are:')
-            for voice in google_voice.keys():
-                print(voice)
+            print([voice for voice in google_voice.keys()])
+            print("You can check the sample audio here: "
+                  "https://cloud.google.com/text-to-speech/docs/voices")
             sys.exit(0)
         elif args.tts == 'azure' and args.voice_name not in azure_voice:
             print('Invalid voice_name. Avaliable voices are:')
-            for voice in azure_voice.keys():
-                print(voice)
+            print([voice for voice in azure_voice.keys()])
             sys.exit(0)
     output_dir = Path(make_fancy_output_dir(
         args.out, no_save=True))
     output_slide_path = add_synthesize_audio(
         args.input, output_dir, voice_name=args.voice_name)
     termcolor.cprint('=> Saved to {}'.format(output_slide_path), 'green')
```

### Comparing `pptx-tools-0.1.1/pptx_tools/data/hello.pptx` & `pptx-tools-0.1.2/pptx_tools/data/hello.pptx`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-00000000: 504b 0304 1400 0600 0800 0000 2100 34ee  PK..........!.4.
-00000010: e66e d701 0000 dd0d 0000 1300 0802 5b43  .n............[C
+00000000: 504b 0304 1400 0600 0800 0000 2100 ef28  PK..........!..(
+00000010: 90b2 e801 0000 720f 0000 1300 0802 5b43  ......r.......[C
 00000020: 6f6e 7465 6e74 5f54 7970 6573 5d2e 786d  ontent_Types].xm
 00000030: 6c20 a204 0228 a000 0200 0000 0000 0000  l ...(..........
 00000040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -29,49 +29,49 @@
 000001c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000001f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000230: 0000 0000 0000 0000 00cc 97db 52db 3010  ............R.0.
-00000240: 86ef 99e1 1d3c ba65 6225 b4a5 d089 c345  .....<.eb%.....E
-00000250: 0f57 2d30 033c 80b0 3789 4096 34d2 2625  .W-0.<..7.@.4.&%
-00000260: 6fcf 5a4e a861 9238 6de2 a96e 3c5e 6bff  o.ZN.a.8m..n<^k.
-00000270: 7f3f d9d6 6978 f95c aa64 0ece 4ba3 3336  .?..ix.\.d..K.36
-00000280: 48fb 2c01 9d9b 42ea 49c6 eeef 7ef4 ce59  H.,...B.I...~..Y
-00000290: e251 e842 28a3 2163 0bf0 ec72 747c 34bc  .Q.B(.!c...rt|4.
-000002a0: 5b58 f009 a9b5 cfd8 14d1 7ee1 dce7 5328  [X........~...S(
-000002b0: 854f 8d05 4d2d 63e3 4a81 14ba 09b7 227f  .O..M-c.J.....".
-000002c0: 1213 e0a7 fdfe 19cf 8d46 d0d8 c3ca 838d  .........F......
-000002d0: 86df 602c 660a 93ef cff4 b826 79b4 3061  ..`,f......&y.0a
-000002e0: c9d7 3ab1 aa95 3159 5606 a181 afd5 3850  ..:...1YV.....8P
-000002f0: fe9d 4658 ab64 2e90 daf9 5c17 efc8 7a4b  ..FX.d....\...zK
-00000300: aa94 9421 c74f a5f5 2794 b0a1 42d5 b2b9  ...!.O..'...B...
-00000310: c052 774d afd3 c902 921b e1f0 4a94 94c5  .RwM........J...
-00000320: ad45 6e1d 78d2 85dc 74bb d31a 5433 1ecb  .En.x...t...T3..
-00000330: 1c0a 93cf 4a92 a44d b352 bd09 d352 48bd  ....J..M.R...RH.
-00000340: eac4 2618 afe8 e12f e191 3e7d 3318 1c9a  ..&..../..>}3...
-00000350: ace1 bd13 d392 a61b 8e36 026d 10fc eaad  .........6.m....
-00000360: 3482 83d3 34bc db98 2ae5 8d33 d677 f1cf  4...4...*..3.w..
-00000370: 04e3 3682 b984 df9d 10bc 1ab7 1120 cd2b  ..6.......... .+
-00000380: 505f f7ff 14c1 a6b5 a278 5070 8b0b 0507  P_.......xPp....
-00000390: ef75 c37a a711 f153 2ccc 0c97 e3a2 0eba  .u.z...S,.......
-000003a0: 191d b5f7 bf32 9d46 c8f4 2142 a68f 1132  .....2.F..!B...2
-000003b0: 7d8a 90e9 2c42 a6cf 1132 9d47 c874 1121  }...,B...2.G.t.!
-000003c0: d3a0 1f23 d4ff 9cc9 1bab eafe 93f7 4eab  ...#..........N.
-000003d0: 6ad8 f6dc d6db bc3f f7dd ecae 82f5 3620  j......?......6 
-000003e0: 5287 cd07 1d47 1cfc 3dc2 eaec 50a9 7b96  R....G..=...P.{.
-000003f0: 8cc0 a1dc bea4 bf56 24eb bdfb 0cd5 b1a4  .......V$.......
-00000400: 8062 4d6d 1e0e 67a3 1700 0000 ffff 0300  .bMm..g.........
-00000410: 504b 0304 1400 0600 0800 0000 2100 68f8  PK..........!.h.
-00000420: 74a1 0301 0000 e202 0000 0b00 0802 5f72  t............._r
-00000430: 656c 732f 2e72 656c 7320 a204 0228 a000  els/.rels ...(..
-00000440: 0200 0000 0000 0000 0000 0000 0000 0000  ................
-00000450: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000230: 0000 0000 0000 0000 00cc 97cd 72da 3010  ............r.0.
+00000240: c7ef 99c9 3b78 74cd 6041 da7c b483 c921  ....;xt.`A.|...!
+00000250: 694f 4dc3 0cf4 0154 7b01 b5b2 a491 161a  iOM....T{.......
+00000260: debe 6b19 a89b 8140 623c f8c2 78ad ddff  ..k....@b<..x...
+00000270: fe64 a1d5 aa7f f79c ab68 01ce 4ba3 13d6  .d.......h..K...
+00000280: 8bbb 2c02 9d9a 4cea 69c2 7e8c bf76 6e59  ..,...L.i.~..vnY
+00000290: e451 e84c 28a3 2161 4bf0 ec6e 707e d61f  .Q.L(.!aK..np~..
+000002a0: 2f2d f888 a2b5 4fd8 0cd1 7ee6 dca7 33c8  /-....O...~...3.
+000002b0: 858f 8d05 4d23 13e3 7281 64ba 29b7 22fd  ....M#..r.d.).".
+000002c0: 2da6 c02f bbdd 6b9e 1a8d a0b1 8385 061b  -../..k.........
+000002d0: f41f 6022 e60a a32f cff4 ba24 f965 61ca  ..`".../...$.ea.
+000002e0: a2fb d2b1 c895 3099 1702 6180 6f8d 71a0  ......0...a.o.q.
+000002f0: fc8b 1861 ad92 a940 1ae7 0b9d bd20 ebac  ...a...@..... ..
+00000300: a862 8a0c 3e7e 26ad bf20 871d 198a 91dd  .b..>~&.. ......
+00000310: 0956 714f f439 9dcc 201a 0a87 df45 4e5e  .VqO.9.. ....EN^
+00000320: dc5a e4d6 81a7 b8e0 1bbf aeb4 05d5 4c26  .Z............L&
+00000330: 3285 cca4 f39c 42e2 aa58 aefe 33e3 5c48  2.....B..X..3.\H
+00000340: bd9e c42e 18af e8e5 a3f0 484b 5f35 7ac7  ..........HK_5z.
+00000350: 26ab 681f c4b4 a269 86e3 2d04 9727 27f8  &.h....i..-..''.
+00000360: 7012 026d 10fc fa9f 5131 8ebe 2215 ed7d  p..m....Q1.."..}
+00000370: 4c45 e4d0 19eb 9bd8 3741 781f c142 c29f  LE......7Ax..B..
+00000380: 4608 36c2 fb08 906a 2b94 bff5 9722 c8ec  F.6....j+...."..
+00000390: cd28 7e2a 18e1 52c1 d167 5d91 3e68 477c  .(~*..R..g].>hG|
+000003a0: 134b 33c7 d5be 288d 662a 44a9 fd5e a666  .K3...(.f*D..^.f
+000003b0: 6a46 3da6 66aa 483d a68f 2d64 ba6a 21d3  jF=.f.H=..-d.j!.
+000003c0: 750b 996e 5ac8 74db 42a6 4f2d 64ea 75db  u..nZ.t.B.O-d.u.
+000003d0: 0875 ca4a 5e39 55eb 17ef 834e d5d0 f68c  .u.J^9U....N....
+000003e0: ca36 efdf 7333 dd55 907e 1fd0 d18f b2c3  .6..s3.U.~......
+000003f0: 8028 3a74 4374 4774 f076 84f5 85ae 88ee  .(:tCtGt.v......
+00000400: 5812 0287 f2f5 1e63 9391 a46b cf19 8abb  X......c...k....
+00000410: 6206 d996 dc3c dc98 077f 0100 00ff ff03  b....<..........
+00000420: 0050 4b03 0414 0006 0008 0000 0021 0068  .PK..........!.h
+00000430: f874 a103 0100 00e2 0200 000b 0008 025f  .t............._
+00000440: 7265 6c73 2f2e 7265 6c73 20a2 0402 28a0  rels/.rels ...(.
+00000450: 0002 0000 0000 0000 0000 0000 0000 0000  ................
 00000460: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000470: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000480: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000490: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000004c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -94,2306 +94,2537 @@
 000005d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000005e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000005f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000640: 00ac 92db 4a03 3110 86ef 05df 21cc 7d37  ....J.1.....!.}7
-00000650: db2a 22d2 6c6f 44e8 9dc8 fa00 6332 bb1b  .*".loD.....c2..
-00000660: dd1c 48a6 d2be bda1 e061 612d 82bd cccc  ..H......aa-....
-00000670: 3f1f df24 596f f66e 14ef 94b2 0d5e c1b2  ?..$Yo.n.....^..
-00000680: aa41 90d7 c158 df2b 786e 1f16 b720 32a3  .A...X.+xn... 2.
-00000690: 3738 064f 0a0e 9461 d35c 5eac 9f68 442e  78.O...a.\^..hD.
-000006a0: 4379 b031 8b42 f159 c1c0 1cef a4cc 7a20  Cy.1.B.Y......z 
-000006b0: 87b9 0a91 7ce9 7421 39e4 724c bd8c a8df  ....|.t!9.rL....
-000006c0: b027 b9aa eb1b 997e 32a0 9930 c5d6 2848  .'.....~2..0..(H
-000006d0: 5b73 05a2 3d44 fa1f 5b3a 6234 c828 7548  [s..=D..[:b4.(uH
-000006e0: b488 a94c 27b6 6517 d162 ea89 1598 a01f  ...L'.e..b......
-000006f0: 4b39 1f13 5521 839c 175a 9d57 8887 9d7b  K9..U!...Z.W...{
-00000700: f168 c719 95af 5ef5 1aa9 ff4d 68f9 77a1  .h....^....Mh.w.
-00000710: d075 56d3 7dd0 3b47 9ee7 bca6 896f a718  .uV.}.;G.....o..
-00000720: 59c6 44b9 148f e953 3774 7d4e 21da 3379  Y.D....S7t}N!.3y
-00000730: 43e6 f4a3 618c 9f46 72f2 339b 0f00 0000  C...a..Fr.3.....
-00000740: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00000750: 2100 d803 826b d600 0000 ce01 0000 2000  !....k........ .
-00000760: 0000 7070 742f 736c 6964 6573 2f5f 7265  ..ppt/slides/_re
-00000770: 6c73 2f73 6c69 6465 312e 786d 6c2e 7265  ls/slide1.xml.re
-00000780: 6c73 ac91 316b c430 0c85 f742 ff83 d15e  ls..1k.0...B...^
-00000790: 3bb9 a194 72ce 2de5 e0e0 a6f6 fa03 8cad  ;...r.-.........
-000007a0: 24a6 896c 2c5d 69fe 7ddd a524 7043 878e  $..l,]i.}..$pC..
-000007b0: 7a7a fade 03ed 0f5f f3a4 3eb1 704c 64a1  zz....._..>.pLd.
-000007c0: d50d 2824 9f42 a4c1 c2fb e5f8 f004 8ac5  ..($.B..........
-000007d0: 5170 5322 b4b0 20c3 a1bb bfdb bfe2 e4a4  QpS".. .........
-000007e0: 1ef1 1833 ab4a 21b6 308a e467 63d8 8f38  ...3.J!.0..gc..8
-000007f0: 3bd6 2923 d54d 9fca eca4 8e65 30d9 f90f  ;.)#.M.....e0...
-00000800: 37a0 d935 cda3 296b 0674 1ba6 3a05 0be5  7..5..)k.t..:...
-00000810: 1476 a02e 4bc6 bfb0 53df 478f 2fc9 5f67  .v..K...S.G./._g
-00000820: 24b9 1161 2809 f2db 1403 56aa 2b03 8a05  $..a(.....V.+...
-00000830: ad57 f2da d2ea ca07 73bb 56fb 9fb5 f827  .W......s.V....'
-00000840: eeec 9674 954d af95 be31 fd36 339b 2f74  ...t.M...1.63./t
-00000850: df00 0000 ffff 0300 504b 0304 1400 0600  ........PK......
-00000860: 0800 0000 2100 a04e 0fb6 b702 0000 fc06  ....!..N........
-00000870: 0000 1500 0000 7070 742f 736c 6964 6573  ......ppt/slides
-00000880: 2f73 6c69 6465 312e 786d 6ccc 54cb 6edb  /slide1.xml.T.n.
-00000890: 3010 bc17 e83f 08ba 337a 512f 234e 60c9  0....?..3zQ/#N`.
-000008a0: 52d1 226d 8c3a f900 46a2 63a1 1249 90b4  R."m.:..F.c..I..
-000008b0: 6323 c8bf 97a4 a4a8 a993 2287 16e8 45bb  c#........"...E.
-000008c0: 5cee 90bb 3b23 9e5f 1eba d6da 632e 1a4a  \...;#._....c..J
-000008d0: e6b6 77e6 da16 2615 ad1b 723f b76f 6f4a  ..w...&...r?.ooJ
-000008e0: 90d8 9690 88d4 a8a5 04cf ed23 16f6 e5c5  ...........#....
-000008f0: c70f e76c 26da da52 6822 6668 6e6f a564  ...l&..Rh"fhno.d
-00000900: 33c7 11d5 1677 489c 5186 89da db50 de21  3....wH.Q....P.!
-00000910: a996 fcde a939 7a50 a776 ade3 bb6e e474  .....9zP.v...n.t
-00000920: a821 f680 e7ef c1d3 cda6 a9f0 9256 bb0e  .!...........V..
-00000930: 13d9 1fc2 718b a4aa 5c6c 1b26 c6d3 d87b  ....q...\l.&...{
-00000940: 4e63 1c0b 758c 41bf 28e9 4275 56ad db5a  Nc..u.A.(.BuV..Z
-00000950: 5bc1 6e38 c6da 23fb 4f9c add9 8a9b ed6f  [.n8..#.O......o
-00000960: fb15 b79a 5acd cbb6 08ea d458 6c67 d818  ....Z......Xlg..
-00000970: d2cc 92ec 8de3 fc06 bf1f 5d34 3b6c 78a7  ..........]4;lx.
-00000980: adea cd3a cc6d 35fc a3fe 3a3a 860f d2aa  ...:.m5...::....
-00000990: fa60 3545 abed f52b b9d5 b678 25db 192f  .`5E...+...x%../
-000009a0: 707e b954 77d5 1777 da8e 3fb6 73d3 c816  p~.Tw..w..?.s...
-000009b0: 5b9e 3dd4 7125 e458 d18e 3773 fbb1 2cfd  [.=.q%.X..7s..,.
-000009c0: 2c2c 4a08 4ae5 01e8 6610 6405 4c41 e907  ,,J.J...f.d.LA..
-000009d0: 49e1 c765 ee07 d193 467b d1ac e2d8 4cf9  I..e....F{....L.
-000009e0: f3b3 5abc e884 a1ae a938 1574 23cf 2ada  ..Z......8.t#.*.
-000009f0: 0d54 8f8a 51e4 7870 d08b aef2 3129 0337  .T..Q.xp....1).7
-00000a00: 0ae1 0278 690c c132 ca4b e015 cb04 8461  ...xi..2.K.....a
-00000a10: 1ae6 411a 2745 b47c 1a06 a06a 1ead e9c2  ..A.'E.|...j....
-00000a20: 19fa 1d1a 1f89 10ec 8a56 3f84 45a8 224a  .........V?.E."J
-00000a30: f3da f3f6 9cd1 93a9 2ddb 5af2 c8d4 8c2a  ........-.Z....*
-00000a40: c9cd 9886 d47e df38 d3a0 0721 c843 46eb  .....~.8...!.CF.
-00000a50: a3be e74e 5913 44b3 56c8 b53c b6d8 2c98  ...NY.D.V..<..,.
-00000a60: fe98 4ab8 e2a2 45fa efc3 04dc ae6d ab6e  ..J...E......m.n
-00000a70: b89c 9896 174c b7d3 37d5 034e 505f 56af  .....L..7..NP_V.
-00000a80: a0e4 0148 4a5b f102 ed98 9b9d a942 6794  ...HJ[.......Bg.
-00000a90: c7db 2209 4691 ac77 77d2 e8c4 ff4f 7502  ..".F..ww....Ou.
-00000aa0: 532f 4ca3 3004 791c c760 19e6 4b90 0779  S/L.0.y..`..K..y
-00000ab0: 0a16 2984 3029 9482 3cef dfeb 44ec ee7a  ..).0)..<...D..z
-00000ac0: 9da8 a20e 13e4 2fe8 0593 7a85 38fa fe27  ....../...z.8..'
-00000ad0: eedf 62d8 98f1 751b 9b36 de40 5d96 a591  ..b...u..6.@]...
-00000ae0: 9f27 19c8 3c58 02b8 4c63 b028 a310 9461  .'..<X..Lc.(...a
-00000af0: 0061 9e25 8b3c 2834 75cc 83a7 d4a9 e0fb  .a.%.<(4u.......
-00000b00: a863 f401 7346 1bf3 a07b eec0 de1e b56a  .c..sF...{.....j
-00000b10: 5049 10bb a9ef 86c1 30b1 9ea2 a95a 3df7  PI......0....Z=.
-00000b20: e1a1 ae5a fe15 b1eb bde1 485d 2631 cf4d  ...Z......H]&1.M
-00000b30: 8869 5df4 a953 8aee 5de1 7e02 0000 ffff  .i]..S..].~.....
-00000b40: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-00000b50: 3f2d 199e 1a01 0000 6704 0000 1f00 0801  ?-......g.......
-00000b60: 7070 742f 5f72 656c 732f 7072 6573 656e  ppt/_rels/presen
-00000b70: 7461 7469 6f6e 2e78 6d6c 2e72 656c 7320  tation.xml.rels 
-00000b80: a204 0128 a000 0100 0000 0000 0000 0000  ...(............
-00000b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000be0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000bf0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000c00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000c10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000c20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000c30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000c40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000c50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000c60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000c70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000c80: 0000 0000 0000 00ac 94c1 4ac4 3010 86ef  ..........J.0...
-00000c90: 82ef 10e6 6ed3 aeba 8a6c ba17 11f6 2088  ....n....l.... .
-00000ca0: ae0f 906d a76d 304d 4212 57fb f686 556b  ...m.m0MB.W...Uk
-00000cb0: ba2c c543 8ef3 67e6 cfc7 3f21 abf5 672f  .,.C..g...?!..g/
-00000cc0: c91e ad13 5a31 28b2 1c08 aa4a d742 b50c  ....Z1(....J.B..
-00000cd0: 5eb7 0f17 b740 9ce7 aae6 522b 6430 a083  ^....@....R+d0..
-00000ce0: 7579 7eb6 7a46 c97d 1872 9d30 8e04 17e5  uy~.zF.}.r.0....
-00000cf0: 1874 de9b 3b4a 5dd5 61cf 5da6 0daa 70d2  .t..;J].a.]...p.
-00000d00: 68db 731f 4adb 52c3 ab37 de22 5de4 f992  h.s.J.R..7."]...
-00000d10: dad8 03ca 8927 d9d4 0cec a6be 04b2 1d0c  .....'..........
-00000d20: fec7 5b37 8da8 f05e 57ef 3d2a 7fe2 0aaa  ..[7...^W.=*....
-00000d30: b447 f7c8 9d47 1b6c b96d d133 88c4 4947  .G...G.l.m.3..IG
-00000d40: 9105 7fa0 a7b1 6e52 6279 be93 f8e2 0719  ......nRby......
-00000d50: c21d b122 710e 6491 12c4 4951 e31f c2a1  ..."q.d...IQ....
-00000d60: fc51 67d3 2892 431c 2f29 1227 1db3 58cb  .Qg.(.C./).'..X.
-00000d70: a44b 0ab3 5136 87f2 5b9c 65b8 4ec9 b017  .K..Q6..[.e.N...
-00000d80: f8f1 64b5 899e c928 cd41 5ca5 8430 16dd  ..d....(.A\..0..
-00000d90: 11c4 28fd 42d0 c9f7 507e 0100 00ff ff03  ..(.B...P~......
-00000da0: 0050 4b03 0414 0006 0008 0000 0021 0023  .PK..........!.#
-00000db0: cdd5 4546 0200 00ec 0c00 0014 0000 0070  ..EF...........p
-00000dc0: 7074 2f70 7265 7365 6e74 6174 696f 6e2e  pt/presentation.
-00000dd0: 786d 6cec 97e1 6eda 3010 c7bf 4fda 3b58  xml...n.0...O.;X
-00000de0: fe3a d190 1092 8008 95d6 0969 1393 a2c2  .:.........i....
-00000df0: 1ec0 4d0c 4475 ecc8 7618 f4e9 7736 2609  ..M.Du..v...w6&.
-00000e00: b49a fa00 f966 fbee fe77 f7cb c584 c5e3  .....f...w......
-00000e10: a962 e848 a52a 054f b1ff 30c6 88f2 5c14  .b.H.*.O..0...\.
-00000e20: 25df a7f8 cf76 354a 3052 9af0 8230 c169  %....v5J0R...0.i
-00000e30: 8acf 54e1 c7e5 d72f 8b7a 5e4b aa28 d744  ..T..../.z^K.(.D
-00000e40: 4328 0219 aee6 24c5 07ad ebb9 e7a9 fc40  C(....$........@
-00000e50: 2ba2 1e44 4d39 d876 4256 44c3 56ee bd42  +..DM9.vBVD.V..B
-00000e60: 92bf 205f 312f 188f 23af 2225 c72e 5e7e  .. _1/..#."%..^~
-00000e70: 265e ec76 654e 7f88 bca9 20fd 4544 5266  &^.veN.... .EDRf
-00000e80: eb50 87b2 5657 b5fa 336a fd2e 6e4b 52e4  .P..VW..3j..nKR.
-00000e90: 4837 cd8b a27a 25b8 5640 0723 d268 f124  H7...z%.V@.#.h.$
-00000ea0: 2a13 a4b2 32d7 0d2c 523c c64b e0a1 58f1  *...2..,R<.K..X.
-00000eb0: 9b28 4de5 cf62 adf4 dd09 2a8b 1407 7e18  .(M..b....*...~.
-00000ec0: 87c9 240a 01aa 9c9b 13b0 f8d8 5b2e bc8f  ..$.........[...
-00000ed0: c2b9 d054 fdef ac13 9938 918f 4240 f876  ...T.....8..B@.v
-00000ee0: 7da9 651a f58a 08ba 22fa be9b 3794 9fa0  }.e....."...7...
-00000ef0: f1c0 9f01 1898 8dfc 9ce2 2899 2666 e3b5  ..........(.&f..
-00000f00: f538 b7ab c17a cdfc 306c bd0a ba23 0dd3  .8...z..0l...#..
-00000f10: 5b7a d21b 7d66 74b9 20e6 2ccb a45b 3d67  [z..}ft. .,..[=g
-00000f20: 1231 6266 8ef2 d1af cc56 d377 6147 e6d7  .1bf.....V.waG..
-00000f30: e053 11b9 36bc 1161 7b98 5786 11f8 6cc9  .S..6..a{.W...l.
-00000f40: cbe6 ed9a 119a d2cc ba50 b2e6 dfe5 ab7d  .........P.....}
-00000f50: 6e66 3ab8 db82 e900 a960 04b3 86e7 dad8  nf:......`......
-00000f60: 7b55 2850 f213 a3f3 4aa5 7925 a071 6b57  {U(P....J.y%.qkW
-00000f70: 8295 c5aa 64cc 6ecc 40d1 2726 d191 4036  ....d.n.@.'&..@6
-00000f80: 7dba 3cc5 3b2f 9b15 e973 0ded e7f0 f27c  }.<.;/...s.....|
-00000f90: abf8 8869 e349 e694 dc19 28b9 1872 7567  ...i.I....(..rug
-00000fa0: c855 87e3 d9e0 f05a 1e0e 4dd0 a109 a7b1  .U.....Z..M.....
-00000fb0: 2978 e063 a138 3e93 8ecf 15c2 c0c7 4071  )x.c.8>.......@q
-00000fc0: 7cc2 8e8f 3f89 fd68 0074 a5e2 004d 7b80  |...?..h.t...M{.
-00000fd0: 9220 b1d5 0f80 0c15 0728 ea00 0541 12d9  . .......(...A..
-00000fe0: 5f81 0190 a1e2 00c5 3d40 7138 19ee e896  _.......=@q8....
-00000ff0: 8a03 9474 800c 9de1 926e a938 40b3 1ea0  ...t.....n.8@...
-00001000: 681a 0f97 744b c57e b9be ffc4 f46e ffa2  h...tK.~.....n..
-00001010: 2cff 0100 00ff ff03 0050 4b03 0414 0006  ,........PK.....
-00001020: 0008 0000 0021 00c6 9e72 35cf 0200 00eb  .....!...r5.....
-00001030: 0600 001f 0000 0070 7074 2f6e 6f74 6573  .......ppt/notes
-00001040: 536c 6964 6573 2f6e 6f74 6573 536c 6964  Slides/notesSlid
-00001050: 6531 2e78 6d6c ac55 6d6f da30 10fe 3e69  e1.xml.Umo.0..>i
-00001060: ffc1 caf7 1002 294d 50a1 2214 b64e 1d45  ......)MP."..N.E
-00001070: a5fb 01ae 6348 34c7 f66c 4361 53ff fbce  ....cH4..lCaS...
-00001080: 4e52 684b 5f3e 548a 62fb ecbb 7b9e 7b9c  NRhK_>T.b...{.{.
-00001090: cbd9 f9b6 6468 4395 2e04 1f78 61ab ed21  ....dhC....xa..!
-000010a0: ca89 c80a be1a 78bf 6ea7 7eec 216d 30cf  ......x.n.~.!m0.
-000010b0: 3013 9c0e bc1d d5de f9f0 eb97 33d9 e7c2  0...........3...
-000010c0: 508d c09f eb3e 1e78 b931 b21f 049a e4b4  P....>.x.1......
-000010d0: c4ba 2524 e5b0 b714 aac4 0696 6a15 640a  ..%$........j.d.
-000010e0: df43 dc92 059d 76bb 1794 b8e0 5eed af3e  .C....v.....^..>
-000010f0: e22f 96cb 82d0 0b41 d625 e5a6 0aa2 28c3  ./.....A.%....(.
-00001100: 06b0 ebbc 90ba 8926 3f12 4d2a aa21 8cf3  .......&?.M*.!..
-00001110: 7e02 6908 dcc8 8265 76d4 f256 516a 677c  ~.i....ev..VQjg|
-00001120: f34d c985 9c2b b73d dbcc 152a 32a8 9887  .M...+.=...*2...
-00001130: 382e a130 5e50 6fd4 c7dc 926f dc24 78e6  8..0^Po....o.$x.
-00001140: be6a a6b8 bf5d aad2 8ec0 0d6d 071e 947f  .j...].....m....
-00001150: 67df 81b5 d1ad 41a4 3292 bd95 e4d7 47ce  g.....A.2.....G.
-00001160: 927c 72e4 74d0 2408 0e92 5a56 15b8 9774  .|r.t.$...ZV...t
-00001170: 3a0d 9d05 2b32 8a2e 4bbc a268 ce30 a1b9  :...+2..K..h.0..
-00001180: 6019 5528 7ce4 d930 d0f2 4a90 df1a 7101  `.U(|..0..J...q.
-00001190: 0cab 8288 1b61 ead9 38c7 7c45 475a 52e2  .....a..8.|EGZR.
-000011a0: 4c55 351e ddab 12d9 51e6 c8ec 2464 d62c  LU5.....Q...$d.,
-000011b0: bb2c 57f5 c16a d74d f6e0 9b9a 5634 5e27  .,W..j.M....V4^'
-000011c0: d36d c8cc dc4d 3da4 d179 9fc6 fb48 ef44  .m...M=..y...H.D
-000011d0: b6f3 20d3 767f fc75 bcb2 6fb6 2938 d85c  .. .v..u..o.)8.\
-000011e0: d6d1 1971 9f69 b330 3b46 dd42 da97 43a3  ...q.i.0;F.B..C.
-000011f0: 8002 c3f6 1ba4 dcff 31f7 5056 28b3 57db  ........1.PV(.W.
-00001200: 0cbf 53c6 440b 5985 8dd3 b972 3be6 5b7b  ..S.D.Y....r;.[{
-00001210: dce6 8546 f060 24a5 d9fa 4608 a611 2bee  ...F.`$...F...+.
-00001220: 1456 bbd6 b338 9467 73ac f0cd 5b28 0287  .V...8.gs...[(..
-00001230: 37d8 f3fa 8022 d1d3 eb35 5b97 7720 c6a1  7...."...5[.w ..
-00001240: 30dd cf10 06ae 1084 86c6 f577 e0fd 5963  0..........w..Yc
-00001250: 65a8 aa75 3af9 3c9d 962c 739c fec5 c934  e..u:.<..,s....4
-00001260: 1975 db89 9f4c 7a27 7eda 8b26 7e7a 1a87  .u...Lz'~..&~z..
-00001270: 7e3b 09bb f145 1276 c2b8 f7e0 3d42 03e2  ~;...E.v....=B..
-00001280: 1cc0 1d55 5997 66cc 28e6 0742 877b 6996  ...UY.f.(..B.{i.
-00001290: b627 bd2a ce1b 92b8 a169 64d0 55ae b4a9  .'.*.....id.U...
-000012a0: 6768 ad0a a090 a649 af33 8e53 3f0d a3a9  gh.....I.3.S?...
-000012b0: 1f5d 24a7 fe68 0a64 a627 dd28 1aa7 f168  .]$..h.d.'.(...h
-000012c0: dc9d 3cd8 c618 467d a2a8 eb99 9759 d36d  ..<...F}.....Y.m
-000012d0: c3e8 45bf 2d0b a284 164b d322 a2ac 1b77  ..E.-....K."...w
-000012e0: 20c5 3d55 5214 ae77 87ed fa07 b0c1 0cfa   .=UR..w........
-000012f0: 4ed2 6d87 4912 c671 2d10 606b 4687 d62a  N.m.I..q-.`kF..*
-00001300: 5ef7 64c2 d44f 2caf 37ee 7640 3250 77ec  ^.d..O,.7.v@2Pw.
-00001310: 4c12 7e2e f5e5 d81f b11a dbcf 7ff8 1f00  L.~.............
-00001320: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00001330: 0021 004a af75 39d2 0000 00bf 0100 002a  .!.J.u9........*
-00001340: 0000 0070 7074 2f6e 6f74 6573 536c 6964  ...ppt/notesSlid
-00001350: 6573 2f5f 7265 6c73 2f6e 6f74 6573 536c  es/_rels/notesSl
-00001360: 6964 6531 2e78 6d6c 2e72 656c 73ac 90b1  ide1.xml.rels...
-00001370: 6a03 310c 86f7 42df c168 8f7d 9721 9412  j.1...B..h.}.!..
-00001380: 5f96 52c8 90a5 a40f 606c dd9d c99d 6c2c  _.R.....`l....l,
-00001390: 2524 6f5f 434b c941 860e 1df5 4bfa f4a1  %$o_CK.A....K...
-000013a0: edee 3a4f ea82 8563 220b ad6e 4021 f914  ..:O...c"..n@!..
-000013b0: 220d 163e 8fef ab17 502c 8e82 9b12 a185  "..>....P,......
-000013c0: 1b32 ecba e7a7 ed07 4e4e ea12 8f31 b3aa  .2......NN...1..
-000013d0: 1462 0ba3 487e 3586 fd88 b363 9d32 52ed  .b..H~5....c.2R.
-000013e0: f4a9 cc4e 6a59 0693 9d3f b901 cdba 6936  ...NjY...?....i6
-000013f0: a6dc 33a0 5b30 d53e 5828 fbb0 0675 bc65  ..3.[0.>X(...u.e
-00001400: fc0b 3bf5 7df4 f896 fc79 4692 0727 0c4f  ..;.}....yF..'.O
-00001410: 3160 05ba 32a0 58d0 fa3b f969 b4ba 02c1  1`..2.X..;.i....
-00001420: 3cf6 68ff d383 9220 1f1c 0b96 85cd 5dbe  <.h.... ......].
-00001430: 18fa 3533 8bb7 775f 0000 00ff ff03 0050  ..53..w_.......P
-00001440: 4b03 0414 0006 0008 0000 0021 00e5 a661  K..........!...a
-00001450: cc05 0500 007e 1200 0021 0000 0070 7074  .....~...!...ppt
-00001460: 2f73 6c69 6465 4c61 796f 7574 732f 736c  /slideLayouts/sl
-00001470: 6964 654c 6179 6f75 7431 2e78 6d6c cc58  ideLayout1.xml.X
-00001480: dd72 9b46 14be ef4c df81 a1d7 1bb1 bf80  .r.F...L........
-00001490: 2772 0610 74da 7112 4f95 3c00 8695 c584  'r..t.q.O.<.....
-000014a0: bfc2 4ab1 9bf1 4c5e ab7d 9c3c 49cf 2e60  ..J...L^.}.<I..`
-000014b0: 49b1 93da b1dd f18d f6b0 9cfd f69c f37d  I..............}
-000014c0: 1c56 bc7c 7551 95d6 5676 7dd1 d473 1bbf  .V.|uQ..Vv}..s..
-000014d0: 706c 4bd6 5993 17f5 f9dc 7eff 2e41 9e6d  plK.Y.....~..A.m
-000014e0: f52a adf3 b46c 6a39 b72f 656f bf3a fef9  .*...lj9./eo.:..
-000014f0: a797 ed51 5fe6 27e9 65b3 5116 60d4 fd51  ...Q_.'.e.Q.`..Q
-00001500: 3ab7 d74a b547 b359 9fad 6595 f62f 9a56  :..J.G.Y..e../.V
-00001510: d670 6fd5 7455 aae0 b23b 9fe5 5dfa 11b0  .po.tU...;..]...
-00001520: ab72 461c 47cc aab4 a8ed 717d 7797 f5cd  .rF.G.....q}w...
-00001530: 6a55 6472 d164 9b4a d66a 00e9 6499 2a88  jUdr.d.J.j..d.*.
-00001540: bf5f 176d 3fa1 b577 416b 3bd9 038c 597d  ._.m?..wAk;...Y}
-00001550: 1892 ba6c 215b 55a8 52da 9671 ebb6 3081  ...l![U.R..q..0.
-00001560: ed63 c83c 5b96 b955 a715 4cbc d31e d6b2  .c.<[..U..L.....
-00001570: 2c72 696e f5ed bb4e 4a6d d5db 5fbb 76d9  ,rin...NJm.._.v.
-00001580: 9e76 66c5 9bed 6967 15b9 4618 57da b3f1  .vf...ig..F.W...
-00001590: c6e8 662e ebad 3166 5f2d 3f9f ccf4 e862  ..f...1f_-?....b
-000015a0: d555 7a84 4258 1773 1bf8 bad4 bf33 3d27  .Uz.BX.s.....3='
-000015b0: 2f94 950d 93d9 6e36 5bbf bdc5 375b c7b7  /.....n6[...7[..
-000015c0: 78cf a60d 667b 9bea ac86 e06e a643 a674  x...f{.....n.C.t
-000015d0: 8642 e8fa 9838 4e7a 3545 b4e9 8ab9 fd29  .B...8Nz5E.....)
-000015e0: 4948 c8e3 84a1 042c c49c 90a1 3066 3e4a  IH.....,....0f>J
-000015f0: 08f5 62e2 2611 a1e2 4aaf c6e2 28eb a4a1  ..b.&...J...(...
-00001600: e4b7 7c92 1616 37e8 ac8a ac6b fa66 a55e  ..|...7....k.f.^
-00001610: 644d 35ea 6292 1730 89d9 c8a4 8ef2 5318  dM5.b..0......S.
-00001620: b989 cf03 0ff1 10c7 c88b 7c8c 5810 2d10  ..........|.X.-.
-00001630: c1c4 c5d8 0f03 8293 abb1 0010 f334 9a2c  .............4.,
-00001640: 6663 be63 e213 117d 7bd2 641f 7aab 6e80  fc.c...}{.d.z.n.
-00001650: 28cd ebc0 dbb5 c740 a61e dbf5 28a7 4c75  (......@....(.Lu
-00001660: a64c a3eb 70df 18bb 42df ca32 e684 39ce  .L..p...B..2..9.
-00001670: c01f c604 4a45 0f19 f731 1b1c 3493 5051  ....JE...1..4.PQ
-00001680: 5738 37f8 1cb0 db23 7511 36f9 a55e 7d06  W87....#u.6..^}.
-00001690: 23f0 98d6 d9ba 81a7 ef6c c02c 7bb5 5497  #........l.,{.T.
-000016a0: a534 f6b6 c4ad 7629 cf6b 13bf e137 97ab  .4....v).k...7..
-000016b0: 3f60 b2ff 6b6e 0bbd ebb0 d1e8 3bd8 7b18  ?`..kn......;.{.
-000016c0: adfe 3159 75b0 a84c 7567 9135 7abf 1cb6  ..1Yu..Lug.5z...
-000016d0: 53c7 5159 641f 2cd5 5832 2f94 f53a ed95  S.QYd.,.X2/..:..
-000016e0: ec2c f3e8 41eb 0110 0d38 5062 5064 9d9f  .,..A....8PbPd..
-000016f0: a65d aa23 b806 fbfd 740c a235 a94e 299a  .].#....t..5.N).
-00001700: acbf 2f60 3a09 78b9 391b f624 cf54 c3dc  ../`:.x.9..$.T..
-00001710: 2594 7187 211a 7b89 0e41 20e2 7282 7cee  %.q.!.{..A .r.|.
-00001720: 078e a06e b870 dda7 d770 bf39 1b34 0c41  ...n.p...p.9.4.A
-00001730: 6965 3e48 cb54 38c4 a1de 77b4 8c05 e7ae  ie>H.T8...w.....
-00001740: 2077 d5f2 3705 5ca5 dd89 6975 459d 43c7   w..7.\...iuE.C.
-00001750: 37e6 a1a8 cf36 6fe0 0d67 00f6 f4ad 63fd  7....6o..g....c.
-00001760: 5adf c624 3b54 06cc e878 ef0b 7df0 e868  Z..$;T...x..}..h
-00001770: bc11 9aee a087 5adc 1b1a 7bfb d01a 6f84  ......Z...{...o.
-00001780: 663b 684c 5dac bbc4 bdb1 77ad 6504 1cb1  f;hL].....w.e...
-00001790: f91e b647 3c1d c2c3 b035 e088 2d76 d884  ...G<....5..-v..
-000017a0: 78a6 e93c 0c5b 038e d8ee 1eb6 cbe8 8f50  x..<.[.........P
-000017b0: 7988 ad01 476c 6f87 ad81 7f88 cb03 6c0d  y...Glo.......l.
-000017c0: 3862 fb7b d882 9b8e ff30 6c0d f848 ddbb  8b.{.....0l..H..
-000017d0: 9f9a e9d3 3770 3635 f045 aaa4 755a a699  ....7p65.E..uZ..
-000017e0: 5c37 650e 41d0 67da c863 47c4 9c13 8e7c  \7e.A.g..cG....|
-000017f0: 217c b4f0 b88b 02e2 0788 b024 0e92 30a4  !|.........$..0.
-00001800: 3ca0 4fdf c873 651b 0dac d372 3535 f341  <.O..se....r55.A
-00001810: 0cdf ece6 e688 fadd 966b 2e8c 6456 7044  .........k..dVpD
-00001820: 1e5e 5b1e 4d44 18c5 8851 c836 a1cc 85bc  .^[.MD...Q.6....
-00001830: a987 8288 9305 7363 dfc3 d1d5 74e0 ce81  ......sc....t...
-00001840: 4355 5432 29ce 379d 7cbb 5186 c203 e581  CUT2).7.|.Q.....
-00001850: 52ac be52 5129 d3fa fa34 ab8e 8943 c8cc  R..RQ)...4...C..
-00001860: e133 ecec d406 313c bede f8a4 b7a4 69b4  .3....1<......i.
-00001870: d4f7 15c7 9ea9 e230 e8ca 6301 459c c604  .......0..c.E...
-00001880: 2dc4 2240 220c 8088 248a 4440 b808 a2f0  -."@"...$.D@....
-00001890: e915 b782 5e64 24f7 e726 eda0 7493 eafe  ....^d$..&..t...
-000018a0: e30c 711f d53d 2ed5 e2fa 6ca8 ffdf 596f  ..q..=....l...Yo
-000018b0: 36d5 d957 84f3 674a 78c4 23c7 7508 4391  6..W..gJx.#.u.C.
-000018c0: eb46 28f2 160c 0561 1001 ff4c f0d8 09c0  .F(....a...L....
-000018d0: 9ffc 0f67 c532 879a ddca f970 a27b dc4e  ...g.2.....p.{.N
-000018e0: 2358 48fd 8543 e1ff 1dfc 2c22 0625 a771  #XH..C....,".%.q
-000018f0: 8030 f7c2 d00f 221f ce92 d79d a6d7 94d6  .0....".........
-00001900: 10dd 5d1b cc97 cf7f fff2 e5f3 3f8f d05d  ..].........?..]
-00001910: cc30 7d26 98aa 6eac 513b 10ad 2091 17a2  .0}&..n.Q;.. ...
-00001920: 10b3 04b1 850f 2f88 4470 9400 7d2c 0abd  ....../.Dp..},..
-00001930: 20a2 b1d6 4e8b d94d edc0 e4dd b4d3 361f   ...N..M......6.
-00001940: 65d7 3685 f98c 829d 513e dbb4 84f3 844b  e.6.....Q>.....K
-00001950: b9c7 84cb f848 d3a0 915d b49a f8a5 ce1f  .....H...]......
-00001960: c6b2 7b9d b66f b746 2495 79fd 4766 aad5  ..{..o.F$.y.Gf..
-00001970: c21c 5c77 2e3a f7e9 bbd1 f1bf 0000 00ff  ..\w.:..........
-00001980: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-00001990: 000d c673 aa54 0400 0089 0f00 0021 0000  ...s.T.......!..
-000019a0: 0070 7074 2f73 6c69 6465 4c61 796f 7574  .ppt/slideLayout
-000019b0: 732f 736c 6964 654c 6179 6f75 7432 2e78  s/slideLayout2.x
-000019c0: 6d6c cc57 db6e dc36 107d 2fd0 7f10 d467  ml.W.n.6.}/....g
-000019d0: 4637 8a92 16b1 035d 8b16 4e6c 749d 0fa0  F7.....]..Nlt...
-000019e0: 25ae 578d 24aa 1477 b3db c040 7eab fd9c  %.W.$..w...@~...
-000019f0: 7c49 8794 e47b 9b2d b006 fc22 52d4 f070  |I...{.-..."R..p
-00001a00: 66ce 1992 7afb 6ed7 36c6 9689 a1e6 dd89  f...z.n.6.......
-00001a10: e9bc b14d 8375 25af eaee fac4 fc78 59a0  ...M.u%......xY.
-00001a20: d034 0649 bb8a 36bc 6327 e69e 0de6 bbd3  .4.I..6.c'......
-00001a30: 1f7f 78db 2f86 a63a a37b be91 0660 74c3  ..x./..:.{...`t.
-00001a40: 829e 986b 29fb 8565 0de5 9ab5 7478 c37b  ...k)..e....tx.{
-00001a50: d6c1 b715 172d 95f0 2aae ad4a d0cf 80dd  .....-..*..J....
-00001a60: 3696 6bdb c46a 69dd 99d3 7c71 c87c be5a  6.k..ji...|q.|.Z
-00001a70: d525 cb78 b969 5927 4710 c11a 2ac1 ff61  .%.x.iY'G...*..a
-00001a80: 5df7 c38c d61f 82d6 0b36 008c 9efd d025  ]........6.....%
-00001a90: b9ef 215a 7ef5 bb69 6823 b185 57c7 3c85  ..!Z~..ih#..W.<.
-00001aa0: b8cb 6553 191d 6d61 e0b2 960d 3320 3b46  ..eS..ma....3 ;F
-00001ab0: ca3b 0948 da60 e82f 0563 aad7 6d7f 16fd  .;.H.`./.c..m...
-00001ac0: b2bf 107a de87 ed85 30ea 4ae1 4cf3 4d6b  ...z....0.J.L.Mk
-00001ad0: fa30 99e9 d76e ab3b d6a3 e9d7 7397 2e76  .0...n.;....s..v
-00001ae0: 2bd1 aa16 9261 ec4e 4ce0 6caf 9e96 1a63  +....a.NL.l....c
-00001af0: 3b69 94e3 6079 375a aecf 9fb1 2dd7 f933  ;i..`y7Z....-..3
-00001b00: d6d6 bc80 756f 5115 d5e8 dcd3 70dc 399c  ....uoQ.....p.9.
-00001b10: 311d 2a4b da8f b341 ce1e 6d44 7d62 7e29  1.*K...A..mD}b~)
-00001b20: 0a37 f1f3 02a3 027a 08db 0946 498e 2354  .7.....z...FI.#T
-00001b30: b85e 98bb 4191 ba1e b951 b31d b228 05d3  .^..A....Q...(..
-00001b40: b4fc 52cd f272 c813 4adb ba14 7ce0 2bf9  ..R..r..J...|.+.
-00001b50: a6e4 eda4 8d59 62c0 a683 2736 9597 5f62  .....Yb...'6.._b
-00001b60: 2ff4 7044 2244 ecd4 4771 1aa4 c84e 6270  /.pD"D..Gq...Nbp
-00001b70: 2172 a214 1307 1392 dd4c 0900 9fe7 5647  !r.......L....VG
-00001b80: 614d f14e 81cf 440c fd19 2f3f 0d46 c781  aM.N..D.../?.F..
-00001b90: 28c5 ebc8 dbad c548 a66a fbf5 2429 a972  (......H.j..$).r
-00001ba0: 34d9 8d1f 75e7 2ecb 930a e42e e1d5 5e2d  4...u.........^-
-00001bb0: 7205 ad1e a48b 6690 4bb9 6f98 7ee9 d543  r.....f.K.o.~..C
-00001bc0: bb21 8088 86aa 8a65 1dfa b81c c995 a769  .!.....e.......i
-00001bd0: 5397 9f0c c90d 56d5 d278 4f07 c984 a1d7  S.....V..xO.....
-00001be0: 8792 0614 15e0 18a6 4661 5d75 4105 fded  ........Fa]uA...
-00001bf0: 3ed8 af17 5342 7aed e7ec 9435 cbe1 df45  >...SBz....5...E
-00001c00: e1cd a298 2ac3 b868 68c9 d6bc a9c0 09f7  ....*..hh.......
-00001c10: 954a c4c1 b6eb 1499 8762 823d 9410 62a3  .J.......b.=..b.
-00001c20: 248c 3022 b9e3 0659 14bb 5194 bfa4 44ea  $.0"...Y..Q...D.
-00001c30: 6a77 6772 0475 f48a cb6d 735b f0ff 5f2d  jwgr.u...ms[.._-
-00001c40: 8a19 2d96 e181 5a46 453c 5e45 7bfe dfab  ..-...ZFE<^E{...
-00001c50: 2c59 c961 bb6c d896 3507 20ba df47 bc5c  ,Y.a.l..5. ..G.\
-00001c60: d7e2 7040 effb 8005 df08 b93e 1811 1f80  ..p@.......>....
-00001c70: 58af 9e05 3c76 cde1 b9e6 322a d983 82f3  X...<v....2*....
-00001c80: 5e69 c191 2473 0237 0c51 1166 364a b19f  ^i..$s.7.Q.f6J..
-00001c90: a32c b06d 841d 2fc5 5e41 323b 212f bf27  .,.m../.^A2;!/.'
-00001ca0: 5712 2e39 7f42 24b4 5929 c754 118e 47e1  W..9.B$.Y).T..G.
-00001cb0: 51aa 7005 f705 1dad 1f42 4849 9a23 ecc1  Q.p......BHI.#..
-00001cc0: 3154 7838 4011 f142 388b 7c37 c341 1e85  1Tx8@..B8.|7.A..
-00001cd0: 4e7a 33df 3d2a e050 d62d 2bea eb8d 60e7  Nz3.=*.P.-+...`.
-00001ce0: 1b75 b778 a430 508a 31b4 326d 18ed 6e6b  .u.x.0P.1.2m..nk
-00001cf0: 5c9e bab6 eb5a b66f 39f6 9dda c087 e3eb  \....Z.o9.......
-00001d00: cd9f f556 70ae 768b fb8a c3af 758b 2738  ...Vp.v.....u.'8
-00001d10: 0e43 3b47 4118 4608 960b 91ed 1017 c589  .C;GA.F.........
-00001d20: 1d15 4962 0779 12bd bce2 5652 8c92 fb63  ..Ib.y....VR...c
-00001d30: 4305 a46e 56dd 11f7 fee3 524d 66aa 974d  C..nV.....RMf..M
-00001d40: 5d31 e3c3 a6bd 7a44 b8ff 6acf f438 4d03  ]1....zD..j..8M.
-00001d50: 0c45 e7bb 298a 6337 4699 e760 1404 7112  .E..).c7F..`..q.
-00001d60: 470e f66d 2f78 79c2 e167 0972 f62c e7fa  G..m/xy..g.r.,..
-00001d70: 8c3b f24e 4370 e245 99ed a130 8547 9662  .;.NCp.E...0.G.b
-00001d80: 48b9 97c7 c8f1 c324 89e2 3422 be7f bbd3  H......$..4"....
-00001d90: 0c8a d20e bc3b 7483 f9f6 f5af 9fbe 7dfd  .....;t.......}.
-00001da0: fb08 bb8b 6ee6 bfa5 39eb ba37 6907 bc25  ....n...9..7i..%
-00001db0: 6e1a 2628 7170 8170 1605 282e 888f 0adf  n.&(qp.p..(.....
-00001dc0: c338 4dc2 38f5 72a5 9dde c14f b503 8387  .8M.8.r....O....
-00001dd0: 69a7 e79f 99e8 79ad ff28 1d7b 92cf 96aa  i.....y..(.{....
-00001de0: 3b4d e044 7e10 f891 be39 58da b7b9 bdd5  ;M.D~....9X.....
-00001df0: c852 c50f 6d23 ded3 fe7c ab45 d2ea 1b54  .R..m#...|.E...T
-00001e00: aa87 7a25 ccd1 f4ce 44c5 3eff 429f fe03  ..z%....D.>.B...
-00001e10: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
-00001e20: 0000 2100 8408 ff76 3e05 0000 5e15 0000  ..!....v>...^...
-00001e30: 2100 0000 7070 742f 736c 6964 654c 6179  !...ppt/slideLay
-00001e40: 6f75 7473 2f73 6c69 6465 4c61 796f 7574  outs/slideLayout
-00001e50: 332e 786d 6ccc 58db 929c 3610 7d4f 55fe  3.xml.X...6.}OU.
-00001e60: 8122 cf32 e886 60cb b32e aeb9 d4da deca  .".2..`.........
-00001e70: d81f 8041 b343 995b 8466 bc1b d756 f9b7  ...A.C.[.f...V..
-00001e80: 92cf f197 4412 3033 6baf 9d71 e2dd 9a17  ....D.03k..q....
-00001e90: 10a2 bb39 dde7 4834 3c7d 76dd d4d6 968b  ...9..H4<}v.....
-00001ea0: a1ea da85 0d9f b8b6 c5db a22b abf6 6a61  ...........+..ja
-00001eb0: bf7e 9501 dfb6 0699 b765 5e77 2d5f d837  .~.......e^w-_.7
-00001ec0: 7cb0 9f9d fff8 c3d3 fe6c a8cb 8bfc a6db  |........l......
-00001ed0: 484b c568 87b3 7c61 afa5 eccf 1c67 28d6  HK.h..|a.....g(.
-00001ee0: bcc9 8727 5dcf 5b75 6fd5 8926 97ea 525c  ...'].[uo..&..R\
-00001ef0: 39a5 c8df a9d8 4ded 20d7 f59c 26af 5a7b  9.....M. ...&.Z{
-00001f00: f217 c7f8 77ab 5555 f0a4 2b36 0d6f e518  ....w.UU..+6.o..
-00001f10: 44f0 3a97 0aff b0ae fa61 8ed6 1f13 ad17  D.:......a......
-00001f20: 7c50 618c f75d 48f2 a657 d90e bcf8 85e7  |Pa..]H..W......
-00001f30: a56d 1943 b155 53d0 3e57 b917 cbba b4da  .m.C.US.>W......
-00001f40: bc51 134b 5e68 774b 1b72 61ee 0efd 2bc1  .Q.K^hwK.ra...+.
-00001f50: b91e b5db 9f45 bfec 2f85 717a b1bd 1456  .....E../.qz...V
-00001f60: 55ea 2093 b3ed 4c37 2633 73d9 6ecd c0f9  U. ...L7&3s.n...
-00001f70: c4fd 6a1e e667 d72b d1e8 b3aa 8675 bdb0  ..j..g.+.....u..
-00001f80: 1569 37fa e8e8 397e 2dad 629c 2cf6 b3c5  .i7...9~-.b.,...
-00001f90: fae5 3db6 c53a bdc7 da99 1fe0 1c3c 5467  ..=..:.......<Tg
-00001fa0: 3582 fb3c 1d34 a7f3 aa92 35b7 7489 0c8e  5..<.4....5.t...
-00001fb0: 8b41 ce88 36a2 5ad8 efb3 0c45 34cd 08c8  .A..6.Z....E4...
-00001fc0: d408 1037 2220 4a49 0032 84fd 14b1 2c46  ...7" JI.2....,F
-00001fd0: d8bb d5de d03b 2b04 37bc fc5a cefa 82de  .....;+.7..Z....
-00001fe0: 679c 3655 21ba a15b c927 45d7 4ce2 9835  g.6U!..[.'E.L..5
-00001ff0: a6e8 8464 a253 a37c cf18 2534 8421 802e  ...d.S.|..%4.!..
-00002000: 7641 cc32 0f44 348e 00c5 01f5 bc30 f2b3  vA.2.D4......0..
-00002010: 84dc 4e05 5098 e7b3 c9c2 99f2 9d12 9f89  ..N.P...........
-00002020: 18fa 8bae 783b 586d a788 d2bc 8ebc ed2c  ....x;Xm.......,
-00002030: 4632 f5b9 5f4f 9a92 ba46 93dd 78d3 0cf6  F2.._O...F..x...
-00002040: 55be 9762 1f43 9f8e dc41 e606 0cfb 77d9  U..b.C...A....w.
-00002050: 862e 85d4 7327 1a91 4f11 c3ec 5332 c7d8  ....s'..O...S2..
-00002060: fd99 bc8e baf2 46bb bf51 6745 62de 16eb  ......F..QgEb...
-00002070: 4ead bf37 63d0 7a90 4b79 5373 33de d670  N..7c.z.KySs3..p
-00002080: 8254 f2d5 efca 78f8 7361 ab27 cd52 d919  .T....x.sa.'.R..
-00002090: e8f1 8163 af0f c64f 28a7 3ad7 1b0a 6fc1  ...c...O(.:...o.
-000020a0: ebe5 f80c 791e d755 f1d6 929d c5cb 4a5a  ....y..U......JZ
-000020b0: cff3 4172 6199 eaa8 1d47 05d1 0147 124c  ..Ara....G...G.L
-000020c0: 14de 9697 b9c8 3582 5db0 df2e 2710 bdc9  ......5.]...'...
-000020d0: 6fce cba4 fa75 c9e2 9d64 7505 2feb bce0  o....u...du./...
-000020e0: ebae 560b d842 27aa de24 8963 8249 0292  ..V..B'..$.c.I..
-000020f0: 8052 8048 1483 8805 1484 994f 2396 429a  .R.H.......O#.B.
-00002100: 79d1 c3ab 570b 4603 d292 fb3f 2226 d40f  y...W.F....?"&..
-00002110: 8887 bf26 6248 5d17 fa47 8bf8 4bca b59a  ...&bH]..G..K...
-00002120: 5c5c 980d ae6a 4bb5 d9eb a1f1 dabc 506f  \\...jK.......Po
-00002130: 34e3 7520 6c44 dcf1 f6d0 d555 9955 756d  4.u lD.....U.Uum
-00002140: 2e34 613c ae85 b5cd 6bb5 84af c72d 4e56  .4a<....k....-NV
-00002150: ad1c 6718 dd2f 889d f178 b58f e3cc 4fba  ..g../...x....O.
-00002160: bb6e cc10 ed91 12ca 90ae c151 70f5 631f  .n.........Qp.c.
-00002170: 0bae c638 c1c5 7bb8 0124 ba66 47c1 85fe  ...8..{..$.fG...
-00002180: 23c2 d518 27b8 640f 1762 068d c48e c2ab  #...'.d..b......
-00002190: 2d1f 0baf 0639 e1a5 0778 7de4 ebaa 9d1e  -....9...x}.....
-000021a0: 5e0d 72c2 ebed f122 e49b 97c3 e9e1 d520  ^.r...."....... 
-000021b0: 27bc ec00 2f23 f8e8 e5f6 a878 35c8 09af  '.../#.....x5...
-000021c0: bfc7 abc1 1ebf de1e 13af 0639 e10d 0ef0  ...........9....
-000021d0: 7a94 9de6 7ad3 20ef ef5a 347a 65b0 6b93  z...z. ..Z4ze.k.
-000021e0: bfbd 8bd1 6f34 d3c4 0c77 ba98 ffd2 a990  ....o4...w......
-000021f0: b953 4972 c9ef 742a f844 3b95 d00d c3c0  .SIr..t*.D;.....
-00002200: a729 4813 8601 f362 35f2 7000 529c c0d8  .)H....b5.p.R...
-00002210: 8d42 3ff4 d287 ef54 4a69 1b4d adf3 7a35  .B?....TJi.M..z5
-00002220: 772c a348 bed8 b298 afaf aff6 15e6 c268  w,.H...........h
-00002230: 64a5 3e00 4db6 d4c7 aaf3 5239 12ec a90a  d.>.M.....R9....
-00002240: 63c2 40e0 611f 8431 4509 6169 e0c3 f876  c.@.a..1E.ai...v
-00002250: fea0 2c15 87b2 6a78 565d 6d04 7fb9 9186  ..,...jxV]m.....
-00002260: c23b d252 3dad 3534 32ae 79de ee14 28cf  .;.R=.542.y...(.
-00002270: 918b 90e3 5207 ba7b 4529 0cdf bf33 a6b3  ....R..{E)...3..
-00002280: deb2 aed3 5a3e 541c 3951 c591 2022 1479  ....Z>T.9Q.. ".y
-00002290: 1170 0314 033f c419 c858 1600 3507 699c  .p...?...X..5.i.
-000022a0: aa2e 3280 0faf b895 14a3 e4fe d8e4 4295  ..2...........B.
-000022b0: 6e56 ddbf 34ca dfa2 baef 4bb5 3753 bd54  nV..4.....K.7S.T
-000022c0: bb24 b75e 6c9a 379f 104e 4f94 70e4 a66e  .$.^l.7..NO.p..n
-000022d0: e6c5 0cb8 1eca d421 8420 f251 0452 0669  .......!. .Q.R.i
-000022e0: 9a60 8461 841e 9ef0 a12e 55cd eee5 1c3d  .`.a......U....=
-000022f0: c04e e391 0807 898b 811f ab43 1213 5572  .N.........C..Ur
-00002300: 9c86 0052 3f8a 8230 0e3c 4a77 3bcd a029  ...R?..0.<Jw;..)
-00002310: 6d15 ba63 3798 8f1f fefa e9e3 87bf bfc3  m..c7...........
-00002320: ee62 4ef3 1fb0 b9ea 6634 6947 a1f5 50ec  .bN.....f4iG..P.
-00002330: 4720 8224 0324 0998 fa8a f528 c828 2624  G .$.$.....(.(&$
-00002340: 8efc 30c6 a9d6 4e0f c9e7 da51 93c7 69a7  ..0...N....Q..i.
-00002350: efde 71d1 7795 f94d 08dd 493e a661 c018  ..q.w..M..I>.a..
-00002360: 056a 4b60 8c4c 348d 1ad9 a3d5 c42f 75fe  .jK`.L4....../u.
-00002370: ea5c 8be7 79ff 726b 44d2 98f7 7b6c a67a  .\..y.rkD...{l.z
-00002380: 2dcc d174 6fa2 739f ff8b 9eff 0300 00ff  -..to.s.........
-00002390: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-000023a0: 00ec 3204 97b5 0400 00c3 1300 0021 0000  ..2..........!..
-000023b0: 0070 7074 2f73 6c69 6465 4c61 796f 7574  .ppt/slideLayout
-000023c0: 732f 736c 6964 654c 6179 6f75 7434 2e78  s/slideLayout4.x
-000023d0: 6d6c ec58 5b6e dc36 14fd 2fd0 3d08 ea37  ml.X[n.6../.=..7
-000023e0: 2df1 29c9 881d e859 b470 62a3 e32c 4096  -.)....Y.pb..,@.
-000023f0: 381e 357a 95e2 8ced 0606 b2ad 7639 5949  8.5z........v9YI
-00002400: 494a f23b f1b8 b003 7f64 3e86 1445 5ede  IJ.;.....d>..E^.
-00002410: 7bcf 3957 94de bc3d 6f6a 6bc3 c550 75ed  {.9W...=ojk..Pu.
-00002420: 9e0d 775c dbe2 6dd1 9555 7bba 677f 38ce  ..w\..m..U{.g.8.
-00002430: 806f 5b83 ccdb 32af bb96 efd9 177c b0df  .o[...2......|..
-00002440: eeff fcd3 9b7e 77a8 cb83 fca2 5b4b 4bd9  .....~w.....[KK.
-00002450: 6887 dd7c cf5e 49d9 ef3a ce50 ac78 930f  h..|.^I..:.P.x..
-00002460: 3b5d cf5b 756f d989 2697 ea52 9c3a a5c8  ;].[uo..&..R.:..
-00002470: cf94 eda6 7690 eb32 a7c9 abd6 9ed6 8b6d  ....v..2.......m
-00002480: d677 cb65 55f0 a42b d60d 6fe5 6844 f03a  .w.eU..+..o.hD.:
-00002490: 97ca ff61 55f5 c36c addf c65a 2ff8 a0cc  ...aU..l...Z/...
-000024a0: 98d5 b75d 9217 bd8a 569e 7587 277f da96  ...]....V.u.'...
-000024b0: 9927 366a 04da fb2a f462 5197 569b 376a  .'6j...*.bQ.V.7j
-000024c0: e0f8 acb3 e2ae 95ca 8cb9 35f4 c782 73dd  ..........5...s.
-000024d0: 6b37 bf8a 7ed1 1f09 b3e2 fde6 4858 55a9  k7..~.......HXU.
-000024e0: 2d4c 2b6d 67ba 314d 3397 edc6 749c 3bcb  -L+mg.1M3...t.;.
-000024f0: 4fe7 6ebe 7bbe 148d 6e55 26ac f33d 5b01  O.n.{...nU&..=[.
-00002500: 76a1 ff1d 3dc6 cfa5 558c 83c5 f568 b13a  v...=...U....h.:
-00002510: 7c60 6eb1 4a1f 98ed cc1b 3837 36d5 518d  |`n.J.....876.Q.
-00002520: cedd 0f07 cde1 1c57 b2e6 96ce 8ff1 e360  .......W.......`
-00002530: 90b3 476b 51ed d99f b20c 4534 cd08 c854  ..GkQ.....E4...T
-00002540: 0f10 3722 204a 4900 3284 fd14 7959 8c30  ..7" JI.2...yY.0
-00002550: bbd4 ab21 db2d 0437 98fc 56ce dc82 ec1e  ...!.-.7..V.....
-00002560: 9e4d 5588 6ee8 9672 a7e8 9a89 1833 bf14  .MU.n..r.....3..
-00002570: 9490 4c50 6a2f 3fa1 3860 ea97 8090 2102  ..LPj/?.8`....!.
-00002580: 7c8c 2280 fdc4 0728 2481 9750 98e1 24b9  |."....($..P..$.
-00002590: 9c12 a07c 9e5b 1385 33c5 3b05 3e03 31f4  ...|.[..3.;.>.1.
-000025a0: 075d f171 b0da 4e01 a571 1d71 bb9a 3182  .].q..N..q.q..1.
-000025b0: a9db 7e35 f349 e768 9a37 de34 9deb 2c4f  ..~5.I.h.7.4..,O
-000025c0: 2c90 e751 575e e84d 4e54 6b06 f3dd 7a90  ,..QW^.MNTk...z.
-000025d0: 0b79 5173 73d1 eb3f e386 5040 d4b9 962b  .yQss..?..P@...+
-000025e0: 6fc1 87c5 08ae dc8f ebaa f868 c9ce e265  o..........h...e
-000025f0: 25ad 77f9 20b9 b0cc fe4a cfca 8a0e 700c  %.w. ....J....p.
-00002600: d358 e16d 7994 8bfc 8f9b c67e 3f9a 12d2  .X.my......~?...
-00002610: 1b3f 67a7 9c99 0e5f 2705 9e49 3129 c33a  .?g...._'..I1).:
-00002620: aaf3 82af baba 544e a057 4a91 c823 30a1  ......TN.WJ..#0.
-00002630: 0101 71e6 3390 c590 8284 463e c892 8c30  ..q.3.....F>...0
-00002640: 0833 1667 e425 2932 fcad fccf eba5 76e7  .3.g.%)2......v.
-00002650: fc7a f257 78f2 4029 f0b1 af2a 98d1 38f4  .z.Wx.@)...*..8.
-00002660: 1165 88de ae0a 14fa 90e9 095a ed04 5388  .e.........Z..S.
-00002670: b17f 57f3 a3e9 ad19 d86b be6c eaab a2f2  ..W......k.l....
-00002680: 7446 6ae7 0c21 875b 8c1c 5977 7717 9393  tFj..!.[..Yww...
-00002690: 6fef b2e0 45d7 9656 cd37 bcde c222 7adc  o...E..V.7..."z.
-000026a0: e2f1 aa12 db1b c48f 1bcc bab5 90ab ad2d  ...............-
-000026b0: 922d 2c56 cb07 0d3e b7ae c9b7 748d 5fa9  .-,V...>....t._.
-000026c0: aea1 cb58 9af9 18a4 5918 8130 c942 1007  ...X....Y..0.B..
-000026d0: ae0b 28f2 594a 7d16 a624 fd8e ba36 8c7b  ..(.YJ}..$...6.{
-000026e0: 92ae 19f4 d00f 61ff 10f6 0b0a 9bce c24e  ......a........N
-000026f0: 72c9 6fa9 9abc 5255 2714 0730 0830 4862  r.o...RU'..0.0Hb
-00002700: 9f80 34c1 2940 3ec2 4069 3af4 951f 3049  ..4.)@>.@i:...0I
-00002710: 5f54 d5e3 81ae 94f6 bde7 f678 8e7e 9603  _T.........x.~..
-00002720: de52 bd66 9868 a98f 3316 c529 2098 a90c  .R.f.h..3..) ...
-00002730: 63e2 8180 611f 8431 4509 f1d2 c087 f1e5  c...a..1E.......
-00002740: fcd6 522a 0c65 d5f0 ac3a 5d0b 7eb8 d62f  ..R*.e...:].~../
-00002750: 2677 18a6 9862 0d8d 8c6b 9eb7 571a 97fb  &w...b...k..W...
-00002760: c845 c871 a903 dd6b b629 1f9e 9f6f 6ce6  .E.q...k.)...ol.
-00002770: 5bd6 75ba 5adc 641c 7dad 8ccb 088a 55fd  [.u.Z.d.}.....U.
-00002780: 550f 8e04 82c8 a309 a084 7980 859e 1b27  U.........y....'
-00002790: 618a c234 7879 c62d a518 29f7 d73a 172a  a..4xy.-..)..:.*
-000027a0: 7533 eb1e 392e 3e85 75cf 0bb5 3743 bda8  u3..9.>.u...7C..
-000027b0: ab92 5bef d7cd c91d c0d9 2b05 3c4e 298e  ..[.......+.<N).
-000027c0: 11f4 4018 2a98 a340 9518 9f44 0188 6812  ..@.*..@...D..h.
-000027d0: 449e 0b11 c5df a1c4 0c75 a972 f620 e68f  D........u.r. ..
-000027e0: 1c25 fe57 a561 24c2 41e2 aa42 1abb bab8  .%.W.a$.A..B....
-000027f0: 1295 729c 8600 523f 8a82 50bd 4653 7a55  ..r...R?..P.FSzU
-00002800: 6906 0d69 abbc dbb6 c07c f9fc cf2f 5f3e  i..i.....|.../_>
-00002810: fffb 0cd5 c534 f3a7 9639 eba6 3771 4779  .....4...9..7qGy
-00002820: cb50 ec47 2082 2403 2409 148e 19a3 20a3  .P.G .$.$..... .
-00002830: 9890 38f2 c358 a3a7 d640 729f 3b6a 703b  ..8..X...@r.;jp;
-00002840: eef4 dd19 177d 5799 6f51 d09d e8b3 c9f5  .....}W.oQ......
-00002850: 8101 63cf f302 3708 2698 468e 5c7b ab81  ..c...7.&.F.\{..
-00002860: 5fe8 f855 5b8b 7779 7fb8 3124 69cc 092a  _..U[.wy..1$i..*
-00002870: 3643 bd26 e638 f57a 8a8e 7dfe f8b6 ff1f  6C.&.8.z..}.....
-00002880: 0000 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-00002890: 0000 0021 00eb ed0a 8213 0600 0055 1f00  ...!.........U..
-000028a0: 0021 0000 0070 7074 2f73 6c69 6465 4c61  .!...ppt/slideLa
-000028b0: 796f 7574 732f 736c 6964 654c 6179 6f75  youts/slideLayou
-000028c0: 7435 2e78 6d6c ec59 eb6e db36 14fe 3f60  t5.xml.Y.n.6..?`
-000028d0: ef20 78bf 59f3 2e2a 6852 e83a 6c48 9b60  . x.Y..*hR.:lH.`
-000028e0: 491f 4091 e85a ab6e 9364 2759 51a0 afb5  I.@..Z.n.d'YQ...
-000028f0: 3d4e 9f64 2425 c576 e2a4 4e9a 1401 961f  =N.d$%.v..N.....
-00002900: b668 8afc 780e bfef 1c1d 53af df5c 14b9  .h..x.....S..\..
-00002910: b594 4d9b 55e5 fe04 bd82 134b 9649 9566  ..M.U......K.I.f
-00002920: e587 fdc9 fbd3 0888 89d5 7671 99c6 7955  ..........vq..yU
-00002930: cafd c9a5 6c27 6f0e 7efe e975 bdd7 e6e9  ....l'o.~..u....
-00002940: 617c 592d 3a4b 6194 ed5e bc3f 9977 5dbd  a|Y-:Ka..^.?.w].
-00002950: 379d b6c9 5c16 71fb aaaa 65a9 eecd aaa6  7...\.q...e.....
-00002960: 883b f5b3 f930 4d9b f85c 6117 f914 43c8  .;...0M..\a...C.
-00002970: a745 9c95 9361 7eb3 cbfc 6a36 cb12 1954  .E...a~...j6...T
-00002980: c9a2 9065 d783 3432 8f3b 657f 3bcf ea76  ...e..42.;e.;..v
-00002990: 44ab 7741 ab1b d92a 1833 7bd3 a4ee b256  D.wA...*.3{....V
-000029a0: de76 e7d5 e9c5 e979 7574 f6e7 c432 839b  .v.....yut...2..
-000029b0: a5ea 4693 03e5 7f72 92a7 5619 17aa c3af  ..F....r..V.....
-000029c0: 8a3a 6eb2 b62a cd9d b63e 6da4 d4ad 72f9  .:n..*...>m...r.
-000029d0: 6b53 9fd4 c78d 99f0 6e79 dc58 59aa 0186  kS......ny.XY...
-000029e0: 8993 e970 6318 667e 964b d398 5e9b fe61  ...pc.f~.K..^..a
-000029f0: 6cc6 7b17 b3a6 d057 b51b d6c5 fe44 9176  l.{....W.....D.v
-00002a00: a9bf a7ba 4f5e 7456 d277 26ab de64 7eb4  ....O^tV.w&..d~.
-00002a10: 656c 320f b78c 9e8e 0b4c d716 d55e f5c6  el2......L...^..
-00002a20: dd74 078f ee9c 665d 2e2d bd3d c68e c3b6  .t....f].-.=....
-00002a30: 1b2d 5a34 d9fe e453 1461 8f85 1105 916a  .-Z4...S.a.....j
-00002a40: 010a 3d0a bc90 3a20 c244 84d8 8e7c 4cf8  ..=...: .D...|L.
-00002a50: 673d 1bf1 bda4 9186 97df d251 5f88 dfe0  g=.........Q_...
-00002a60: b4c8 92a6 6aab 59f7 2aa9 8a41 1ca3 c614  ....j.Y.*..A....
-00002a70: 9d88 0e74 6a2b 3fd9 81cb 1d5b 60c0 a0e7  ...tj+?....[`...
-00002a80: 029f 610f 4430 525f c215 9440 3fb2 91fd  ..a.D0R_...@?...
-00002a90: 79d8 0065 f378 355e 4c07 7f07 c747 22da  y..e.x5^L....G".
-00002aa0: fab0 4a3e b656 5929 a234 af3d 6f57 237a  ..J>.VY).4.=oW#z
-00002ab0: 32f5 b59e 8f9a d27b 348c eb6f 9ac6 6a97  2......{4..o..j.
-00002ac0: b752 2c88 b25c 18ee 0867 08b3 4db2 1164  .R,..\...g..M..d
-00002ad0: 8871 38b0 8808 668c 93eb 5cf6 d0f5 5e77  .q8...f...\...^w
-00002ae0: e155 e9a5 9e7e a6ae 466b f15e de76 27dd  .U...~..Fk.^.v'.
-00002af0: 652e cd8f 5a7f 1933 1a45 711e eb64 204b  e...Z..3.Eq..d K
-00002b00: f0fe a45f b53b f0f3 2cf9 6875 9525 d3ac  ..._.;..,.hu.%..
-00002b10: b3de c66d 271b cb78 a6b2 8542 d1eb f61b  ...m'..x...B....
-00002b20: 6850 6499 1ec7 4dfc c73a d8ef c783 7db5  hPd...M..:....}.
-00002b30: 316e 34ca d879 b7dc c895 dcb4 fbc7 799c  1n4..y........y.
-00002b40: c879 95a7 ca02 fc4c 9517 3981 e728 8501  .y.....L..9..(..
-00002b50: 427d 0ff0 880a e086 a10d 9840 a1e7 84d4  B}.........@....
-00002b60: c338 7a7a e569 b6b5 415a 2fdf 2340 c405  .8zz.i..AZ/.#@..
-00002b70: 42bd bc56 0a54 fab3 6d61 f702 1498 3808  B..V.T..ma....8.
-00002b80: efaa 3f2b 2e93 79a5 d2ff 590f 394a d1b4  ..?+..y...Y.9J..
-00002b90: 9739 52d3 ac22 6e0e 4d96 caca 5465 6cdd  .9R.."n.M...Tel.
-00002ba0: 3400 8b77 eab1 6466 a572 a6f5 d5fe adf2  4..w..df.r......
-00002bb0: 11d5 9170 36ba 7985 3200 e215 2065 36d6  ...p6.y.2... e6.
-00002bc0: 6377 4285 3751 35d4 804a 56a8 0ea2 c682  cwB.7Q5..JV.....
-00002bd0: 5d50 91b8 89aa a106 54ba 4245 c446 26c4  ]P......T.BE.F&.
-00002be0: 7782 3523 3761 35d6 00cb d660 0516 c686  w.5#7a5....`....
-00002bf0: 87c2 6aac 0196 af60 3116 dc6c d843 6135  ..j....`1..l.Ca5
-00002c00: d600 6baf c1da 94ec ccd8 3658 8d35 c08a  ..k.......6X.5..
-00002c10: 15ac c6dc 9db2 2db0 1a6b 8075 d660 39b3  ......-..k.u.`9.
-00002c20: bf8b 328d d5b7 d762 c264 67bd 881a 70f5  ..2....b.dg...p.
-00002c30: 28bf 7fb6 d691 6b92 75bb 91ad 1f92 91e9  (.....k.u.......
-00002c40: 9891 fdaa ec94 a31b 4999 3cd3 a48c 3981  ........I.<...9.
-00002c50: 51e4 2110 2024 0043 2402 d085 1408 8f61  Q.!. $.C$......a
-00002c60: 9f22 8712 8f3f 6552 d69c cfe3 7c36 a4e4  ."...?eR....|6..
-00002c70: 3e5d 3e30 2563 0619 b4af 1505 1b29 9970  >]>0%c.......).p
-00002c80: 4199 1afd 7d35 c113 abee fa2a 6603 ef5e  A...}5.....*f..^
-00002c90: e544 2655 995a b95c ca7c 0744 b3cb 7723  .D&U.Z.\.|.D..w#
-00002ca0: 9ece b366 77c0 e131 7817 6054 2d9a 6ebe  ...fw..1x.`T-.n.
-00002cb0: 3322 dd01 319b 6d05 7cec 4a8b dd5a 69d1  3"..1.m.|.J..Zi.
-00002cc0: 671a d414 0997 84d0 032c b07d 1060 b53a  g........,.}.`.:
-00002cd0: 76b9 0f3c e442 e240 e287 2ef9 5195 960e  v..<.B.@....Q...
-00002ce0: f0bf 1671 a374 3fc4 785f 92df 27c6 39b2  ...q.t?.x_..'.9.
-00002cf0: b179 dedd 5e77 0982 7416 78a9 bb5e eaae  .y..^w..t.x..^..
-00002d00: 97ba ebff 5577 f1bb ea2e f64c 5334 5455  ....Uw.....LS4TU
-00002d10: 8be3 e310 2004 85fa 474c 0200 11a7 0085  .... ...GL......
-00002d20: 14a9 f4a5 0c63 ee53 d75d 9b69 d93c 711f  .....c.S.].i.<q.
-00002d30: 9c96 6fa9 bdd6 d2f2 4bed f552 7bdd 3bb6  ..o.....K..R{.;.
-00002d40: ed31 b683 b893 1b81 cd9f eb29 97f0 422c  .1.........)..B,
-00002d50: 6c07 84be 8000 61cc 8007 a90b 0822 98bb  l.....a......"..
-00002d60: 30f2 c2e0 079c afa6 5d5f 79ad fdb5 42fd  0.......]_y...B.
-00002d70: b1f6 ad01 6e4e dd77 8cc2 599e f6de 3241  ....nN.w..Y...2A
-00002d80: 22ee f921 a084 ab1d 26d4 060e 2702 b83e  "..!....&...'..>
-00002d90: c301 b543 4720 fff3 f822 2155 1c76 5921  ...CG ..."!U.vY!
-00002da0: a3ec c3a2 9147 8bce 50b8 a130 a514 ab2d  .....G..P..0...-
-00002db0: 3a3f 9771 7915 e3dd 0186 184f 219b 22b8  :?.qy......O!.".
-00002dc0: 529b b2e1 f1f5 2646 bd45 55a5 b3c5 bae2  R.....&F.EU.....
-00002dd0: ec67 aa38 cf63 9e87 0204 3074 11f0 3d41  .g.8.c....0t..=A
-00002de0: d5f6 731b 501e d090 091f 53ef 079c abce  ..s.P.....S.....
-00002df0: ba66 5bb1 8fbe 71c8 7a1f d53d 2ed5 ce48  .f[...q.z..=...H
-00002e00: f549 9ea5 d27a b728 ceae 112e 9e6b ed10  .I...z.(.....k..
-00002e10: 081f 06ae 0d98 2d6c a02a 68aa 4fd3 3960  ......-l.*h.O.9`
-00002e20: c275 c250 7d88 f3a4 b543 4f78 9ba7 6acf  .u.P}....COx..j.
-00002e30: b672 fe8d 539c 0765 1a4e 3de2 0490 00e5  .r..S..e.N=.....
-00002e40: 3b01 814f d596 93d0 0588 09cf 735c dfe1  ;..O........s\..
-00002e50: 8c5d 659a 5653 5a2a eb76 4d30 5fbf fcf3  .]e.VSZ*.vM0_...
-00002e60: cbd7 2fff 3e42 7631 97f1 cde7 b8eb a635  ../.>Bv1.......5
-00002e70: 6847 59cb b12f 3cf5 6f9c 4680 068e 0ddc  hGY../<.o.F.....
-00002e80: 8833 1031 42a9 8a5e d727 a1d6 4e8d e84d  .3.1B..^.'..N..M
-00002e90: eda8 cedd b453 57e7 b2a9 abcc bc1e 4670  .....SW.......Fp
-00002ea0: 90cf 32d6 1588 4338 150c 8fcf 835e 222b  ..2...C8.....^"+
-00002eb0: 6335 ef27 da7d 75cd 9bb7 717d b434 1a29  c5.'.}u...q}.4.)
-00002ec0: 4c01 e59b ae5a ebb2 1fba 1aa2 5d1f 5f87  L....Z......]._.
-00002ed0: 1ffc 0700 00ff ff03 0050 4b03 0414 0006  .........PK.....
-00002ee0: 0008 0000 0021 0077 d06c dcdc 0300 0014  .....!.w.l......
-00002ef0: 0c00 0021 0000 0070 7074 2f73 6c69 6465  ...!...ppt/slide
-00002f00: 4c61 796f 7574 732f 736c 6964 654c 6179  Layouts/slideLay
-00002f10: 6f75 7436 2e78 6d6c cc56 db6e dc36 107d  out6.xml.V.n.6.}
-00002f20: 2fd0 7f10 d467 5a12 2fba 2cb2 0e74 2d1a  /....gZ./.,..t-.
-00002f30: 38b1 d175 3e80 91b8 5e21 ba95 e26e bc0d  8..u>...^!...n..
-00002f40: 0ce4 b7da cfc9 9774 4849 b613 bb80 1f6c  .......tHI.....l
-00002f50: c02f 2245 cd0c cfcc 391c f1cd dbeb b6b1  ./"E....9.......
-00002f60: 0e42 8e75 dfad 6def c4b5 2dd1 957d 5577  .B.u..m...-..}Uw
-00002f70: 576b fbe3 6581 42db 1a15 ef2a def4 9d58  Wk..e.B....*...X
-00002f80: db47 31da 6f4f 7ffd e5cd b01a 9bea 8c1f  .G1.oO..........
-00002f90: fbbd b220 4637 aef8 dade 2935 ac1c 672c  ... F7....)5..g,
-00002fa0: 77a2 e5e3 493f 880e be6d 7bd9 7205 aff2  w...I?...m{.r...
-00002fb0: caa9 24ff 02b1 dbc6 c1ae eb3b 2daf 3b7b  ..$........;-.;{
-00002fc0: f697 4ff1 efb7 dbba 1459 5fee 5bd1 a929  ..O......Y_.[..)
-00002fd0: 8814 0d57 807f dcd5 c3b8 441b 9e12 6d90  ...W......D...m.
-00002fe0: 6284 30c6 fb47 48ea 3840 b6aa 568d 38ef  b.0..GH.8@..V.8.
-00002ff0: 9aa3 6d19 5379 8045 cf3e 85ec cb4d 5359  ..m.Sy.E.>...MSY
-00003000: 1d6f 61e1 525b 59c6 4c7f 1987 4b29 849e  .oa.R[Y.L...K)..
-00003010: 7587 dfe5 b019 2ea4 71f8 70b8 9056 5de9  u.......q.p..V].
-00003020: 00b3 a3ed cc1f 6633 f3da 1dcc c4f9 c9fd  ......f3........
-00003030: 6a99 f2d5 f556 b67a 845a 58d7 6b1b 283b  j....V.z.ZX.k.(;
-00003040: eaa7 a3d7 c4b5 b2ca 69b1 bc5b 2d77 e78f  ........i..[-w..
-00003050: d896 bbfc 116b 67d9 c0b9 b7a9 ce6a 02f7  .....kg......j..
-00003060: 301d bca4 33d5 4197 c7e0 381b d582 682f  0...3.A...8...h/
-00003070: ebb5 fdb5 2870 c2f2 82a2 0266 88ba 0945  ....(p.....f...E
-00003080: 494e 2354 6012 e638 2852 4cfc 1bed edf9  IN#T`..8(RL.....
-00003090: ab52 0ac3 ca1f d5a2 2ecf 7fc0 685b 97b2  .R..........h[..
-000030a0: 1ffb ad3a 29fb 7696 c6a2 3020 d3a3 3399  ...:).v...0 ..3.
-000030b0: 1ae5 571c d184 15d4 476e e6a7 88e1 3843  ..W.....Gn....8C
-000030c0: b4f0 180a bd34 202c 0a7d 9ae5 3773 0100  .....4 ,.}..7s..
-000030d0: f332 9a2c 9c39 df39 f185 8871 38eb cbcf  .2.,.9.9...q8...
-000030e0: a3d5 f540 94e6 75e2 edd6 6222 538f c3ee  ...@..u...b"S...
-000030f0: bea2 66bb e9a3 99dc 5579 5681 ba4e faea  ..f.....UyV..N..
-00003100: a837 f904 a359 e4ab 6654 1b75 6c84 7919  .7...Y..fT.ul.y.
-00003110: f4c3 c090 4044 c3f5 8115 1dfa b899 c855  ....@D.........U
-00003120: a769 5397 9f2d d55b a2aa 95f5 9e8f 4a48  .iS..-.[......JH
-00003130: cbec 0f27 1aa2 e804 a734 4d14 d155 175c  ...'.....4M..U.\
-00003140: f23f ef07 7b77 3117 6430 3817 50ce 2287  .?..{w1.d08.P.".
-00003150: ff17 0559 4491 7125 ac8b 8697 62d7 3715  ...YD.q%....b.7.
-00003160: 20c0 af54 1f61 cc02 1644 05c2 3863 c8cd   ..T.a...D..8c..
-00003170: 4317 c549 e823 ec66 ae97 146e c2d2 e0e5  C..I.#.f...n....
-00003180: f551 29e8 b77f 4326 bcd9 6a60 7038 bde9  .Q)...C&..j`p8..
-00003190: 583e 8b5e b6d0 b44c b62c 2485 9fa4 39a2  X>.^...L.,$...9.
-000031a0: c487 0a13 1aa0 c827 218a 5386 331a e411  .......'!.S.3...
-000031b0: 1c8b 9ba5 0d56 c0a1 aa5b 51d4 577b 29ce  .....V...[Q.W{).
-000031c0: f7ca 50f8 83ec 4029 d6d8 aab4 11bc bb6d  ..P...@).......m
-000031d0: 30ea 14bb 183b 2e73 3cf7 4e6d 80e1 f9f5  0....;.s<.Nm....
-000031e0: 4617 bd15 7daf 757e 5f71 e495 2ace a769  F...}.u~_q..*..i
-000031f0: 9c16 0541 9e0f 1cc4 aeeb 0211 1143 819b  ...A.........C..
-00003200: e220 2369 92b2 f0e5 15b7 5572 92dc 5f7b  . #i......Ur.._{
-00003210: 2ea1 748b ea16 df67 50dd f352 cd16 aa37  ..t....gP..R...7
-00003220: 4d5d 09eb c3be fdf4 13e1 f495 129e 1042  M].............B
-00003230: 80e1 08e1 388c 5082 dd04 7959 067d 86b8  ....8.P...yY.}..
-00003240: 7e9c e63e 262c 7e79 c2e1 de06 357b 9473  ~..>&,~y....5{.s
-00003250: fc02 9dc6 a709 8932 97a0 3085 4796 5228  .......2..0.G.R(
-00003260: 39c9 63e4 b130 49a2 388d 7cc6 6e3b cda8  9.c..0I.8.|.n;..
-00003270: 29ed 00dd 531b ccf7 6fff fcf6 fddb bfcf  )...S...o.......
-00003280: d05d ccb0 dcdc 96aa 9bd9 ac1d 40eb e334  .]..........@..4
-00003290: 4c50 e2d1 02d1 2c0a 505c f80c 158c 509a  LP....,.P\....P.
-000032a0: 2661 9c92 5c6b 67f0 e843 edc0 e2d3 b433  &a..\kg..C.....3
-000032b0: f45f 841c fada 5c6e 3d77 96cf 8137 70d1  ._....\n=w...7p.
-000032c0: 0abc 10b3 c823 0b4d 9346 eed0 6ae2 373a  .....#.M.F..j.7:
-000032d0: 7f18 1bf9 9e0f e707 2392 d6fc fb53 b334  ........#....S.4
-000032e0: 6861 4ea6 7726 3af7 e536 7ffa 1f00 0000  haN.w&:..6......
-000032f0: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00003300: 2100 45ea e258 8703 0000 f609 0000 2100  !.E..X........!.
-00003310: 0000 7070 742f 736c 6964 654c 6179 6f75  ..ppt/slideLayou
-00003320: 7473 2f73 6c69 6465 4c61 796f 7574 372e  ts/slideLayout7.
-00003330: 786d 6ccc 96db 6edc 3610 86ef 0bf4 1d04  xml...n.6.......
-00003340: f59a d689 92a8 45d6 81a8 43d1 c28d 1775  ......E...C....u
-00003350: fa00 b4c4 f50a d1a9 1477 b3db c040 5eab  .........w...@^.
-00003360: 799c 3c49 8694 68a7 b60b f8c2 0672 2352  y.<I..h......r#R
-00003370: a319 7266 be5f 94de bc3d 76ad 75e0 626a  ..rf._...=v.u.bj
-00003380: 867e 6d7b 67ae 6df1 be1a eaa6 bf59 db7f  .~m{g.m......Y..
-00003390: bd2f 11b1 ad49 b2be 66ed d0f3 b57d e293  ./...I..f....}..
-000033a0: fdf6 fce7 9fde 8cab a9ad 2fd8 69d8 4b0b  ........../.i.K.
-000033b0: d6e8 a715 5bdb 3b29 c795 e34c d58e 776c  ....[.;)...L..wl
-000033c0: 3a1b 46de c3b3 ed20 3a26 e156 dc38 b560  :.F.... :&.V.8.`
-000033d0: 1f61 edae 757c d78d 9c8e 35bd bdc4 8be7  .a..u|....5.....
-000033e0: c40f db6d 53f1 7ca8 f61d efe5 bc88 e02d  ...mS.|........-
-000033f0: 9390 ffb4 6bc6 c9ac 363e 67b5 51f0 0996  ....k...6>g.Q...
-00003400: d1d1 ff4d 499e 46a8 f6ba 65fd 07db d26e  ...MI.F...e....n
-00003410: e200 06cf 3e87 caab abb6 b67a d681 816a  ....>......z...j
-00003420: 0f65 9cc6 f782 7335 eb0f bf8a f16a dc08  .e....s5.....j..
-00003430: edfb eeb0 1156 53ab d825 c676 9607 8b9b  .....VS..%.v....
-00003440: beed 0f7a e23c 08bf 3153 b63a 6e45 a746  ...z.<..1S.:nE.F
-00003450: 6881 755c db40 eaa4 ae8e b2f1 a3b4 aad9  h.u\.@..........
-00003460: 58dd 5bab dde5 13be d5ae 78c2 db31 1b38  X.[.......x..1.8
-00003470: df6d aaaa 9a93 7b5c 8e6f cac9 99e4 d6a6  .m....{\.o......
-00003480: 6515 df0d 6dcd 85a5 9aa4 53ba 98a4 496e  e...m.....S...In
-00003490: 2f9a b5fd a92c 7d1a 1625 4625 cc10 7629  /....,}..%F%..v)
-000034a0: 46b4 c009 2afd 8014 7e5c 667e 10dd aa68  F...*...~\f~...h
-000034b0: 2f5a 5582 6b2e bfd5 465f 5ef4 8869 d754  /ZU.k...F_^..i.T
-000034c0: 6298 86ad 3cab 866e 1187 d118 e0f4 f082  b...<..n........
-000034d0: 5325 fc89 e2ac 2808 7551 1e90 0c85 619a  S%....(.uQ....a.
-000034e0: a23c 4e08 ca8b 24ca 0abf c461 4c6e 975e  .<N...$....aLn.^
-000034f0: 40ce 66d4 5538 4be9 4b0f 0c93 69bc 18aa  @.f.U8K.K...i...
-00003500: 0f93 d50f c04c 219e 11de 79cc 5cd5 38ee  .....L!...y.\.8.
-00003510: 164d d512 dea8 7fa0 12d6 6e55 62c0 c19b  .M........nUb...
-00003520: 0918 673d b907 b008 441e e950 9fd4 a6d7  ..g=....D..P....
-00003530: 306a 235b b593 bc92 a796 eb9b 515d b620  0j#[........Q]. 
-00003540: 4d5d 6d48 8232 a259 8170 1041 8703 1ca3  M]mH.2.Y.p.A....
-00003550: 240a 084a b3d0 cf71 5c24 c4cb 6e8d d06b  $..J...q\$..n..k
-00003560: 6028 9b8e 97cd cd5e f0cb bdd4 0805 a006  `(.....^........
-00003570: 7dc3 49c0 7bf4 fb06 f2ee 64d6 72d6 df69  }.I.{.....d.r..i
-00003580: 499e fbae ef3b 6ee8 78ae 6ad7 dc34 c841  I....;n.x.j..4.A
-00003590: 73ef eb0d 13ec cf07 abcc 0d1e 759d a628  s...........u..(
-000035a0: c728 edff f516 18bd 95c3 2041 65df 2bce  .(........ Ae.+.
-000035b0: ff41 1517 a531 f6a8 9721 2fa7 0495 799c  .A...1...!/...y.
-000035c0: a238 80dd 8b88 d020 a524 74f3 ecf5 15b7  .8..... .$t.....
-000035d0: 9562 96dc df7b 26a0 7546 7526 f605 54f7  .b...{&.uFu&..T.
-000035e0: b2a8 b141 7dd5 3635 b7de edbb eb07 c083  ...A}.65........
-000035f0: 1f14 784a e234 0623 c224 8a50 4993 1c95  ..xJ.4.#.$.PI...
-00003600: d825 288c d28c 0624 f470 11bd 3e70 f832  .%(....$.p..>p.2
-00003610: 43cf 9e64 eebf c249 1361 1a24 b91b 2092  C..d...I.a.$.. .
-00003620: c125 cf30 b43c 2852 e485 84d2 24cd 9228  .%.0.<(R....$..(
-00003630: 0cef 4e9a 4921 ed21 bbe7 1e30 5f3f fffb  ..N.I!.!...0_?..
-00003640: cbd7 cf5f 5ee0 74d1 83f9 489b aeeb d9a2  ..._^.t...H.....
-00003650: 1dc8 36f2 3342 11f5 7089 709e c428 2da3  ..6.3B..p.p..(-.
-00003660: 1095 6180 7146 499a 0585 d2ce e8e1 c7da  ..a.qFI.........
-00003670: 01e3 f3b4 330e 1fb9 1887 46ff be78 ee22  ....3.....F..x."
-00003680: 9f03 6be1 8c8b e238 0c02 df27 0ba6 5923  ..k....8...'..Y#
-00003690: f7d9 2af0 57aa 7e18 5bf1 071b 2f0f 5a24  ..*.W.~.[.../.Z$
-000036a0: b019 40ce b469 54c2 9c5d ef5d 54ed e67f  ..@..iT..].]T...
-000036b0: edfc 1b00 0000 ffff 0300 504b 0304 1400  ..........PK....
-000036c0: 0600 0800 0000 2100 337a e3c3 b205 0000  ......!.3z......
-000036d0: 7817 0000 2100 0000 7070 742f 736c 6964  x...!...ppt/slid
-000036e0: 654c 6179 6f75 7473 2f73 6c69 6465 4c61  eLayouts/slideLa
-000036f0: 796f 7574 382e 786d 6ccc 58ed 729b 4614  yout8.xml.X.r.F.
-00003700: fddf 99be 03a3 fe26 623f 80c5 133b 0308  .......&b?...;..
-00003710: 3aed 3889 a772 1e00 c3ca a2e1 abb0 92e5  :.8..r..........
-00003720: 6632 93d7 6a1f 274f d2bb 0b2b 4bb2 6229  f2..j.'O...+K.b)
-00003730: 8e3d f51f b8a0 b387 bb7b 0ef7 2e7a fd66  .=.......{...z.f
-00003740: 5516 c692 b75d 5e57 a723 f4ca 1a19 bc4a  U....]^W.#.....J
-00003750: eb2c afae 4f47 1f2e 6393 8d8c 4e24 5596  .,..OG..c...N$U.
-00003760: 1475 c54f 47b7 bc1b bd39 fbf9 a7d7 cd49  .u.OG....9.....I
-00003770: 5764 e7c9 6dbd 1006 7054 dd49 723a 9a0b  Wd..m...pT.Ir:..
-00003780: d19c 8cc7 5d3a e765 d2bd aa1b 5ec1 6fb3  ....]:.e....^.o.
-00003790: ba2d 1301 97ed f538 6b93 1be0 2e8b 31b6  .-.....8k.....1.
-000037a0: 2c67 5c26 7935 1ac6 b7c7 8caf 67b3 3ce5  ,g\&y5......g.<.
-000037b0: 933a 5d94 bc12 3d49 cb8b 4440 fedd 3c6f  .:]...=I..D@..<o
-000037c0: 3acd d61c c3d6 b4bc 031a 357a 3b25 71db  :.........5z;%q.
-000037d0: c06c ebab 3f2f 5723 43c1 da25 dc40 a333  .l..?/W#C..%.@.3
-000037e0: 9879 3a2d 32a3 4a4a b811 d695 0006 e326  .y:-2.JJ.......&
-000037f0: 1773 234c 1ac9 a430 5d73 d972 2ea3 6af9  .s#L...0]s.r..j.
-00003800: 6bdb 4c9b 8b56 0d7d b7bc 688d 3c93 5403  k.L..V.}..h.<.T.
-00003810: c568 3cfc 30c0 d465 b554 c178 67f8 b50e  .h<.0..e.T.xg...
-00003820: 9393 d5ac 2de5 1956 c458 9d8e 40b8 5b79  ....-..V.X..@.[y
-00003830: 1ccb 7b7c 258c b4bf 99de dd4d e7ef f760  ..{|%......M...`
-00003840: d379 b407 3dd6 0f18 6f3c 54ce aa4f eefe  .y..=...o<T..O..
-00003850: 74b0 9ece 652e 0a6e c885 5279 9c77 4267  t...e..n..Ry.wBg
-00003860: b468 f3d3 d1a7 38c6 811d c5d4 8c21 32a9  .h....8......!2.
-00003870: 1550 3388 a867 c698 b008 bb71 8889 f359  .P3..g.....q...Y
-00003880: 8e46 ce49 da72 a5cd 6f99 f618 72ee e95a  .F.I.r..o...r..Z
-00003890: e669 5b77 f54c bc4a eb72 3088 f619 488a  .i[w.L.J.r0...H.
-000038a0: e820 a9cc f253 ecb9 91ed c5b1 892d db35  . ...S.......-.5
-000038b0: 6dec 4466 3c41 aee9 3913 e27b cc45 2c64  m.Df<A..9..{.E,d
-000038c0: 9f87 0580 9cf5 59cd 623c cc77 98b8 16a2  ......Y.b<.w....
-000038d0: 6bce ebf4 6367 5435 0825 75ed 755b 237a  k...cgT5.%u.u[#z
-000038e0: 31e5 b999 0fbe 1272 8d06 5cff a30a ee56  1......r..\....V
-000038f0: 79af c48c 782e 634a 3b6a bb60 d66d b189  y...x.cJ;j.`.m..
-00003900: 4730 266e 2f22 722c 6b40 6c4a d933 3727  G0&n/"r,k@lJ.37'
-00003910: 6215 d4d9 ad1c 7d05 6790 30a9 d279 0d6f  b.....}.g.0..y.o
-00003920: e055 cf59 7462 2a6e 0bae e265 8186 8432  .U.Ytb*n...e...2
-00003930: 3efb 03c0 dddf f0b4 3bf6 3540 c61b 031b  >.......;.5@....
-00003940: 7950 e35a 1854 24b2 a4f0 cafc 30ed 9f21  yP.Z.T$.....0..!
-00003950: cec2 224f 3f1a a236 7896 0be3 6dd2 09de  .."O?..6x...m...
-00003960: 1a6a 6da0 e600 8924 ec25 502c bcca 2e92  .jm....$.%P,....
-00003970: 3691 19ac c97e bf18 9268 d4fc f4bc d454  6....~...h.....T
-00003980: 1f36 2cd1 86d5 aff0 4591 a47c 5e17 1924  .6,.....E..|^..$
-00003990: 815f a87d 2962 7e4c 5c6c 3a01 8dcc d009  ._.})b~L\l:.....
-000039a0: 43c8 83c0 a5e7 dbc8 c29e ed05 e839 ed9b  C............9..
-000039b0: 67ab 3bc8 f1ce b511 2368 b02e bc64 14db  g.;.....#h...d..
-000039c0: dbd6 7590 8ba5 9f94 7529 7389 d323 8eb1  ..u.....u)s..#..
-000039d0: ee0f f855 85f8 3e16 b34d ac06 4048 f660  ...U..>..M..@H.`
-000039e0: e926 5603 20a4 7bb0 d626 5603 20b4 0f61  .&V. .{..&V. ..a
-000039f0: 3500 42e7 1056 0320 740f 6135 0042 7608  5.B..V. t.a5.Bv.
-00003a00: ab01 107a 87b0 3d60 5f3d 68e4 dbbb 2cd6  ...z..=`_=h...,.
-00003a10: ede7 fbeb 8334 8d2a 0fdd 567d e86b c0ee  .....4.*..V}.k..
-00003a20: 5394 571f 7eca 94a7 7595 1905 5ff2 e208  S.W.~...u..._...
-00003a30: 467c 98f1 729e b7c7 1392 c384 71bd 6861  F|..r.......q.ha
-00003a40: 7f71 2c23 3d82 319f ed25 7cea 2a4b d7db  .q,#=.1..%|.*K..
-00003a50: 0229 db66 8925 2fb4 c462 ea7b 813d 9998  .).f.%/..b.{.=..
-00003a60: ae15 7866 4826 b669 7970 8823 826d 0f91  ..xfH&.iyp.#.m..
-00003a70: c0b5 c3e7 df21 c8da 3652 2fd6 3c29 6632  .....!..6R/.<)f2
-00003a80: b5d5 60bd c76e 19e4 8667 a855 dfd8 3310  ..`..n...g.U..3.
-00003a90: 8690 0de8 1f2c bc46 99b4 e76a 3799 5719  .....,.F...j7.W.
-00003aa0: 3456 19aa 518b 77f0 09a1 466d d40d b951  4V..Q.w...Fm...Q
-00003ab0: f966 5d1e a886 ddce 717c 5bf5 78a7 760f  .f].....q|[.x.v.
-00003ac0: 7c1e a212 751c df56 dfd8 a9ef 031f 22ae  |...u..V......".
-00003ad0: 9ac6 7184 0f35 014d c830 933d e811 843b  ..q..5.M.0.=...;
-00003ae0: 9d62 20c4 9839 12f6 08c2 9d76 a209 5daa  .b ..9.....v..].
-00003af0: 3aea 2308 777a ce40 28d9 8e17 e5a1 c6a4  :.#.wz.@(.......
-00003b00: 091d db7d a428 ff5b f7fa beda 6aeb da3a  ...}.(.[....j..:
-00003b10: 4904 dfaa adf4 85d6 569b f831 f62c 6612  I.......V..1.,f.
-00003b20: 2b44 664c 8865 32db 714c eaf9 0ea3 f0f4  +DfL.e2.qL......
-00003b30: c0a3 cf5f 5b33 71af b2a2 5efd 6f96 56f5  ..._[3q...^.o.V.
-00003b40: 4dfe 6001 5417 ca23 b322 1b66 cb48 ec04  M.`.T..#.".f.H..
-00003b50: 6164 52e2 c00a 132a 3f33 0933 fdd0 c613  adR....*?3.3....
-00003b60: ea46 1e43 d049 7452 a0a1 c84b 1ee7 d78b  .F.C.ItR...K....
-00003b70: 96bf 5f08 25e1 96b5 a00b 1b5d 29c2 8227  .._.%......])..'
-00003b80: d5da 81e2 0c5b 188f 2d7b 8cac 3b47 410e  .....[..-{..;GA.
-00003b90: 4fdf cb1d edb7 b8ae a597 371d 67bf d46e  O.........7.g..n
-00003ba0: 1ec6 21f5 5d58 f908 5a7a 1462 c823 7423  ..!.]X..Zz.b.#t#
-00003bb0: 68e9 0c11 1432 12fa d6f3 3b6e 26da de72  h....2....;n&..r
-00003bc0: 7f2d 9216 964e bbee c097 d4f7 b8ee 69a5  .-...N........i.
-00003bd0: 76b5 d4d3 22cf b8f1 6e51 5eed 08ee bc54  v..."...nQ^....T
-00003be0: c1bd 8987 221b 993e c3be e94d 8200 548f  ...."..>...M..T.
-00003bf0: e040 233f b06c e447 983c bfe0 5d91 c19a  .@#?.l.G.<..]...
-00003c00: edd5 fcc0 26ee 5195 c6a1 01f1 2616 3159  ....&.Q.....&.1Y
-00003c10: 0887 4948 61c9 49e4 9bb0 9d0b 02cf 0f3d  ..IHa.I........=
-00003c20: c7b6 d795 a693 9256 90dd b105 e6eb 977f  .......V........
-00003c30: 7ef9 fae5 df27 a82e eaa4 ff17 d5ab aea2  ~....'..........
-00003c40: c13b 90ad 8343 1698 01a2 b149 279e 6bfa  .;...C.....I'.k.
-00003c50: b103 9b6f 9b50 1a06 cc0f 4924 bdd3 207a  ...o.P....I$.. z
-00003c60: df3b 70f3 38ef 34f5 0d6f 9b3a 577f 2023  .;p.8.4..o.:W. #
-00003c70: 6bb0 cf32 919f 4ed8 752d e660 4fab dc7b  k..2..N.u-.`O..{
-00003c80: e42e 5b29 fc54 ce1f ce45 fb36 69de 2f95  ..[).T...E.6i./.
-00003c90: 494a d5df 4375 ab91 c6ec a177 1039 77fd  IJ..Cu.....w.9w.
-00003ca0: 8ff9 d97f 0000 00ff ff03 0050 4b03 0414  ...........PK...
-00003cb0: 0006 0008 0000 0021 0067 f05a c784 0500  .......!.g.Z....
-00003cc0: 0027 1700 0021 0000 0070 7074 2f73 6c69  .'...!...ppt/sli
-00003cd0: 6465 4c61 796f 7574 732f 736c 6964 654c  deLayouts/slideL
-00003ce0: 6179 6f75 7439 2e78 6d6c cc58 dd72 9b38  ayout9.xml.X.r.8
-00003cf0: 18bd df99 7d07 86bd 568d 7e91 324d 3a80  ....}...V.~.2M:.
-00003d00: 6167 3b69 9bd9 a40f 4001 c74c f95b 905d  ag;i....@..L.[.]
-00003d10: 673b 9de9 6bed 3e4e 9f64 2501 b669 92d6  g;..k.>N.d%..i..
-00003d20: 4d9d 9ddc 802c 3e1d be4f e7e8 48f8 f98b  M....,>..O..H...
-00003d30: 4d59 58eb aced f2ba 3ab5 e133 c7b6 b22a  MYX.....:..3...*
-00003d40: a9d3 bcba 3eb5 df5e 4580 db56 27e3 2a8d  ....>..^E..V'.*.
-00003d50: 8bba ca4e ed9b acb3 5f9c fdfa cbf3 e6a4  ...N...._.......
-00003d60: 2bd2 f3f8 a65e 494b 6154 dd49 7c6a 2fa5  +....^IKaT.I|j/.
-00003d70: 6c4e 66b3 2e59 6665 dc3d ab9b ac52 cf16  lNf..Yfe.=...R..
-00003d80: 755b c652 fd6c af67 691b 7f50 d865 3143  u[.R.l.gi..P.e1C
-00003d90: 8ec3 6665 9c57 f630 be3d 647c bd58 e449  ..fe.W.0.=d|.X.I
-00003da0: 36af 9355 9955 b207 69b3 2296 2aff 6e99  6..U.U..i.".*.n.
-00003db0: 37dd 88d6 1c82 d6b4 59a7 60cc e869 4af2  7.......Y.`..iJ.
-00003dc0: a651 d536 7972 b5b1 2d13 d6ae 5507 b4cf  .Q.6yr..-...U...
-00003dd0: 54e5 c965 915a 555c aa8e 8b3c 91ab 36b3  T..e.ZU\...<..6.
-00003de0: 3ee4 7269 0571 a391 4c4c d75c b559 a65b  >.ri.q..LL.\.Y.[
-00003df0: d5fa f7b6 b96c 2e5a 33f4 f5fa a2b5 f254  .....l.Z3......T
-00003e00: 430d 10f6 6c78 3084 999f d5da 3466 5f0d  C...lx0.....4f_.
-00003e10: bf1e 9bf1 c966 d196 faae 66c4 da9c da8a  .....f....f.....
-00003e20: b81b 7d9d e9be 6c23 ada4 ef4c 76bd c9f2  ..}...l#...Lv...
-00003e30: cd1d b1c9 32bc 237a 36be 60b6 f752 5d55  ....2.#z6.`..R]U
-00003e40: 9fdc ed72 d058 ce55 2e8b ccd2 1365 f238  ...r.X.U.....e.8
-00003e50: efe4 98d1 aacd 4fed 8f51 847c 1a46 0444  ......O..Q.|.F.D
-00003e60: aa05 88e3 13e0 8744 8008 611e 2237 0a10  .......D..a."7..
-00003e70: 669f f468 c84e 9236 33dc fc91 8e1a 83ec  f..h.N.63.......
-00003e80: 16af 659e b475 572f e4b3 a42e 0781 8c3a  ..e..uW/.......:
-00003e90: 5394 4232 50aa b3fc e853 1672 02e7 8005  S.B2P....S.r....
-00003ea0: 5e08 22e2 4600 79d8 01c4 9fab a45c c485  ^.".F.y......\..
-00003eb0: 177c 1a26 40e5 3cde 4d15 b3a1 dea1 f091  .|.&@.<.M.......
-00003ec0: 88ae 39af 93f7 9d55 d58a 28cd 6bcf db36  ..9....U..(.k..6
-00003ed0: a227 53df 9be5 a02b a9e7 6888 eb1f 9ac6  .'S....+..h.....
-00003ee0: 6e96 efa4 9863 e172 6eb8 23d4 5562 9d92  n....c.rn.#.Ub..
-00003ef0: 8d05 4608 bb3d 8990 39ce 10b1 4f65 8fdc  ..F..=..9...Oe..
-00003f00: 9cc8 8d5f a737 7af4 3b75 5714 c655 b2ac  ..._.7z.;uW..U..
-00003f10: d50a 7cd7 6316 9dbc 9437 4566 daeb 020e  ..|.c....7Ef....
-00003f20: 09a5 d9e2 4f15 dcfd adde b643 df06 e8f6  ....O......C....
-00003f30: dec0 465f ccb8 560d 2a62 6d29 5905 de5e  ..F_..V.*bm)Y..^
-00003f40: f6ef 9067 4191 27ef 2d59 5b59 9a4b eb55  ...gA.'.-Y[Y.K.U
-00003f50: dcc9 acb5 ccdc 28cf 5120 1ab0 a7c0 a064  ......(.Q .....d
-00003f60: 557a 11b7 b1ce 600b f6f2 6248 a231 f58d  Uz....`...bH.1..
-00003f70: 7599 52bf 2d58 3c0a 765c c217 459c 64cb  u.R.-X<.v\..E.d.
-00003f80: ba48 5512 e889 ca17 63cf f119 c300 f938  .HU.....c......8
-00003f90: 020e 7608 7020 7780 0b29 82fe 1c8b 803b  ..v.p w..).....;
-00003fa0: 8f2f 5f65 8b3a 9fcd 2efa 7011 53c8 311c  ./_e.:....p.S.1.
-00003fb0: 542c b84b 109d aa98 4117 6969 1915 13ee  T,.K....A.ii....
-00003fc0: 62d6 471c a2e2 fba4 6b95 717b 6efc 2daf  b.G.....k.q{n.-.
-00003fd0: 52e5 f7ba 6946 ad5e ab4d cd8c fa8e b24d  R...iF.^.M.....M
-00003fe0: 13ed a086 f577 101e e2fb 781a 64c0 c33b  .....w....x.d..;
-00003ff0: 3c01 0939 184f 476e f134 c880 4776 7810  <..9.OGn.4..Gvx.
-00004000: bbda 010e 0474 f601 35ca 0048 f700 39e2  .....t..5..H..9.
-00004010: ba8e 0700 6a94 0190 ed00 11e2 4c87 3d00  ....j.......L.=.
-00004020: 50a3 0c80 ee1e a04b 0c73 0f00 d428 0320  P......K.s...(. 
-00004030: df01 6ab4 c349 9900 6a94 0150 ec01 32ea  ..j..I..j..P..2.
-00004040: 3e90 148d 72b7 bf1e d714 c976 17d7 eb71  >...r......v...q
-00004050: df11 f113 7544 3ee7 0142 cc03 0e81 08b8  ....uD>..B......
-00004060: aecf 01f6 a80f 3c65 1d91 0899 6082 3fbe  ......<e....`.?.
-00004070: 236a ffb1 0d6f cbb8 580c e688 7e66 8747  #j...o..X...~f.G
-00004080: 0e75 8785 7ecf 168f 3984 5445 ffaf e668  .u..~...9.TE...h
-00004090: 5ce5 88e6 0827 66f6 f3e6 0827 e67d 0473  \....'f....'.}.s
-000040a0: 84c7 36c7 29e0 11cc 710a 7804 739c 021e  ..6.)...q.x.s...
-000040b0: c11c a780 4730 c729 e0fd e6a8 e155 c0f6  ....G0.).....U..
-000040c0: 5be7 c70f a37a e599 b368 3739 8c3e c45b  [....z...h79.>.[
-000040d0: e9e8 adf3 584e 4f9b e489 7aab 2330 1191  ....XNO...z.#0..
-000040e0: 9803 e545 42d9 aae7 010f 110a 02ee 7944  ...EB.........yD
-000040f0: b884 539f 3dbe b7a6 f296 b3c2 9efd 7bad  ..S.=.........{.
-00004100: d57c 427f d300 cd0f a391 85fa 9637 d552  .|B..........7.R
-00004110: 8e23 e607 2120 98a9 19c6 c405 8261 0ebc  .#..! .......a..
-00004120: 80a2 3971 43c1 a1fa 341c 9352 1cca bccc  ..9qC...4..R....
-00004130: a2fc 5a7d 3bbc 5949 43e1 445a 6a17 b6ba  ..Z};.YIC.DZj...
-00004140: 5206 4516 575b 05ca 33e4 2034 73e8 0c3a  R.E.W[..3. 4s..:
-00004150: 3b45 a91c 8ebf 97b3 516f 515d 6b2d ef2b  ;E......QoQ]k-.+
-00004160: 8e3e 51c5 21ea 532a 420a 229f 40e0 3882  .>Q.!.S*B.".@.8.
-00004170: 8040 841c 40ca 3ca5 b688 6201 1f5f 710b  .@..@.<...b.._q.
-00004180: d9f6 92fb 6b15 b76a ea46 d57d e76b e747  ....k..j.F.}.k.G
-00004190: 5477 5caa dd91 eacb 224f 33eb f5aa 7cf7  Tw\....."O3...|.
-000041a0: 15e1 ec89 12ce 5ce1 8648 598c 10d4 011e  ......\..HY.....
-000041b0: 5127 373c f730 085c 9784 1c05 9e60 e1e3  Q'7<.0.\.....`..
-000041c0: 13de 15a9 9ab3 3b39 ffce 21ee 414e c388  ......;9..!.AN..
-000041d0: 8fc5 dcc1 8007 ea32 0f88 9a72 1c7a 4ae5  .......2...r.zJ.
-000041e0: dcf7 8517 0846 e9d6 693a 4d69 a5b2 3bd4  .....F..i:Mi..;.
-000041f0: 60be 7cfe e7b7 2f9f ff3d 82bb 98db f837  `.|.../..=.....7
-00004200: e638 eba6 3568 4765 cb50 c07d e043 1201  .8..5hGe.P.}.C..
-00004210: 3217 2ef0 22a6 562f c584 043e f702 1c6a  2...".V/...>...j
-00004220: ed34 90dc d68e ea3c 4c3b 4dfd 216b 9b3a  .4.....<L;M.!k.:
-00004230: 37ff f742 6790 cf3a 2efa 03b1 4390 52d1  7..Bg..:....C.R.
-00004240: 4053 af91 5db6 9af8 4b5d bfba 17ed abb8  @S..]...K]......
-00004250: 79b3 3622 29cd fe1e 98ae 460b b30f dd85  y.6").....F.....
-00004260: e8da c73f b8cf fe03 0000 ffff 0300 504b  ...?..........PK
-00004270: 0304 1400 0600 0800 0000 2100 206e d1c5  ..........!. n..
-00004280: 7104 0000 c00f 0000 2200 0000 7070 742f  q......."...ppt/
-00004290: 736c 6964 654c 6179 6f75 7473 2f73 6c69  slideLayouts/sli
-000042a0: 6465 4c61 796f 7574 3130 2e78 6d6c cc57  deLayout10.xml.W
-000042b0: db8e db36 107d 2fd0 7f10 d467 ae2e a464  ...6.}/....g...d
-000042c0: c988 37d0 8d45 8b4d 7651 6ffa ce48 f45a  ..7..E.MvQo..H.Z
-000042d0: 886e a568 c76e b040 7eab fd9c 7c49 8794  .n.h.n.@~...|I..
-000042e0: b4f7 344e e12d f645 a428 f270 66ce 9921  ..4N.-.E.(.pf..!
-000042f0: f5ea f5ae ae8c 2d17 7dd9 360b d339 b14d  ......-.}.6..9.M
-00004300: 8337 795b 94cd d5c2 7c77 4951 601a bd64  .7y[....|wIQ`..d
-00004310: 4dc1 aab6 e10b 73cf 7bf3 f5e9 8f3f bcea  M.....s.{....?..
-00004320: e67d 559c b17d bb91 0660 34fd 9c2d ccb5  .}U..}...`4..-..
-00004330: 94dd dcb2 fa7c cd6b d69f b41d 6fe0 dbaa  .....|.k....o...
-00004340: 1535 93f0 2aae ac42 b08f 805d 5796 6bdb  .5..*..B...]W.k.
-00004350: be55 b3b2 31c7 f5e2 90f5 ed6a 55e6 3c6d  .U..1......jU.<m
-00004360: f34d cd1b 3980 085e 3109 f6f7 ebb2 eb27  .M..9..^1......'
-00004370: b4ee 10b4 4ef0 1e60 f4ea fb26 c97d 07de  ....N..`...&.}..
-00004380: 4260 e4e5 ce34 f43c b185 11c7 3c05 d7f3  B`...4.<....<...
-00004390: 6555 180d ab61 e0b2 9415 3720 40c6 ef30  eU...a....7 @..0
-000043a0: b9cc 5965 5cf2 9dd4 d3fa ee52 70ae 7acd  ..Ye\......Rp.z.
-000043b0: f667 d12d bb0b a157 bfdd 5e08 a32c 14da  .g.-...W..^..,..
-000043c0: 8862 5ae3 8771 9a7e 6db6 ba63 3d58 7e35  .bZ..q.~m..c=X~5
-000043d0: 75d9 7cb7 12b5 6a21 2ac6 6e61 0279 7bf5  u.|...j!*.na.y{.
-000043e0: b4d4 1818 61e4 c360 7e3b 9aaf cf9f 989b  ....a..`~;......
-000043f0: afb3 2766 5bd3 06d6 9d4d 9557 8371 8fdd  ..'f[....M.W.q..
-00004400: 7127 7786 a0a8 5869 3bce 7a39 59b4 11e5  q'w...Xi;.z9Y...
-00004410: c2fc 44a9 1b7b 1925 8842 0f11 3b26 28ce  ..D..{.%.B..;&(.
-00004420: 4888 a88b 83cc 9dd1 c4c5 feb5 5aed f8f3  H...........Z...
-00004430: 5c70 cdcf 2fc5 a433 c77f c46d 5de6 a2ed  \p../..3...m]...
-00004440: db95 3cc9 db7a 14c9 a435 a0d5 2123 adca  ..<..z...5..!#..
-00004450: ca4f 4980 b19f 7819 8add c046 d427 36c2  .OI...x....F.'6.
-00004460: 4934 4338 cc08 c6a9 97fa eeec 7a0c 00d8  I4C8........z...
-00004470: 3cb5 da0b 6bf4 7774 7c22 a2ef ceda fc43  <...k.wt|".....C
-00004480: 6f34 2d10 a578 1d78 bb99 3190 a9da 6e3d  o4-..x.x..1...n=
-00004490: 6a4b aa18 8df3 868f ba73 1be5 5105 7217  jK.......s..Q.r.
-000044a0: b7c5 5e6d f21e 5a3d c8e6 552f 9772 5f71  ..^m..Z=..U/.r_q
-000044b0: fdd2 a987 3643 0011 1553 a9cb 1bf4 6e39  ....6C...S....n9
-000044c0: 902b 4f93 aacc 3f18 b235 7851 4ae3 0deb  .+O...?..5xQJ...
-000044d0: 2517 86de 1f72 1b50 9483 839b 1a85 37c5  %....r.P......7.
-000044e0: 0513 ecb7 bb60 bf5e 8c01 e9b4 9d93 51d6  .....`.^......Q.
-000044f0: 2487 af8b 024f a2b8 971f c645 c572 be6e  $....O.....E.r.n
-00004500: ab02 4c71 5fa8 5048 10b9 b0a5 8f52 db71  ..Lq_.PH.....R.q
-00004510: 511c 608a bc2c 4c51 9a45 b3cc 8e70 84bd  Q.`..,LQ.E...p..
-00004520: ff41 288a 76d3 6845 0995 6a28 49ca bcdd  .A(.v.hE..j(I...
-00004530: ede2 ef51 8faa f580 c299 6263 d0c7 632d  ...Q......bc..c-
-00004540: 758a f96d 7553 1ebe 5f5b 8a41 2dad fe9e  u..muS.._[.A-...
-00004550: b606 fd3c dc45 fbf1 efbb 2c79 de42 89ad  ...<.E....,y.B..
-00004560: f896 5707 20ba df46 bc5c 97e2 7040 fc6d  ..W. ..F.\..p@.m
-00004570: 40da 6e84 5c1f 8c48 0e40 2c57 4f02 1e3b  @.n.\..H.@,WO..;
-00004580: 43c9 94a1 2993 fc5e 62e2 179a 98a1 9764  C...)..^b......d
-00004590: 1971 3de4 468e 83dc 9866 288b 2307 d9d8  .q=.F....f(.#...
-000045a0: c671 98d1 d4a6 d1f3 2766 0189 d8ff 099e  .q......'f......
-000045b0: b06a 35a5 e470 701e a5a2 afe0 8ea1 bdf5  .j5..pp.........
-000045c0: a0f0 f871 9221 827d 8830 2633 14fa 3840  ...q.!.}.0&3..8@
-000045d0: 51e2 b929 9965 61e0 24d7 d395 a500 0e65  Q..).ea.$......e
-000045e0: 5973 5a5e 6d04 3fdf a89b c803 8581 528c  YsZ^m.?.......R.
-000045f0: be96 49c5 5973 93e3 f2d4 b55d d7b2 3dcb  ..I.Ys.....]..=.
-00004600: b16f d506 361c 5f6f dea4 37da b6aa 5adc  .o..6._o..7...Z.
-00004610: 551c 79a1 8a73 74b0 7d8a 629a 4488 2671  U.y..st.}.b.D.&q
-00004620: 8c1c 0a87 0249 1d0c f28b 6990 79cf afb8  .....I....i.y...
-00004630: 9514 83e4 fed8 3001 a19b 54f7 5f4e 82af  ......0...T._N..
-00004640: a8ee b854 fb13 d5cb aa2c b8f1 7653 bf7f  ...T.....,..vS..
-00004650: 40b8 f742 098f bccc 7783 c447 5188 3314  @..B....w..GQ.3.
-00004660: 454e 0275 2624 2801 ee69 90ce 7c9a e1e7  EN.u&$(..i..|...
-00004670: 271c feb1 2066 4f72 aecf b823 571a 9fc4  '... fOr...#W...
-00004680: 384c 6d8c 8204 1e69 4220 e438 8b90 e305  8Lm....iB .8....
-00004690: 711c 4649 e87b de4d a5e9 15a5 0d58 7768  q.FI.{.M.....Xwh
-000046a0: 81f9 f2f9 af9f be7c fefb 08d5 4537 d3bf  .......|....E7..
-000046b0: d514 75dd 1bb5 03d6 fa6e 12c4 2876 0885  ..u......n..(v..
-000046c0: 240d 6728 a2be 87a8 8709 49e2 204a 70a6  $.g(......I. Jp.
-000046d0: b4d3 39e4 b176 60f0 30ed 74ed 472e bab6  ..9..v`.0.t.G...
-000046e0: d43f a28e 3dca 67cb d40d 64e6 9260 466c  .?..=.g...d..`Fl
-000046f0: 47df 1c2c 6ddb d4de 6864 a9fc 87b6 126f  G..,m...hd.....o
-00004700: 5877 bed5 22a9 f50d 2ad1 439d 12e6 30f5  Xw.."...*.C...0.
-00004710: 768a f27d faf3 3efd 0700 00ff ff03 0050  v..}..>........P
-00004720: 4b03 0414 0006 0008 0000 0021 00e9 c94b  K..........!...K
-00004730: 50a6 0400 00a0 1000 0022 0000 0070 7074  P........"...ppt
-00004740: 2f73 6c69 6465 4c61 796f 7574 732f 736c  /slideLayouts/sl
-00004750: 6964 654c 6179 6f75 7431 312e 786d 6ccc  ideLayout11.xml.
-00004760: 58db 6edc 3610 7d2f d07f 10d4 675a 122f  X.n.6.}/....gZ./
-00004770: ba18 5907 ba16 0d9c c4e8 3a7d 5724 ae57  ..Y.......:}W$.W
-00004780: 886e a5b8 9b75 8300 f9ad f673 f225 1d52  .n...u.....s.%.R
-00004790: 921d af9d 780d d881 5f96 1435 1c9e 9973  ....x..._..5...s
-000047a0: 86a4 f6c5 cb5d 531b 5b2e 86aa 6b17 a673  .....]S.[...k..s
-000047b0: 649b 066f 8bae acda 8b85 f9ee 3c43 be69  d..o........<C.i
-000047c0: 0c32 6fcb bcee 5abe 302f f960 be3c f9f5  .2o...Z.0/.`.<..
-000047d0: 9717 fdf1 5097 a7f9 65b7 9106 f868 87e3  ....P...e....h..
-000047e0: 7c61 aea5 ec8f 2d6b 28d6 bcc9 87a3 aee7  |a....-k(.......
-000047f0: 2dbc 5b75 a2c9 253c 8a0b ab14 f947 f0dd  -.[u..%<.....G..
-00004800: d416 b66d d76a f2aa 35a7 f9e2 90f9 dd6a  ...m.j..5......j
-00004810: 5515 3ce9 8a4d c35b 393a 11bc ce25 e01f  U.<..M.[9:...%..
-00004820: d655 3fcc defa 43bc f582 0fe0 46cf be09  .U?...C.....F...
-00004830: 495e f610 2d24 469e 57b2 e661 5b9e ef4c  I^..-$F.W..a[..L
-00004840: 43db 8b2d bc71 cc13 4841 b1ac 4ba3 cd1b  C..-.q..HA..K...
-00004850: 18f8 0b4c ab22 af0d 6d6f 40c6 8c73 be93  ...L."..mo@..s..
-00004860: da6c e8cf 05e7 aad7 6e7f 17fd b23f 137a  .l......n....?.z
-00004870: f69b ed99 30aa 5279 9bbc 98d6 f462 32d3  ....0.Ry.....b2.
-00004880: 8fed 5677 acbd e917 7337 3fde ad44 a35a  ..Vw....s7?..D.Z
-00004890: c88e b15b 9840 e2a5 fab5 d418 8030 8a71  ...[.@.......0.q
-000048a0: b0b8 1e2d d66f efb0 2dd6 e91d d6d6 bc80  ...-.o..-.......
-000048b0: f5cd a22a aa11 dced 70f0 1cce 5e52 54d2  ...*....p...^RT.
-000048c0: 34a0 d341 ced0 36a2 5a98 9fb2 0c47 2ccd  4..A..6.Z....G,.
-000048d0: 28ca a087 a81d 5114 a534 4019 267e 8abd  (.....Q..4@.&~..
-000048e0: 2cc6 c4fd ac66 3bee 7121 b826 ec8f 7216  ,....f;.q!.&..r.
-000048f0: 9ee3 de22 bba9 0ad1 0ddd 4a1e 155d 33a9  ..."......J..]3.
-00004900: 6616 1ff0 ecd0 8967 05f7 9347 9cd0 4903  f......g...G..I.
-00004910: 1ff9 4948 50e0 0680 8362 8040 290d 63cf  ..IHP....b.@).c.
-00004920: 27b1 9b7d 9e32 0198 e756 4761 4d81 4f19  '..}.2...VGaM.O.
-00004930: 9819 19fa d3ae f830 186d 078c 2982 4702  .......0.m..).G.
-00004940: af2c 4656 55db af27 b149 9523 d3e8 4405  .,FVU..'.I.#..D.
-00004950: 921c b537 cd1a 4d75 e73a f977 32ef 7b98  ...7..Mu.:.w2.{.
-00004960: 06f6 c829 7199 83d9 4d11 6017 fbfa bd22  ...)q...M.`...."
-00004970: 97f9 8ee3 137f 9fe2 d175 7f2c 7751 575e  .........u.,wQW^
-00004980: aad9 efa1 056a 15a2 85c9 73c5 eae8 b61e  .....j....s.....
-00004990: e452 5ed6 5c3f f4ea 4783 1260 5ce7 6a07  .R^.\?..G..`\.j.
-000049a0: e12d 7ab7 1c6d e549 5c57 c507 4376 062f  .-z..m.I\W..Cv./
-000049b0: 2b69 bcce 07c9 85a1 a386 2d06 bc28 1463  +i........-..(.c
-000049c0: 72b5 17de 9667 b9c8 fffc d6d9 abb3 096d  r....g.........m
-000049d0: afa1 ce10 35ea 1f6b 92dc d6a4 4aca 599d  ....5..k....J.Y.
-000049e0: 177c ddd5 2540 c1cf 549e 3808 8893 b918  .|..%@..T.8.....
-000049f0: 258c d988 c5b1 0f38 1845 8e93 da09 8b3c  %......8.E.....<
-00004a00: 2708 eca7 97a7 12c1 9e3a 01de ee7a f203  '........:...z..
-00004a10: 544a 7cfc 0391 7a1e a1e4 2945 da2b 496d  TJ|...z...)E.+Im
-00004a20: ebab 6def e1a2 5550 b566 871b a21d 85b9  ..m...UP.f......
-00004a30: bf8a 4ed0 8f57 59f2 a283 13a3 e65b 5e1f  ..N..WY......[^.
-00004a40: e011 dfef f17c 5d89 c31d 92fb 1d66 dd46  .....|]......f.F
-00004a50: c8f5 c11e e901 1eab d59d 0e1f bbf4 e95c  ...............\
-00004a60: fa49 2ef9 8d8a 27cf b4e2 6dd7 8b03 1c46  .I....'...m....F
-00004a70: 087b 9e8f bc2c 25c8 755c 0fb9 c4b3 431f  .{...,%.u\....C.
-00004a80: 6701 633f e140 2aa1 c287 7f20 92bc 5ecd  g.c?.@*.... ..^.
-00004a90: b53e 5e08 be5b ecfa beb2 5f93 dfa9 c215  .>^..[...._.....
-00004aa0: dc9d 74b4 cc27 991b c529 a2c4 850c 13ea  ..t..'...)......
-00004ab0: c119 4c7c 14c6 0c27 d483 83d9 893f cf57  ..L|...'.....?.W
-00004ac0: b212 3894 55c3 b3ea 6223 f8db 8dba 61ed  ..8.U...b#....a.
-00004ad0: 290c 9462 0c8d 8c6b 9eb7 5735 2e4f b08d  )..b...k..W5.O..
-00004ae0: b165 33cb b1af d506 181e 5f6f 6cd6 5bd6  .e3......._ol.[.
-00004af0: 756a b7f8 5671 f499 2a2e b383 d867 418c  uj..Vq..*....gA.
-00004b00: 70c8 304a 6d16 22b8 27d8 2880 5569 10e0  p.0Jm.".'.(.Ui..
-00004b10: 288b 9ca7 57dc 4a8a 5172 7f6f 7201 a99b  (...W.J.Qr.or...
-00004b20: 5577 cf11 f310 d53d 2ed5 ee4c f5b2 ae4a  Uw.....=...L...J
-00004b30: 6ebc d934 eff7 0867 cf94 f034 4813 3721  n..4...g...4H.7!
-00004b40: 2162 7e18 209c c0ee 1267 7102 d4fb b107  !b~. ....gq.....
-00004b50: 2770 4083 9fb0 c5c0 3724 e4ec 4ece f519  'p@.....7$..N...
-00004b60: f7c8 3b8d 4b23 1224 3641 7e0c 3f49 4c21  ..;.K#.$6A~.?IL!
-00004b70: e524 0d91 c3fc 280a c238 7019 bbda 6906  .$....(..8p...i.
-00004b80: 4569 0be8 0edd 60be 7ef9 f7b7 af5f fe7b  Ei....`.~...._.{
-00004b90: 84dd 4537 f337 e39c 75dd 9bb4 0368 5d1c  ..E7.7..u....h].
-00004ba0: fb11 8a1c 9a21 9a04 1e0a 3397 a18c 114a  .....!....3....J
-00004bb0: e3c8 0f63 922a edf4 0ebd ad1d 183c 4c3b  ...c.*.......<L;
-00004bc0: 7df7 918b beab f487 b663 4ff2 d9e6 ea06  }........cO.....
-00004bd0: c2e0 8c62 81e7 eabb 9ba5 b1cd ed95 4696  ...b..........F.
-00004be0: 2a7e 686b f13a efdf 6eb5 481a 7d83 8af5  *~hk.:..n.H.}...
-00004bf0: 50af 8439 9a5e 9ba8 d8e7 7f16 4efe 0700  P..9.^......N...
-00004c00: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00004c10: 0021 00d5 d192 f1bc 0000 0037 0100 002c  .!.........7...,
-00004c20: 0000 0070 7074 2f73 6c69 6465 4c61 796f  ...ppt/slideLayo
-00004c30: 7574 732f 5f72 656c 732f 736c 6964 654c  uts/_rels/slideL
-00004c40: 6179 6f75 7437 2e78 6d6c 2e72 656c 738c  ayout7.xml.rels.
-00004c50: cfbd 0ac2 3010 07f0 5df0 1dc2 ed26 ad83  ....0...]....&..
-00004c60: 8834 7511 c1c1 45f4 018e e4da 06db 24e4  .4u...E.......$.
-00004c70: a2e8 db9b d182 83e3 7dfd fe5c b37f 4da3  ........}..\..M.
-00004c80: 7852 6217 bc86 5a56 20c8 9b60 9def 35dc  xRb...ZV ..`..5.
-00004c90: aec7 d516 0467 f416 c7e0 49c3 9b18 f6ed  .....g....I.....
-00004ca0: 72d1 5c68 c45c 8e78 7091 4551 3c6b 1872  r.\h.\.xp.EQ<k.r
-00004cb0: 8e3b a5d8 0c34 21cb 10c9 9749 17d2 84b9  .;...4!....I....
-00004cc0: 94a9 5711 cd1d 7b52 ebaa daa8 f46d 403b  ..W...{R.....m@;
-00004cd0: 33c5 c96a 4827 5b83 b8be 23fd 6387 ae73  3..jH'[...#.c..s
-00004ce0: 860e c13c 26f2 f947 84e2 d159 3a23 674a  ...<&..G...Y:#gJ
-00004cf0: 85c5 d453 d620 e577 7fb6 54cb 1201 aa6d  ...S. .w..T....m
-00004d00: d4ec ddf6 0300 00ff ff03 0050 4b03 0414  ...........PK...
-00004d10: 0006 0008 0000 0021 00d5 d192 f1bc 0000  .......!........
-00004d20: 0037 0100 002d 0000 0070 7074 2f73 6c69  .7...-...ppt/sli
-00004d30: 6465 4c61 796f 7574 732f 5f72 656c 732f  deLayouts/_rels/
-00004d40: 736c 6964 654c 6179 6f75 7431 312e 786d  slideLayout11.xm
-00004d50: 6c2e 7265 6c73 8ccf bd0a c230 1007 f05d  l.rels.....0...]
-00004d60: f01d c2ed 26ad 8388 3475 11c1 c145 f401  ....&...4u...E..
-00004d70: 8ee4 da06 db24 e4a2 e8db 9bd1 8283 e37d  .....$.........}
-00004d80: fdfe 5cb3 7f4d a378 5262 17bc 865a 5620  ..\..M.xRb...ZV 
-00004d90: c89b 609d ef35 dcae c7d5 1604 67f4 16c7  ..`..5......g...
-00004da0: e049 c39b 18f6 ed72 d15c 68c4 5c8e 7870  .I.....r.\h.\.xp
-00004db0: 9145 513c 6b18 728e 3ba5 d80c 3421 cb10  .EQ<k.r.;...4!..
-00004dc0: c997 4917 d284 b994 a957 11cd 1d7b 52eb  ..I......W...{R.
-00004dd0: aada a8f4 6d40 3b33 c5c9 6a48 275b 83b8  ....m@;3..jH'[..
-00004de0: be23 fd63 87ae 7386 0ec1 3c26 f2f9 4784  .#.c..s...<&..G.
-00004df0: e2d1 593a 2367 4a85 c5d4 53d6 20e5 777f  ..Y:#gJ...S. .w.
-00004e00: b654 cb12 01aa 6dd4 ecdd f603 0000 ffff  .T....m.........
-00004e10: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-00004e20: d5d1 92f1 bc00 0000 3701 0000 2c00 0000  ........7...,...
-00004e30: 7070 742f 736c 6964 654c 6179 6f75 7473  ppt/slideLayouts
-00004e40: 2f5f 7265 6c73 2f73 6c69 6465 4c61 796f  /_rels/slideLayo
-00004e50: 7574 362e 786d 6c2e 7265 6c73 8ccf bd0a  ut6.xml.rels....
-00004e60: c230 1007 f05d f01d c2ed 26ad 8388 3475  .0...]....&...4u
-00004e70: 11c1 c145 f401 8ee4 da06 db24 e4a2 e8db  ...E.......$....
-00004e80: 9bd1 8283 e37d fdfe 5cb3 7f4d a378 5262  .....}..\..M.xRb
-00004e90: 17bc 865a 5620 c89b 609d ef35 dcae c7d5  ...ZV ..`..5....
-00004ea0: 1604 67f4 16c7 e049 c39b 18f6 ed72 d15c  ..g....I.....r.\
-00004eb0: 68c4 5c8e 7870 9145 513c 6b18 728e 3ba5  h.\.xp.EQ<k.r.;.
-00004ec0: d80c 3421 cb10 c997 4917 d284 b994 a957  ..4!....I......W
-00004ed0: 11cd 1d7b 52eb aada a8f4 6d40 3b33 c5c9  ...{R.....m@;3..
-00004ee0: 6a48 275b 83b8 be23 fd63 87ae 7386 0ec1  jH'[...#.c..s...
-00004ef0: 3c26 f2f9 4784 e2d1 593a 2367 4a85 c5d4  <&..G...Y:#gJ...
-00004f00: 53d6 20e5 777f b654 cb12 01aa 6dd4 ecdd  S. .w..T....m...
-00004f10: f603 0000 ffff 0300 504b 0304 1400 0600  ........PK......
-00004f20: 0800 0000 2100 d5d1 92f1 bc00 0000 3701  ....!.........7.
-00004f30: 0000 2d00 0000 7070 742f 736c 6964 654c  ..-...ppt/slideL
-00004f40: 6179 6f75 7473 2f5f 7265 6c73 2f73 6c69  ayouts/_rels/sli
-00004f50: 6465 4c61 796f 7574 3130 2e78 6d6c 2e72  deLayout10.xml.r
-00004f60: 656c 738c cfbd 0ac2 3010 07f0 5df0 1dc2  els.....0...]...
-00004f70: ed26 ad83 8834 7511 c1c1 45f4 018e e4da  .&...4u...E.....
-00004f80: 06db 24e4 a2e8 db9b d182 83e3 7dfd fe5c  ..$.........}..\
-00004f90: b37f 4da3 7852 6217 bc86 5a56 20c8 9b60  ..M.xRb...ZV ..`
-00004fa0: 9def 35dc aec7 d516 0467 f416 c7e0 49c3  ..5......g....I.
-00004fb0: 9b18 f6ed 72d1 5c68 c45c 8e78 7091 4551  ....r.\h.\.xp.EQ
-00004fc0: 3c6b 1872 8e3b a5d8 0c34 21cb 10c9 9749  <k.r.;...4!....I
-00004fd0: 17d2 84b9 94a9 5711 cd1d 7b52 ebaa daa8  ......W...{R....
-00004fe0: f46d 403b 33c5 c96a 4827 5b83 b8be 23fd  .m@;3..jH'[...#.
-00004ff0: 6387 ae73 860e c13c 26f2 f947 84e2 d159  c..s...<&..G...Y
-00005000: 3a23 674a 85c5 d453 d620 e577 7fb6 54cb  :#gJ...S. .w..T.
-00005010: 1201 aa6d d4ec ddf6 0300 00ff ff03 0050  ...m...........P
-00005020: 4b03 0414 0006 0008 0000 0021 00d5 d192  K..........!....
-00005030: f1bc 0000 0037 0100 002c 0000 0070 7074  .....7...,...ppt
-00005040: 2f73 6c69 6465 4c61 796f 7574 732f 5f72  /slideLayouts/_r
-00005050: 656c 732f 736c 6964 654c 6179 6f75 7438  els/slideLayout8
-00005060: 2e78 6d6c 2e72 656c 738c cfbd 0ac2 3010  .xml.rels.....0.
-00005070: 07f0 5df0 1dc2 ed26 ad83 8834 7511 c1c1  ..]....&...4u...
-00005080: 45f4 018e e4da 06db 24e4 a2e8 db9b d182  E.......$.......
-00005090: 83e3 7dfd fe5c b37f 4da3 7852 6217 bc86  ..}..\..M.xRb...
-000050a0: 5a56 20c8 9b60 9def 35dc aec7 d516 0467  ZV ..`..5......g
-000050b0: f416 c7e0 49c3 9b18 f6ed 72d1 5c68 c45c  ....I.....r.\h.\
-000050c0: 8e78 7091 4551 3c6b 1872 8e3b a5d8 0c34  .xp.EQ<k.r.;...4
-000050d0: 21cb 10c9 9749 17d2 84b9 94a9 5711 cd1d  !....I......W...
-000050e0: 7b52 ebaa daa8 f46d 403b 33c5 c96a 4827  {R.....m@;3..jH'
-000050f0: 5b83 b8be 23fd 6387 ae73 860e c13c 26f2  [...#.c..s...<&.
-00005100: f947 84e2 d159 3a23 674a 85c5 d453 d620  .G...Y:#gJ...S. 
-00005110: e577 7fb6 54cb 1201 aa6d d4ec ddf6 0300  .w..T....m......
-00005120: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00005130: 0021 00d5 d192 f1bc 0000 0037 0100 002c  .!.........7...,
-00005140: 0000 0070 7074 2f73 6c69 6465 4c61 796f  ...ppt/slideLayo
-00005150: 7574 732f 5f72 656c 732f 736c 6964 654c  uts/_rels/slideL
-00005160: 6179 6f75 7439 2e78 6d6c 2e72 656c 738c  ayout9.xml.rels.
-00005170: cfbd 0ac2 3010 07f0 5df0 1dc2 ed26 ad83  ....0...]....&..
-00005180: 8834 7511 c1c1 45f4 018e e4da 06db 24e4  .4u...E.......$.
-00005190: a2e8 db9b d182 83e3 7dfd fe5c b37f 4da3  ........}..\..M.
-000051a0: 7852 6217 bc86 5a56 20c8 9b60 9def 35dc  xRb...ZV ..`..5.
-000051b0: aec7 d516 0467 f416 c7e0 49c3 9b18 f6ed  .....g....I.....
-000051c0: 72d1 5c68 c45c 8e78 7091 4551 3c6b 1872  r.\h.\.xp.EQ<k.r
-000051d0: 8e3b a5d8 0c34 21cb 10c9 9749 17d2 84b9  .;...4!....I....
-000051e0: 94a9 5711 cd1d 7b52 ebaa daa8 f46d 403b  ..W...{R.....m@;
-000051f0: 33c5 c96a 4827 5b83 b8be 23fd 6387 ae73  3..jH'[...#.c..s
-00005200: 860e c13c 26f2 f947 84e2 d159 3a23 674a  ...<&..G...Y:#gJ
-00005210: 85c5 d453 d620 e577 7fb6 54cb 1201 aa6d  ...S. .w..T....m
-00005220: d4ec ddf6 0300 00ff ff03 0050 4b03 0414  ...........PK...
-00005230: 0006 0008 0000 0021 00d5 d192 f1bc 0000  .......!........
-00005240: 0037 0100 002c 0000 0070 7074 2f73 6c69  .7...,...ppt/sli
-00005250: 6465 4c61 796f 7574 732f 5f72 656c 732f  deLayouts/_rels/
-00005260: 736c 6964 654c 6179 6f75 7435 2e78 6d6c  slideLayout5.xml
-00005270: 2e72 656c 738c cfbd 0ac2 3010 07f0 5df0  .rels.....0...].
-00005280: 1dc2 ed26 ad83 8834 7511 c1c1 45f4 018e  ...&...4u...E...
-00005290: e4da 06db 24e4 a2e8 db9b d182 83e3 7dfd  ....$.........}.
-000052a0: fe5c b37f 4da3 7852 6217 bc86 5a56 20c8  .\..M.xRb...ZV .
-000052b0: 9b60 9def 35dc aec7 d516 0467 f416 c7e0  .`..5......g....
-000052c0: 49c3 9b18 f6ed 72d1 5c68 c45c 8e78 7091  I.....r.\h.\.xp.
-000052d0: 4551 3c6b 1872 8e3b a5d8 0c34 21cb 10c9  EQ<k.r.;...4!...
-000052e0: 9749 17d2 84b9 94a9 5711 cd1d 7b52 ebaa  .I......W...{R..
-000052f0: daa8 f46d 403b 33c5 c96a 4827 5b83 b8be  ...m@;3..jH'[...
-00005300: 23fd 6387 ae73 860e c13c 26f2 f947 84e2  #.c..s...<&..G..
-00005310: d159 3a23 674a 85c5 d453 d620 e577 7fb6  .Y:#gJ...S. .w..
-00005320: 54cb 1201 aa6d d4ec ddf6 0300 00ff ff03  T....m..........
-00005330: 0050 4b03 0414 0006 0008 0000 0021 0069  .PK..........!.i
-00005340: a25f 2115 0100 00c7 0700 002c 0000 0070  ._!........,...p
-00005350: 7074 2f73 6c69 6465 4d61 7374 6572 732f  pt/slideMasters/
-00005360: 5f72 656c 732f 736c 6964 654d 6173 7465  _rels/slideMaste
-00005370: 7231 2e78 6d6c 2e72 656c 73c4 d54d 6ac3  r1.xml.rels..Mj.
-00005380: 3010 05e0 7da1 7730 b38f 253b 8993 94c8  0...}.w0..%;....
-00005390: d984 42a0 ab92 1e40 58e3 1f6a 4b46 524a  ..B....@X..jKFRJ
-000053a0: 7dfb 8a96 420c 6168 21a0 8dc0 92f5 e6e3  }...B.ah!.......
-000053b0: 6db4 3f7c 0e7d f281 d675 460b c852 0e09  m.?|.}...uF..R..
-000053c0: eaca a84e 3702 dece cf8b 2d24 ce4b ad64  ...N7.....-$.K.d
-000053d0: 6f34 0a98 d0c1 a17c 7cd8 bf62 2f7d b8e4  o4.....||..b/}..
-000053e0: da6e 7449 48d1 4e40 ebfd f8c4 98ab 5a1c  .ntIH.N@......Z.
-000053f0: a44b cd88 3a9c d4c6 0ed2 874f dbb0 5156  .K..:......O..QV
-00005400: efb2 4196 735e 307b 9d01 e52c 3339 2901  ..A.s^0{...,39).
-00005410: f6a4 c2fc f334 e25f b24d 5d77 151e 4d75  .....4._.M]w..Mu
-00005420: 1950 fb1b 2398 eb3b 852f 7232 171f 62a5  .P..#..;./r2..b.
-00005430: 6dd0 0b48 d3eb fdd9 4fdb 348c 0076 5bb6  m..H....O.4..v[.
-00005440: 8c29 5b52 b24d 4cd9 8692 65f9 3d69 3edc  .)[R.ML...e.=i>.
-00005450: c519 ea7b e767 cd28 c75d 19ff 6d28 271b  ...{.g.(.]..m('.
-00005460: 8a29 233b 2b62 ca0a b2b3 b8a5 91ad ad63  .)#;+b.........c
-00005470: d2d6 646b 3c6a 6b9c b2ad 62d2 5694 6c17  ..dk<jk...b.V.l.
-00005480: 53b6 fb95 b1d9 f35b 7e01 0000 ffff 0300  S......[~.......
-00005490: 504b 0304 1400 0600 0800 0000 2100 8d23  PK..........!..#
-000054a0: 2faf 1408 0000 6c36 0000 2100 0000 7070  /.....l6..!...pp
-000054b0: 742f 736c 6964 654d 6173 7465 7273 2f73  t/slideMasters/s
-000054c0: 6c69 6465 4d61 7374 6572 312e 786d 6cec  lideMaster1.xml.
-000054d0: 5afd 6ee3 3612 ffbf c0bd 83a0 fbf3 a0b5  Z.n.6...........
-000054e0: 2891 fa30 d629 acaf 768b 741b 34e9 03d0  (..0.)..v.t.4...
-000054f0: 121d eb22 4baa 44a7 c916 05f6 59fa 16ed  ..."K.D.....Y...
-00005500: e3ec 93dc 9012 6d39 89bd c95d 7270 0223  ......m9...]rp.#
-00005510: 8045 8f46 a3e1 fce6 3743 d279 ffed cdb2  .E.F....7C.y....
-00005520: d0ae 59d3 e655 39d1 d13b 53d7 5899 5659  ..Y..U9..;S.X.VY
-00005530: 5e5e 4ef4 5f2e 12c3 d3b5 96d3 32a3 4555  ^^N._.......2.EU
-00005540: b289 7ecb 5afd db93 7f7c f3be 1eb7 45f6  ..~.Z....|....E.
-00005550: 236d 396b 34b0 51b6 633a d117 9cd7 e3d1  #m9k4.Q.c:......
-00005560: a84d 176c 49db 7755 cd4a b837 af9a 25e5  .M.lI.wU.J.7..%.
-00005570: f0b5 b91c 650d fd0d 6c2f 8b91 659a ce68  ....e...l/..e..h
-00005580: 49f3 52ef 9f6f 1ef3 7c35 9fe7 298b aa74  I.R..o..|5..)..t
-00005590: b564 25ef 8c34 aca0 1cfc 6f17 79dd 2a6b  .d%..4....o.y.*k
-000055a0: f563 acd5 0d6b c18c 7c7a cba5 1398 5f7a  .c...k..|z...._z
-000055b0: 5e64 e23a bbec 3e7f 6673 2dcf 6e20 4aa6  ^d.:..>.fs-.n J.
-000055c0: 8940 838e a565 1616 8d76 4d8b 893e bb44  .@...e...vM..>.D
-000055d0: fae8 e4fd a857 ee47 e2e1 b6be 6818 13a3  .....W.G....h...
-000055e0: f2fa bba6 3eaf cf1a f986 8fd7 670d d804  ....>.......g...
-000055f0: 93ba 56d2 25c4 5718 9037 7a35 f9b5 bc96  ..V.%.W..7z5....
-00005600: 83d1 9dc7 2fd5 908e 6fe6 cd52 5c21 3c1a  ..../...o..R\!<.
-00005610: 7808 28de 8acf 9190 b11b aea5 9d30 dd48  x.(..........0.H
-00005620: d3c5 4f0f e8a6 8bf8 01ed 917a c168 f052  ..O........z.h.R
-00005630: 31ab ceb9 fbd3 b1d4 742e 725e 30ed aca0  1.......t.r^0...
-00005640: 295b 5445 06b9 d245 0e7c 3a6d b9f2 6ed5  )[TE...E.|:m..n.
-00005650: e413 fdf7 24b1 0212 27d8 4860 6460 33c0  ....$...'.H`d`3.
-00005660: 4610 63df 482c db8b 2d37 092d dbf9 433c  F.c.H,..-7.-..C<
-00005670: 8d9c 71da 3009 da87 4c25 1f72 ee01 becc  ..q.0...L%.r....
-00005680: d3a6 6aab 397f 9756 cb3e 7354 0202 d608  ..j.9..V.>sT....
-00005690: f7e9 273c fe3d 8a83 c8f7 a6be 8131 b810  ..'<.=.......1..
-000056a0: 12d7 3412 14c4 c6d4 4708 c7ae 134d 03f4  ..4.....G....M..
-000056b0: 471f 0cf0 595d e52c 46fd dcfb 2028 50da  G...Y].,F... (P.
-000056c0: fab4 4aaf 5aad ac00 3481 7187 e15a a303  ..J.Z...4.q..Z..
-000056d0: 565c eb85 c66f 6b88 1717 f1ea f5ba 9b72  V\...ok........r
-000056e0: b089 f883 707b b607 a92b 71b4 1d82 2cb2  ....p{...+q...,.
-000056f0: 0d3c 3209 228e 5010 8822 db22 c4b1 b770  .<2.".P.."."...p
-00005700: a5e3 ba69 f977 ac5a 6a62 30d1 1b96 7209  ...i.w.Zjb0...r.
-00005710: 14bd 8619 76aa 4a45 fad4 7952 8ff9 4d50  ....v.JE..yR..MP
-00005720: 65b7 4273 0657 801f 6a09 3cbf a89a 4fba  e.Bs.W..j.<...O.
-00005730: 567c 28db 89ee 238c e1dd 5c7e c1c4 b5e0  V|(...#...\~....
-00005740: 4b33 bc33 dbba c38b b02a 64fe d132 053b  K3.3.....*d..2.;
-00005750: 133d e58d f4a5 04e6 4e57 bc9a e7bd 47dd  .=......NW....G.
-00005760: 2bc5 ada2 e5e7 fcb6 6072 deb5 f890 e206  +.......`r......
-00005770: 1c2a a828 65ac 347e 39ef c2c2 4fc2 224f  .*.(e.4~9...O."O
-00005780: af34 5e69 2ccb b9d6 1731 197a a875 6045  .4^i,....1.z.u`E
-00005790: d8ee 1096 5658 999d d186 fe3c 34f6 c359  ....VX.....<4..Y
-000057a0: 1fc0 5a86 4385 4146 663f 37ec 3537 043e  ..Z.C.AFf?7.57.>
-000057b0: 436a 5807 4a0d 2f42 51ec 24a6 4162 cf33  CjX.J./BQ.$.Ab.3
-000057c0: 6cd7 8c0c 12d9 9181 1dc7 4d82 c80b 4344  l.........M...CD
-000057d0: 5e9e 1a02 6ce1 9048 e8ff 8521 c8b3 88b3  ^...l..H...!....
-000057e0: 9f22 d826 c8b6 bdc3 a7c8 9359 518b 1cbe  .".&.......YQ...
-000057f0: 96cf 4ae1 d359 2222 2649 d26e b1a4 63c2  ..J..Y""&I.n..c.
-00005800: ddb7 48a0 f6bf e59c a555 9969 05bb 66c5  ..H......U.i..f.
-00005810: 232c 5a5f b778 b1c8 9bc7 1b94 8570 bfc1  #,Z_.x.......p..
-00005820: a45a 357c f168 8bf8 1116 f3f9 8306 9fbb  .Z5|.h..........
-00005830: d660 556b 22ca b7db b07d a86d d88a 4ddb  .`Uk"....}.m..M.
-00005840: 092c c3f6 cdd8 303d 736a f881 450c db31  .,....0=sj..E..1
-00005850: dd28 f25c 8b98 e1cb d79a 8cc3 aaf7 13cc  .(.\............
-00005860: 8416 f3be e6c8 c4fb 6f6b 8e63 43c7 2577  ........ok.cC.%w
-00005870: d663 968b 6da9 204a cea6 6fbf a2a6 2ca7  .c..m. J..o...,.
-00005880: a38a 8c1c 5f17 48f0 8016 97b0 9b28 a4b3  ...._.H......(..
-00005890: 199b 8b6c 16e1 4462 ba12 92aa c8b3 242f  ...l..Db......$/
-000058a0: 8a07 56d1 fca6 5b22 f2bc e49d c425 a6a9  ..V...[".....%..
-000058b0: d6a1 6be5 eedb c6ce 48bd 490e 7b47 baf1  ..k.....H.I.{G..
-000058c0: c041 c9d4 7991 75c9 463c 3b71 8230 36b0  .A..y.u.F<;q.06.
-000058d0: ed40 82db d835 7cc7 f68c 6948 ac08 bbb1  .@...5|...iH....
-000058e0: ef21 4836 9513 4021 9e2f 5992 5fae 1af6  .!H6..@!./Y._...
-000058f0: d3aa 8362 8be0 4054 ad5d f2b0 60b4 5c97  ...b..@T.]..`.\.
-00005900: 587e 6299 9635 32c9 0899 1bb2 cfc5 dee2  X~b..52.........
-00005910: b9e9 4e14 dd93 aa12 c57a 4878 7ca0 84c7  ..N......zHx|...
-00005920: 2889 a636 890d 8876 6000 d0b1 e1bb 4162  (..6...v`.....Ab
-00005930: 6077 9a04 2470 7168 fe1f d6dd 73c8 6699  `w..$pqh....s.f.
-00005940: a2bf ae68 03a1 eb49 dfad 929f 427a 6cda  ...h...I....Bzl.
-00005950: 9e5c 47ec 623d 86ed 84f7 9659 af56 eb87  .\G.b=.....Y.V..
-00005960: c7fb e725 9ba3 c876 0ebe 30ed e36a 39bb  ...%...v..0..j9.
-00005970: 4339 72a0 9443 41e2 61c7 f40c 0b11 6c90  C9r..CA.a.....l.
-00005980: c074 0d2f 8a4d c3f4 51ec 0638 72a0 d7be  .t./.M..Q..8r...
-00005990: 3ce5 da22 8398 3dc4 3ab9 807a 5aab 7590  <.."..=.:..zZ.u.
-000059a0: b997 756f bed7 1e2a e7d6 bdd6 c181 ed47  ..uo...*.......G
-000059b0: a66d 7821 7c44 2186 94b7 e3a9 8188 1704  .mx!|D!.........
-000059c0: fe34 f41d 42d6 bdb6 1594 2a21 3b1e db62  .4..B.....*!;..b
-000059d0: bf7c feeb 9f5f 3eff fd0c fd55 5ed4 699d  .|..._>....U^.i.
-000059e0: ca7a 39ea b90b de3a 5608 bd2a 4018 da54  .z9....:V..*@..T
-000059f0: e4bb c634 7188 9110 1be3 30f0 a6a1 1d0b  ...4q.....0.....
-00005a00: eed6 08df e72e 081f c7dd bafa 8d35 7595  .............5u.
-00005a10: cb33 4e64 f6f4 9510 210f c1f6 d432 7dc5  .3Nd....!....2}.
-00005a20: 938e a31b 6f05 f1fa b3cb b468 7ea4 b536  ....o......h~..6
-00005a30: bb44 b01c e308 e27b 03a3 ec0a 46b3 4b4b  .D.....{....F.KK
-00005a40: c82c 21b3 840c 4634 4d59 c941 a31f 2889  .,!...F4MY.A..(.
-00005a50: a524 6b1d 5b49 6c25 c14a 8295 8428 0951  .$k.[Il%.J...(.Q
-00005a60: 1247 49a0 782e 8abc bc82 6088 8bae cdab  .GI.x.....`.....
-00005a70: e2fb 4ea0 46dd 4928 5489 537a 5bad f887  ..N.F.I(T.Sz[...
-00005a80: ac47 6220 e9ce 1a11 76b1 673b d807 ee8c  .Gb ....v.g;....
-00005a90: 85a4 f990 c902 b45b 9708 9e29 5db9 b2df  .......[...)]...
-00005aa0: a38b 06ba 7241 b047 d71a e84a 78f6 e8da  ....rA.G...Jx...
-00005ab0: 035d 598d f6e8 e281 aef3 155d 32d0 75bf  .]Y........]2.u.
-00005ac0: a2eb 0c74 e579 c71e 5d77 a0eb 7f45 d71b  ...t.y..]w...E..
-00005ad0: 6221 59ba 4779 0b38 d53a ee03 cf6f 6469  b!Y.Gy.8.:...odi
-00005ae0: 69e5 581c d6ed dc76 6850 9d2e e8ec fc53  i.X....vhP.....S
-00005af0: 5f61 bbaa 2a4b 2aa3 a765 d05c c913 77f1  _a..*K*..e.\..w.
-00005b00: ab41 d97f 855b 0b28 10d0 2ecf 5665 cac5  .A...[.(....Ve..
-00005b10: 7d69 b93c afd3 aec1 a567 695f 237d 7353  }i.<.....gi_#}sS
-00005b20: 2387 0a81 38f3 df56 5d97 d2f5 ddd9 ea63  #...8..V]......c
-00005b30: 5576 2732 836a dd39 79c5 1af1 23cc 632b  Uv'2.j.9y...#.c+
-00005b40: 776f 7aa8 25a7 248b e81c d621 13fd 5fcb  woz.%.$....!.._.
-00005b50: 7f1b 05ef 7b21 bd73 83d1 fed0 bfbd 7323  ....{!.s......s#
-00005b60: 6d7b db0f 56f9 ede8 d7b2 efdd 8362 499b  m{..V........bI.
-00005b70: 5380 d8ea 16c3 7909 e51c 826a 28c1 e120  S.....y....j(.. 
-00005b80: c5db beaa 0efa de00 aca4 82ce b889 ceb4  ................
-00005b90: c929 785d d3b2 6ae1 ab69 9901 2c3c 305c  .)x]..j..i..,<0\
-00005ba0: d51f 30b5 ce79 ba48 e832 2fc4 6203 04e9  ..0..y.H.2/.b...
-00005bb0: 8236 2de3 eb7e 355b 8520 91e2 89fe e5f3  .6-..~5[. ......
-00005bc0: 9f9d 7490 0e96 dc21 bc44 3a94 bbd2 a1dc  ..t....!.D:.....
-00005bd0: 950e e5fe 7490 436b 03b9 e311 e9fc 2b80  ....t.Ck......+.
-00005be0: 9c1c 12e2 2f56 009e 1171 0173 8fb8 bd41  ..../V...q.s...A
-00005bf0: 1c36 b4b6 88f9 11f2 2742 2e83 76e0 900b  .6......'B..v...
-00005c00: 9c7b c8f1 0072 8057 6ea7 8e90 3f09 72f4  .{...r.Wn...?.r.
-00005c10: 1aea bac0 b987 9c0c 5ab9 495c 09e3 11f2  ........Z.I\....
-00005c20: b707 b9c0 b987 dc19 404e 107e 2dcb b723  ........@N.~-..#
-00005c30: e44f 845c e0dc 43ee 0e20 f7dd cefb 23e4  .O.\..C.. ....#.
-00005c40: 6f0f 7281 730f b9b7 81dc c696 08fa 11f2  o.r.s...........
-00005c50: b708 b9c0 b987 dc1f 40ee 79ce 71f9 f646  ........@.y.q..F
-00005c60: 2117 3877 ff7a ba39 97a9 c715 5fb0 667d  !.8w.z.9...._.f}
-00005c70: 4a03 4f9c 7589 d1cf eefe e1f8 4665 fb48  J.O.u.......Fe.H
-00005c80: e745 92e4 b5c5 f8e1 a30f f903 ce31 3e3b  .E...........1>;
-00005c90: 0f0a 5410 8ef1 d9b1 abb6 5db1 b13e 0668  ..T.......]..>.h
-00005ca0: d71e 1479 9627 bd3f 0668 c78e 4db6 f163  ...y.'.?.h..M..c
-00005cb0: 8076 ef6f d4ff 011c 03b4 6337 00ee 1e8b  .v.o......c7....
-00005cc0: f4be b5b3 43dc 6391 de5e 690e 1797 f23f  ....C.c..^i....?
-00005cd0: 2ad4 0fb5 ddef b8dd bf8e 9ffc 0700 00ff  *...............
-00005ce0: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-00005cf0: 00d5 d192 f1bc 0000 0037 0100 002c 0000  .........7...,..
-00005d00: 0070 7074 2f73 6c69 6465 4c61 796f 7574  .ppt/slideLayout
-00005d10: 732f 5f72 656c 732f 736c 6964 654c 6179  s/_rels/slideLay
-00005d20: 6f75 7434 2e78 6d6c 2e72 656c 738c cfbd  out4.xml.rels...
-00005d30: 0ac2 3010 07f0 5df0 1dc2 ed26 ad83 8834  ..0...]....&...4
-00005d40: 7511 c1c1 45f4 018e e4da 06db 24e4 a2e8  u...E.......$...
-00005d50: db9b d182 83e3 7dfd fe5c b37f 4da3 7852  ......}..\..M.xR
-00005d60: 6217 bc86 5a56 20c8 9b60 9def 35dc aec7  b...ZV ..`..5...
-00005d70: d516 0467 f416 c7e0 49c3 9b18 f6ed 72d1  ...g....I.....r.
-00005d80: 5c68 c45c 8e78 7091 4551 3c6b 1872 8e3b  \h.\.xp.EQ<k.r.;
-00005d90: a5d8 0c34 21cb 10c9 9749 17d2 84b9 94a9  ...4!....I......
-00005da0: 5711 cd1d 7b52 ebaa daa8 f46d 403b 33c5  W...{R.....m@;3.
-00005db0: c96a 4827 5b83 b8be 23fd 6387 ae73 860e  .jH'[...#.c..s..
-00005dc0: c13c 26f2 f947 84e2 d159 3a23 674a 85c5  .<&..G...Y:#gJ..
-00005dd0: d453 d620 e577 7fb6 54cb 1201 aa6d d4ec  .S. .w..T....m..
-00005de0: ddf6 0300 00ff ff03 0050 4b03 0414 0006  .........PK.....
-00005df0: 0008 0000 0021 00d5 d192 f1bc 0000 0037  .....!.........7
-00005e00: 0100 002c 0000 0070 7074 2f73 6c69 6465  ...,...ppt/slide
-00005e10: 4c61 796f 7574 732f 5f72 656c 732f 736c  Layouts/_rels/sl
-00005e20: 6964 654c 6179 6f75 7431 2e78 6d6c 2e72  ideLayout1.xml.r
-00005e30: 656c 738c cfbd 0ac2 3010 07f0 5df0 1dc2  els.....0...]...
-00005e40: ed26 ad83 8834 7511 c1c1 45f4 018e e4da  .&...4u...E.....
-00005e50: 06db 24e4 a2e8 db9b d182 83e3 7dfd fe5c  ..$.........}..\
-00005e60: b37f 4da3 7852 6217 bc86 5a56 20c8 9b60  ..M.xRb...ZV ..`
-00005e70: 9def 35dc aec7 d516 0467 f416 c7e0 49c3  ..5......g....I.
-00005e80: 9b18 f6ed 72d1 5c68 c45c 8e78 7091 4551  ....r.\h.\.xp.EQ
-00005e90: 3c6b 1872 8e3b a5d8 0c34 21cb 10c9 9749  <k.r.;...4!....I
-00005ea0: 17d2 84b9 94a9 5711 cd1d 7b52 ebaa daa8  ......W...{R....
-00005eb0: f46d 403b 33c5 c96a 4827 5b83 b8be 23fd  .m@;3..jH'[...#.
-00005ec0: 6387 ae73 860e c13c 26f2 f947 84e2 d159  c..s...<&..G...Y
-00005ed0: 3a23 674a 85c5 d453 d620 e577 7fb6 54cb  :#gJ...S. .w..T.
-00005ee0: 1201 aa6d d4ec ddf6 0300 00ff ff03 0050  ...m...........P
-00005ef0: 4b03 0414 0006 0008 0000 0021 00d5 d192  K..........!....
-00005f00: f1bc 0000 0037 0100 002c 0000 0070 7074  .....7...,...ppt
-00005f10: 2f73 6c69 6465 4c61 796f 7574 732f 5f72  /slideLayouts/_r
-00005f20: 656c 732f 736c 6964 654c 6179 6f75 7432  els/slideLayout2
-00005f30: 2e78 6d6c 2e72 656c 738c cfbd 0ac2 3010  .xml.rels.....0.
-00005f40: 07f0 5df0 1dc2 ed26 ad83 8834 7511 c1c1  ..]....&...4u...
-00005f50: 45f4 018e e4da 06db 24e4 a2e8 db9b d182  E.......$.......
-00005f60: 83e3 7dfd fe5c b37f 4da3 7852 6217 bc86  ..}..\..M.xRb...
-00005f70: 5a56 20c8 9b60 9def 35dc aec7 d516 0467  ZV ..`..5......g
-00005f80: f416 c7e0 49c3 9b18 f6ed 72d1 5c68 c45c  ....I.....r.\h.\
-00005f90: 8e78 7091 4551 3c6b 1872 8e3b a5d8 0c34  .xp.EQ<k.r.;...4
-00005fa0: 21cb 10c9 9749 17d2 84b9 94a9 5711 cd1d  !....I......W...
-00005fb0: 7b52 ebaa daa8 f46d 403b 33c5 c96a 4827  {R.....m@;3..jH'
-00005fc0: 5b83 b8be 23fd 6387 ae73 860e c13c 26f2  [...#.c..s...<&.
-00005fd0: f947 84e2 d159 3a23 674a 85c5 d453 d620  .G...Y:#gJ...S. 
-00005fe0: e577 7fb6 54cb 1201 aa6d d4ec ddf6 0300  .w..T....m......
-00005ff0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00006000: 0021 00d5 d192 f1bc 0000 0037 0100 002c  .!.........7...,
-00006010: 0000 0070 7074 2f73 6c69 6465 4c61 796f  ...ppt/slideLayo
-00006020: 7574 732f 5f72 656c 732f 736c 6964 654c  uts/_rels/slideL
-00006030: 6179 6f75 7433 2e78 6d6c 2e72 656c 738c  ayout3.xml.rels.
-00006040: cfbd 0ac2 3010 07f0 5df0 1dc2 ed26 ad83  ....0...]....&..
-00006050: 8834 7511 c1c1 45f4 018e e4da 06db 24e4  .4u...E.......$.
-00006060: a2e8 db9b d182 83e3 7dfd fe5c b37f 4da3  ........}..\..M.
-00006070: 7852 6217 bc86 5a56 20c8 9b60 9def 35dc  xRb...ZV ..`..5.
-00006080: aec7 d516 0467 f416 c7e0 49c3 9b18 f6ed  .....g....I.....
-00006090: 72d1 5c68 c45c 8e78 7091 4551 3c6b 1872  r.\h.\.xp.EQ<k.r
-000060a0: 8e3b a5d8 0c34 21cb 10c9 9749 17d2 84b9  .;...4!....I....
-000060b0: 94a9 5711 cd1d 7b52 ebaa daa8 f46d 403b  ..W...{R.....m@;
-000060c0: 33c5 c96a 4827 5b83 b8be 23fd 6387 ae73  3..jH'[...#.c..s
-000060d0: 860e c13c 26f2 f947 84e2 d159 3a23 674a  ...<&..G...Y:#gJ
-000060e0: 85c5 d453 d620 e577 7fb6 54cb 1201 aa6d  ...S. .w..T....m
-000060f0: d4ec ddf6 0300 00ff ff03 0050 4b03 0414  ...........PK...
-00006100: 0006 0008 0000 0021 00b4 cf58 19b9 0000  .......!...X....
-00006110: 0024 0100 002c 0000 0070 7074 2f6e 6f74  .$...,...ppt/not
-00006120: 6573 4d61 7374 6572 732f 5f72 656c 732f  esMasters/_rels/
-00006130: 6e6f 7465 734d 6173 7465 7231 2e78 6d6c  notesMaster1.xml
-00006140: 2e72 656c 738c cfc1 0ac2 300c 06e0 bbe0  .rels.....0.....
-00006150: 3b94 dc6d b71d 4464 ed2e 22ec 2af3 014a  ;..m..Dd..".*..J
-00006160: 9775 c5ad 2d6d 15f7 f616 7671 e0c1 4b20  .u..-m....vq..K 
-00006170: 09ff 1752 37ef 7922 2f0c d138 cba1 a405  ...R7.y"/..8....
-00006180: 10b4 caf5 c66a 0ef7 ee7a 3801 8949 da5e  .....j...z8..I.^
-00006190: 4ece 2287 0523 3462 bfab 6f38 c994 4371  N."..#4b..o8..Cq
-000061a0: 343e 92ac d8c8 614c c99f 198b 6ac4 5946  4>....aL....j.YF
-000061b0: ea3c dabc 195c 9865 ca6d d0cc 4bf5 901a  .<...\.e.m..K...
-000061c0: 5955 1447 16be 0d10 1b93 b43d 87d0 f625  YU.G.......=...%
-000061d0: 906e f1f8 8fed 86c1 28bc 38f5 9cd1 a61f  .n......(.8.....
-000061e0: 2758 ca59 cca0 0c1a 1307 4ad7 c95a 2b9a  'X.Y......J..Z+.
-000061f0: 3d60 a266 9bdf c407 0000 ffff 0300 504b  =`.f..........PK
-00006200: 0304 1400 0600 0800 0000 2100 de2c 26f5  ..........!..,&.
-00006210: b605 0000 8c1d 0000 2100 0000 7070 742f  ........!...ppt/
-00006220: 6e6f 7465 734d 6173 7465 7273 2f6e 6f74  notesMasters/not
-00006230: 6573 4d61 7374 6572 312e 786d 6cec 58ef  esMaster1.xml.X.
-00006240: 6edb 3610 ff3e 60ef 2068 1f07 55ff 65c9  n.6..>`. h..U.e.
-00006250: a853 d84e dc66 48db a04e 1f80 9668 5b30  .S.N.fH..N...h[0
-00006260: 456a 14ed 261d 0af4 b5b6 c7e9 93ec 4891  Ej..&.........H.
-00006270: fe97 2c75 036f 5851 7fb1 4ec7 e391 f7e3  ..,u.oXQ..N.....
-00006280: ef4e 673e 7f71 5b11 6b85 7953 32da b3fd  .Ng>.q[.k.yS2...
-00006290: 679e 6d61 9ab3 a2a4 b39e fdfe 66e4 a4b6  g.ma........f...
-000062a0: d508 440b 4418 c53d fb0e 37f6 8bb3 9f7f  ..D.D..=..7.....
-000062b0: 7a5e 7729 13b8 798d 1a81 b905 5e68 d345  z^w)..y.....^h.E
-000062c0: 3d7b 2e44 dd75 dd26 9fe3 0a35 cf58 8d29  ={.D.u.&...5.X.)
-000062d0: 8c4d 19af 9080 573e 730b 8e3e 80f7 8ab8  .M....W>s..>....
-000062e0: 81e7 256e 854a 6aeb f9fc 90f9 6c3a 2d73  ..%n.Jj.....l:-s
-000062f0: 7cce f265 85a9 689d 704c 9080 089a 7959  |..e..h.pL....yY
-00006300: 37c6 5b7d 88b7 9ae3 06dc a8d9 3b5b 3a83  7.[}........;[:.
-00006310: 08f3 3129 e473 326b 7fdf e1a9 5516 b780  ..1).s2k....U...
-00006320: 93e7 f960 81ba ca33 1e12 6ead 10e9 d993  ...`...3..n.....
-00006330: 996f bb67 cf5d 6dac 2539 b9a9 6f38 c652  .o.g.]m.%9..o8.R
-00006340: a2ab 97bc 1ed7 d75c adf0 6675 cdc1 27b8  .......\..fu..'.
-00006350: b42d 8a2a 4058 3a50 03da 4cbd d295 12dc  .-.*@X:P..L.....
-00006360: bde9 3323 a2ee ed94 57f2 09f0 58b0 4338  ..3#....W...X.C8
-00006370: c73b f9eb 4a1d be15 56de 2af3 8d36 9fbf  .;..J...V.*..6..
-00006380: 7dc0 369f 5f3c 60ed 9a05 dcad 4565 54ed  }.6._<`.....EeT.
-00006390: e6ee 8713 9870 5e61 5400 41ae 09ca f19c  .....p^aT.A.....
-000063a0: 1129 2b8c 94b1 d97c 535f b17c d158 9441  .)+....|S_.|.X.A
-000063b0: 7012 8b36 d6b5 450b 807c d673 4bdc d5e0  p..6..E..|.sK...
-000063c0: 775e 7060 e6c7 9efd fb12 71a0 a09e d2da  w^p`......q.....
-000063d0: 2961 b3c9 c311 0ab2 8e9f 7a3a f228 4e3b  )a........z:.(N;
-000063e0: 69ba 133e ead6 bc11 2f31 ab2c 29f4 6c8e  i..>..../1.,).l.
-000063f0: 73a1 9880 5657 8d68 4d8d 89da 47bb 7add  s...VW.hM...G.z.
-00006400: 15b7 0356 dc49 cb09 3c01 2548 3a98 3f67  ...V.I..<.%H:.?g
-00006410: fca3 6d91 4bda f4ec cc8f 2258 5aa8 9728  ..m.K....."XZ..(
-00006420: ee04 f0c2 b747 263b 2382 0c19 5947 401a  .....G&;#...YG@.
-00006430: 3116 7704 2b79 457c 58d6 4264 0649 4dd4  1.w.+yE|X.Bd.IM.
-00006440: fe0a 3c7d 072a 8998 0f2c d751 69cb 56de  ..<}.*...,.Qi.V.
-00006450: f250 2b50 6871 8d38 92d3 0892 f500 53e7  .P+Phq.8......S.
-00006460: b76b 3db3 56d1 99a8 54a0 8f33 2234 8c38  .k=.V...T..3"4.8
-00006470: 4702 eff0 2138 061f 0a61 ebdc fc66 2684  G...!8...a...f&.
-00006480: 691a 257e f8a3 f081 3f95 0f53 52a8 93fc  i.%~....?..SR...
-00006490: 23cd 82cc f3fd 8193 8451 e0a4 1751 e6a4  #........Q...Q..
-000064a0: 6130 72fc 288b bcfe f979 bf1f 259f 6c73  a0r.(....y..%.ls
-000064b0: 3070 dca2 acf0 a89c 2d39 7ebb 6ce1 e17b  0p......-9~.l..{
-000064c0: a4b2 9a4a 0c09 4674 1d80 380b bc20 70bd  ...J..Ft..8.. p.
-000064d0: d8f5 3db9 1da1 3635 9515 f9d8 d48c 0c35  ..=...65.......5
-000064e0: c7a4 2cb0 7559 a1d9 2e43 c3af 3314 a477  ..,.uY...C..3..w
-000064f0: 4c68 6938 874d e17e 5303 1b0e a36f 438a  Lhi8.M.~S....oC.
-00006500: cb6a a629 ac12 e29b 289c a4b1 a229 b0d4  .j.)....(....)..
-00006510: f7a3 d06b 0f74 c3e3 384a 93c8 f038 f4d2  ...k.t..8J...8..
-00006520: c45f 1ff9 9388 8ce0 eb3f 2a09 69a9 46ad  ._.......?*.i.F.
-00006530: 0f92 451d f0a9 b061 00a3 1c35 6e37 df47  ..E....a...5n7.G
-00006540: c074 a1d7 ddb2 9264 a3ff 5576 5888 e6e0  .t.....d..UvX...
-00006550: a767 e742 7d34 3644 572f ff42 e58b 0dbd  .g.B}46DW/.B....
-00006560: dec8 8e69 8758 d131 4a9f 8468 f75b d8d2  ...i.X.1J..h.[..
-00006570: 48b1 f6a9 3402 08bd 387e 9446 89e7 45ad  H...4...8~.F..E.
-00006580: c577 540f 3787 2c2b 22d4 bbb5 8502 64a7  .wT.7.,+".....d.
-00006590: 2ebd 1f9b 5234 2465 beb0 04b3 7051 0a4b  ....R4$e....pQ.K
-000065a0: 37bd 42c2 d248 a7cd a640 b5b5 b35d 6067  7.B..H...@...]`g
-000065b0: 1575 928f af32 c639 a385 45f0 0a93 033c  .u...2.9..E....<
-000065c0: aa32 f1b8 c79b 79c9 0f77 a808 f3b8 c311  .2....y..w......
-000065d0: 5b72 313f d8a3 e2f7 573c 96d3 071d 1e3b  [r1?....W<.....;
-000065e0: 0b13 9385 23c6 e4e9 6da7 617c 8c34 9c8a  ....#...m.a|.4..
-000065f0: bd8e b4cd 4205 c113 3ad3 1492 31f0 f591  ....B...:...1...
-00006600: fc73 3fd2 f9ff e7df bae2 4ebe 9356 b5b3  .s?.......N..V..
-00006610: db0f bc59 5693 3dc2 24c7 200c 7cf3 c1f5  ...YV.=.$. .|...
-00006620: 439c 517c 7c72 0ffb 2332 e718 4ded 28eb  C.Q||r..#2..M.(.
-00006630: 875e e664 1749 ec0c 92e8 c219 7452 dff1  .^.d.I......tR..
-00006640: 323f 4ccf 333f f0d3 4d53 db48 6250 38bc  2?L.3?..MS.HbP8.
-00006650: 437b d92f 9fff fce5 cbe7 bf8e d0c8 aa87  C{./............
-00006660: b94c 80d3 85c3 d192 b5e4 2504 3218 6449  .L........%.2.dI
-00006670: 304c 07ce c08f 464e 749e 759c fe08 421a  0L....FNt.u...B.
-00006680: c561 140d 0769 7f18 5e7c 92f7 1b7e d4cd  .a...i..^|...~..
-00006690: 3956 571f 9785 b934 f1a3 7bd7 2655 9973  9VW....4..{.&U.s
-000066a0: d6b0 a978 96b3 4adf bfb8 35fb 8079 cd4a  ...x..J...5..y.J
-000066b0: 7505 e37b fa1e 4775 7971 9284 9d38 d1ad  u..{..Guyq...8..
-000066c0: 81da 9a79 aacd cab4 d037 2b39 e1af 516d  ...y.....7+9..Qm
-000066d0: 4d66 3e24 bf80 de59 dc82 542c 409a cc02  Mf>$...Y..T,@...
-000066e0: a90b a42e 903a 9050 9e63 2ac0 420b 4613  .....:.P.c*.B.F.
-000066f0: 18cd da26 349a d068 22a3 898c 2636 9ad8  ...&4..h"...&6..
-00006700: 6812 a381 8fc5 9c94 7401 58c8 876d 4d19  h.......t.X..mM.
-00006710: 79d5 2a8c d456 0075 0976 8f93 15e2 572d  y.*..V.u.v....W-
-00006720: 7f75 59b3 8099 3768 32fe a819 dfb2 5c99  .uY...7h2.....\.
-00006730: 6074 4507 7ca1 fe39 c85b 2caa 5f61 48fe  `tE.|..9.[,._aH.
-00006740: 8b28 e9ec 7a49 dbbf 110f 51dc 5a60 2e6f  .(..zI....Q.Z`.o
-00006750: eea4 7caf f9de bb9e 0270 ef37 dfb0 6bb9  ..|......p.7..k.
-00006760: aa22 f614 2a5c cffe b5a2 0e11 ba7c a0bd  ."..*\.......|..
-00006770: 018c f43d 51b3 3790 37da 77bb c3dd cc53  ...=Q.7.7.w....S
-00006780: 62b0 8146 65fa 091f 0d8a c627 dce0 6340  b..Fe......'..c@
-00006790: 38e1 2341 d1f8 441b 7cfc b0e3 2727 800c  8.#A..D.|...''..
-000067a0: 2a1a a078 0ba0 3448 d5e7 fe04 9044 4503  *..x..4H.....DE.
-000067b0: 946c 000a 8234 91d7 2427 8014 2a1a a0ce  .l...4..$'..*...
-000067c0: 1640 9d28 3cd5 e835 2a1a a074 0390 44e7  .@.(<..5*..t..D.
-000067d0: 54a4 d7a8 6880 b22d 8092 b873 2ad2 6b54  T...h..-...s*.kT
-000067e0: da3f 725b fda2 796d af93 cefe 0600 00ff  .?r[..ym........
-000067f0: ff03 0050 4b03 040a 0000 0000 0000 0021  ...PK..........!
-00006800: 0066 9f93 72be 0800 00be 0800 0017 0000  .f..r...........
-00006810: 0064 6f63 5072 6f70 732f 7468 756d 626e  .docProps/thumbn
-00006820: 6169 6c2e 6a70 6567 ffd8 ffe0 0010 4a46  ail.jpeg......JF
-00006830: 4946 0001 0100 0060 0060 0000 ffe1 0080  IF.....`.`......
-00006840: 4578 6966 0000 4d4d 002a 0000 0008 0004  Exif..MM.*......
-00006850: 011a 0005 0000 0001 0000 003e 011b 0005  ...........>....
-00006860: 0000 0001 0000 0046 0128 0003 0000 0001  .......F.(......
-00006870: 0002 0000 8769 0004 0000 0001 0000 004e  .....i.........N
-00006880: 0000 0000 0000 0060 0000 0001 0000 0060  .......`.......`
-00006890: 0000 0001 0003 a001 0003 0000 0001 0001  ................
-000068a0: 0000 a002 0004 0000 0001 0000 0100 a003  ................
-000068b0: 0004 0000 0001 0000 0090 0000 0000 ffed  ................
-000068c0: 0038 5068 6f74 6f73 686f 7020 332e 3000  .8Photoshop 3.0.
-000068d0: 3842 494d 0404 0000 0000 0000 3842 494d  8BIM........8BIM
-000068e0: 0425 0000 0000 0010 d41d 8cd9 8f00 b204  .%..............
-000068f0: e980 0998 ecf8 427e ffc0 0011 0800 9001  ......B~........
-00006900: 0003 0122 0002 1101 0311 01ff c400 1f00  ..."............
-00006910: 0001 0501 0101 0101 0100 0000 0000 0000  ................
-00006920: 0001 0203 0405 0607 0809 0a0b ffc4 00b5  ................
-00006930: 1000 0201 0303 0204 0305 0504 0400 0001  ................
-00006940: 7d01 0203 0004 1105 1221 3141 0613 5161  }........!1A..Qa
-00006950: 0722 7114 3281 91a1 0823 42b1 c115 52d1  ."q.2....#B...R.
-00006960: f024 3362 7282 090a 1617 1819 1a25 2627  .$3br........%&'
-00006970: 2829 2a34 3536 3738 393a 4344 4546 4748  ()*456789:CDEFGH
-00006980: 494a 5354 5556 5758 595a 6364 6566 6768  IJSTUVWXYZcdefgh
-00006990: 696a 7374 7576 7778 797a 8384 8586 8788  ijstuvwxyz......
-000069a0: 898a 9293 9495 9697 9899 9aa2 a3a4 a5a6  ................
-000069b0: a7a8 a9aa b2b3 b4b5 b6b7 b8b9 bac2 c3c4  ................
-000069c0: c5c6 c7c8 c9ca d2d3 d4d5 d6d7 d8d9 dae1  ................
-000069d0: e2e3 e4e5 e6e7 e8e9 eaf1 f2f3 f4f5 f6f7  ................
-000069e0: f8f9 faff c400 1f01 0003 0101 0101 0101  ................
-000069f0: 0101 0100 0000 0000 0001 0203 0405 0607  ................
-00006a00: 0809 0a0b ffc4 00b5 1100 0201 0204 0403  ................
-00006a10: 0407 0504 0400 0102 7700 0102 0311 0405  ........w.......
-00006a20: 2131 0612 4151 0761 7113 2232 8108 1442  !1..AQ.aq."2...B
-00006a30: 91a1 b1c1 0923 3352 f015 6272 d10a 1624  .....#3R..br...$
-00006a40: 34e1 25f1 1718 191a 2627 2829 2a35 3637  4.%.....&'()*567
-00006a50: 3839 3a43 4445 4647 4849 4a53 5455 5657  89:CDEFGHIJSTUVW
-00006a60: 5859 5a63 6465 6667 6869 6a73 7475 7677  XYZcdefghijstuvw
-00006a70: 7879 7a82 8384 8586 8788 898a 9293 9495  xyz.............
-00006a80: 9697 9899 9aa2 a3a4 a5a6 a7a8 a9aa b2b3  ................
-00006a90: b4b5 b6b7 b8b9 bac2 c3c4 c5c6 c7c8 c9ca  ................
-00006aa0: d2d3 d4d5 d6d7 d8d9 dae2 e3e4 e5e6 e7e8  ................
-00006ab0: e9ea f2f3 f4f5 f6f7 f8f9 faff db00 4300  ..............C.
-00006ac0: 0202 0202 0202 0302 0203 0503 0303 0506  ................
-00006ad0: 0505 0505 0608 0606 0606 0608 0a08 0808  ................
-00006ae0: 0808 080a 0a0a 0a0a 0a0a 0a0c 0c0c 0c0c  ................
-00006af0: 0c0e 0e0e 0e0e 0f0f 0f0f 0f0f 0f0f 0f0f  ................
-00006b00: ffdb 0043 0102 0202 0404 0407 0404 0710  ...C............
-00006b10: 0b09 0b10 1010 1010 1010 1010 1010 1010  ................
-00006b20: 1010 1010 1010 1010 1010 1010 1010 1010  ................
-00006b30: 1010 1010 1010 1010 1010 1010 1010 1010  ................
-00006b40: 1010 1010 10ff dd00 0400 10ff da00 0c03  ................
-00006b50: 0100 0211 0311 003f 00fd fca2 8a28 00a2  .......?.....(..
-00006b60: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
-00006b70: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
-00006b80: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
-00006b90: 8a28 00a2 8a28 00a2 8a28 03ff d0fd fca2  .(...(...(......
-00006ba0: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
-00006bb0: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
-00006bc0: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
-00006bd0: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 03ff  .(...(...(...(..
-00006be0: d1fd fca2 8a28 00a2 8a28 00a2 8a28 00a2  .....(...(...(..
-00006bf0: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
-00006c00: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
-00006c10: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
-00006c20: 8a28 03ff d2fd fca2 8a28 00a2 8a28 00a2  .(.......(...(..
-00006c30: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
-00006c40: be5d b0fd a974 2bdb d49e 4f08 ebb6 9e1a  .]...t+...O.....
-00006c50: ff00 8482 4f0c 49ae cd15 bad9 26a6 97ad  ....O.I.....&...
-00006c60: 6083 679e 6e1a 192e 1446 2758 8c61 9955  `.g.n....F'X.a.U
-00006c70: 883b b6a5 c7ed 4fe1 fb5b fd56 49bc 25ae  .;....O..[.VI.%.
-00006c80: af86 fc3f ae9f 0eea 7aeb 456c b636 b7bf  ...?....z.El.6..
-00006c90: 695b 456d a67f 3e58 7cc7 40f2 c713 2c7b  i[Em..>X|.@...,{
-00006ca0: be6c 61f6 807d 4745 7c87 a0fe d29e 288e  .la..}GE|.....(.
-00006cb0: 3f8a 3ac7 8cfc 01a9 db68 7f0f 7579 2d4d  ?.:......h..uy-M
-00006cc0: cd99 b49d c59c 5059 cb23 3c31 dd3c af24  ......PY.#<1.<.$
-00006cd0: 693b dc36 c4db e4a8 0332 8287 db3c 05f1  i;.6.....2...<..
-00006ce0: 6fc2 5f12 1b5a bbf0 b4a6 e346 d26e c594  o._..Z.....F.n..
-00006cf0: 5aa6 e8fe c57f 32a0 79be c920 6265 4859  Z.....2.y.. beHY
-00006d00: bcb7 7c05 f303 2a93 b4d0 07a8 515f 28e9  ..|...*.....Q_(.
-00006d10: 3fb4 76a9 65e2 6f8b 4bf1 0bc2 f73a 1784  ?.v.e.o.K....:..
-00006d20: fe1b 4fff 0021 5df6 d22f 90b6 16f7 5878  ..O..!]../....Xx
-00006d30: e2b8 9267 9663 2968 8471 6361 446c 4995  ...g.c)h.qcaDlI.
-00006d40: add8 7f69 5d07 499e fadf e277 86b5 7f87  ...i].I....w....
-00006d50: e6db 45bb f104 2755 5b69 16e7 4eb0 d9f6  ..E...'U[i..N...
-00006d60: a643 673d c6d9 a112 465e 07c4 9f38 da1b  .Cg=....F^...8..
-00006d70: 9c00 7d23 457c b1a9 7ed0 3717 da6e ade1  ..}#E|..~.7..n..
-00006d80: dd5b c2da d781 35cd 4bc3 da9e afa2 3ea6  .[....5.K.....>.
-00006d90: 2d7f d2a3 b284 349b 0db4 f3f9 53c3 e646  -.....4.....S..F
-00006da0: ed0c a15c 0390 0ed6 da7c 38f8 e979 7f67  ...\.....|8..y.g
-00006db0: e09f 0447 a1ea 7e29 d7a6 f0d6 81aa eb37  ...G..~).......7
-00006dc0: 903d a469 6b1e aa86 34b8 916e 2786 4977  .=.ik...4..n'.Iw
-00006dd0: 4914 8d27 928f b40e 7921 4807 d4f4 5145  I..'....y!H...QE
-00006de0: 0014 5145 0014 5145 0014 5145 0014 5145  ..QE..QE..QE..QE
-00006df0: 0014 5145 007f ffd3 fdfc a28a 2800 a28a  ..QE........(...
-00006e00: 2800 a28a 2800 a28a 2800 a28a 2800 a28a  (...(...(...(...
-00006e10: 2803 f3f3 e1b7 c23f 8bde 32f0 d4fe 16f1  (......?..2.....
-00006e20: 36a7 63a7 7814 78ef 56d6 dedd ec67 8b57  6.c.x.x.V....g.W
-00006e30: 68ac 7c43 3df4 16c1 99c4 4619 a68e 397c  h.|C=.....F...9|
-00006e40: fda1 8c4d b154 e449 5178 5fe1 0fc5 bf1f  ...M.T.IQx_.....
-00006e50: d8f8 ff00 c11a aea1 65a5 780b 5cf1 dea7  ........e.x.\...
-00006e60: 7d70 93d9 4e9a a9b5 8351 5b83 15bb 9710  }p..N....Q[.....
-00006e70: bc57 4631 8999 7288 cdb4 3fca 57f4 228a  .WF1..r...?.W.".
-00006e80: 00f9 72fb e11f c58b 3bdf 893a 6f83 7c4b  ..r.....;..:o.|K
-00006e90: a769 5a47 c41b e5d4 12f0 dbca fa9e 9f2c  .iZG...........,
-00006ea0: f05a 59dd 08fe 6f25 f105 bbbc 0c40 db2b  .ZY...o%.....@.+
-00006eb0: aee0 554e e9fe 1e7e cc9e 08f0 6e81 73f0  ..UN...~....n.s.
-00006ec0: df5d d2b4 cf13 f813 49bb 371e 19b1 d4ed  .]......I.7.....
-00006ed0: 12f2 6d26 1b85 0d71 6de6 4e1f 7a09 b73c  ..m&...qm.N.z..<
-00006ee0: 4df7 c2b6 c624 2a9a fa72 8a00 f943 c5ff  M....$*..r...C..
-00006ef0: 00b3 df88 bc57 a87c 52d0 0eb1 6969 e12f  .....W.|R...ii./
-00006f00: 89b6 f04a cc90 bff6 8e9f a8da d9c1 670b  ...J..........g.
-00006f10: 45f3 7932 42bf 668e 5dac 01ce 57a1 c8c9  E.y2B.f.]...W...
-00006f20: f127 ecf7 f10b e320 be6f 8e3a fe99 194f  .'..... .o.:...O
-00006f30: 0f6a 9a0e 9eba 0db4 d188 e4d5 c422 7bf9  .j..........."{.
-00006f40: 4dcb b92e be44 7e5c 23e5 5f9b 73be 463e  M....D~\#._.s.F>
-00006f50: c5a2 803e 4d97 e0c7 c57f 1dea d0eb bf17  ...>M...........
-00006f60: 35ed 1e5b ad0f 45d5 74ad 2d34 8b59 e28e  5..[..E.t.-4.Y..
-00006f70: 4b9d 5a15 826b db9f 3a46 2084 4c24 2990  K.Z..k..:F .L$).
-00006f80: bbdc 976f 9718 5e21 fd9c fc77 addb fc3f  ...o..^!...w...?
-00006f90: d0e1 d434 2b48 3c15 6ba2 c50e b915 a5cc  ...4+H<.k.......
-00006fa0: 7afd ab69 a623 731d acc9 2843 0dd8 8f61  z..i.#s...(C...a
-00006fb0: 57c2 8576 de92 f15f 67d1 4005 1451 4005  W..v..._g.@..Q@.
-00006fc0: 1451 4005 1451 4005 1451 4005 1451 4005  .Q@..Q@..Q@..Q@.
-00006fd0: 1451 401f ffd4 fdfc a28a 2800 a28a 2800  .Q@.......(...(.
-00006fe0: a28a 2800 a28a 2800 a28a 2800 a28a 2800  ..(...(...(...(.
-00006ff0: a28a 2800 a28a 2800 a28a 2800 a28a 2800  ..(...(...(...(.
-00007000: a28a 2800 a28a 2800 a28a 2800 a28a 2800  ..(...(...(...(.
-00007010: a28a 2800 a28a 2803 ffd5 fdfc a28a 2800  ..(...(.......(.
-00007020: a28a 2800 a28a 2800 a28a 2800 a28a 2800  ..(...(...(...(.
-00007030: a28a 2800 a28a 2800 a28a 2800 a28a 2800  ..(...(...(...(.
-00007040: a28a 2800 a28a 2800 a28a 2800 a28a 2800  ..(...(...(...(.
-00007050: a28a 2800 a28a 2800 a28a 2803 ffd6 fdfc  ..(...(...(.....
-00007060: a28a 2800 a28a 2800 a28a 2800 a28a 2800  ..(...(...(...(.
-00007070: a28a 2800 a28a 2800 a28a 2800 a28a 2800  ..(...(...(...(.
-00007080: a28a 2800 a28a 2800 a28a 2800 a28a 2800  ..(...(...(...(.
-00007090: a28a 2800 a28a 2800 a28a 2800 a28a 2803  ..(...(...(...(.
-000070a0: ffd7 fdfc a28a 2800 a28a 2800 a28a 2800  ......(...(...(.
-000070b0: a28a 2800 a28a 2800 a28a 2800 a28a 2800  ..(...(...(...(.
-000070c0: a28a 2800 a28a 2800 a28a 2800 a28a 2800  ..(...(...(...(.
-000070d0: a28a 2800 a28a 2800 a28a 2800 a28a 2800  ..(...(...(...(.
-000070e0: a28a 2803 ffd9 504b 0304 1400 0600 0800  ..(...PK........
-000070f0: 0000 2100 7b43 bc5d c406 0000 cf20 0000  ..!.{C.]..... ..
-00007100: 1400 0000 7070 742f 7468 656d 652f 7468  ....ppt/theme/th
-00007110: 656d 6532 2e78 6d6c ec59 cd8b 1b37 14bf  eme2.xml.Y...7..
-00007120: 17fa 3f0c 7377 fc35 e38f 1027 d863 3b9b  ..?.sw.5...'.c;.
-00007130: 6437 59b2 9b94 1cb5 b63c a358 3332 92bc  d7Y......<.X32..
-00007140: 1b13 0225 39f5 5228 a4a5 9742 6f3d 94d2  ...%9.R(...Bo=..
-00007150: 4003 0dbd f48f 0924 b4e9 1fd1 278d ed19  @......$....'...
-00007160: d99a e66b 1302 5d2f d892 e6f7 9e7e 7aef  ...k..]/.....~z.
-00007170: e9e9 ade6 c2a5 7b31 758e 3117 8425 1db7  ......{1u.1..%..
-00007180: 7aae e23a 3819 b131 49c2 8e7b eb70 586a  z..:8..1I..{.pXj
-00007190: b98e 9028 1923 ca12 dc71 1758 b897 2e7e  ...(.#...q.X...~
-000071a0: fed9 0574 5e46 38c6 0ec8 27e2 3cea b891  ...t^F8...'.<...
-000071b0: 94b3 f3e5 b218 c130 12e7 d80c 27f0 6cc2  .......0....'.l.
-000071c0: 788c 2474 7958 1e73 7402 7a63 5aae 552a  x.$tyX.st.zcZ.U*
-000071d0: 8d72 8c48 e23a 098a 41ed 8dc9 848c b073  .r.H.:..A......s
-000071e0: a854 ba17 57ca 0714 be12 29d4 c088 f203  .T..W.....).....
-000071f0: a51a 1b12 1a3b 9e56 d58f 5888 8072 e718  .....;.V..X..r..
-00007200: d18e 0bf3 8cd9 c921 be27 5d87 2221 e141  .......!.']."!.A
-00007210: c7ad e88f 5bbe 78a1 bc16 a2b2 4036 2737  ....[.x.....@6'7
-00007220: d49f a5dc 5260 3cad 6939 1e1e ad05 3dcf  ....R`<.i9....=.
-00007230: f71a ddb5 7e0d a072 1b37 680e 1a83 c65a  ....~..r.7h....Z
-00007240: 9f06 a0d1 0856 9a72 3175 366b 81b7 c4e6  .....V.r1u6k....
-00007250: 4069 d3a2 bbdf ecd7 ab06 3ea7 bfbe 85ef  @i........>.....
-00007260: faea cfc0 6b50 daf4 b6f0 c361 90d9 3007  ....kP.....a..0.
-00007270: 4a9b fe16 deef b57b 7d53 bf06 a5cd c616  J......{}S......
-00007280: be59 e9f6 bda6 81d7 a088 9264 ba85 aef8  .Y.........d....
-00007290: 8d7a b05a ed1a 3261 74c7 0a6f fbde b059  .z.Z..2at..o...Y
-000072a0: 5bc2 3354 3917 5da9 7c22 8b62 2d46 7719  [.3T9.].|".b-Fw.
-000072b0: 1f02 403b 1749 9238 7231 c313 3402 5c80  ..@;.I.8r1..4.\.
-000072c0: 2839 e2c4 d925 6104 8137 4309 1330 5ca9  (9...%a..7C..0\.
-000072d0: 5586 953a 7cab 3f4f b7b4 47d1 798c 72d2  U..:|.?O..G.y.r.
-000072e0: e9d0 486c 0d29 3e8e 1871 3293 1df7 2a68  ..Hl.)>..q2...*h
-000072f0: 7573 9017 cf9e 3d7f f8f4 f9c3 df9f 3f7a  us....=.......?z
-00007300: f4fc e1af cbb9 b7e5 7650 12e6 e55e fdf4  ........vP...^..
-00007310: cd3f 3f7c e9fc fddb 8faf 1e7f 6bc7 8b3c  .??|........k..<
-00007320: fee5 2f5f bdfc e3cf ff52 2f0d 5adf 3d79  ../_.....R/.Z.=y
-00007330: f9f4 c98b efbf feeb e7c7 1678 97a3 a33c  ...........x...<
-00007340: fc90 c458 38d7 f189 7393 c5b0 40cb 04f8  ...X8...s...@...
-00007350: 88bf 9dc4 6184 485e a29b 8402 2548 c958  ....a.H^....%H.X
-00007360: d003 1919 e8eb 0b44 9105 d7c3 a61d 6f73  .......D......os
-00007370: 4817 36e0 e5f9 5d83 f041 c4e7 9258 80d7  H.6...]..A...X..
-00007380: a2d8 00ee 3146 7b8c 5bd7 744d cd95 b7c2  ....1F{.[.tM....
-00007390: 3c09 ed93 f379 1e77 13a1 63db dcc1 8697  <....y.w..c.....
-000073a0: 07f3 19c4 3db1 a90c 226c d0dc a7e0 7214  ....=..."l....r.
-000073b0: e204 4b47 3d63 538c 2d62 7708 31ec ba47  ..KG=cS.-bw.1..G
-000073c0: 469c 0936 91ce 1de2 f410 b19a e490 1c19  F..6............
-000073d0: d194 09ed 9018 fcb2 b011 047f 1bb6 d9bb  ................
-000073e0: edf4 18b5 a9ef e363 1309 7b03 519b 4a4c  .......c..{.Q.JL
-000073f0: 0d33 5e46 7389 622b 6314 d33c 7217 c9c8  .3^Fs.b+c..<r...
-00007400: 46f2 60c1 4786 c185 044f 8798 3267 30c6  F.`.G....O..2g0.
-00007410: 42d8 646e f085 41f7 1aa4 19bb dbf7 e822  B.dn..A........"
-00007420: 3691 5c92 a90d b98b 18cb 23fb 6c1a 4428  6.\.......#.l.D(
-00007430: 9e59 3993 24ca 63af 8829 8428 72f6 99b4  .Y9.$.c..).(r...
-00007440: 9260 e60e 517d f003 4a0a dd7d 9b60 c3dd  .`..Q}..J..}.`..
-00007450: afdf dbb7 200d d903 443d 9973 db96 c0cc  .... ...D=.s....
-00007460: dc8f 0b3a 41d8 a6bc cb63 23c5 7639 b146  ...:A....c#.v9.F
-00007470: 476f 1e1a a1bd 8b31 4527 688c b173 eb8a  Go.....1E'h..s..
-00007480: 0dcf 6686 cd33 d257 23c8 2a3b d866 9bab  ..f..3.W#.*;.f..
-00007490: c88c 55d5 4fb0 805a 4915 3716 c712 6184  ..U.O..ZI.7...a.
-000074a0: ec01 0e59 019f bdc5 46e2 59a0 2446 bc48  ...Y....F.Y.$F.H
-000074b0: f3f5 a919 3203 38ea 626b bcd2 d1d4 48a5  ....2.8.bk....H.
-000074c0: 84ab 4d6b 2771 43c4 c6fa 0ab5 ee47 c808  ..Mk'qC......G..
-000074d0: 2bd5 17f6 785d 70c3 7f6f b2c7 40e6 ee3b  +...x]p..o..@..;
-000074e0: c8e0 b796 81c4 fec6 b639 44d4 9820 0b98  .........9D.. ..
-000074f0: 4304 5586 2ddd 8288 e1fe 4c44 6d27 2d36  C.U.-.....LDm'-6
-00007500: b7ca 4dcc 4d9b b9a1 bc51 f4c4 2479 6d05  ..M.M....Q..$ym.
-00007510: b451 fbf8 1fa7 f6f9 6055 cfe9 d73b 4529  .Q......`U...;E)
-00007520: 65b3 ca29 c26d d636 01e3 63f2 e997 367d  e..).m.6..c...6}
-00007530: 344f f631 9c26 6795 cd59 65f3 7fac 6c8a  4O.1.&g..Ye...l.
-00007540: f6f3 593d 7356 cf9c d533 1fad 9ec9 4a18  ..Y=sV...3....J.
-00007550: 7d11 b4ba eed1 5ae2 c2bb 9f09 a1f4 402e  }.....Z.......@.
-00007560: 28de 15ba f811 b0f7 c743 18d4 1d2d b4be  (........C...-..
-00007570: 6a9a 45d0 5c4e 67e0 428e 74db e14c 7e41  j.E.\Ng.B.t..L~A
-00007580: 6474 10a1 194c 53d5 3384 62a9 3a14 ce8c  dt...LS.3.b.:...
-00007590: 0928 9ff4 b055 b72e bfe6 f11e 1ba7 a3d5  .(...U..........
-000075a0: eaea 7613 0490 ccc6 a1fc 5a8d 43b1 26d3  ..v.......Z.C.&.
-000075b0: d146 33bb c65b abd7 bd50 5fb7 ae08 28d9  .F3..[...P_...(.
-000075c0: b721 919b cc24 51b7 9068 ae06 5f43 42af  .!...$Q..h.._CB.
-000075d0: ec54 58b4 2d2c 5a4a 7d21 0bfd b3f4 0a1c  .TX.-,ZJ}!......
-000075e0: 4e0e 5217 e3be 9732 8270 8390 1e2b 3fa5  N.R....2.p...+?.
-000075f0: f22b ef9e baa7 8b8c 692e bb66 595e 5b71  .+......i..fY^[q
-00007600: 3d1d 4f1b 2472 e166 92c8 8561 0487 c7e6  =.O.$r.f...a....
-00007610: f029 fbba 9db9 d4a0 a74c b14d a3d9 fa10  .).......L.M....
-00007620: be56 4964 2337 d0c4 ec39 27b0 e7ea 3ea8  .VId#7...9'...>.
-00007630: 19a1 59c7 9dc0 3f4e d08c 67a0 4fa8 4c85  ..Y...?N..g.O.L.
-00007640: 6898 74dc 915c 1afa 5d32 cb8c 0bd9 4722  h.t..\..]2....G"
-00007650: 4a61 fa51 bafe 9848 cc1d 4a62 88f5 bc1b  Ja.Q...H..Jb....
-00007660: 6892 71ab d69a 6a8d 9f28 b976 e5d3 b39c  h.q...j..(.v....
-00007670: fec9 3b19 4f26 7824 0b46 b22e 3c4b 9558  ..;.O&x$.F..<K.X
-00007680: 9fbe 2758 75d8 1c48 1f44 e313 e788 cef9  ..'Xu..H.D......
-00007690: 4d04 86f2 9b55 65c0 3111 726d cd31 e1b9  M....Ue.1.rm.1..
-000076a0: e0ce acb8 91ae 965b d178 eb92 6d51 4467  .......[.x..mQDg
-000076b0: 115a 9e28 f964 9ec2 757b 4d27 b70e cd74  .Z.(.d..u{M'...t
-000076c0: 7355 667f b998 a350 39e9 bd4f ddd7 0b6d  sUf....P9..O...m
-000076d0: 24cd 8203 449d 9af6 fcf1 e10e f91c ab2c  $...D..........,
-000076e0: ef1b acd2 d4bd 99eb daab 5c57 744a bcff  ..........\WtJ..
-000076f0: 8190 a396 4d66 5053 8c2d d48a ce8e 532c  ....MfPS.-....S,
-00007700: 0872 d3ad 43b3 e88c 38ed d360 336a d501  .r..C...8..`3j..
-00007710: b1aa 2b75 6feb f536 3bba 0b91 df87 6a75  ..+uo..6;.....ju
-00007720: 4ea5 482f c8ee 41f9 1dac 5e4c a699 408f  N.H/..A...^L..@.
-00007730: aeb2 cb3d e9cc 39e9 b8f7 2b7e d70b 6a7e  ...=..9...+~..j~
-00007740: 50aa b4fc 41c9 ab7b 9552 cbef d64b 5ddf  P...A..{.R...K].
-00007750: af57 077e b5d2 efd5 1e80 5164 1457 fd74  .W.~......Qd.W.t
-00007760: ee21 fcb3 4f17 cbb7 f77a 7ceb 0d7e bc2a  .!..O....z|..~.*
-00007770: b5cf 8d58 5c66 ba0e 2e6b 61fd 06bf 5a2b  ...X\f...ka...Z+
-00007780: 7e83 ef10 b0cc fd46 6dd8 aeb7 7b8d 52bb  ~......Fm...{.R.
-00007790: de1d 96bc 7eaf 556a 078d 5ea9 df08 9afd  ....~.Uj..^.....
-000077a0: 613f f05b ede1 03d7 39d6 60af 5b0f bcc6  a?.[....9.`.[...
-000077b0: a055 6a54 83a0 e435 2a8a 7eab 5d6a 7ab5  .UjT...5*.~.]jz.
-000077c0: 5ad7 6b76 5b03 affb 6069 6b58 f9ea 7765  Z.kv[...`ikX..we
-000077d0: 5ecd ebe2 bf00 0000 ffff 0300 504b 0304  ^...........PK..
-000077e0: 1400 0600 0800 0000 2100 7b43 bc5d c406  ........!.{C.]..
-000077f0: 0000 cf20 0000 1400 0000 7070 742f 7468  ... ......ppt/th
-00007800: 656d 652f 7468 656d 6531 2e78 6d6c ec59  eme/theme1.xml.Y
-00007810: cd8b 1b37 14bf 17fa 3f0c 7377 fc35 e38f  ...7....?.sw.5..
-00007820: 1027 d863 3b9b 6437 59b2 9b94 1cb5 b63c  .'.c;.d7Y......<
-00007830: a358 3332 92bc 1b13 0225 39f5 5228 a4a5  .X32.....%9.R(..
-00007840: 9742 6f3d 94d2 4003 0dbd f48f 0924 b4e9  .Bo=..@......$..
-00007850: 1fd1 278d ed19 d99a e66b 1302 5d2f d892  ..'......k..]/..
-00007860: e6f7 9e7e 7aef e9e9 ade6 c2a5 7b31 758e  ...~z.......{1u.
-00007870: 3117 8425 1db7 7aae e23a 3819 b131 49c2  1..%..z..:8..1I.
-00007880: 8e7b eb70 586a b98e 9028 1923 ca12 dc71  .{.pXj...(.#...q
-00007890: 1758 b897 2e7e fed9 0574 5e46 38c6 0ec8  .X...~...t^F8...
-000078a0: 27e2 3cea b891 94b3 f3e5 b218 c130 12e7  '.<..........0..
-000078b0: d80c 27f0 6cc2 788c 2474 7958 1e73 7402  ..'.l.x.$tyX.st.
-000078c0: 7a63 5aae 552a 8d72 8c48 e23a 098a 41ed  zcZ.U*.r.H.:..A.
-000078d0: 8dc9 848c b073 a854 ba17 57ca 0714 be12  .....s.T..W.....
-000078e0: 29d4 c088 f203 a51a 1b12 1a3b 9e56 d58f  )..........;.V..
-000078f0: 5888 8072 e718 d18e 0bf3 8cd9 c921 be27  X..r.........!.'
-00007900: 5d87 2221 e141 c7ad e88f 5bbe 78a1 bc16  ]."!.A....[.x...
-00007910: a2b2 4036 2737 d49f a5dc 5260 3cad 6939  ..@6'7....R`<.i9
-00007920: 1e1e ad05 3dcf f71a ddb5 7e0d a072 1b37  ....=.....~..r.7
-00007930: 680e 1a83 c65a 9f06 a0d1 0856 9a72 3175  h....Z.....V.r1u
-00007940: 366b 81b7 c4e6 4069 d3a2 bbdf ecd7 ab06  6k....@i........
-00007950: 3ea7 bfbe 85ef faea cfc0 6b50 daf4 b6f0  >.........kP....
-00007960: c361 90d9 3007 4a9b fe16 deef b57b 7d53  .a..0.J......{}S
-00007970: bf06 a5cd c616 be59 e9f6 bda6 81d7 a088  .......Y........
-00007980: 9264 ba85 aef8 8d7a b05a ed1a 3261 74c7  .d.....z.Z..2at.
-00007990: 0a6f fbde b059 5bc2 3354 3917 5da9 7c22  .o...Y[.3T9.].|"
-000079a0: 8b62 2d46 7719 1f02 403b 1749 9238 7231  .b-Fw...@;.I.8r1
-000079b0: c313 3402 5c80 2839 e2c4 d925 6104 8137  ..4.\.(9...%a..7
-000079c0: 4309 1330 5ca9 5586 953a 7cab 3f4f b7b4  C..0\.U..:|.?O..
-000079d0: 47d1 798c 72d2 e9d0 486c 0d29 3e8e 1871  G.y.r...Hl.)>..q
-000079e0: 3293 1df7 2a68 7573 9017 cf9e 3d7f f8f4  2...*hus....=...
-000079f0: f9c3 df9f 3f7a f4fc e1af cbb9 b7e5 7650  ....?z........vP
-00007a00: 12e6 e55e fdf4 cd3f 3f7c e9fc fddb 8faf  ...^...??|......
-00007a10: 1e7f 6bc7 8b3c fee5 2f5f bdfc e3cf ff52  ..k..<../_.....R
-00007a20: 2f0d 5adf 3d79 f9f4 c98b efbf feeb e7c7  /.Z.=y..........
-00007a30: 1678 97a3 a33c fc90 c458 38d7 f189 7393  .x...<...X8...s.
-00007a40: c5b0 40cb 04f8 88bf 9dc4 6184 485e a29b  ..@.......a.H^..
-00007a50: 8402 2548 c958 d003 1919 e8eb 0b44 9105  ..%H.X.......D..
-00007a60: d7c3 a61d 6f73 4817 36e0 e5f9 5d83 f041  ....osH.6...]..A
-00007a70: c4e7 9258 80d7 a2d8 00ee 3146 7b8c 5bd7  ...X......1F{.[.
-00007a80: 744d cd95 b7c2 3c09 ed93 f379 1e77 13a1  tM....<....y.w..
-00007a90: 63db dcc1 8697 07f3 19c4 3db1 a90c 226c  c.........=..."l
-00007aa0: d0dc a7e0 7214 e204 4b47 3d63 538c 2d62  ....r...KG=cS.-b
-00007ab0: 7708 31ec ba47 469c 0936 91ce 1de2 f410  w.1..GF..6......
-00007ac0: b19a e490 1c19 d194 09ed 9018 fcb2 b011  ................
-00007ad0: 047f 1bb6 d9bb edf4 18b5 a9ef e363 1309  .............c..
-00007ae0: 7b03 519b 4a4c 0d33 5e46 7389 622b 6314  {.Q.JL.3^Fs.b+c.
-00007af0: d33c 7217 c9c8 46f2 60c1 4786 c185 044f  .<r...F.`.G....O
-00007b00: 8798 3267 30c6 42d8 646e f085 41f7 1aa4  ..2g0.B.dn..A...
-00007b10: 19bb dbf7 e822 3691 5c92 a90d b98b 18cb  ....."6.\.......
-00007b20: 23fb 6c1a 4428 9e59 3993 24ca 63af 8829  #.l.D(.Y9.$.c..)
-00007b30: 8428 72f6 99b4 9260 e60e 517d f003 4a0a  .(r....`..Q}..J.
-00007b40: dd7d 9b60 c3dd afdf dbb7 200d d903 443d  .}.`...... ...D=
-00007b50: 9973 db96 c0cc dc8f 0b3a 41d8 a6bc cb63  .s.......:A....c
-00007b60: 23c5 7639 b146 476f 1e1a a1bd 8b31 4527  #.v9.FGo.....1E'
-00007b70: 688c b173 eb8a 0dcf 6686 cd33 d257 23c8  h..s....f..3.W#.
-00007b80: 2a3b d866 9bab c88c 55d5 4fb0 805a 4915  *;.f....U.O..ZI.
-00007b90: 3716 c712 6184 ec01 0e59 019f bdc5 46e2  7...a....Y....F.
-00007ba0: 59a0 2446 bc48 f3f5 a919 3203 38ea 626b  Y.$F.H....2.8.bk
-00007bb0: bcd2 d1d4 48a5 84ab 4d6b 2771 43c4 c6fa  ....H...Mk'qC...
-00007bc0: 0ab5 ee47 c808 2bd5 17f6 785d 70c3 7f6f  ...G..+...x]p..o
-00007bd0: b2c7 40e6 ee3b c8e0 b796 81c4 fec6 b639  ..@..;.........9
-00007be0: 44d4 9820 0b98 4304 5586 2ddd 8288 e1fe  D.. ..C.U.-.....
-00007bf0: 4c44 6d27 2d36 b7ca 4dcc 4d9b b9a1 bc51  LDm'-6..M.M....Q
-00007c00: f4c4 2479 6d05 b451 fbf8 1fa7 f6f9 6055  ..$ym..Q......`U
-00007c10: cfe9 d73b 4529 65b3 ca29 c26d d636 01e3  ...;E)e..).m.6..
-00007c20: 63f2 e997 367d 344f f631 9c26 6795 cd59  c...6}4O.1.&g..Y
-00007c30: 65f3 7fac 6c8a f6f3 593d 7356 cf9c d533  e...l...Y=sV...3
-00007c40: 1fad 9ec9 4a18 7d11 b4ba eed1 5ae2 c2bb  ....J.}.....Z...
-00007c50: 9f09 a1f4 402e 28de 15ba f811 b0f7 c743  ....@.(........C
-00007c60: 18d4 1d2d b4be 6a9a 45d0 5c4e 67e0 428e  ...-..j.E.\Ng.B.
-00007c70: 74db e14c 7e41 6474 10a1 194c 53d5 3384  t..L~Adt...LS.3.
-00007c80: 62a9 3a14 ce8c 0928 9ff4 b055 b72e bfe6  b.:....(...U....
-00007c90: f11e 1ba7 a3d5 eaea 7613 0490 ccc6 a1fc  ........v.......
-00007ca0: 5a8d 43b1 26d3 d146 33bb c65b abd7 bd50  Z.C.&..F3..[...P
-00007cb0: 5fb7 ae08 28d9 b721 919b cc24 51b7 9068  _...(..!...$Q..h
-00007cc0: ae06 5f43 42af ec54 58b4 2d2c 5a4a 7d21  .._CB..TX.-,ZJ}!
-00007cd0: 0bfd b3f4 0a1c 4e0e 5217 e3be 9732 8270  ......N.R....2.p
-00007ce0: 8390 1e2b 3fa5 f22b ef9e baa7 8b8c 692e  ...+?..+......i.
-00007cf0: bb66 595e 5b71 3d1d 4f1b 2472 e166 92c8  .fY^[q=.O.$r.f..
-00007d00: 8561 0487 c7e6 f029 fbba 9db9 d4a0 a74c  .a.....).......L
-00007d10: b14d a3d9 fa10 be56 4964 2337 d0c4 ec39  .M.....VId#7...9
-00007d20: 27b0 e7ea 3ea8 19a1 59c7 9dc0 3f4e d08c  '...>...Y...?N..
-00007d30: 67a0 4fa8 4c85 6898 74dc 915c 1afa 5d32  g.O.L.h.t..\..]2
-00007d40: cb8c 0bd9 4722 4a61 fa51 bafe 9848 cc1d  ....G"Ja.Q...H..
-00007d50: 4a62 88f5 bc1b 6892 71ab d69a 6a8d 9f28  Jb....h.q...j..(
-00007d60: b976 e5d3 b39c fec9 3b19 4f26 7824 0b46  .v......;.O&x$.F
-00007d70: b22e 3c4b 9558 9fbe 2758 75d8 1c48 1f44  ..<K.X..'Xu..H.D
-00007d80: e313 e788 cef9 4d04 86f2 9b55 65c0 3111  ......M....Ue.1.
-00007d90: 726d cd31 e1b9 e0ce acb8 91ae 965b d178  rm.1.........[.x
-00007da0: eb92 6d51 4467 115a 9e28 f964 9ec2 757b  ..mQDg.Z.(.d..u{
-00007db0: 4d27 b70e cd74 7355 667f b998 a350 39e9  M'...tsUf....P9.
-00007dc0: bd4f ddd7 0b6d 24cd 8203 449d 9af6 fcf1  .O...m$...D.....
-00007dd0: e10e f91c ab2c ef1b acd2 d4bd 99eb daab  .....,..........
-00007de0: 5c57 744a bcff 8190 a396 4d66 5053 8c2d  \WtJ......MfPS.-
-00007df0: d48a ce8e 532c 0872 d3ad 43b3 e88c 38ed  ....S,.r..C...8.
-00007e00: d360 336a d501 b1aa 2b75 6feb f536 3bba  .`3j....+uo..6;.
-00007e10: 0b91 df87 6a75 4ea5 482f c8ee 41f9 1dac  ....juN.H/..A...
-00007e20: 5e4c a699 408f aeb2 cb3d e9cc 39e9 b8f7  ^L..@....=..9...
-00007e30: 2b7e d70b 6a7e 50aa b4fc 41c9 ab7b 9552  +~..j~P...A..{.R
-00007e40: cbef d64b 5ddf af57 077e b5d2 efd5 1e80  ...K]..W.~......
-00007e50: 5164 1457 fd74 ee21 fcb3 4f17 cbb7 f77a  Qd.W.t.!..O....z
-00007e60: 7ceb 0d7e bc2a b5cf 8d58 5c66 ba0e 2e6b  |..~.*...X\f...k
-00007e70: 61fd 06bf 5a2b 7e83 ef10 b0cc fd46 6dd8  a...Z+~......Fm.
-00007e80: aeb7 7b8d 52bb de1d 96bc 7eaf 556a 078d  ..{.R.....~.Uj..
-00007e90: 5ea9 df08 9afd 613f f05b ede1 03d7 39d6  ^.....a?.[....9.
-00007ea0: 60af 5b0f bcc6 a055 6a54 83a0 e435 2a8a  `.[....UjT...5*.
-00007eb0: 7eab 5d6a 7ab5 5ad7 6b76 5b03 affb 6069  ~.]jz.Z.kv[...`i
-00007ec0: 6b58 f9ea 7765 5ecd ebe2 bf00 0000 ffff  kX..we^.........
-00007ed0: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
-00007ee0: a364 236b 8d01 0000 3203 0000 1100 0000  .d#k....2.......
-00007ef0: 7070 742f 7072 6573 5072 6f70 732e 786d  ppt/presProps.xm
-00007f00: 6cac d251 6fdb 2010 00e0 f749 fb0f 16ef  l..Qo. ....I....
-00007f10: 0430 368e ad38 951d 1c69 d21e a6aa fd01  .06..8...i......
-00007f20: c8c6 099a 3108 48db a9ea 7f1f 73d2 2add  ....1.H.....s.*.
-00007f30: 34a9 9af6 7420 74c7 7770 9b9b 273d 250f  4...t t.wp..'=%.
-00007f40: d279 65e6 1a90 1506 899c 7b33 a8f9 5083  .ye.......{3..P.
-00007f50: fbbb 3d5c 83c4 0731 0f62 32b3 acc1 0fe9  ..=\...1.b2.....
-00007f60: c1cd f6f3 a78d adac 935e ce41 8498 facd  .........^.A....
-00007f70: 25b1 d0ec 2b51 8363 08b6 42c8 f747 a985  %...+Q.c..B..G..
-00007f80: 5f19 2be7 7836 1aa7 4588 5b77 4083 138f  _.+.x6..E.[w@...
-00007f90: f102 3da1 1463 86b4 5033 b8e4 bb8f e49b  ..=..c..P3......
-00007fa0: 7154 bde4 a63f e908 3817 7172 5a24 fea8  qT...?..8.qrZ$..
-00007fb0: ac7f ad66 3f52 edba 8f77 a46d 6c52 3e85  ...f?R...w.mlR>.
-00007fc0: af3e 5c56 c9c9 a91a 3c77 05db 7565 d640  .>\V....<w..ue.@
-00007fd0: 86e9 0e66 244b 615b 762d 649c d002 6382  ...f$Ka[v-d...c.
-00007fe0: 9bb4 78f9 954d b26a 50be 176e f8a2 c541  ..x..M.jP..n...A
-00007ff0: 7683 0a5c 04f1 8a23 d91f 3cad 7a67 bc19  v..\...#..<.zg..
-00008000: c3aa 37fa d227 b2e6 513a 6bd4 d22a c197  ..7..'..Q:k..*..
-00008010: f77a 1053 0d30 40db 0d5a 70ef 8d9c 9206  .z.S.0@..Zp.....
-00008020: b3b4 8145 b96e 6046 d312 362d e7b0 6d9b  ...E.n`F..6-..m.
-00008030: 75ce 588a 7382 df8c 7214 a729 2c46 6ed5  u.X.s...r..),Fn.
-00008040: 7fe4 d1b4 60c5 df88 7b9e 77fb a6e1 1077  ....`...{.w....w
-00008050: bb0e 6639 ed60 b9a6 0466 ac4d 69db c540  ..f9.`...f.Mi..@
-00008060: b333 31af faa3 70e1 ce89 fe7b 9c9b 5b39  .31...p....{..[9
-00008070: b6c2 cbe1 0d9a ff0b 34bd 8692 6be4 392e  ........4...k.9.
-00008080: df8e 7e1f f3ed 4f00 0000 ffff 0300 504b  ..~...O.......PK
-00008090: 0304 1400 0600 0800 0000 2100 ea15 8dc8  ..........!.....
-000080a0: 7701 0000 1703 0000 1100 0000 7070 742f  w...........ppt/
-000080b0: 7669 6577 5072 6f70 732e 786d 6c8c 52c9  viewProps.xml.R.
-000080c0: 6ec2 3010 bd57 ea3f 58be 9704 0a94 4624  n.0..W.?X.....F$
-000080d0: 5caa f682 d44a d0de 5d67 125c 25b6 e531  \....J..]g.\%..1
-000080e0: 10fa f59d 2c6c 8503 27fb cdf2 e6cd 329d  ....,l..'.....2.
-000080f0: 5565 c136 e050 191d f37e 2fe4 0cb4 34a9  Ue.6.P...~/...4.
-00008100: d279 cc3f 97af 0f13 ced0 0b9d 8ac2 6888  .y.?..........h.
-00008110: f90e 90cf 92fb bba9 8d36 0ab6 1f8e 1181  .........6......
-00008120: c648 c47c e5bd 8d82 00e5 0a4a 813d 6341  .H.|.......J.=cA
-00008130: 932f 33ae 149e a0cb 83d4 892d 1197 4530  ./3........-..E0
-00008140: 08c3 7150 0aa5 7997 ef6e c937 59a6 24bc  ..qP..y..n.7Y.$.
-00008150: 18b9 2e41 fb96 c441 213c 89c7 95b2 b867  ...A...A!<.....g
-00008160: b3b7 b059 0748 344d f699 a484 9ad3 7560  ...Y.H4M......u`
-00008170: f1d5 b458 638a f5c6 413a 87cc 33fc a551  ...Xc...A:..3..Q
-00008180: 8dc6 833e 0f4e 7d4b 631b d7f3 70fc 3cac  ...>.N}Kc...p.<.
-00008190: 5dc1 250f 162a 8523 948b 226d 1143 2dec  ].%..*.#.."m.C-.
-000081a0: d2bc 3995 c69c b6d0 c2f7 ef1f 901e a95c  ..9............\
-000081b0: a34a 76b1 1be1 1652 14b0 b763 0d92 a988  .Jv....R...c....
-000081c0: b062 f51a c321 6769 fd86 b50c 32ef ae98  .b...!gi....2...
-000081d0: 8343 9e8d 8c53 b9d2 ac8a f9e0 71c0 d92e  .C...S......q...
-000081e0: e6a3 f1a4 0bea 8ad6 61f9 9ad4 cfd1 778e  ........a.....w.
-000081f0: 83f8 96ec bc35 6d3c e012 2a7f d2ed c91c  .....5m<..*.....
-00008200: fe29 6e85 9da9 3d9a ae2b 0d1b 9dfb 560e  .)n...=..+....V.
-00008210: dccd d02f 4ae7 34d7 8515 92ce 8f49 4a7e  .../J.4......IJ~
-00008220: a275 d369 cbdd fedb b2b4 379d fc01 0000  .u.i......7.....
-00008230: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00008240: 2100 d8fd 8d8f ac00 0000 b600 0000 1300  !...............
-00008250: 0000 7070 742f 7461 626c 6553 7479 6c65  ..ppt/tableStyle
-00008260: 732e 786d 6c0c cc49 0e82 3018 40e1 bd89  s.xml..I..0.@...
-00008270: 7768 fe7d 2d43 5124 14c2 202b 77ea 012a  wh.}-CQ$.. +w..*
-00008280: 9421 e940 68a3 12e3 dd65 f9f2 922f cd3f  .!.@h....e.../.?
-00008290: 4aa2 9758 ec64 3403 ffe0 0112 ba35 dda4  J..X.d4......5..
-000082a0: 0706 8f7b 8363 40d6 71dd 7169 b460 b00a  ...{.c@.q.qi.`..
-000082b0: 0b79 b6df a53c 714f 7973 ab14 57eb d0a6  .y...<qOys..W...
-000082c0: 689b 7006 a373 7342 886d 47a1 b83d 9859  h.p..ssB.mG..=.Y
-000082d0: e8ed f566 51dc 6db9 0ca4 5bf8 7bd3 9524  ...fQ.m...[.{..$
-000082e0: 81e7 1d89 e293 06d4 899e c137 aa82 20a2  ...........7.. .
-000082f0: b4c0 a7cb e588 6948 035c 7a34 c671 54d6  ......iH.\z4.qT.
-00008300: d5b9 a9fd 2a2c 7e40 b23f 0000 00ff ff03  ....*,~@.?......
-00008310: 0050 4b03 0414 0006 0008 0000 0021 007b  .PK..........!.{
-00008320: 0dc2 2670 0100 00b0 0200 0011 0008 0164  ..&p...........d
-00008330: 6f63 5072 6f70 732f 636f 7265 2e78 6d6c  ocProps/core.xml
-00008340: 20a2 0401 28a0 0001 0000 0000 0000 0000   ...(...........
-00008350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008370: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008380: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008390: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000083a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000083b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000083c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000083d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000083e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000083f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008400: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008410: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008420: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008430: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008440: 0000 0000 0000 0000 9492 414b c330 14c7  ..........AK.0..
-00008450: ef82 dfa1 e4de a5e9 a848 693b 50d9 c981  .........Hi;P...
-00008460: e044 f116 d2b7 2dd8 2621 89eb 76db 4df4  .D....-.&!..v.M.
-00008470: e0c9 bbe0 b710 fc36 2ac3 6f61 dbad dd86  .......6*.oa....
-00008480: bb78 4cfe bff7 cbcb 4ba2 de2c cf9c 2968  .xL.....K..,..)h
-00008490: c3a5 8811 e978 c801 c164 cac5 3846 57c3  .....x...d..8FW.
-000084a0: be7b 8c1c 63a9 4869 2605 c468 0e06 f592  .{..c.Hi&..h....
-000084b0: c383 88a9 9049 0d17 5a2a d096 8371 4a93  .....I..Z*...qJ.
-000084c0: 3021 5331 9a58 ab42 8c0d 9b40 4e4d a724  0!S1.X.B...@NM.$
-000084d0: 4419 8ea4 cea9 2d97 7a8c 1565 7774 0cd8  D.....-.z..ewt..
-000084e0: f7bc 239c 83a5 29b5 1457 4257 b546 b456  ..#...)..WBW.F.V
-000084f0: a6ac 55aa 7b9d d582 9461 c820 0761 0d26  ..U.{....a. .a.&
-00008500: 1d82 37ac 059d 9bbd 0575 b245 e6dc ce15  ..7......u.E....
-00008510: ec45 9bb0 a567 86b7 6051 149d a25b a365  .E...g..`Q...[.e
-00008520: ff04 df0c ce2f ebab ba5c 54b3 6280 9228  ...../...\T.b..(
-00008530: 65a1 e536 8344 293b 73ad 9499 8970 bb59  e..6.D);s....p.Y
-00008540: c54c 03b5 5227 cbd7 b79f 87e7 efc5 e3e7  .L..R'..........
-00008550: 62f1 f5f1 b47c 7fa9 c126 ae26 9d51 6307  b....|...&.&.Qc.
-00008560: e5a3 8c38 a427 f3bd 157f a9aa 50c3 9457  ...8.'......P..W
-00008570: 4f9b 909a 6897 d17a 4eab 5320 75ca fb85  O...h..zN.S u...
-00008580: ab69 34c9 75f7 f46c d847 89ef f9be eb05  .i4.u..l.G......
-00008590: 2ef1 865e 1006 24f4 c86d d5e0 4efd 4698  ...^..$..m..N.F.
-000085a0: af1b f88f b11b 6c19 1b41 5277 bcfb c792  ......l..ARw....
-000085b0: 5f00 0000 ffff 0300 504b 0304 1400 0600  _.......PK......
-000085c0: 0800 0000 2100 7442 f7a4 0d02 0000 0a05  ....!.tB........
-000085d0: 0000 1000 0801 646f 6350 726f 7073 2f61  ......docProps/a
-000085e0: 7070 2e78 6d6c 20a2 0401 28a0 0001 0000  pp.xml ...(.....
-000085f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008600: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008610: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008620: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008630: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008650: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008660: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008670: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00008690: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000086a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000086b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000086c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000086d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000086e0: 0000 0000 0000 0000 0000 0000 0000 a454  ...............T
-000086f0: 4d8f da30 10bd 57ea 7fb0 7287 403f 5085  M..0..W...r.@?P.
-00008700: 4c56 2b56 88c3 d245 22ec 9ebd f184 5875  LV+V...E".....Xu
-00008710: 6ccb 9e52 e8af ef24 de64 a1a0 95b6 cde9  l..R...$.d......
-00008720: cdcc cbf3 f8d9 637e 73a8 35db 830f ca9a  ......c~s.5.....
-00008730: 5932 1e8e 1206 a6b0 5299 dd2c d9e6 8bc1  Y2......R..,....
-00008740: b784 0514 460a 6d0d cc92 2384 e426 fbf8  ....F.m...#..&..
-00008750: 81af bd75 e051 4160 2461 c22c a910 dd34  ...u.QA`$a.,...4
-00008760: 4d43 5141 2dc2 90ca 862a a5f5 b540 0afd  MCQA-....*...@..
-00008770: 2eb5 65a9 0ab8 b3c5 cf1a 0ca6 9f46 a349  ..e..........F.I
-00008780: 0a07 0423 410e 5c2f 9844 c5e9 1eff 5554  ...#A.\/.D....UT
-00008790: daa2 e92f 3ce6 4747 7a19 cf2d 0a9d ab1a  .../<.GGz..-....
-000087a0: b211 4f5f 03fe 64bd 0cd9 78cc d388 f8ad  ..O_..d...x.....
-000087b0: 735a 1502 c98e 6ca5 0a6f 832d 91ad 44a1  sZ....l..o.-..D.
-000087c0: 0cda 50b1 b5fd 057e 6d29 e2e9 2997 fc80  ..P....~m)..)...
-000087d0: 40eb b7d1 a26d 2f7b 5212 42e1 010c 4faf  @....m/{R.B...O.
-000087e0: 94f9 5a78 b1f3 c255 21fb 4c8c d788 6f74  ..Zx...U!.L...ot
-000087f0: f36b 466d bd20 fedd 624c 44c0 974a 4a30  .kFm. ..bLD..JJ0
-00008800: 2f55 dad3 59cc 57ab b956 ae2d 7490 6f0a  /U..Y.W..V.-t.o.
-00008810: a161 4eae 64a5 d001 48ba 4ff0 2588 e6c4  .aN.d...H.O.%...
-00008820: d742 7962 ee71 ba87 02ad 6741 fda6 339f  .Byb.q....gA..3.
-00008830: 24ec 5904 68bc 9c25 7be1 9530 9844 5a0c  $.Y.h..%{..0.DZ.
-00008840: 5aac 5d40 9f2d acc1 c0b6 0124 4ffb 640b  Z.]@.-.....$O.d.
-00008850: 4fb9 a758 7d69 761f c19b c4a8 95d3 4580  O..X}iv.......E.
-00008860: 7768 8fdf a1dd dac7 7285 1ac2 ff2f d106  wh......r..../..
-00008870: ad8f 84cf 1d8e 4b3c 9474 e678 c5f0 afa7  ......K<.t.x....
-00008880: 86b7 3d44 bb63 3bb7 a4af 4fdb ebd1 5c68  ..=D.c;...O...\h
-00008890: f5ec d55b 3576 af76 155e 653c b483 c42e  ...[5v.v.^e<....
-000088a0: 0cee 9173 7818 a0b5 fad2 9c6e 9b7f 6d6c  ...sx......n..ml
-000088b0: 6e6b 27cc 910a 3dba 57e6 47d8 badc de09  nk'...=.W.G.....
-000088c0: 84ee 2a9e 27f9 a612 1e24 8d74 7f55 fb04  ..*.'....$.t.U..
-000088d0: 5f92 295e 37fc 7925 cc0e 64c7 b92c 34c3  _.)^7.y%..d..,4.
-000088e0: fc18 9fb6 6c3c 198e e86b 87b6 cb35 53d9  ....l<...k...5S.
-000088f0: bd39 d91f 0000 00ff ff03 0050 4b01 022d  .9.........PK..-
-00008900: 0014 0006 0008 0000 0021 0034 eee6 6ed7  .........!.4..n.
-00008910: 0100 00dd 0d00 0013 0000 0000 0000 0000  ................
-00008920: 0000 0000 0000 0000 005b 436f 6e74 656e  .........[Conten
-00008930: 745f 5479 7065 735d 2e78 6d6c 504b 0102  t_Types].xmlPK..
-00008940: 2d00 1400 0600 0800 0000 2100 68f8 74a1  -.........!.h.t.
-00008950: 0301 0000 e202 0000 0b00 0000 0000 0000  ................
-00008960: 0000 0000 0000 1004 0000 5f72 656c 732f  .........._rels/
-00008970: 2e72 656c 7350 4b01 022d 0014 0006 0008  .relsPK..-......
-00008980: 0000 0021 00d8 0382 6bd6 0000 00ce 0100  ...!....k.......
-00008990: 0020 0000 0000 0000 0000 0000 0000 0044  . .............D
-000089a0: 0700 0070 7074 2f73 6c69 6465 732f 5f72  ...ppt/slides/_r
-000089b0: 656c 732f 736c 6964 6531 2e78 6d6c 2e72  els/slide1.xml.r
-000089c0: 656c 7350 4b01 022d 0014 0006 0008 0000  elsPK..-........
-000089d0: 0021 00a0 4e0f b6b7 0200 00fc 0600 0015  .!..N...........
-000089e0: 0000 0000 0000 0000 0000 0000 0058 0800  .............X..
-000089f0: 0070 7074 2f73 6c69 6465 732f 736c 6964  .ppt/slides/slid
-00008a00: 6531 2e78 6d6c 504b 0102 2d00 1400 0600  e1.xmlPK..-.....
-00008a10: 0800 0000 2100 3f2d 199e 1a01 0000 6704  ....!.?-......g.
-00008a20: 0000 1f00 0000 0000 0000 0000 0000 0000  ................
-00008a30: 420b 0000 7070 742f 5f72 656c 732f 7072  B...ppt/_rels/pr
-00008a40: 6573 656e 7461 7469 6f6e 2e78 6d6c 2e72  esentation.xml.r
-00008a50: 656c 7350 4b01 022d 0014 0006 0008 0000  elsPK..-........
-00008a60: 0021 0023 cdd5 4546 0200 00ec 0c00 0014  .!.#..EF........
-00008a70: 0000 0000 0000 0000 0000 0000 00a1 0d00  ................
-00008a80: 0070 7074 2f70 7265 7365 6e74 6174 696f  .ppt/presentatio
-00008a90: 6e2e 786d 6c50 4b01 022d 0014 0006 0008  n.xmlPK..-......
-00008aa0: 0000 0021 00c6 9e72 35cf 0200 00eb 0600  ...!...r5.......
-00008ab0: 001f 0000 0000 0000 0000 0000 0000 0019  ................
-00008ac0: 1000 0070 7074 2f6e 6f74 6573 536c 6964  ...ppt/notesSlid
-00008ad0: 6573 2f6e 6f74 6573 536c 6964 6531 2e78  es/notesSlide1.x
-00008ae0: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
-00008af0: 2100 4aaf 7539 d200 0000 bf01 0000 2a00  !.J.u9........*.
-00008b00: 0000 0000 0000 0000 0000 0000 2513 0000  ............%...
-00008b10: 7070 742f 6e6f 7465 7353 6c69 6465 732f  ppt/notesSlides/
-00008b20: 5f72 656c 732f 6e6f 7465 7353 6c69 6465  _rels/notesSlide
-00008b30: 312e 786d 6c2e 7265 6c73 504b 0102 2d00  1.xml.relsPK..-.
-00008b40: 1400 0600 0800 0000 2100 e5a6 61cc 0505  ........!...a...
-00008b50: 0000 7e12 0000 2100 0000 0000 0000 0000  ..~...!.........
-00008b60: 0000 0000 3f14 0000 7070 742f 736c 6964  ....?...ppt/slid
-00008b70: 654c 6179 6f75 7473 2f73 6c69 6465 4c61  eLayouts/slideLa
-00008b80: 796f 7574 312e 786d 6c50 4b01 022d 0014  yout1.xmlPK..-..
-00008b90: 0006 0008 0000 0021 000d c673 aa54 0400  .......!...s.T..
-00008ba0: 0089 0f00 0021 0000 0000 0000 0000 0000  .....!..........
-00008bb0: 0000 0083 1900 0070 7074 2f73 6c69 6465  .......ppt/slide
-00008bc0: 4c61 796f 7574 732f 736c 6964 654c 6179  Layouts/slideLay
-00008bd0: 6f75 7432 2e78 6d6c 504b 0102 2d00 1400  out2.xmlPK..-...
-00008be0: 0600 0800 0000 2100 8408 ff76 3e05 0000  ......!....v>...
-00008bf0: 5e15 0000 2100 0000 0000 0000 0000 0000  ^...!...........
-00008c00: 0000 161e 0000 7070 742f 736c 6964 654c  ......ppt/slideL
-00008c10: 6179 6f75 7473 2f73 6c69 6465 4c61 796f  ayouts/slideLayo
-00008c20: 7574 332e 786d 6c50 4b01 022d 0014 0006  ut3.xmlPK..-....
-00008c30: 0008 0000 0021 00ec 3204 97b5 0400 00c3  .....!..2.......
-00008c40: 1300 0021 0000 0000 0000 0000 0000 0000  ...!............
-00008c50: 0093 2300 0070 7074 2f73 6c69 6465 4c61  ..#..ppt/slideLa
-00008c60: 796f 7574 732f 736c 6964 654c 6179 6f75  youts/slideLayou
-00008c70: 7434 2e78 6d6c 504b 0102 2d00 1400 0600  t4.xmlPK..-.....
-00008c80: 0800 0000 2100 ebed 0a82 1306 0000 551f  ....!.........U.
-00008c90: 0000 2100 0000 0000 0000 0000 0000 0000  ..!.............
-00008ca0: 8728 0000 7070 742f 736c 6964 654c 6179  .(..ppt/slideLay
-00008cb0: 6f75 7473 2f73 6c69 6465 4c61 796f 7574  outs/slideLayout
-00008cc0: 352e 786d 6c50 4b01 022d 0014 0006 0008  5.xmlPK..-......
-00008cd0: 0000 0021 0077 d06c dcdc 0300 0014 0c00  ...!.w.l........
-00008ce0: 0021 0000 0000 0000 0000 0000 0000 00d9  .!..............
-00008cf0: 2e00 0070 7074 2f73 6c69 6465 4c61 796f  ...ppt/slideLayo
-00008d00: 7574 732f 736c 6964 654c 6179 6f75 7436  uts/slideLayout6
-00008d10: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
-00008d20: 0000 2100 45ea e258 8703 0000 f609 0000  ..!.E..X........
-00008d30: 2100 0000 0000 0000 0000 0000 0000 f432  !..............2
-00008d40: 0000 7070 742f 736c 6964 654c 6179 6f75  ..ppt/slideLayou
-00008d50: 7473 2f73 6c69 6465 4c61 796f 7574 372e  ts/slideLayout7.
-00008d60: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
-00008d70: 0021 0033 7ae3 c3b2 0500 0078 1700 0021  .!.3z......x...!
-00008d80: 0000 0000 0000 0000 0000 0000 00ba 3600  ..............6.
-00008d90: 0070 7074 2f73 6c69 6465 4c61 796f 7574  .ppt/slideLayout
-00008da0: 732f 736c 6964 654c 6179 6f75 7438 2e78  s/slideLayout8.x
-00008db0: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
-00008dc0: 2100 67f0 5ac7 8405 0000 2717 0000 2100  !.g.Z.....'...!.
-00008dd0: 0000 0000 0000 0000 0000 0000 ab3c 0000  .............<..
-00008de0: 7070 742f 736c 6964 654c 6179 6f75 7473  ppt/slideLayouts
-00008df0: 2f73 6c69 6465 4c61 796f 7574 392e 786d  /slideLayout9.xm
-00008e00: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-00008e10: 0020 6ed1 c571 0400 00c0 0f00 0022 0000  . n..q......."..
-00008e20: 0000 0000 0000 0000 0000 006e 4200 0070  ...........nB..p
-00008e30: 7074 2f73 6c69 6465 4c61 796f 7574 732f  pt/slideLayouts/
-00008e40: 736c 6964 654c 6179 6f75 7431 302e 786d  slideLayout10.xm
-00008e50: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-00008e60: 00e9 c94b 50a6 0400 00a0 1000 0022 0000  ...KP........"..
-00008e70: 0000 0000 0000 0000 0000 001f 4700 0070  ............G..p
-00008e80: 7074 2f73 6c69 6465 4c61 796f 7574 732f  pt/slideLayouts/
-00008e90: 736c 6964 654c 6179 6f75 7431 312e 786d  slideLayout11.xm
-00008ea0: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-00008eb0: 00d5 d192 f1bc 0000 0037 0100 002c 0000  .........7...,..
-00008ec0: 0000 0000 0000 0000 0000 0005 4c00 0070  ............L..p
-00008ed0: 7074 2f73 6c69 6465 4c61 796f 7574 732f  pt/slideLayouts/
-00008ee0: 5f72 656c 732f 736c 6964 654c 6179 6f75  _rels/slideLayou
-00008ef0: 7437 2e78 6d6c 2e72 656c 7350 4b01 022d  t7.xml.relsPK..-
-00008f00: 0014 0006 0008 0000 0021 00d5 d192 f1bc  .........!......
-00008f10: 0000 0037 0100 002d 0000 0000 0000 0000  ...7...-........
-00008f20: 0000 0000 000b 4d00 0070 7074 2f73 6c69  ......M..ppt/sli
-00008f30: 6465 4c61 796f 7574 732f 5f72 656c 732f  deLayouts/_rels/
-00008f40: 736c 6964 654c 6179 6f75 7431 312e 786d  slideLayout11.xm
-00008f50: 6c2e 7265 6c73 504b 0102 2d00 1400 0600  l.relsPK..-.....
-00008f60: 0800 0000 2100 d5d1 92f1 bc00 0000 3701  ....!.........7.
-00008f70: 0000 2c00 0000 0000 0000 0000 0000 0000  ..,.............
-00008f80: 124e 0000 7070 742f 736c 6964 654c 6179  .N..ppt/slideLay
-00008f90: 6f75 7473 2f5f 7265 6c73 2f73 6c69 6465  outs/_rels/slide
-00008fa0: 4c61 796f 7574 362e 786d 6c2e 7265 6c73  Layout6.xml.rels
-00008fb0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-00008fc0: d5d1 92f1 bc00 0000 3701 0000 2d00 0000  ........7...-...
-00008fd0: 0000 0000 0000 0000 0000 184f 0000 7070  ...........O..pp
-00008fe0: 742f 736c 6964 654c 6179 6f75 7473 2f5f  t/slideLayouts/_
-00008ff0: 7265 6c73 2f73 6c69 6465 4c61 796f 7574  rels/slideLayout
-00009000: 3130 2e78 6d6c 2e72 656c 7350 4b01 022d  10.xml.relsPK..-
-00009010: 0014 0006 0008 0000 0021 00d5 d192 f1bc  .........!......
-00009020: 0000 0037 0100 002c 0000 0000 0000 0000  ...7...,........
-00009030: 0000 0000 001f 5000 0070 7074 2f73 6c69  ......P..ppt/sli
-00009040: 6465 4c61 796f 7574 732f 5f72 656c 732f  deLayouts/_rels/
-00009050: 736c 6964 654c 6179 6f75 7438 2e78 6d6c  slideLayout8.xml
-00009060: 2e72 656c 7350 4b01 022d 0014 0006 0008  .relsPK..-......
-00009070: 0000 0021 00d5 d192 f1bc 0000 0037 0100  ...!.........7..
-00009080: 002c 0000 0000 0000 0000 0000 0000 0025  .,.............%
-00009090: 5100 0070 7074 2f73 6c69 6465 4c61 796f  Q..ppt/slideLayo
-000090a0: 7574 732f 5f72 656c 732f 736c 6964 654c  uts/_rels/slideL
-000090b0: 6179 6f75 7439 2e78 6d6c 2e72 656c 7350  ayout9.xml.relsP
-000090c0: 4b01 022d 0014 0006 0008 0000 0021 00d5  K..-.........!..
-000090d0: d192 f1bc 0000 0037 0100 002c 0000 0000  .......7...,....
-000090e0: 0000 0000 0000 0000 002b 5200 0070 7074  .........+R..ppt
-000090f0: 2f73 6c69 6465 4c61 796f 7574 732f 5f72  /slideLayouts/_r
-00009100: 656c 732f 736c 6964 654c 6179 6f75 7435  els/slideLayout5
-00009110: 2e78 6d6c 2e72 656c 7350 4b01 022d 0014  .xml.relsPK..-..
-00009120: 0006 0008 0000 0021 0069 a25f 2115 0100  .......!.i._!...
-00009130: 00c7 0700 002c 0000 0000 0000 0000 0000  .....,..........
-00009140: 0000 0031 5300 0070 7074 2f73 6c69 6465  ...1S..ppt/slide
-00009150: 4d61 7374 6572 732f 5f72 656c 732f 736c  Masters/_rels/sl
-00009160: 6964 654d 6173 7465 7231 2e78 6d6c 2e72  ideMaster1.xml.r
-00009170: 656c 7350 4b01 022d 0014 0006 0008 0000  elsPK..-........
-00009180: 0021 008d 232f af14 0800 006c 3600 0021  .!..#/.....l6..!
-00009190: 0000 0000 0000 0000 0000 0000 0090 5400  ..............T.
-000091a0: 0070 7074 2f73 6c69 6465 4d61 7374 6572  .ppt/slideMaster
-000091b0: 732f 736c 6964 654d 6173 7465 7231 2e78  s/slideMaster1.x
-000091c0: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
-000091d0: 2100 d5d1 92f1 bc00 0000 3701 0000 2c00  !.........7...,.
-000091e0: 0000 0000 0000 0000 0000 0000 e35c 0000  .............\..
-000091f0: 7070 742f 736c 6964 654c 6179 6f75 7473  ppt/slideLayouts
-00009200: 2f5f 7265 6c73 2f73 6c69 6465 4c61 796f  /_rels/slideLayo
-00009210: 7574 342e 786d 6c2e 7265 6c73 504b 0102  ut4.xml.relsPK..
-00009220: 2d00 1400 0600 0800 0000 2100 d5d1 92f1  -.........!.....
-00009230: bc00 0000 3701 0000 2c00 0000 0000 0000  ....7...,.......
-00009240: 0000 0000 0000 e95d 0000 7070 742f 736c  .......]..ppt/sl
-00009250: 6964 654c 6179 6f75 7473 2f5f 7265 6c73  ideLayouts/_rels
-00009260: 2f73 6c69 6465 4c61 796f 7574 312e 786d  /slideLayout1.xm
-00009270: 6c2e 7265 6c73 504b 0102 2d00 1400 0600  l.relsPK..-.....
-00009280: 0800 0000 2100 d5d1 92f1 bc00 0000 3701  ....!.........7.
-00009290: 0000 2c00 0000 0000 0000 0000 0000 0000  ..,.............
-000092a0: ef5e 0000 7070 742f 736c 6964 654c 6179  .^..ppt/slideLay
-000092b0: 6f75 7473 2f5f 7265 6c73 2f73 6c69 6465  outs/_rels/slide
-000092c0: 4c61 796f 7574 322e 786d 6c2e 7265 6c73  Layout2.xml.rels
-000092d0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
-000092e0: d5d1 92f1 bc00 0000 3701 0000 2c00 0000  ........7...,...
-000092f0: 0000 0000 0000 0000 0000 f55f 0000 7070  ..........._..pp
-00009300: 742f 736c 6964 654c 6179 6f75 7473 2f5f  t/slideLayouts/_
-00009310: 7265 6c73 2f73 6c69 6465 4c61 796f 7574  rels/slideLayout
-00009320: 332e 786d 6c2e 7265 6c73 504b 0102 2d00  3.xml.relsPK..-.
-00009330: 1400 0600 0800 0000 2100 b4cf 5819 b900  ........!...X...
-00009340: 0000 2401 0000 2c00 0000 0000 0000 0000  ..$...,.........
-00009350: 0000 0000 fb60 0000 7070 742f 6e6f 7465  .....`..ppt/note
-00009360: 734d 6173 7465 7273 2f5f 7265 6c73 2f6e  sMasters/_rels/n
-00009370: 6f74 6573 4d61 7374 6572 312e 786d 6c2e  otesMaster1.xml.
-00009380: 7265 6c73 504b 0102 2d00 1400 0600 0800  relsPK..-.......
-00009390: 0000 2100 de2c 26f5 b605 0000 8c1d 0000  ..!..,&.........
-000093a0: 2100 0000 0000 0000 0000 0000 0000 fe61  !..............a
-000093b0: 0000 7070 742f 6e6f 7465 734d 6173 7465  ..ppt/notesMaste
-000093c0: 7273 2f6e 6f74 6573 4d61 7374 6572 312e  rs/notesMaster1.
-000093d0: 786d 6c50 4b01 022d 000a 0000 0000 0000  xmlPK..-........
-000093e0: 0021 0066 9f93 72be 0800 00be 0800 0017  .!.f..r.........
-000093f0: 0000 0000 0000 0000 0000 0000 00f3 6700  ..............g.
-00009400: 0064 6f63 5072 6f70 732f 7468 756d 626e  .docProps/thumbn
-00009410: 6169 6c2e 6a70 6567 504b 0102 2d00 1400  ail.jpegPK..-...
-00009420: 0600 0800 0000 2100 7b43 bc5d c406 0000  ......!.{C.]....
-00009430: cf20 0000 1400 0000 0000 0000 0000 0000  . ..............
-00009440: 0000 e670 0000 7070 742f 7468 656d 652f  ...p..ppt/theme/
-00009450: 7468 656d 6532 2e78 6d6c 504b 0102 2d00  theme2.xmlPK..-.
-00009460: 1400 0600 0800 0000 2100 7b43 bc5d c406  ........!.{C.]..
-00009470: 0000 cf20 0000 1400 0000 0000 0000 0000  ... ............
-00009480: 0000 0000 dc77 0000 7070 742f 7468 656d  .....w..ppt/them
-00009490: 652f 7468 656d 6531 2e78 6d6c 504b 0102  e/theme1.xmlPK..
-000094a0: 2d00 1400 0600 0800 0000 2100 a364 236b  -.........!..d#k
-000094b0: 8d01 0000 3203 0000 1100 0000 0000 0000  ....2...........
-000094c0: 0000 0000 0000 d27e 0000 7070 742f 7072  .......~..ppt/pr
-000094d0: 6573 5072 6f70 732e 786d 6c50 4b01 022d  esProps.xmlPK..-
-000094e0: 0014 0006 0008 0000 0021 00ea 158d c877  .........!.....w
-000094f0: 0100 0017 0300 0011 0000 0000 0000 0000  ................
-00009500: 0000 0000 008e 8000 0070 7074 2f76 6965  .........ppt/vie
-00009510: 7750 726f 7073 2e78 6d6c 504b 0102 2d00  wProps.xmlPK..-.
-00009520: 1400 0600 0800 0000 2100 d8fd 8d8f ac00  ........!.......
-00009530: 0000 b600 0000 1300 0000 0000 0000 0000  ................
-00009540: 0000 0000 3482 0000 7070 742f 7461 626c  ....4...ppt/tabl
-00009550: 6553 7479 6c65 732e 786d 6c50 4b01 022d  eStyles.xmlPK..-
-00009560: 0014 0006 0008 0000 0021 007b 0dc2 2670  .........!.{..&p
-00009570: 0100 00b0 0200 0011 0000 0000 0000 0000  ................
-00009580: 0000 0000 0011 8300 0064 6f63 5072 6f70  .........docProp
-00009590: 732f 636f 7265 2e78 6d6c 504b 0102 2d00  s/core.xmlPK..-.
-000095a0: 1400 0600 0800 0000 2100 7442 f7a4 0d02  ........!.tB....
-000095b0: 0000 0a05 0000 1000 0000 0000 0000 0000  ................
-000095c0: 0000 0000 b885 0000 646f 6350 726f 7073  ........docProps
-000095d0: 2f61 7070 2e78 6d6c 504b 0506 0000 0000  /app.xmlPK......
-000095e0: 2a00 2a00 dd0c 0000 fb88 0000 0000       *.*...........
+00000640: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00000650: 0000 ac92 db4a 0331 1086 ef05 df21 cc7d  .....J.1.....!.}
+00000660: 37db 2a22 d26c 6f44 e89d c8fa 0063 32bb  7.*".loD.....c2.
+00000670: 1bdd 1c48 a6d2 bebd a1e0 6161 2d82 bdcc  ...H......aa-...
+00000680: cc3f 1fdf 2459 6ff6 6e14 ef94 b20d 5ec1  .?..$Yo.n.....^.
+00000690: b2aa 4190 d7c1 58df 2b78 6e1f 16b7 2032  ..A...X.+xn... 2
+000006a0: a337 3806 4f0a 0e94 61d3 5c5e ac9f 6844  .78.O...a.\^..hD
+000006b0: 2e43 79b0 318b 42f1 59c1 c01c efa4 cc7a  .Cy.1.B.Y......z
+000006c0: 2087 b90a 917c e974 2139 e472 4cbd 8ca8   ....|.t!9.rL...
+000006d0: dfb0 27b9 aaeb 1b99 7e32 a099 30c5 d628  ..'.....~2..0..(
+000006e0: 485b 7305 a23d 44fa 1f5b 3a62 34c8 2875  H[s..=D..[:b4.(u
+000006f0: 48b4 88a9 4c27 b665 17d1 62ea 8915 98a0  H...L'.e..b.....
+00000700: 1f4b 391f 1355 2183 9c17 5a9d 5788 879d  .K9..U!...Z.W...
+00000710: 7bf1 68c7 1995 af5e f51a a9ff 4d68 f977  {.h....^....Mh.w
+00000720: a1d0 7556 d37d d03b 479e e7bc a689 6fa7  ..uV.}.;G.....o.
+00000730: 1859 c644 b914 8fe9 5337 747d 4e21 da33  .Y.D....S7t}N!.3
+00000740: 7943 e6f4 a361 8c9f 4672 f233 9b0f 0000  yC...a..Fr.3....
+00000750: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+00000760: 0021 00a0 4e0f b6b7 0200 00fc 0600 0015  .!..N...........
+00000770: 0000 0070 7074 2f73 6c69 6465 732f 736c  ...ppt/slides/sl
+00000780: 6964 6531 2e78 6d6c cc54 cb6e db30 10bc  ide1.xml.T.n.0..
+00000790: 17e8 3f08 ba33 7a51 2f23 4e60 c952 d122  ..?..3zQ/#N`.R."
+000007a0: 6d8c 3af9 0046 a263 a112 4990 b463 23c8  m.:..F.c..I..c#.
+000007b0: bf97 a4a4 a8a9 9322 8716 e845 bb5c ee90  ......."...E.\..
+000007c0: bb3b 239e 5f1e bad6 da63 2e1a 4ae6 b677  .;#._....c..J..w
+000007d0: e6da 1626 15ad 1b72 3fb7 6f6f 4a90 d896  ...&...r?.ooJ...
+000007e0: 9088 d4a8 a504 cfed 2316 f6e5 c5c7 0fe7  ........#.......
+000007f0: 6c26 dada 5268 2266 686e 6fa5 6433 c711  l&..Rh"fhno.d3..
+00000800: d516 7748 9c51 8689 dadb 50de 21a9 96fc  ..wH.Q....P.!...
+00000810: dea9 397a 50a7 76ad e3bb 6ee4 74a8 21f6  ..9zP.v...n.t.!.
+00000820: 80e7 efc1 d3cd a6a9 f092 56bb 0e13 d91f  ..........V.....
+00000830: c271 8ba4 aa5c 6c1b 26c6 d3d8 7b4e 631c  .q...\l.&...{Nc.
+00000840: 0b75 8c41 bf28 e942 7556 addb 5a5b c16e  .u.A.(.BuV..Z[.n
+00000850: 38c6 da23 fb4f 9cad d98a 9bed 6ffb 15b7  8..#.O......o...
+00000860: 9a5a cdcb b608 ead4 586c 67d8 18d2 cc92  .Z......Xlg.....
+00000870: ec8d e3fc 06bf 1f5d 343b 6c78 a7ad eacd  .......]4;lx....
+00000880: 3acc 6d35 fca3 fe3a 3a86 0fd2 aafa 6035  :.m5...::.....`5
+00000890: 45ab edf5 2bb9 d5b6 7825 db19 2f70 7eb9  E...+...x%../p~.
+000008a0: 5477 d517 77da 8e3f b673 d3c8 165b 9e3d  Tw..w..?.s...[.=
+000008b0: d471 25e4 58d1 8e37 73fb b12c fd2c 2c4a  .q%.X..7s..,.,,J
+000008c0: 084a e501 e866 1064 054c 41e9 0749 e1c7  .J...f.d.LA..I..
+000008d0: 65ee 07d1 9346 7bd1 ace2 d84c f9f3 b35a  e....F{....L...Z
+000008e0: bce8 84a1 aea9 3815 7423 cf2a da0d 548f  ......8.t#.*..T.
+000008f0: 8a51 e478 70d0 8bae f231 2903 370a e102  .Q.xp....1).7...
+00000900: 7869 0cc1 32ca 4be0 15cb 0484 611a e641  xi..2.K.....a..A
+00000910: 1a27 45b4 7c1a 06a0 6a1e ade9 c219 fa1d  .'E.|...j.......
+00000920: 1a1f 8910 ec8a 563f 8445 a822 4af3 daf3  ......V?.E."J...
+00000930: f69c d193 a92d db5a f2c8 d48c 2ac9 cd98  .....-.Z....*...
+00000940: 86d4 7edf 38d3 a007 21c8 4346 eba3 bee7  ..~.8...!.CF....
+00000950: 4e59 1344 b356 c8b5 3cb6 d82c 98fe 984a  NY.D.V..<..,...J
+00000960: b8e2 a245 faef c304 dcae 6dab 6eb8 9c98  ...E......m.n...
+00000970: 9617 4cb7 d337 d503 4e50 5f56 afa0 e401  ..L..7..NP_V....
+00000980: 484a 5bf1 02ed 989b 9da9 4267 94c7 db22  HJ[.......Bg..."
+00000990: 0946 91ac 7777 d2e8 c4ff 4f75 0253 2f4c  .F..ww....Ou.S/L
+000009a0: a330 0479 1cc7 6019 e64b 9007 790a 1629  .0.y..`..K..y..)
+000009b0: 8430 2994 823c efdf eb44 ecee 7a9d a8a2  .0)..<...D..z...
+000009c0: 0e13 e42f e805 937a 8538 fafe 27ee df62  .../...z.8..'..b
+000009d0: d898 f175 1b9b 36de 405d 96a5 919f 2719  ...u..6.@]....'.
+000009e0: c83c 5802 b84c 63b0 28a3 1094 6100 619e  .<X..Lc.(...a.a.
+000009f0: 258b 3c28 3475 cc83 a7d4 a9e0 fba8 63f4  %.<(4u........c.
+00000a00: 0173 461b f3a0 7bee c0de 1eb5 6a50 4910  .sF...{.....jPI.
+00000a10: bba9 ef86 c130 b19e a2a9 5a3d f7e1 a1ae  .....0....Z=....
+00000a20: 5afe 15b1 ebbd e148 5d26 31cf 4d88 695d  Z......H]&1.M.i]
+00000a30: f4a9 538a ee5d e17e 0200 00ff ff03 0050  ..S..].~.......P
+00000a40: 4b03 0414 0006 0008 0000 0021 0022 7d32  K..........!."}2
+00000a50: 3bbe 0200 00fd 0600 0015 0000 0070 7074  ;............ppt
+00000a60: 2f73 6c69 6465 732f 736c 6964 6532 2e78  /slides/slide2.x
+00000a70: 6d6c cc54 5d4f db30 147d 9fb4 ff60 e5dd  ml.T]O.0.}...`..
+00000a80: e4b3 21ad 2828 4993 6913 1bd5 0a3f c073  ..!.((I.i....?.s
+00000a90: 5c1a cdb1 2ddb 9456 88ff 8eed 2474 ac30  \...-..V....$t.0
+00000aa0: f1b0 497b c9b5 afef bdbe e79e 139f 5dec  ..I{..........].
+00000ab0: 3a0a b644 aa96 b3b9 179e 041e 200c f3a6  :..D........ ...
+00000ac0: 65b7 73ef e6ba 8699 0794 46ac 4194 3332  e.s.......F.A.32
+00000ad0: f7f6 4479 17e7 1f3f 9c89 99a2 0d30 d94c  ..Dy...?.....0.L
+00000ae0: cdd0 dcdb 682d 66be aff0 8674 489d 7041  ....h-f....tH.pA
+00000af0: 9839 5b73 d921 6db6 f2d6 6f24 ba37 553b  .9[s.!m...o$.7U;
+00000b00: ea47 4190 fa1d 6a99 37e4 cbf7 e4f3 f5ba  .GA...j.7.......
+00000b10: c564 c1f1 5d47 98ee 8b48 4291 369d ab4d  .d..]G...HB.6..M
+00000b20: 2bd4 584d bca7 9a90 4499 322e fb45 4be7  +.XM....D.2..EK.
+00000b30: 0619 5ed1 c65a 25ae 2521 76c5 b69f a458  ..^..Z%.%!v....X
+00000b40: 89a5 74c7 dfb6 4b09 dac6 cccb 030c 7566  ..t...K.......uf
+00000b50: 2c9e 3f1c 0c61 6ecb b66e e1ff 967e 3b2e  ,.?..an..n...~;.
+00000b60: d16c b796 9db5 061b d8cd 3d33 fcbd fdfa  .l........=3....
+00000b70: d647 761a e0de 890f 5ebc b97a 2516 6faa  .Gv.....^..z%.o.
+00000b80: 57a2 fdf1 02ff 974b 2daa beb9 6338 d108  W......K-...c8..
+00000b90: e7ba d594 80d0 1bfa b854 7aec e84e b673  .........Tz..N.s
+00000ba0: efa1 aea3 6252 d509 accd 0a26 4191 c0a2  ....bR.....&A...
+00000bb0: 4aa6 b08e e2ac 8a4e eb32 8ad3 479b 1da6  J......N.2..G...
+00000bc0: 332c 899b f2e7 67b5 84e9 1143 5d8b 2557  3,....g....C].%W
+00000bd0: 7cad 4f30 ef06 aa47 c518 72c2 64d0 8bed  |.O0...G..r.d...
+00000be0: f221 5804 595e 5521 0ceb a082 4519 e470  .!X.Y^U!....E..p
+00000bf0: 5ae7 13b8 9854 5939 ad17 6599 578f c300  Z....TY9..e.W...
+00000c00: 4ccf a375 28fc 01ef 007c 2442 894b 8e7f  L..u(....|$B.K..
+00000c10: 2ac0 b821 caf2 daf3 f61c d193 69ad d800  *..!........i...
+00000c20: bd17 6646 dace 6888 eb0f dde2 30e5 4105  ..fF..h.....0.A.
+00000c30: 7a57 f066 6f2f f961 ac73 a219 557a a5f7  zW.fo/.a.s..Uz..
+00000c40: 94b8 8db0 1fd7 8634 4450 647f 3dc2 e0cd  .......4DPd.=...
+00000c50: ca03 4d2b f581 667d 5e59 2c3d a23e e128  ..M+..f}^Y,=.>.(
+00000c60: ebcb f238 ab13 7a0f cc60 ed8f 0314 6d1b  ...8..z..`....m.
+00000c70: f2a2 8cef 5af0 0fad faa3 48de 964a 3c4a  ....Z.....H..J<J
+00000c80: a5e4 4cdb b24b 8a30 d970 da10 09a2 ff54  ..L..K.0.p.....T
+00000c90: 38f1 b49c 5455 9ac1 38cf 1730 34c7 30c9  8...TU..8..04.0.
+00000ca0: d2d8 dc9e 64f5 699a 8793 38fe 97c2 699b  ....d.i...8...i.
+00000cb0: dd21 e42f 6886 b066 8924 fafe 27fe df22  .!./h..f.$..'.."
+00000cc0: d799 f179 1b41 bad5 4055 514c d3a8 cc0a  ...y.A..@UQL....
+00000cd0: 5884 490d 93c5 f414 e675 3a81 f524 4e92  X.I......u:..$N.
+00000ce0: b2c8 f232 ae2c 5522 4c8e a932 cef7 5125  ...2.,U"L..2..Q%
+00000cf0: f83d 9182 b7ee 450f 8381 ad2d a246 6269  .=....E....-.Fbi
+00000d00: 685e e524 8ea2 6162 3d25 876e ed9c 8797  h^.$..ab=%.n....
+00000d10: 1a53 f915 89ab ade3 c45c a689 2c9d 4b58  .S.......\..,.KX
+00000d20: 1df4 a187 108b dde4 3d01 0000 ffff 0300  ........=.......
+00000d30: 504b 0304 1400 0600 0800 0000 2100 23f3  PK..........!.#.
+00000d40: 70a4 d600 0000 ce01 0000 2000 0000 7070  p......... ...pp
+00000d50: 742f 736c 6964 6573 2f5f 7265 6c73 2f73  t/slides/_rels/s
+00000d60: 6c69 6465 332e 786d 6c2e 7265 6c73 ac91  lide3.xml.rels..
+00000d70: 316b c430 0c85 f742 ff83 d15e 3b97 a194  1k.0...B...^;...
+00000d80: 72ce 2da5 70d0 a9bd fe00 612b 8969 6219  r.-.p.....a+.ib.
+00000d90: cb77 5cfe 7ddd a524 7043 878e 7a7a fade  .w\.}..$pC..zz..
+00000da0: 03ed 0fd7 7952 17ca 1238 5ad8 e906 1445  ....yR...8Z....E
+00000db0: c73e c4c1 c2e7 e9f5 e109 9414 8c1e 278e  .>............'.
+00000dc0: 6461 2181 4377 7fb7 7fa7 094b 3d92 3124  da!.Cw.....K=.1$
+00000dd0: 5195 12c5 c258 4a7a 3646 dc48 338a e644  Q....XJz6F.H3..D
+00000de0: b16e 7ace 3396 3ae6 c124 745f 3890 699b  .nz.3.:..$t_8.i.
+00000df0: e6d1 e435 03ba 0d53 1dbd 857c f42d a8d3  ...5...S...|.-..
+00000e00: 92e8 2f6c eefb e0e8 85dd 79a6 586e 4498  ../l......y.XnD.
+00000e10: c885 e463 0a9e 2a15 f340 c582 d62b 796d  ...c..*..@...+ym
+00000e20: 6975 e583 b95d 6bf7 9fb5 e427 ee0d 173e  iu...]k....'...>
+00000e30: 974d af95 be31 fd36 339b 2f74 df00 0000  .M...1.63./t....
+00000e40: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+00000e50: 2100 4bf5 3dec bd00 0000 3701 0000 2000  !.K.=.....7... .
+00000e60: 0000 7070 742f 736c 6964 6573 2f5f 7265  ..ppt/slides/_re
+00000e70: 6c73 2f73 6c69 6465 322e 786d 6c2e 7265  ls/slide2.xml.re
+00000e80: 6c73 8ccf bd0a c230 1007 f05d f01d c2ed  ls.....0...]....
+00000e90: 26d5 4144 9aba 8820 3889 3ec0 915c db60  &.AD... 8.>..\.`
+00000ea0: 9b84 5c14 fbf6 66b4 e0e0 785f bf3f 571f  ..\...f...x_.?W.
+00000eb0: dee3 205e 94d8 05af 612d 2b10 e44d b0ce  .. ^....a-+..M..
+00000ec0: 771a eeb7 d36a 0782 337a 8b43 f0a4 6122  w....j..3z.C..a"
+00000ed0: 8643 b35c d457 1a30 9723 ee5d 6451 14cf  .C.\.W.0.#.]dQ..
+00000ee0: 1afa 9ce3 5e29 363d 8dc8 3244 f265 d286  ....^)6=..2D.e..
+00000ef0: 3462 2e65 ea54 44f3 c08e d4a6 aab6 2a7d  4b.e.TD.......*}
+00000f00: 1bd0 cc4c 71b6 1ad2 d9ae 41dc a648 ffd8  ...Lq.....A..H..
+00000f10: a16d 9da1 6330 cf91 7cfe 11a1 7870 962e  .m..c0..|...xp..
+00000f20: 3885 672e 2ca6 8eb2 0629 bffb b3a5 8d2c  8.g.,....).....,
+00000f30: 11a0 9a5a cdde 6d3e 0000 00ff ff03 0050  ...Z..m>.......P
+00000f40: 4b03 0414 0006 0008 0000 0021 00d8 0382  K..........!....
+00000f50: 6bd6 0000 00ce 0100 0020 0000 0070 7074  k........ ...ppt
+00000f60: 2f73 6c69 6465 732f 5f72 656c 732f 736c  /slides/_rels/sl
+00000f70: 6964 6531 2e78 6d6c 2e72 656c 73ac 9131  ide1.xml.rels..1
+00000f80: 6bc4 300c 85f7 42ff 83d1 5e3b b9a1 9472  k.0...B...^;...r
+00000f90: ce2d e5e0 e0a6 f6fa 038c ad24 a689 6c2c  .-.........$..l,
+00000fa0: 5d69 fe7d dda5 2470 4387 8e7a 7afa de03  ]i.}..$pC..zz...
+00000fb0: ed0f 5ff3 a43e b170 4c64 a1d5 0d28 249f  .._..>.pLd...($.
+00000fc0: 42a4 c1c2 fbe5 f8f0 048a c551 7053 22b4  B..........QpS".
+00000fd0: b020 c3a1 bbbf dbbf e2e4 a41e f118 33ab  . ............3.
+00000fe0: 4a21 b630 8ae4 6763 d88f 383b d629 23d5  J!.0..gc..8;.)#.
+00000ff0: 4d9f caec a48e 6530 d9f9 0f37 a0d9 35cd  M.....e0...7..5.
+00001000: a329 6b06 741b a63a 050b e514 76a0 2e4b  .)k.t..:....v..K
+00001010: c6bf b053 df47 8f2f c95f 6724 b911 6128  ...S.G./._g$..a(
+00001020: 09f2 db14 0356 aa2b 038a 05ad 57f2 dad2  .....V.+....W...
+00001030: eaca 0773 bb56 fb9f b5f8 27ee ec96 7495  ...s.V....'...t.
+00001040: 4daf 95be 31fd 3633 9b2f 74df 0000 00ff  M...1.63./t.....
+00001050: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00001060: 009c 6339 c529 0100 0071 0500 001f 0008  ..c9.)...q......
+00001070: 0170 7074 2f5f 7265 6c73 2f70 7265 7365  .ppt/_rels/prese
+00001080: 6e74 6174 696f 6e2e 786d 6c2e 7265 6c73  ntation.xml.rels
+00001090: 20a2 0401 28a0 0001 0000 0000 0000 0000   ...(...........
+000010a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000010b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000010c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000010d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000010e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000010f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001130: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001140: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001150: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001160: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001170: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001180: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001190: 0000 0000 0000 0000 bc94 4d4f c330 0c86  ..........MO.0..
+000011a0: ef48 fc87 2a77 9ab6 83f1 a1a5 bb20 a41d  .H..*w....... ..
+000011b0: 9010 8c1f 90b5 ee87 4893 280e 83fe 7ba2  ........H.(...{.
+000011c0: 0daa b69a 220e d18e 7e63 bf7e 6447 5ead  ...."...~c.~dG^.
+000011d0: bf3b 11ed c160 ab24 2369 9c90 0864 a1ca  .;...`.$#i...d..
+000011e0: 56d6 8cbc 6f9f aeee 4884 96cb 920b 2581  V...o...H.....%.
+000011f0: 911e 90ac f3cb 8bd5 2b08 6e5d 1136 adc6  ........+.n].6..
+00001200: c8b9 4864 a4b1 563f 508a 4503 1dc7 5869  ..Hd..V?P.E...Xi
+00001210: 90ee a552 a6e3 d685 a6a6 9a17 1fbc 069a  ...R............
+00001220: 25c9 929a b107 c927 9ed1 a664 c46c 4ad7  %......'...d.lJ.
+00001230: 7fdb 6bf8 8fb7 aaaa b680 4755 7c76 20ed  ..k.......GU|v .
+00001240: 8916 d4ba 5a70 86dc d460 1939 8447 318d  ....Zp...`.9.G1.
+00001250: 9d19 a1a7 1916 2119 50b4 e588 e110 feaa  ......!.P.......
+00001260: 990f e236 24c4 be85 af17 a3dc d407 9041  ...6$..........A
+00001270: f241 6467 9a84 771d 6970 8867 8e16 cc0c  .Adg..w.ip.g....
+00001280: e528 4e32 bc58 cb90 58da 00ce 1634 483e  .(N2.X..X....4H>
+00001290: 889b 9010 5259 c0f9 6c46 e224 c33b 9beb  ....RY..lF.$.;..
+000012a0: 33fd 9b85 0fe2 3ee8 29e1 3b01 6fb6 1730  3.....>.).;.o..0
+000012b0: 5ad1 48fc 03a1 9343 99ff 0000 00ff ff03  Z.H....C........
+000012c0: 0050 4b03 0414 0006 0008 0000 0021 00ad  .PK..........!..
+000012d0: 2b3e 30af 0200 00b5 0600 0015 0000 0070  +>0............p
+000012e0: 7074 2f73 6c69 6465 732f 736c 6964 6533  pt/slides/slide3
+000012f0: 2e78 6d6c cc94 dd6e db20 14c7 ef27 ed1d  .xml...n. ...'..
+00001300: 2cdf 537f 11c7 8e9a 56b6 1b4f 9bba 355a  ,.S.....V..O..5Z
+00001310: bb07 6098 34d6 3020 a069 a2aa ef3e c0b8  ..`.4.0 .i...>..
+00001320: d9da 4eea c526 edc6 07c3 3987 f33f 3fe0  ..N..&....9..??.
+00001330: f47c 3fd0 6047 a4ea 395b 86c9 491c 0684  .|?.`G..9[..I...
+00001340: 61de f5ec 7619 7ebb 6941 1106 4a23 d621  a...v.~.iA..J#.!
+00001350: ca19 5986 07a2 c2f3 b3f7 ef4e c542 d12e  ..Y........N.B..
+00001360: 30d1 4c2d d032 dc6a 2d16 51a4 f096 0c48  0.L-.2.j-.Q....H
+00001370: 9d70 4198 59db 7039 206d 7ee5 6dd4 4974  .pA.Y.p9 m~.m.It
+00001380: 6fb2 0e34 4ae3 388f 06d4 b3d0 c7cb b7c4  o..4J.8.........
+00001390: f3cd a6c7 e482 e3bb 8130 3d26 9184 226d  .........0=&.."m
+000013a0: 2a57 db5e a829 9b78 4b36 2189 3269 5cf4  *W.^.).xK6!.2i\.
+000013b0: 6f25 9d19 65f8 9a76 d62a 7123 09b1 23b6  o%..e..v.*q#..#.
+000013c0: fb20 c5b5 584b b7fc 65b7 9641 df99 7e85  . ..XK..e..A..~.
+000013d0: 0143 8369 4b18 f905 efe6 7ed9 ce0d a267  .C.iK.....~....g
+000013e0: e1b7 d310 2df6 1b39 586b b405 fb65 689a  ....-..9Xk...eh.
+000013f0: 7fb0 dfc8 ce91 bd0e f038 898f b378 7bf5  .........8...x{.
+00001400: 8a2f deae 5ef1 8ea6 0da2 5f36 b5aa c6e2  ./..^....._6....
+00001410: 5eca 4927 3937 bda6 2448 425f c7a5 d253  ^.I'97..$HB_...S
+00001420: 4577 b25f 860f 6d9b d6b3 550b 416b 4600  Ew._..m...U.AkF.
+00001430: c635 04f5 0a96 a04d b362 95ce db26 cdf2  .5.....M.b...&..
+00001440: 471b 9de4 0b2c 89eb f2c7 a7d3 92e4 2f08  G....,......../.
+00001450: 0d3d 965c f18d 3ec1 7cf0 a8a7 1363 e024  .=.\..>.|....c.$
+00001460: d09f 175b e543 5535 5579 5116 605e cf1a  ...[.CU5UyQ.`^..
+00001470: 1097 ab0b 90b7 ab14 14f3 b42c 6095 c212  ...........,`...
+00001480: 568f be01 a6e6 c93a 1591 d7eb 854f 2094  V......:.....O .
+00001490: b8e4 f887 0a18 37a0 2cd7 91db 93c7 08d3  ......7.,.......
+000014a0: 5ab1 0df4 4198 1e69 db23 ef37 2eba c1b1  Z...A..i.#.7....
+000014b0: cbfe 14e8 7dcd bb83 dde4 bbb1 6e12 2da8  ....}.......n.-.
+000014c0: d2d7 fa40 89fb 11f6 e3ca 9006 0445 f6ea  ...@.........E..
+000014d0: 1106 3ead c3a0 eba5 3e62 d667 0d67 98de  ..>.....>b.g.g..
+000014e0: d9cb 6a45 8dd2 ecce 2e49 74dc 2c9a 30ff  ..jE.....It.,.0.
+000014f0: 1976 36c1 3639 b5b9 0ac1 9a22 4cb6 9c76  .v6.69....."L..v
+00001500: 4406 e97f 8abe 88ab b49a c30c e44d 9383  D............M..
+00001510: ac29 e7a0 ca93 04e4 312c db0a e649 3acb  .)......1,...I:.
+00001520: ff25 fabe db1f 5dfe 0275 c2ba 3592 e8eb  .%....]..u..5...
+00001530: 33ee a380 5791 3a33 3d4b 9334 37f2 80ea  3...W.:3=K.47...
+00001540: bacc d3a6 a841 9dc0 16c0 0bdb a236 9f81  .....A.......6..
+00001550: 7696 41d8 d445 d564 2b0b 4824 f025 2033  v.A..E.d+.H$.% 3
+00001560: f936 4082 df13 2978 ef5e e224 f68c 7688  .6@...)x.^.$..v.
+00001570: 9a83 0593 5956 ce8a 79e6 fb34 8238 566b  ....YV..y..4.8Vk
+00001580: bbeb 5f58 4ce5 6724 ae76 8e84 d94c 13d9  .._XL.g$.v...L..
+00001590: b829 61e9 8fae 4717 abdd c4fd 0400 00ff  .)a...G.........
+000015a0: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+000015b0: 00d7 c1b4 c3b4 0200 00d2 0d00 0014 0000  ................
+000015c0: 0070 7074 2f70 7265 7365 6e74 6174 696f  .ppt/presentatio
+000015d0: 6e2e 786d 6cec 97dd 6e9b 3014 80ef 27ed  n.xml...n.0...'.
+000015e0: 1d90 6fa7 94f0 4fa2 90aa 69c7 b4a9 93a2  ..o...O...i.....
+000015f0: a67b 0017 9c06 d5d8 c836 69b2 69ef be63  .{.......6i.i..c
+00001600: c709 24ad a63e 0057 d83e bffe 3818 9fd9  ..$..>.W.>..8...
+00001610: f5ae a6ce 9608 5971 9621 ef6a 8c1c c20a  ......Yq.!.j....
+00001620: 5e56 ec39 43bf 1ef3 518a 1ca9 302b 31e5  ^V.9C...Q...0+1.
+00001630: 8c64 684f 24ba 9e7f fe34 6ba6 8d20 9230  .dhO$....4k.. .0
+00001640: 8515 983a e086 c929 ced0 46a9 66ea bab2  ...:...)..F.f...
+00001650: d890 1acb 2bde 1006 b235 1735 5630 15cf  ....+....5.5V0..
+00001660: 6e29 f02b b8af a9eb 8fc7 b15b e38a 216b  n).+.......[..!k
+00001670: 2f3e 62cf d7eb aa20 77bc 686b 087f 7022  />b.... w.hk..p"
+00001680: 0835 79c8 4dd5 c8a3 b7e6 23de fabb 384f  .5y.M.....#...8O
+00001690: 49e2 2d59 b54f 92a8 9c33 2581 0e72 70ab  I.-Y.O...3%..rp.
+000016a0: f82d afb5 915c 5685 6a61 90a1 319a 030f  .-...\V.ja..1...
+000016b0: 49cb 9f58 2a22 be97 f752 5dac 3855 9921  I..X*"...R].8U.!
+000016c0: df0b 9330 0de2 10a0 8aa9 5e01 8987 dcf9  ...0......^.....
+000016d0: cc7d cf9c 7145 e4ff d63a 2791 75f2 9e09  .}..qE...:'.u...
+000016e0: 383e 1f1f 7289 e25e 12be b63f 1727 3d71  8>..r..^...?.'=q
+000016f0: f056 dcdf 42d8 6da1 1f69 f5db 2976 80cd  .V..B.m..i..)v..
+00001700: f726 8015 2aab d867 284e a354 4f8c 4393  .&..*..g(N.TO.C.
+00001710: ae55 3b0a 8cd6 c40b c393 5649 d6b8 a5ea  .U;.......VI....
+00001720: 91ec d44a ed29 99cf b05e 5b2e 851d 3d2c  ...J.)...^[...=,
+00001730: 8543 b1ae 58c2 463f 9626 9bbe 0add 52af  .C..X.F?.&....R.
+00001740: 019d 1a8b 7bfd b61c 4c9f a1da 2972 40e7  ....{...L...)r@.
+00001750: 113f ad7e 1f23 c2a6 1435 2a04 dfb3 8578  .?.~.#...5*....x
+00001760: 316f 5dd7 16b3 5310 6d20 1414 f0b2 6585  1o]...S.m ....e.
+00001770: d2f2 5e16 123c 79a9 f6f3 4284 fea0 60e3  ..^..<y...B...`.
+00001780: 462e 39ad cabc a2d4 4c74 3992 5b2a 9c2d  F.9.....Lt9.[*.-
+00001790: 8668 6a77 a881 0b2d 13d5 51fb 06b6 5fc0  .hjw...-..Q..._.
+000017a0: a7f7 a566 23aa b426 9e12 7c21 20f8 2028  ...f#..&..|! . (
+000017b0: e485 a090 1d8e 078d c33d f1b0 68fc 0e4d  .........=..h..M
+000017c0: 1825 3ae1 818f 8162 f904 1d9f 2384 818f  .%:....b....#...
+000017d0: 8662 f984 1d1f 2f48 bc78 0074 a462 0145  .b..../H.x.t.b.E
+000017e0: 3d40 a99f 9aec 0740 9a8a 0514 7780 7c3f  =@.....@....w.|?
+000017f0: 8dcd 5f60 00a4 a958 4049 0f50 1206 c319  .._`...X@I.P....
+00001800: 7da2 6201 a51d 204d 6738 a44f 542c a049  }.b... Mg8.OT,.I
+00001810: 0f50 1c25 c321 7da2 626e ae6f af98 cd14  .P.%.!}.bn.o....
+00001820: c6f6 2e0b 23a7 1555 86fe 7ccd 6ff2 851f  ....#..U..|.o...
+00001830: 04a3 711c e4a3 d05f 44a3 147e 7aa3 c95d  ..q...._D..~z..]
+00001840: 1ee4 91b7 b8f1 c637 7f75 37e0 45fa 06fc  .......7.u7.E...
+00001850: adad 4a02 4e8e 0d89 17bd 6949 eaaa 105c  ..J.N.....iI...\
+00001860: f2b5 ba2a 786d 7b1b b7e1 af44 34bc 32ed  ...*xm{....D4.2.
+00001870: 8de7 1f1a 92c3 1d1b 7239 3e4d 76ee 7923  ........r9>Mv.y#
+00001880: 36ff 0700 00ff ff03 0050 4b03 0414 0006  6........PK.....
+00001890: 0008 0000 0021 00a2 796c 2105 0500 007e  .....!..yl!....~
+000018a0: 1200 0021 0000 0070 7074 2f73 6c69 6465  ...!...ppt/slide
+000018b0: 4c61 796f 7574 732f 736c 6964 654c 6179  Layouts/slideLay
+000018c0: 6f75 7431 2e78 6d6c cc58 dd72 9b46 14be  out1.xml.X.r.F..
+000018d0: ef4c df81 a1d7 1bb1 bf80 2772 0610 74da  .L........'r..t.
+000018e0: 7112 4f95 3c00 8695 c584 bfc2 4ab1 9bf1  q.O.<.......J...
+000018f0: 4c5e ab7d 9c3c 49cf 2e60 49b1 93da b1dd  L^.}.<I..`I.....
+00001900: f18d f6b0 9cfd f69c f37d 1c56 bc7c 7551  .........}.V.|uQ
+00001910: 95d6 5676 7dd1 d473 1bbf 706c 4bd6 5993  ..Vv}..s..plK.Y.
+00001920: 17f5 f9dc 7eff 2e41 9e6d f52a adf3 b46c  ....~..A.m.*...l
+00001930: 6a39 b72f 656f bf3a fef9 a797 ed51 5fe6  j9./eo.:.....Q_.
+00001940: 27e9 65b3 5116 60d4 fd51 3ab7 d74a b547  '.e.Q.`..Q:..J.G
+00001950: b359 9fad 6595 f62f 9a56 d670 6fd5 7455  .Y..e../.V.po.tU
+00001960: aae0 b23b 9fe5 5dfa 11b0 ab72 461c 47cc  ...;..]....rF.G.
+00001970: aab4 a8ed 717d 7797 f5cd 6a55 6472 d164  ....q}w...jUdr.d
+00001980: 9b4a d66a 00e9 6499 2a88 bf5f 176d 3fa1  .J.j..d.*.._.m?.
+00001990: b577 416b 3bd9 038c 597d 1892 ba6c 215b  .wAk;...Y}...l![
+000019a0: 55a8 52da 9671 ebb6 3081 ed63 c83c 5b96  U.R..q..0..c.<[.
+000019b0: b955 a715 4cbc d31e d6b2 2c72 696e f5ed  .U..L.....,rin..
+000019c0: bb4e 4a6d d5db 5fbb 76d9 9e76 66c5 9bed  .NJm.._.v..vf...
+000019d0: 6967 15b9 4618 57da b3f1 c6e8 662e ebad  ig..F.W.....f...
+000019e0: 3166 5f2d 3f9f ccf4 e862 d555 7a84 4258  1f_-?....b.Uz.BX
+000019f0: 1773 1bf8 bad4 bf33 3d27 2f94 950d 93d9  .s.....3='/.....
+00001a00: 6e36 5bbf bdc5 375b c7b7 78cf a60d 667b  n6[...7[..x...f{
+00001a10: 9bea ac86 e06e a643 a674 8642 e8fa 9838  .....n.C.t.B...8
+00001a20: 4e7a 3545 b4e9 8ab9 fd29 4948 c8e3 84a1  Nz5E.....)IH....
+00001a30: 042c c49c 90a1 3066 3e4a 08f5 62e2 2611  .,....0f>J..b.&.
+00001a40: a1e2 4aaf c6e2 28eb a4a1 e4b7 7c92 1616  ..J...(.....|...
+00001a50: 37e8 ac8a ac6b fa66 a55e 644d 35ea 6292  7....k.f.^dM5.b.
+00001a60: 1730 89d9 c8a4 8ef2 5318 b989 cf03 0ff1  .0......S.......
+00001a70: 10c7 c88b 7c8c 5810 2d10 c1c4 c5d8 0f03  ....|.X.-.......
+00001a80: 8293 abb1 0010 f334 9a2c 6663 be63 e213  .......4.,fc.c..
+00001a90: 117d 7bd2 641f 7aab 6e80 28cd ebc0 dbb5  .}{.d.z.n.(.....
+00001aa0: c740 a61e dbf5 28a7 4c75 a64c a3eb 70df  .@....(.Lu.L..p.
+00001ab0: 18bb 42df ca32 e684 39ce c01f c604 4a45  ..B..2..9.....JE
+00001ac0: 0f19 f731 1b1c 3493 5051 5738 37f8 1cb0  ...1..4.PQW87...
+00001ad0: db23 7511 36f9 a55e 7d06 23f0 98d6 d9ba  .#u.6..^}.#.....
+00001ae0: 81a7 ef6c c02c 7bb5 5497 a534 f6b6 c4ad  ...l.,{.T..4....
+00001af0: 7629 cf6b 13bf e137 97ab 3f60 b2ff 6b6e  v).k...7..?`..kn
+00001b00: 0bbd ebb0 d1e8 3bd8 7b18 adfe 3159 75b0  ......;.{...1Yu.
+00001b10: a84c 7567 9135 7abf 1cb6 53c7 5159 641f  .Lug.5z...S.QYd.
+00001b20: 2cd5 5832 2f94 f53a ed95 ec2c f3e8 41eb  ,.X2/..:...,..A.
+00001b30: 0110 0d38 5062 5064 9d9f a65d aa23 b806  ...8PbPd...].#..
+00001b40: fbfd 740c a235 a94e 299a acbf 2f60 3a09  ..t..5.N).../`:.
+00001b50: 78b9 391b f624 cf54 c3dc 2594 7187 211a  x.9..$.T..%.q.!.
+00001b60: 7b89 0e41 20e2 7282 7cee 078e a06e b870  {..A .r.|....n.p
+00001b70: dda7 d770 bf39 1b34 0c41 6965 3e48 cb54  ...p.9.4.Aie>H.T
+00001b80: 38c4 a1de 77b4 8c05 e7ae 2077 d5f2 3705  8...w..... w..7.
+00001b90: 5ca5 dd89 6975 459d 43c7 37e6 a1a8 cf36  \...iuE.C.7....6
+00001ba0: 6fe0 0d67 00f6 f4ad 63fd 5adf c624 3b54  o..g....c.Z..$;T
+00001bb0: 06cc e878 ef0b 7df0 e868 bc11 9aee a087  ...x..}..h......
+00001bc0: 5adc 1b1a 7bfb d01a 6f84 663b 684c 5dac  Z...{...o.f;hL].
+00001bd0: bbc4 bdb1 77ad 6504 1cb1 f91e b647 3c1d  ....w.e......G<.
+00001be0: c2c3 b035 e088 2d76 d884 78a6 e93c 0c5b  ...5..-v..x..<.[
+00001bf0: 038e d8ee 1eb6 cbe8 8f50 7988 ad01 476c  .........Py...Gl
+00001c00: 6f87 ad81 7f88 cb03 6c0d 3862 fb7b d882  o.......l.8b.{..
+00001c10: 9b8e ff30 6c0d f848 ddbb 9f9a e9d3 3770  ...0l..H......7p
+00001c20: 3635 f045 aaa4 755a a699 5c37 650e 41d0  65.E..uZ..\7e.A.
+00001c30: 67da c863 47c4 9c13 8e7c 217c b4f0 b88b  g..cG....|!|....
+00001c40: 02e2 0788 b024 0e92 30a4 3ca0 4fdf c873  .....$..0.<.O..s
+00001c50: 651b 0dac d372 3535 f341 0cdf ece6 e688  e....r55.A......
+00001c60: fadd 966b 2e8c 6456 7044 1e5e 5b1e 4d44  ...k..dVpD.^[.MD
+00001c70: 18c5 8851 c836 a1cc 85bc a987 8288 9305  ...Q.6..........
+00001c80: 7363 dfc3 d1d5 74e0 ce81 4355 5432 29ce  sc....t...CUT2).
+00001c90: 379d 7cbb 5186 c203 e581 52ac be52 5129  7.|.Q.....R..RQ)
+00001ca0: d3fa fa34 ab8e 8943 c8cc e133 e2ee d406  ...4...C...3....
+00001cb0: 313c bede f8a4 b7a4 69b4 d4f7 15c7 9ea9  1<......i.......
+00001cc0: e230 e8ca 6301 459c c604 2dc4 2240 220c  .0..c.E...-."@".
+00001cd0: 8088 248a 4440 b808 a2f0 e915 b782 5e64  ..$.D@........^d
+00001ce0: 24f7 e726 eda0 7493 eafe e30c 711f d53d  $..&..t.....q..=
+00001cf0: 2ed5 e2fa 6ca8 ffdf 596f 36d5 d957 84f3  ....l...Yo6..W..
+00001d00: 674a 78c4 23c7 7508 4391 eb46 28f2 160c  gJx.#.u.C..F(...
+00001d10: 0561 1001 ff4c f0d8 09c0 9ffc 0f67 c532  .a...L.......g.2
+00001d20: 879a ddca f970 a27b dc4e 2358 48fd 8543  .....p.{.N#XH..C
+00001d30: e1ff 1dfc 2c22 0625 a771 8030 f7c2 d00f  ....,".%.q.0....
+00001d40: 221f ce92 d79d a6d7 94d6 10dd 5d1b cc97  "...........]...
+00001d50: cf7f fff2 e5f3 3f8f d05d cc30 7d26 98aa  ......?..].0}&..
+00001d60: 6eac 513b 10ad 2091 17a2 10b3 04b1 850f  n.Q;.. .........
+00001d70: 2f88 4470 9400 7d2c 0abd 20a2 b1d6 4e8b  /.Dp..},.. ...N.
+00001d80: d94d edc0 e4dd b4d3 361f 65d7 3685 f98c  .M......6.e.6...
+00001d90: 829d 513e dbb4 84f3 844b b9c7 84cb f848  ..Q>.....K.....H
+00001da0: d3a0 915d b49a f8a5 ce1f c6b2 7b9d b66f  ...]........{..o
+00001db0: b746 2495 79fd 4766 aad5 c21c 5c77 2e3a  .F$.y.Gf....\w.:
+00001dc0: f7e9 bbd1 f1bf 0000 00ff ff03 0050 4b03  .............PK.
+00001dd0: 0414 0006 0008 0000 0021 004a 197e 4754  .........!.J.~GT
+00001de0: 0400 0089 0f00 0021 0000 0070 7074 2f73  .......!...ppt/s
+00001df0: 6c69 6465 4c61 796f 7574 732f 736c 6964  lideLayouts/slid
+00001e00: 654c 6179 6f75 7432 2e78 6d6c cc57 db6e  eLayout2.xml.W.n
+00001e10: dc36 107d 2fd0 7f10 d467 4637 8a92 16b1  .6.}/....gF7....
+00001e20: 035d 8b16 4e6c 749d 0fa0 25ae 578d 24aa  .]..Nlt...%.W.$.
+00001e30: 1477 b3db c040 7eab fd9c 7c49 8794 e47b  .w...@~...|I...{
+00001e40: 9b2d b006 fc22 52d4 f070 66ce 1992 7afb  .-..."R..pf...z.
+00001e50: 6ed7 36c6 9689 a1e6 dd89 e9bc b14d 8375  n.6..........M.u
+00001e60: 25af eaee fac4 fc78 59a0 d034 0649 bb8a  %......xY..4.I..
+00001e70: 36bc 6327 e69e 0de6 bbd3 1f7f 78db 2f86  6.c'........x./.
+00001e80: a63a a37b be91 0660 74c3 829e 986b 29fb  .:.{...`t....k).
+00001e90: 8565 0de5 9ab5 7478 c37b d6c1 b715 172d  .e....tx.{.....-
+00001ea0: 95f0 2aae ad4a d0cf 80dd 3696 6bdb c46a  ..*..J....6.k..j
+00001eb0: 69dd 99d3 7c71 c87c be5a d525 cb78 b969  i...|q.|.Z.%.x.i
+00001ec0: 5927 4710 c11a 2ac1 ff61 5df7 c38c d61f  Y'G...*..a].....
+00001ed0: 82d6 0b36 008c 9efd d025 b9ef 215a 7ef5  ...6.....%..!Z~.
+00001ee0: bb69 6823 b185 57c7 3c85 b8cb 6553 191d  .ih#..W.<...eS..
+00001ef0: 6d61 e0b2 960d 3320 3b46 ca3b 0948 da60  ma....3 ;F.;.H.`
+00001f00: e82f 0563 aad7 6d7f 16fd b2bf 107a de87  ./.c..m......z..
+00001f10: ed85 30ea 4ae1 4cf3 4d6b fa30 99e9 d76e  ..0.J.L.Mk.0...n
+00001f20: ab3b d6a3 e9d7 7397 2e76 2bd1 aa16 9261  .;....s..v+....a
+00001f30: ec4e 4ce0 6caf 9e96 1a63 3b69 94e3 6079  .NL.l....c;i..`y
+00001f40: 375a aecf 9fb1 2dd7 f933 d6d6 bc80 756f  7Z....-..3....uo
+00001f50: 5115 d5e8 dcd3 70dc 399c 311d 2a4b da8f  Q.....p.9.1.*K..
+00001f60: b341 ce1e 6d44 7d62 7e29 0a37 f1f3 02a3  .A..mD}b~).7....
+00001f70: 027a 08db 0946 498e 2354 b85e 98bb 4191  .z...FI.#T.^..A.
+00001f80: ba1e b951 b31d b228 05d3 b4fc 52cd f272  ...Q...(....R..r
+00001f90: c813 4adb ba14 7ce0 2bf9 a6e4 eda4 8d59  ..J...|.+......Y
+00001fa0: 62c0 a683 2736 9597 5f62 2ff4 7044 2244  b...'6.._b/.pD"D
+00001fb0: ecd4 4771 1aa4 c84e 6270 2172 a214 1307  ..Gq...Nbp!r....
+00001fc0: 1392 dd4c 0900 9fe7 5647 614d f14e 81cf  ...L....VGaM.N..
+00001fd0: 440c fd19 2f3f 0d46 c781 28c5 ebc8 dbad  D.../?.F..(.....
+00001fe0: c548 a66a fbf5 2429 a972 34d9 8d1f 75e7  .H.j..$).r4...u.
+00001ff0: 2ecb 930a e42e e1d5 5e2d 7205 ad1e a48b  ........^-r.....
+00002000: 6690 4bb9 6f98 7ee9 d543 bb21 8088 86aa  f.K.o.~..C.!....
+00002010: 8a65 1dfa b81c c995 a769 5397 9f0c c90d  .e.......iS.....
+00002020: 56d5 d278 4f07 c984 a1d7 8792 0614 15e0  V..xO...........
+00002030: 18a6 4661 5d75 4105 fded 3ed8 af17 5342  ..Fa]uA...>...SB
+00002040: 7aed e7ec 9435 cbe1 df45 e1cd a298 2ac3  z....5...E....*.
+00002050: b868 68c9 d6bc a9c0 09f7 954a c4c1 b6eb  .hh........J....
+00002060: 1499 8762 823d 9410 62a3 248c 3022 b9e3  ...b.=..b.$.0"..
+00002070: 0659 14bb 5194 bfa4 44ea 6a77 6772 0475  .Y..Q...D.jwgr.u
+00002080: f48a cb6d 735b f0ff 5f2d 8a19 2d96 e181  ...ms[.._-..-...
+00002090: 5a46 453c 5e45 7bfe dfab 2c59 c961 bb6c  ZFE<^E{...,Y.a.l
+000020a0: d896 3507 20ba df47 bc5c d7e2 7040 effb  ..5. ..G.\..p@..
+000020b0: 8005 df08 b93e 1811 1f80 58af 9e05 3c76  .....>....X...<v
+000020c0: cde1 b9e6 322a d983 82f3 5e69 c191 2473  ....2*....^i..$s
+000020d0: 0237 0c51 1166 364a b19f a32c b06d 841d  .7.Q.f6J...,.m..
+000020e0: 2fc5 5e41 323b 212f bf27 5712 2e39 7f42  /.^A2;!/.'W..9.B
+000020f0: 24b4 5929 c754 118e 47e1 51aa 7005 f705  $.Y).T..G.Q.p...
+00002100: 1dad 1f42 4849 9a23 ecc1 3154 7838 4011  ...BHI.#..1Tx8@.
+00002110: f142 388b 7c37 c341 1e85 4e7a 33df 3d2a  .B8.|7.A..Nz3.=*
+00002120: e050 d62d 2bea eb8d 60e7 1b75 b778 a430  .P.-+...`..u.x.0
+00002130: 508a 31b4 326d 18ed 6e6b 5c9e bab6 eb5a  P.1.2m..nk\....Z
+00002140: b66f b9c1 9dda c087 e3eb cd9f f556 70ae  .o...........Vp.
+00002150: 768b fb8a c3af 758b 2738 0e43 3b47 4118  v.....u.'8.C;GA.
+00002160: 4608 960b 91ed 1017 c589 1d15 4962 0779  F...........Ib.y
+00002170: 12bd bce2 5652 8c92 fb63 4305 a46e 56dd  ....VR...cC..nV.
+00002180: 11f7 fee3 524d 66aa 974d 5d31 e3c3 a6bd  ....RMf..M]1....
+00002190: 7a44 b8ff 6acf f438 4d03 0c45 e7bb 298a  zD..j..8M..E..).
+000021a0: 6337 4699 e760 1404 7112 470e f66d 2f78  c7F..`..q.G..m/x
+000021b0: 79c2 e167 0972 f62c e7fa 8c3b f24e 4370  y..g.r.,...;.NCp
+000021c0: e245 99ed a130 8547 9662 48b9 97c7 c8f1  .E...0.G.bH.....
+000021d0: c324 89e2 3422 be7f bbd3 0c8a d20e bc3b  .$..4".........;
+000021e0: 7483 f9f6 f5af 9fbe 7dfd fb08 bb8b 6ee6  t.......}.....n.
+000021f0: bfa5 39eb ba37 6907 bc25 6e1a 2628 7170  ..9..7i..%n.&(qp
+00002200: 8170 1605 282e 888f 0adf c338 4dc2 38f5  .p..(......8M.8.
+00002210: 72a5 9dde c14f b503 8387 69a7 e79f 99e8  r....O....i.....
+00002220: 79ad ff28 1d7b 92cf 96aa 3b4d e044 7e10  y..(.{....;M.D~.
+00002230: f891 be39 58da b7b9 bdd5 c852 c50f 6d23  ...9X......R..m#
+00002240: ded3 fe7c ab45 d2ea 1b54 aa87 7a25 ccd1  ...|.E...T..z%..
+00002250: f4ce 44c5 3eff 429f fe03 0000 ffff 0300  ..D.>.B.........
+00002260: 504b 0304 1400 0600 0800 0000 2100 c3d7  PK..........!...
+00002270: f29b 3e05 0000 5e15 0000 2100 0000 7070  ..>...^...!...pp
+00002280: 742f 736c 6964 654c 6179 6f75 7473 2f73  t/slideLayouts/s
+00002290: 6c69 6465 4c61 796f 7574 332e 786d 6ccc  lideLayout3.xml.
+000022a0: 58db 929c 3610 7d4f 55fe 8122 cf32 e886  X...6.}OU..".2..
+000022b0: 60cb b32e aeb9 d4da deca d81f 8041 b343  `............A.C
+000022c0: 995b 8466 bc1b d756 f9b7 92cf f197 4412  .[.f...V......D.
+000022d0: 3033 6baf 9d71 e2dd 9a17 10a2 bb39 dde7  03k..q.......9..
+000022e0: 4834 3c7d 76dd d4d6 968b a1ea da85 0d9f  H4<}v...........
+000022f0: b8b6 c5db a22b abf6 6a61 bf7e 9501 dfb6  .....+..ja.~....
+00002300: 0699 b765 5e77 2d5f d837 7cb0 9f9d fff8  ...e^w-_.7|.....
+00002310: c3d3 fe6c a8cb 8bfc a6db 484b c568 87b3  ...l......HK.h..
+00002320: 7c61 afa5 eccf 1c67 28d6 bcc9 8727 5dcf  |a.....g(....'].
+00002330: 5b75 6fd5 8926 97ea 525c 39a5 c8df a9d8  [uo..&..R\9.....
+00002340: 4ded 20d7 f59c 26af 5a7b f217 c7f8 77ab  M. ...&.Z{....w.
+00002350: 5555 f0a4 2b36 0d6f e518 44f0 3a97 0aff  UU..+6.o..D.:...
+00002360: b0ae fa61 8ed6 1f13 ad17 7c50 618c f75d  ...a......|Pa..]
+00002370: 48f2 a657 d90e bcf8 85e7 a56d 1943 b155  H..W.......m.C.U
+00002380: 53d0 3e57 b917 cbba b4da bc51 134b 5e68  S.>W.......Q.K^h
+00002390: 774b 1b72 61ee 0efd 2bc1 b91e b5db 9f45  wK.ra...+......E
+000023a0: bfec 2f85 717a b1bd 1456 55ea 2093 b3ed  ../.qz...VU. ...
+000023b0: 4c37 2633 73d9 6ecd c0f9 c4fd 6a1e e667  L7&3s.n.....j..g
+000023c0: d72b d1e8 b3aa 8675 bdb0 1569 37fa e8e8  .+.....u...i7...
+000023d0: 397e 2dad 629c 2cf6 b3c5 fae5 3db6 c53a  9~-.b.,.....=..:
+000023e0: bdc7 da99 1fe0 1c3c 5467 3582 fb3c 1d34  .......<Tg5..<.4
+000023f0: a7f3 aa92 35b7 7489 0c8e 8b41 ce88 36a2  ....5.t....A..6.
+00002400: 5ad8 efb3 0c45 34cd 08c8 d408 1037 2220  Z....E4......7" 
+00002410: 4a49 0032 84fd 14b1 2c46 d8bb d5de d03b  JI.2....,F.....;
+00002420: 2b04 37bc fc5a cefa 82de 679c 3655 21ba  +.7..Z....g.6U!.
+00002430: a15b c927 45d7 4ce2 9835 a6e8 8464 a253  .[.'E.L..5...d.S
+00002440: a37c cf18 2534 8421 802e 7641 cc32 0f44  .|..%4.!..vA.2.D
+00002450: 348e 00c5 01f5 bc30 f2b3 84dc 4e05 5098  4......0....N.P.
+00002460: e7b3 c9c2 99f2 9d12 9f89 18fa 8bae 783b  ..............x;
+00002470: 586d a788 d2bc 8ebc ed2c 4632 f5b9 5f4f  Xm.......,F2.._O
+00002480: 9a92 ba46 93dd 78d3 0cf6 55be 9762 1f43  ...F..x...U..b.C
+00002490: 9f8e dc41 e606 0cfb 77d9 862e 85d4 7327  ...A....w.....s'
+000024a0: 1a91 4f11 c3ec 5332 c7d8 fd99 bc8e baf2  ..O...S2........
+000024b0: 46bb bf51 6745 62de 16eb 4ead bf37 63d0  F..QgEb...N..7c.
+000024c0: 7a90 4b79 5373 33de d670 8254 f2d5 efca  z.KySs3..p.T....
+000024d0: 78f8 7361 ab27 cd52 d919 e8f1 8163 af0f  x.sa.'.R.....c..
+000024e0: c64f 28a7 3ad7 1b0a 6fc1 ebe5 f80c 791e  .O(.:...o.....y.
+000024f0: d755 f1d6 929d c5cb 4a5a cff3 4172 6199  .U......JZ..Ara.
+00002500: eaa8 1d47 05d1 0147 124c 14de 9697 b9c8  ...G...G.L......
+00002510: 3582 5db0 df2e 2710 bdc9 6fce cba4 fa75  5.]...'...o....u
+00002520: c9e2 9d64 7505 2feb bce0 ebae 560b d842  ...du./.....V..B
+00002530: 27aa de24 8963 8249 0292 8052 8048 1483  '..$.c.I...R.H..
+00002540: 8805 1484 994f 2396 429a 79d1 c3ab 570b  .....O#.B.y...W.
+00002550: 4603 d292 fb3f 2226 d40f 8887 bf26 6248  F....?"&.....&bH
+00002560: 5d17 fa47 8bf8 4bca b59a 5c5c 980d ae6a  ]..G..K...\\...j
+00002570: 4bb5 d9eb a1f1 dabc 506f 34e3 7520 6c44  K.......Po4.u lD
+00002580: dcf1 f6d0 d555 9955 756d 2e34 613c ae85  .....U.Uum.4a<..
+00002590: b5cd 6bb5 84af c72d 4e56 ad1c 6718 dd2f  ..k....-NV..g../
+000025a0: 889d f178 b58f e3cc 4fba bb6e cc10 ed91  ...x....O..n....
+000025b0: 12ca 90ae c151 70f5 631f 0bae c638 c1c5  .....Qp.c....8..
+000025c0: 7bb8 0124 ba66 47c1 85fe 23c2 d518 27b8  {..$.fG...#...'.
+000025d0: 640f 1762 068d c48e c2ab 2d1f 0baf 0639  d..b......-....9
+000025e0: e1a5 0778 7de4 ebaa 9d1e 5e0d 72c2 ebed  ...x}.....^.r...
+000025f0: f122 e49b 97c3 e9e1 d520 27bc ec00 2f23  ."....... '.../#
+00002600: f8e8 e5f6 a878 35c8 09af bfc7 abc1 1ebf  .....x5.........
+00002610: de1e 13af 0639 e10d 0ef0 7a94 9de6 7ad3  .....9....z...z.
+00002620: 20ef ef5a 347a 65b0 6b93 bfbd 8bd1 6f34   ..Z4ze.k.....o4
+00002630: d3c4 0c77 ba98 ffd2 a990 b953 4972 c9ef  ...w.......SIr..
+00002640: 742a f844 3b95 d00d c3c0 a729 4813 8601  t*.D;......)H...
+00002650: f362 35f2 7000 529c c0d8 8d42 3ff4 d287  .b5.p.R....B?...
+00002660: ef54 4a69 1b4d adf3 7a35 772c a348 bed8  .TJi.M..z5w,.H..
+00002670: b298 afaf aff6 15e6 c268 64a5 3e00 4db6  .........hd.>.M.
+00002680: d4c7 aaf3 5239 12ec a90a 63c2 40e0 611f  ....R9....c.@.a.
+00002690: 8431 4509 6169 e0c3 f876 fea0 2c15 87b2  .1E.ai...v..,...
+000026a0: 6a78 565d 6d04 7fb9 9186 c23b d252 3dad  jxV]m......;.R=.
+000026b0: 3534 32ae 79de ee14 28cf 918b 90e3 5207  542.y...(.....R.
+000026c0: b1bd a214 86ef df19 d359 6f59 d769 2d1f  .........YoY.i-.
+000026d0: 2a8e 9ca8 e248 1011 8abc 08b8 018a 811f  *....H..........
+000026e0: e20c 642c 0b80 9a83 344e 5517 19c0 8757  ..d,....4NU....W
+000026f0: dc4a 8a51 727f 6c72 a14a 37ab ee5f 1ae5  .J.Qr.lr.J7.._..
+00002700: 6f51 ddf7 a5da 9ba9 5eaa 5d92 5b2f 36cd  oQ......^.].[/6.
+00002710: 9b4f 08a7 274a 3872 5337 f362 065c 0f65  .O..'J8rS7.b.\.e
+00002720: ea10 4210 f928 0229 8334 4d30 c230 420f  ..B..(.).4M0.0B.
+00002730: 4ff8 5097 aa66 f772 8e1e 60a7 f148 8483  O.P..f.r..`..H..
+00002740: c4c5 c08f d521 8989 2a39 4e43 00a9 1f45  .....!..*9NC...E
+00002750: 4118 071e a5bb 9d66 d094 b60a ddb1 1bcc  A......f........
+00002760: c70f 7ffd f4f1 c3df df61 7731 a7f9 0fd8  .........aw1....
+00002770: 5c75 339a b4a3 d07a 28f6 2310 4192 0192  \u3....z(.#.A...
+00002780: 044c 7dc5 7a14 6414 1312 477e 18e3 546b  .L}.z.d...G~..Tk
+00002790: a787 e473 eda8 c9e3 b4d3 77ef b8e8 bbca  ...s......w.....
+000027a0: fc26 84ee 241f d330 608c 02b5 2530 4626  .&..$..0`...%0F&
+000027b0: 9a46 8dec d16a e297 3a7f 75ae c5f3 bc7f  .F...j..:.u.....
+000027c0: b935 2269 ccfb 3d36 53bd 16e6 68ba 37d1  .5"i..=6S...h.7.
+000027d0: b9cf ff45 cfff 0100 00ff ff03 0050 4b03  ...E.........PK.
+000027e0: 0414 0006 0008 0000 0021 00ab ed09 7ab5  .........!....z.
+000027f0: 0400 00c3 1300 0021 0000 0070 7074 2f73  .......!...ppt/s
+00002800: 6c69 6465 4c61 796f 7574 732f 736c 6964  lideLayouts/slid
+00002810: 654c 6179 6f75 7434 2e78 6d6c ec58 5b6e  eLayout4.xml.X[n
+00002820: dc36 14fd 2fd0 3d08 ea37 2df1 29c9 881d  .6../.=..7-.)...
+00002830: e859 b470 62a3 e32c 4096 381e 357a 95e2  .Y.pb..,@.8.5z..
+00002840: 8ced 0606 b2ad 7639 5949 494a f23b f1b8  ......v9YIIJ.;..
+00002850: b003 7f64 3e86 1445 5ede 7bcf 3957 94de  ...d>..E^.{.9W..
+00002860: bc3d 6f6a 6bc3 c550 75ed 9e0d 775c dbe2  .=ojk..Pu...w\..
+00002870: 6dd1 9555 7bba 677f 38ce 806f 5b83 ccdb  m..U{.g.8..o[...
+00002880: 32af bb96 efd9 177c b0df eeff fcd3 9b7e  2......|.......~
+00002890: 77a8 cb83 fca2 5b4b 4bd9 6887 dd7c cf5e  w.....[KK.h..|.^
+000028a0: 49d9 ef3a ce50 ac78 930f 3b5d cf5b 756f  I..:.P.x..;].[uo
+000028b0: d989 2697 ea52 9c3a a5c8 cf94 eda6 7690  ..&..R.:......v.
+000028c0: eb32 a7c9 abd6 9ed6 8b6d d677 cb65 55f0  .2.......m.w.eU.
+000028d0: a42b d60d 6fe5 6844 f03a 97ca ff61 55f5  .+..o.hD.:...aU.
+000028e0: c36c addf c65a 2ff8 a0cc 98d5 b75d 9217  .l...Z/......]..
+000028f0: bd8a 569e 7587 277f da96 9927 366a 04da  ..V.u.'....'6j..
+00002900: fb2a f462 5197 569b 376a e0f8 acb3 e2ae  .*.bQ.V.7j......
+00002910: 95ca 8cb9 35f4 c782 73dd 6b37 bf8a 7ed1  ....5...s.k7..~.
+00002920: 1f09 b3e2 fde6 4858 55a9 2d4c 2b6d 67ba  ......HXU.-L+mg.
+00002930: 314d 3397 edc6 749c 3bcb 4fe7 6ebe 7bbe  1M3...t.;.O.n.{.
+00002940: 148d 6e55 26ac f33d 5b01 76a1 ff1d 3dc6  ..nU&..=[.v...=.
+00002950: cfa5 558c 83c5 f568 b13a 7c60 6eb1 4a1f  ..U....h.:|`n.J.
+00002960: 98ed cc1b 3837 36d5 518d cedd 0f07 cde1  ....876.Q.......
+00002970: 1c57 b2e6 96ce 8ff1 e360 90b3 476b 51ed  .W.......`..GkQ.
+00002980: d99f b20c 4534 cd08 c854 0f10 3722 204a  ....E4...T..7" J
+00002990: 4900 3284 fd14 7959 8c30 bbd4 ab21 db2d  I.2...yY.0...!.-
+000029a0: 0437 98fc 56ce dc82 ec1e 9e4d 5588 6ee8  .7..V......MU.n.
+000029b0: 9672 a7e8 9a89 1833 bf14 9490 4c50 6a2f  .r.....3....LPj/
+000029c0: 3fa1 3860 ea97 8090 2102 7c8c 2280 fdc4  ?.8`....!.|."...
+000029d0: 0728 2481 9750 98e1 24b9 9c12 a07c 9e5b  .($..P..$....|.[
+000029e0: 1385 33c5 3b05 3e03 31f4 075d f171 b0da  ..3.;.>.1..].q..
+000029f0: 4e01 a571 1d71 bb9a 3182 a9db 7e35 f349  N..q.q..1...~5.I
+00002a00: e768 9a37 de34 9deb 2c4f 2c90 e751 575e  .h.7.4..,O,..QW^
+00002a10: e84d 4e54 6b06 f3dd 7a90 0b79 5173 73d1  .MNTk...z..yQss.
+00002a20: eb3f e386 5040 d4b9 962b 6fc1 87c5 08ae  .?..P@...+o.....
+00002a30: dc8f ebaa f868 c9ce e265 25ad 77f9 20b9  .....h...e%.w. .
+00002a40: b0cc fe4a cfca 8a0e 700c d358 e16d 7994  ...J....p..X.my.
+00002a50: 8bfc 8f9b c67e 3f9a 12d2 1b3f 67a7 9c99  .....~?....?g...
+00002a60: 0e5f 2705 9e49 3129 c33a aaf3 82af baba  ._'..I1).:......
+00002a70: 544e a057 4a91 c823 30a1 0101 71e6 3390  TN.WJ..#0...q.3.
+00002a80: c590 8284 463e c892 8c30 0833 1667 e425  ....F>...0.3.g.%
+00002a90: 2932 fcad fccf eba5 76e7 fc7a f257 78f2  )2......v..z.Wx.
+00002aa0: 4029 f0b1 af2a 98d1 38f4 1165 88de ae0a  @)...*..8..e....
+00002ab0: 14fa 90e9 095a ed04 5388 b17f 57f3 a3e9  .....Z..S...W...
+00002ac0: ad19 d86b be6c eaab a2f2 7446 6ae7 0c21  ...k.l....tFj..!
+00002ad0: 875b 8c1c 5977 7717 9393 6fef b2e0 45d7  .[..Yww...o...E.
+00002ae0: 9656 cd37 bcde c222 7adc e2f1 aa12 db1b  .V.7..."z.......
+00002af0: c48f 1bcc bab5 90ab ad2d 922d 2c56 cb07  .........-.-,V..
+00002b00: 0d3e b7ae c9b7 748d 5fa9 aea1 cb58 9af9  .>....t._....X..
+00002b10: 18a4 5918 8130 c942 1007 ae0b 28f2 594a  ..Y..0.B....(.YJ
+00002b20: 7d16 a624 fd8e ba36 8c7b 92ae 19f4 d00f  }..$...6.{......
+00002b30: 61ff 10f6 0b0a 9bce c24e 72c9 6fa9 9abc  a........Nr.o...
+00002b40: 5255 2714 0730 0830 4862 9f80 34c1 2940  RU'..0.0Hb..4.)@
+00002b50: 3ec2 4069 3af4 951f 3049 5f54 d5e3 81ae  >.@i:...0I_T....
+00002b60: 94f6 bde7 f678 8e7e 9603 de52 bd66 9868  .....x.~...R.f.h
+00002b70: a98f 3316 c529 2098 a90c 63e2 8180 611f  ..3..) ...c...a.
+00002b80: 8431 4509 f1d2 c087 f1e5 fcd6 522a 0c65  .1E.........R*.e
+00002b90: d5f0 ac3a 5d0b 7eb8 d62f 2677 18a6 9862  ...:].~../&w...b
+00002ba0: 0d8d 8c6b 9eb7 571a 97fb c845 c871 a983  ...k..W....E.q..
+00002bb0: bc6b b629 1f9e 9f6f 6ce6 5bd6 75ba 5adc  .k.)...ol.[.u.Z.
+00002bc0: 641c 7dad 8ccb 088a 55fd 550f 8e04 82c8  d.}.....U.U.....
+00002bd0: a309 a084 7980 859e 1b27 618a c234 7879  ....y....'a..4xy
+00002be0: c62d a518 29f7 d73a 172a 7533 eb1e 392e  .-..)..:.*u3..9.
+00002bf0: 3e85 75cf 0bb5 3743 bda8 ab92 5bef d7cd  >.u...7C....[...
+00002c00: c91d c0d9 2b05 3c4e 298e 11f4 4018 2a98  ....+.<N)...@.*.
+00002c10: a340 9518 9f44 0188 6812 449e 0b11 c5df  .@...D..h.D.....
+00002c20: a1c4 0c75 a972 f620 e68f 1c25 fe57 a561  ...u.r. ...%.W.a
+00002c30: 24c2 41e2 aa42 1abb bab8 1295 729c 8600  $.A..B......r...
+00002c40: 523f 8a82 50bd 4653 7a55 6906 0d69 abbc  R?..P.FSzUi..i..
+00002c50: dbb6 c07c f9fc cf2f 5f3e fffb 0cd5 c534  ...|.../_>.....4
+00002c60: f3a7 9639 eba6 3771 4779 cb50 ec47 2082  ...9..7qGy.P.G .
+00002c70: 2403 2409 148e 19a3 20a3 9890 38f2 c358  $.$..... ...8..X
+00002c80: a3a7 d640 729f 3b6a 703b eef4 dd19 177d  ...@r.;jp;.....}
+00002c90: 5799 6f51 d09d e8b3 c9f5 8101 63cf f302  W.oQ........c...
+00002ca0: 3708 2698 468e 5c7b ab81 5fe8 f855 5b8b  7.&.F.\{.._..U[.
+00002cb0: 7779 7fb8 3124 69cc 092a 3643 bd26 e638  wy..1$i..*6C.&.8
+00002cc0: f57a 8a8e 7dfe f8b6 ff1f 0000 00ff ff03  .z..}...........
+00002cd0: 0050 4b03 0414 0006 0008 0000 0021 006b  .PK..........!.k
+00002ce0: 8a56 3713 0600 0055 1f00 0021 0000 0070  .V7....U...!...p
+00002cf0: 7074 2f73 6c69 6465 4c61 796f 7574 732f  pt/slideLayouts/
+00002d00: 736c 6964 654c 6179 6f75 7435 2e78 6d6c  slideLayout5.xml
+00002d10: ec59 eb6e db36 14fe 3f60 ef20 78bf 59f3  .Y.n.6..?`. x.Y.
+00002d20: 2e2a 6852 e83a 6c48 9b60 491f 4091 e85a  .*hR.:lH.`I.@..Z
+00002d30: ab6e 9364 2759 51a0 afb5 3d4e 9f64 2425  .n.d'YQ...=N.d$%
+00002d40: c576 e2a4 4e9a 1401 961f b668 8afc 780e  .v..N......h..x.
+00002d50: bfef 1c1d 53af df5c 14b9 b594 4d9b 55e5  ....S..\....M.U.
+00002d60: fe04 bd82 134b 9649 9566 e587 fdc9 fbd3  .....K.I.f......
+00002d70: 0888 89d5 7671 99c6 7955 cafd c9a5 6c27  ....vq..yU....l'
+00002d80: 6f0e 7efe e975 bdd7 e6e9 617c 592d 3a4b  o.~..u....a|Y-:K
+00002d90: 6194 ed5e bc3f 9977 5dbd 379d b6c9 5c16  a..^.?.w].7...\.
+00002da0: 71fb aaaa 65a9 eecd aaa6 883b f5b3 f930  q...e......;...0
+00002db0: 4d9b f85c 6117 f914 43c8 a745 9c95 9361  M..\a...C..E...a
+00002dc0: 7eb3 cbfc 6a36 cb12 1954 c9a2 9065 d783  ~...j6...T...e..
+00002dd0: 3432 8f3b 657f 3bcf ea76 44ab 7741 ab1b  42.;e.;..vD.wA..
+00002de0: d92a 1833 7bd3 a4ee b256 de76 e7d5 e9c5  .*.3{....V.v....
+00002df0: e979 7574 f6e7 c432 839b a5ea 4693 03e5  .yut...2....F...
+00002e00: 7f72 92a7 5619 17aa c3af 8a3a 6eb2 b62a  .r..V......:n..*
+00002e10: cd9d b63e 6da4 d4ad 72f9 6b53 9fd4 c78d  ...>m...r.kS....
+00002e20: 99f0 6e79 dc58 59aa 0186 8993 e970 6318  ..ny.XY......pc.
+00002e30: 667e 964b d398 5e9b fe61 6cc6 7b17 b3a6  f~.K..^..al.{...
+00002e40: d057 b51b d6c5 fe44 9176 a9bf a7ba 4f5e  .W.....D.v....O^
+00002e50: 7456 d277 26ab de64 7eb4 656c 320f b78c  tV.w&..d~.el2...
+00002e60: 9e8e 0b4c d716 d55e f5c6 dd74 078f ee9c  ...L...^...t....
+00002e70: 665d 2e2d bd3d c68e c3b6 1b2d 5a34 d9fe  f].-.=.....-Z4..
+00002e80: e453 1461 8f85 1105 916a 010a 3d0a bc90  .S.a.....j..=...
+00002e90: 3a20 c244 84d8 8e7c 4cf8 673d 1bf1 bda4  : .D...|L.g=....
+00002ea0: 9186 97df d251 5f88 dfe0 b4c8 92a6 6aab  .....Q_.......j.
+00002eb0: 59f7 2aa9 8a41 1ca3 c614 9d88 0e74 6a2b  Y.*..A.......tj+
+00002ec0: 3fd9 81cb 1d5b 60c0 a0e7 029f 610f 4430  ?....[`.....a.D0
+00002ed0: 525f c215 9440 3fb2 91fd 79d8 0065 f378  R_...@?...y..e.x
+00002ee0: 355e 4c07 7f07 c747 22da fab0 4a3e b656  5^L....G"...J>.V
+00002ef0: 5929 a234 af3d 6f57 237a 32f5 b59e 8f9a  Y).4.=oW#z2.....
+00002f00: d27b 348c eb6f 9ac6 6a97 b752 2c88 b25c  .{4..o..j..R,..\
+00002f10: 18ee 0867 08b3 4db2 1164 8871 38b0 8808  ...g..M..d.q8...
+00002f20: 668c 93eb 5cf6 d0f5 5e77 e155 e9a5 9e7e  f...\...^w.U...~
+00002f30: a6ae 466b f15e de76 27dd 652e cd8f 5a7f  ..Fk.^.v'.e...Z.
+00002f40: 1933 1a45 711e eb64 204b f0fe a45f b53b  .3.Eq..d K..._.;
+00002f50: f0f3 2cf9 6875 9525 d3ac b3de c66d 271b  ..,.hu.%.....m'.
+00002f60: cb78 a6b2 8542 d1eb f61b 6850 6499 1ec7  .x...B....hPd...
+00002f70: 4dfc c73a d8ef c783 7db5 316e 34ca d879  M..:....}.1n4..y
+00002f80: b7dc c895 dcb4 fbc7 799c c879 95a7 ca02  ........y..y....
+00002f90: fc4c 9517 3981 e728 8501 427d 0ff0 880a  .L..9..(..B}....
+00002fa0: e086 a10d 9840 a1e7 84d4 c338 7a7a e569  .....@.....8zz.i
+00002fb0: b6b5 415a 2fdf 2340 c405 42bd bc56 0a54  ..AZ/.#@..B..V.T
+00002fc0: fab3 6d61 f702 1498 3808 efaa 3f2b 2e93  ..ma....8...?+..
+00002fd0: 79a5 d2ff 590f 394a d1b4 9739 52d3 ac22  y...Y.9J...9R.."
+00002fe0: 6e0e 4d96 caca 5465 6cdd 3400 8b77 eab1  n.M...Tel.4..w..
+00002ff0: 6466 a572 a6f5 d5fe adf2 11d5 9170 36ba  df.r.........p6.
+00003000: 7985 3200 e215 2065 36d6 6377 4285 3751  y.2... e6.cwB.7Q
+00003010: 35d4 804a 56a8 0ea2 c682 5d50 91b8 89aa  5..JV.....]P....
+00003020: a106 54ba 4245 c446 26c4 7782 3523 3761  ..T.BE.F&.w.5#7a
+00003030: 35d6 00cb d660 0516 c686 87c2 6aac 0196  5....`......j...
+00003040: af60 3116 dc6c d843 6135 d600 6baf c1da  .`1..l.Ca5..k...
+00003050: 94ec ccd8 3658 8d35 c08a 15ac c6dc 9db2  ....6X.5........
+00003060: 2db0 1a6b 8075 d660 39b3 bf8b 328d d5b7  -..k.u.`9...2...
+00003070: d762 c264 67bd 881a 70f5 28bf 7fb6 d691  .b.dg...p.(.....
+00003080: 6b92 75bb 91ad 1f92 91e9 9891 fdaa ec94  k.u.............
+00003090: a31b 4999 3cd3 a48c 3981 51e4 2110 2024  ..I.<...9.Q.!. $
+000030a0: 0043 2402 d085 1408 8f61 9f22 8712 8f3f  .C$......a."...?
+000030b0: 6552 d69c cfe3 7c36 a4e4 3e5d 3e30 2563  eR....|6..>]>0%c
+000030c0: 0619 b4af 1505 1b29 9970 4199 1afd 7d35  .......).pA...}5
+000030d0: c113 abee fa2a 6603 ef5e e544 2655 995a  .....*f..^.D&U.Z
+000030e0: b95c ca7c 0744 b3cb 7723 9ece b366 77c0  .\.|.D..w#...fw.
+000030f0: e131 7817 6054 2d9a 6ebe 3322 dd01 319b  .1x.`T-.n.3"..1.
+00003100: 6d05 7cec 4a8b dd5a 69d1 671a d414 0997  m.|.J..Zi.g.....
+00003110: 84d0 032c b07d 1060 b53a 76b9 0f3c e442  ...,.}.`.:v..<.B
+00003120: e240 e287 2ef9 5195 960e f0bf 1671 a374  .@....Q......q.t
+00003130: 3fc4 785f 92df 27c6 39b2 b179 dedd 5e77  ?.x_..'.9..y..^w
+00003140: 0982 7416 78a9 bb5e eaae 97ba ebff 5577  ..t.x..^......Uw
+00003150: f1bb ea2e f64c 5334 5455 8be3 e310 2004  .....LS4TU.... .
+00003160: 85fa 474c 0200 11a7 0085 14a9 f4a5 0c63  ..GL...........c
+00003170: ee53 d75d 9b69 d93c 711f 9c96 6fa9 bdd6  .S.].i.<q...o...
+00003180: d2f2 4bed f552 7bdd 3bb6 ed31 b683 b893  ..K..R{.;..1....
+00003190: 1b81 cd9f eb29 97f0 422c 6c07 84be 8000  .....)..B,l.....
+000031a0: 61cc 8007 a90b 0822 98bb 30f2 c2e0 079c  a......"..0.....
+000031b0: afa6 5d5f 79ad fdb5 42fd b1f6 ad01 6e4e  ..]_y...B.....nN
+000031c0: dd77 8cc2 599e f6de 3241 22ee f921 a084  .w..Y...2A"..!..
+000031d0: ab1d 26d4 060e 2702 b83e c301 b543 4720  ..&...'..>...CG 
+000031e0: fff3 f822 2155 1c76 5921 a3ec c3a2 9147  ..."!U.vY!.....G
+000031f0: 8bce 50b8 a130 a514 ab2d 3a3f 9771 7915  ..P..0...-:?.qy.
+00003200: e3dd 0186 184f 219b 627b a536 65c3 e3eb  .....O!.b{.6e...
+00003210: 4d8c 7a8b aa4a 678b 75c5 d9cf 5471 9ec7  M.z..Jg.u...Tq..
+00003220: 3c0f 0508 60e8 22e0 7b82 aaed e736 a03c  <...`.".{....6.<
+00003230: a021 133e a6de 0f38 579d 75cd b662 1f7d  .!.>...8W.u..b.}
+00003240: e390 f53e aa7b 5caa 9d91 ea93 3c4b a5f5  ...>.{\.....<K..
+00003250: 6e51 9c5d 235c 3cd7 da21 103e 0c5c 1b30  nQ.]#\<..!.>.\.0
+00003260: 5bd8 4055 d054 9fa6 73c0 84eb 84a1 fa10  [.@U.T..s.......
+00003270: e749 6b87 9ef0 364f d59e 6de5 fc1b a738  .Ik...6O..m....8
+00003280: 0fca 349c 7ac4 0920 01ca 7702 029f aa2d  ..4.z.. ..w....-
+00003290: 27a1 0b10 139e e7b8 bec3 19bb ca34 ada6  '............4..
+000032a0: b454 d6ed 9a60 be7e f9e7 97af 5ffe 7d84  .T...`.~...._.}.
+000032b0: ec62 2ee3 9bcf 71d7 4d6b d08e b296 635f  .b....q.Mk....c_
+000032c0: 78ea df38 8d00 0d1c 1bb8 1167 2062 8452  x..8.......g b.R
+000032d0: 15bd ae4f 42ad 9d1a d19b da51 9dbb 69a7  ...OB......Q..i.
+000032e0: aece 6553 5799 793d 8ce0 209f 65ac 2b10  ..eSW.y=.. .e.+.
+000032f0: 8770 2a18 1e9f 07bd 4456 c66a de4f b4fb  .p*.....DV.j.O..
+00003300: ea9a 376f e3fa 6869 3452 9802 ca37 5db5  ..7o..hi4R...7].
+00003310: d665 3f74 3544 bb3e be0e 3ff8 0f00 00ff  .e?t5D.>..?.....
+00003320: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00003330: 0030 0f61 31db 0300 0014 0c00 0021 0000  .0.a1........!..
+00003340: 0070 7074 2f73 6c69 6465 4c61 796f 7574  .ppt/slideLayout
+00003350: 732f 736c 6964 654c 6179 6f75 7436 2e78  s/slideLayout6.x
+00003360: 6d6c cc56 db6e dc36 107d 2fd0 7f10 d467  ml.V.n.6.}/....g
+00003370: 5a12 2fba 2cb2 0e74 2d1a 38b1 d175 3e80  Z./.,..t-.8..u>.
+00003380: 91b8 5e21 ba95 e26e bc0d 0ce4 b7da cfc9  ..^!...n........
+00003390: 9774 4849 b613 bb80 1f6c c02f 2245 cd0c  .tHI.....l./"E..
+000033a0: cfcc 391c f1cd dbeb b6b1 0e42 8e75 dfad  ..9........B.u..
+000033b0: 6def c4b5 2dd1 957d 5577 576b fbe3 6581  m...-..}UwWk..e.
+000033c0: 42db 1a15 ef2a def4 9d58 db47 31da 6f4f  B....*...X.G1.oO
+000033d0: 7ffd e5cd b01a 9bea 8c1f fbbd b220 4637  ............. F7
+000033e0: aef8 dade 2935 ac1c 672c 77a2 e5e3 493f  ....)5..g,w...I?
+000033f0: 880e be6d 7bd9 7205 aff2 caa9 24ff 02b1  ...m{.r.....$...
+00003400: dbc6 c1ae eb3b 2daf 3b7b f697 4ff1 efb7  .....;-.;{..O...
+00003410: dbba 1459 5fee 5bd1 a929 8814 0d57 807f  ...Y_.[..)...W..
+00003420: dcd5 c3b8 441b 9e12 6d90 6284 30c6 fb47  ....D...m.b.0..G
+00003430: 48ea 3840 b6aa 568d 38ef 9aa3 6d19 5379  H.8@..V.8...m.Sy
+00003440: 8045 cf3e 85ec cb4d 5359 1d6f 61e1 525b  .E.>...MSY.oa.R[
+00003450: 59c6 4c7f 1987 4b29 849e 7587 dfe5 b019  Y.L...K)..u.....
+00003460: 2ea4 71f8 70b8 9056 5de9 00b3 a3ed cc1f  ..q.p..V].......
+00003470: 6633 f3da 1dcc c4f9 c9fd 6a99 f2d5 f556  f3........j....V
+00003480: b67a 845a 58d7 6b1b 283b eaa7 a3d7 c4b5  .z.ZX.k.(;......
+00003490: b2ca 69b1 bc5b 2d77 e78f d896 bbfc 116b  ..i..[-w.......k
+000034a0: 67d9 c0b9 b7a9 ce6a 02f7 301d bca4 33d5  g......j..0...3.
+000034b0: 4197 c7e0 381b d582 682f ebb5 fdb5 2870  A...8...h/....(p
+000034c0: c2f2 82a2 0266 88ba 0945 494e 2354 6012  .....f...EIN#T`.
+000034d0: e638 2852 4cfc 1bed edf9 ab52 0ac3 ca1f  .8(RL......R....
+000034e0: d5a2 2ecf 7fc0 685b 97b2 1ffb ad3a 29fb  ......h[.....:).
+000034f0: 7696 c6a2 3020 d3a3 3399 1ae5 571c d184  v...0 ..3...W...
+00003500: 15d4 476e e6a7 88e1 3843 b4f0 180a bd34  ..Gn....8C.....4
+00003510: 202c 0a7d 9ae5 3773 0100 f332 9a2c 9c39   ,.}..7s...2.,.9
+00003520: df39 f185 8871 38eb cbcf a3d5 f540 94e6  .9...q8......@..
+00003530: 75e2 edd6 6222 538f c3ee bea2 66bb e9a3  u...b"S.....f...
+00003540: 99dc 5579 5681 ba4e faea a837 f904 a359  ..UyV..N...7...Y
+00003550: e4ab 6654 1b75 6c84 7919 f4c3 c090 4044  ..fT.ul.y.....@D
+00003560: c3f5 8115 1dfa b899 c855 a769 5397 9f2d  .........U.iS..-
+00003570: d55b a2aa 95f5 9e8f 4a48 cbec 0f27 1aa2  .[......JH...'..
+00003580: e804 a734 4d14 d155 175c f23f ef07 7b77  ...4M..U.\.?..{w
+00003590: 3117 6430 3817 50ce 2287 ff17 0559 4491  1.d08.P."....YD.
+000035a0: 7125 ac8b 8697 62d7 3715 20c0 af54 1f61  q%....b.7. ..T.a
+000035b0: cc02 1644 05c2 3863 c8cd 4317 c549 e823  ...D..8c..C..I.#
+000035c0: ec66 ae97 146e c2d2 e0e5 f551 29e8 b77f  .f...n.....Q)...
+000035d0: 4326 bcd9 6a60 7038 bde9 583e 8b5e b6d0  C&..j`p8..X>.^..
+000035e0: b44c b62c 2485 9fa4 39a2 c487 0a13 1aa0  .L.,$...9.......
+000035f0: c827 218a 5386 331a e411 1c8b 9ba5 0d56  .'!.S.3........V
+00003600: c0a1 aa5b 51d4 577b 29ce f7ca 50f8 83ec  ...[Q.W{)...P...
+00003610: 4029 d6d8 aab4 11bc bb6d 30ea 14bb 183b  @).......m0....;
+00003620: 2e73 7070 a736 c0f0 fc7a a38b de8a bed7  .spp.6...z......
+00003630: 3abf af38 f24a 15e7 d334 4e8b 8220 cf07  :..8.J...4N.. ..
+00003640: 0e62 d775 8188 88a1 c04d 7190 9134 4959  .b.u.....Mq..4IY
+00003650: f8f2 8adb 2a39 49ee af3d 9750 ba45 758b  ....*9I..=.P.Eu.
+00003660: ef33 a8ee 79a9 660b d59b a6ae 84f5 61df  .3..y.f.......a.
+00003670: 7efa 8970 fa4a 094f 0821 c070 8470 1c46  ~..p.J.O.!.p.p.F
+00003680: 28c1 6e82 bc2c 833e 435c 3f4e 731f 1316  (.n..,.>C\?Ns...
+00003690: bf3c e170 6f83 9a3d ca39 7e81 4ee3 d384  .<.po..=.9~.N...
+000036a0: 4499 4b50 98c2 234b 2994 9ce4 31f2 5898  D.KP..#K)...1.X.
+000036b0: 2451 9c46 3e63 b79d 66d4 9476 80ee a90d  $Q.F>c..f..v....
+000036c0: e6fb b77f 7efb feed df67 e82e 6658 6e6e  ....~....g..fXnn
+000036d0: 4bd5 cd6c d60e a0f5 711a 2628 f168 8168  K..l....q.&(.h.h
+000036e0: 1605 282e 7c86 0a46 284d 9330 4e49 aeb5  ..(.|..F(M.0NI..
+000036f0: 3378 f4a1 7660 f169 da19 fa2f 420e 7d6d  3x..v`.i.../B.}m
+00003700: 2eb7 9e3b cbe7 c01b b868 055e 8859 e491  ...;.....h.^.Y..
+00003710: 85a6 4923 7768 35f1 1b9d 3f8c 8d7c cf87  ..I#wh5...?..|..
+00003720: f383 1149 6bfe fda9 591a b430 27d3 3b13  ...Ik...Y..0'.;.
+00003730: 9dfb 729b 3ffd 0f00 00ff ff03 0050 4b03  ..r.?........PK.
+00003740: 0414 0006 0008 0000 0021 0002 35ef b587  .........!..5...
+00003750: 0300 00f6 0900 0021 0000 0070 7074 2f73  .......!...ppt/s
+00003760: 6c69 6465 4c61 796f 7574 732f 736c 6964  lideLayouts/slid
+00003770: 654c 6179 6f75 7437 2e78 6d6c cc96 db6e  eLayout7.xml...n
+00003780: dc36 1086 ef0b f41d 04f5 9ad6 8992 a845  .6.............E
+00003790: d681 a843 d1c2 8d17 75fa 00b4 c4f5 0ad1  ...C....u.......
+000037a0: a914 77b3 dbc0 405e ab79 9c3c 4986 9468  ..w...@^.y.<I..h
+000037b0: a7b6 0bf8 c206 7223 52a3 1972 66be 5f94  ......r#R..rf._.
+000037c0: debc 3d76 ad75 e062 6a86 7e6d 7b67 ae6d  ..=v.u.bj.~m{g.m
+000037d0: f1be 1aea a6bf 59db 7fbd 2f11 b1ad 49b2  ......Y.../...I.
+000037e0: be66 edd0 f3b5 7de2 93fd f6fc e79f de8c  .f....}.........
+000037f0: aba9 ad2f d869 d84b 0bd6 e8a7 155b db3b  .../.i.K.....[.;
+00003800: 29c7 95e3 4cd5 8e77 6c3a 1b46 dec3 b3ed  )...L..wl:.F....
+00003810: 203a 26e1 56dc 38b5 601f 61ed ae75 7cd7   :&.V.8.`.a..u|.
+00003820: 8d9c 8e35 bdbd c48b e7c4 0fdb 6d53 f17c  ...5........mS.|
+00003830: a8f6 1def e5bc 88e0 2d93 90ff b46b c6c9  ........-....k..
+00003840: ac36 3e67 b551 f009 96d1 d1ff 4d49 9e46  .6>g.Q......MI.F
+00003850: a8f6 ba65 fd07 dbd2 6ee2 0006 cf3e 87ca  ...e....n....>..
+00003860: abab b6b6 7ad6 8181 6a0f 659c c6f7 8273  ....z...j.e....s
+00003870: 35eb 0fbf 8af1 6adc 08ed fbee b011 5653  5.....j.......VS
+00003880: abd8 25c6 7696 078b 9bbe ed0f 7ae2 3c08  ..%.v.......z.<.
+00003890: bf31 53b6 3a6e 45a7 4668 8175 5cdb 40ea  .1S.:nE.Fh.u\.@.
+000038a0: a4ae 8eb2 f1a3 b4aa d958 dd5b abdd e513  .........X.[....
+000038b0: bed5 ae78 c2db 311b 38df 6daa aa9a 937b  ...x..1.8.m....{
+000038c0: 5c8e 6fca c999 e4d6 a665 15df 0d6d cd85  \.o......e...m..
+000038d0: a59a a453 ba98 a449 6e2f 9ab5 fda9 2c7d  ...S...In/....,}
+000038e0: 1a16 2546 25cc 1076 2946 b4c0 092a fd80  ..%F%..v)F...*..
+000038f0: 147e 5c66 7e10 ddaa 682f 5a55 826b 2ebf  .~\f~...h/ZU.k..
+00003900: d546 5f5e f488 69d7 5462 9886 ad3c ab86  .F_^..i.Tb...<..
+00003910: 6e11 87d1 18e0 f4f0 8253 25fc 89e2 ac28  n........S%....(
+00003920: 0875 511e 900c 8561 9aa2 3c4e 08ca 8b24  .uQ....a..<N...$
+00003930: ca0a bfc4 614c 6e97 5e40 ce66 d455 384b  ....aLn.^@.f.U8K
+00003940: e94b 0f0c 9369 bc18 aa0f 93d5 0fc0 4c21  .K...i........L!
+00003950: 9e11 de79 cc5c d538 ee16 4dd5 12de a87f  ...y.\.8..M.....
+00003960: a012 d66e 5562 c0c1 9b09 1867 3db9 07b0  ...nUb.....g=...
+00003970: 0844 1ee9 509f d4a6 d730 6a23 5bb5 93bc  .D..P....0j#[...
+00003980: 92a7 96eb 9b51 5db6 204d 5d6d 4882 32a2  .....Q]. M]mH.2.
+00003990: 5981 7010 4187 031c a324 0a08 4ab3 d0cf  Y.p.A....$..J...
+000039a0: 715c 24c4 cb6e 8dd0 6b60 289b 8e97 cdcd  q\$..n..k`(.....
+000039b0: 5ef0 cbbd d408 05a0 067d c349 c07b f4fb  ^........}.I.{..
+000039c0: 06f2 ee64 d672 d6df 6949 9efb aeef 3b6e  ...d.r..iI....;n
+000039d0: e8f8 b16a d7dc 34c8 4173 efeb 0d13 eccf  ...j..4.As......
+000039e0: 07ab cc0d 1e75 9da6 28c7 28ed fff5 1618  .....u..(.(.....
+000039f0: bd95 c320 4165 df2b ceff 4115 17a5 31f6  ... Ae.+..A...1.
+00003a00: a897 212f a704 9579 9ca2 3880 dd8b 88d0  ..!/...y..8.....
+00003a10: 20a5 2474 f3ec f515 b795 6296 dcdf 7b26   .$t......b...{&
+00003a20: a075 4675 26f6 0554 f7b2 a8b1 417d d536  .uFu&..T....A}.6
+00003a30: 35b7 deed bbeb 07c0 831f 1478 4ae2 3406  5..........xJ.4.
+00003a40: 23c2 248a 5049 931c 95d8 2528 8cd2 8c06  #.$.PI....%(....
+00003a50: 24f4 7011 bd3e 70f8 3243 cf9e 64ee bfc2  $.p..>p.2C..d...
+00003a60: 4913 611a 24b9 1b20 92c1 25cf 30b4 3c28  I.a.$.. ..%.0.<(
+00003a70: 52e4 8584 d224 cd92 280c ef4e 9a49 21ed  R....$..(..N.I!.
+00003a80: 21bb e71e 305f 3fff fbcb d7cf 5f5e e074  !...0_?....._^.t
+00003a90: d183 f948 9bae ebd9 a21d c836 f233 4211  ...H.......6.3B.
+00003aa0: f570 8970 9ec4 282d a310 9561 8071 4649  .p.p..(-...a.qFI
+00003ab0: 9a05 85d2 cee8 e1c7 da01 e3f3 b433 0e1f  .............3..
+00003ac0: b918 8746 ffbe 78ee 229f 036b e18c 8be2  ...F..x."..k....
+00003ad0: 380c 02df 270b a659 23f7 d92a f057 aa7e  8...'..Y#..*.W.~
+00003ae0: 185b f107 1b2f 0f5a 24b0 1940 ceb4 6954  .[.../.Z$..@..iT
+00003af0: c29c 5def 5d54 ede6 7fed fc1b 0000 00ff  ..].]T..........
+00003b00: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00003b10: 0074 a5ee 2eb2 0500 0078 1700 0021 0000  .t.......x...!..
+00003b20: 0070 7074 2f73 6c69 6465 4c61 796f 7574  .ppt/slideLayout
+00003b30: 732f 736c 6964 654c 6179 6f75 7438 2e78  s/slideLayout8.x
+00003b40: 6d6c cc58 ed72 9b46 14fd df99 be03 a3fe  ml.X.r.F........
+00003b50: 2662 3f80 c513 3b03 083a ed38 89a7 721e  &b?...;..:.8..r.
+00003b60: 00c3 caa2 e1ab b092 e566 3293 d76a 1f27  .........f2..j.'
+00003b70: 4fd2 bb0b 2b4b b262 298e 3df5 1fb8 a0b3  O...+K.b).=.....
+00003b80: 87bb 7b0e f72e 7afd 6655 16c6 92b7 5d5e  ..{...z.fU....]^
+00003b90: 57a7 23f4 ca1a 19bc 4aeb 2caf ae4f 471f  W.#.....J.,..OG.
+00003ba0: 2e63 938d 8c4e 2455 9614 75c5 4f47 b7bc  .c...N$U..u.OG..
+00003bb0: 1bbd 39fb f9a7 d7cd 4957 64e7 c96d bd10  ..9.....IWd..m..
+00003bc0: 0670 54dd 4972 3a9a 0bd1 9c8c c75d 3ae7  .pT.Ir:......]:.
+00003bd0: 65d2 bdaa 1b5e c16f b3ba 2d13 0197 edf5  e....^.o..-.....
+00003be0: 386b 931b e02e 8b31 b62c 675c 2679 351a  8k.....1.,g\&y5.
+00003bf0: c6b7 c78c af67 b33c e593 3a5d 94bc 123d  .....g.<..:]...=
+00003c00: 49cb 8b44 40fe dd3c 6f3a cdd6 1cc3 d6b4  I..D@..<o:......
+00003c10: bc03 1a35 7a3b 2571 dbc0 6ceb ab3f 2f57  ...5z;%q..l..?/W
+00003c20: 2343 c1da 25dc 40a3 3398 793a 2d32 a34a  #C..%.@.3.y:-2.J
+00003c30: 4ab8 11d6 9500 06e3 2617 7323 4c1a c9a4  J.......&.s#L...
+00003c40: 305d 73d9 722e a36a f96b db4c 9b8b 560d  0]s.r..j.k.L..V.
+00003c50: 7db7 bc68 8d3c 9354 03c5 683c fc30 c0d4  }..h.<.T..h<.0..
+00003c60: 65b5 54c1 7867 f8b5 0e93 93d5 ac2d e519  e.T.xg.......-..
+00003c70: 56c4 589d 8e40 b85b 791c cb7b 7c25 8cb4  V.X..@.[y..{|%..
+00003c80: bf99 dedd 4de7 eff7 60d3 79b4 073d d60f  ....M...`.y..=..
+00003c90: 186f 3c54 ceaa 4fee fe74 b09e ce65 2e0a  .o<T..O..t...e..
+00003ca0: 6ec8 8552 799c 7742 67b4 68f3 d3d1 a738  n..Ry.wBg.h....8
+00003cb0: c681 1dc5 d48c 2132 a915 5033 88a8 67c6  ......!2..P3..g.
+00003cc0: 98b0 08bb 7188 89f3 598e 46ce 49da 72a5  ....q...Y.F.I.r.
+00003cd0: cd6f 99f6 1872 eee9 5ae6 695b 77f5 4cbc  .o...r..Z.i[w.L.
+00003ce0: 4aeb 7230 88f6 1948 8ae8 20a9 ccf2 53ec  J.r0...H.. ...S.
+00003cf0: b991 edc5 b189 2ddb 356d ec44 663c 41ae  ......-.5m.Df<A.
+00003d00: e939 13e2 7bcc 452c 649f 8705 809c f559  .9..{.E,d......Y
+00003d10: cd62 3ccc 7798 b816 a26b ceeb f463 6754  .b<.w....k...cgT
+00003d20: 3508 2575 ed75 5b23 7a31 e5b9 990f be12  5.%u.u[#z1......
+00003d30: 728d 065c ffa3 0aee 5679 afc4 8c78 2e63  r..\....Vy...x.c
+00003d40: 4a3b 6abb 60d6 6db1 8947 3026 6e2f 2272  J;j.`.m..G0&n/"r
+00003d50: 2c6b 406c 4ad9 3337 2762 15d4 d9ad 1c7d  ,k@lJ.37'b.....}
+00003d60: 0567 9030 a9d2 790d 6fe0 55cf 5974 622a  .g.0..y.o.U.Ytb*
+00003d70: 6e0b aee2 6581 8684 323e fb03 c0dd dff0  n...e...2>......
+00003d80: b43b f635 40c6 1b03 1b79 50e3 5a18 5424  .;.5@....yP.Z.T$
+00003d90: b2a4 f0ca fc30 ed9f 21ce c222 4f3f 1aa2  .....0..!.."O?..
+00003da0: 3678 960b e36d d209 de1a 6a6d a0e6 0089  6x...m....jm....
+00003db0: 24ec 2550 2cbc ca2e 9236 9119 acc9 7ebf  $.%P,....6....~.
+00003dc0: 1892 68d4 fcf4 bcd4 541f 362c d186 d5af  ..h.....T.6,....
+00003dd0: f045 91a4 7c5e 1719 2481 5fa8 7d29 627e  .E..|^..$._.})b~
+00003de0: 4c5c 6c3a 018d ccd0 0943 c883 c0a5 e7db  L\l:.....C......
+00003df0: c8c2 9eed 05e8 39ed 9b67 ab3b c8f1 ceb5  ......9..g.;....
+00003e00: 1123 68b0 2ebc 6414 dbdb d675 908b a59f  .#h...d....u....
+00003e10: 9475 2973 89d3 238e b1ee 0ff8 5585 f83e  .u)s..#.....U..>
+00003e20: 16b3 4dac 0640 48f6 60e9 2656 0320 a47b  ..M..@H.`.&V. .{
+00003e30: b0d6 2656 0320 b40f 6135 0042 e710 5603  ..&V. ..a5.B..V.
+00003e40: 2074 0f61 3500 4276 08ab 0110 7a87 b03d   t.a5.Bv....z..=
+00003e50: 605f 3d68 e4db bb2c d6ed e7fb eb83 348d  `_=h...,......4.
+00003e60: 2a0f dd56 7de8 6bc0 ee53 9457 1f7e ca94  *..V}.k..S.W.~..
+00003e70: a775 9519 055f f2e2 0846 7c98 f172 9eb7  .u..._...F|..r..
+00003e80: c713 92c3 8471 bd68 617f 712c 233d 8231  .....q.ha.q,#=.1
+00003e90: 9fed 257c ea2a 4bd7 db02 29db 6689 252f  ..%|.*K...).f.%/
+00003ea0: b4c4 62ea 7b81 3d99 98ae 1578 6648 26b6  ..b.{.=....xfH&.
+00003eb0: 6979 7088 2382 6d0f 91c0 b5c3 e7df 21c8  iyp.#.m.......!.
+00003ec0: da36 522f d63c 2966 32b5 d560 bdc7 6e19  .6R/.<)f2..`..n.
+00003ed0: e486 67a8 55df d833 1086 900d e81f 2cbc  ..g.U..3......,.
+00003ee0: 4699 b4e7 6a37 9957 1934 5619 aa51 8b77  F...j7.W.4V..Q.w
+00003ef0: f009 a146 6dd4 0db9 51f9 665d 1ea8 86dd  ...Fm...Q.f]....
+00003f00: ce71 7c5b f578 a776 0f7c 1ea2 1275 1cdf  .q|[.x.v.|...u..
+00003f10: 56df d8a9 ef03 1f22 ae9a c671 840f 3501  V......"...q..5.
+00003f20: 4dc8 3093 3de8 1184 3b9d 6220 c498 3912  M.0.=...;.b ..9.
+00003f30: f608 c29d 76a2 095d aa3a ea23 0877 7ace  ....v..].:.#.wz.
+00003f40: 4028 d98e 17e5 a1c6 a409 1ddb 7da4 28ff  @(..........}.(.
+00003f50: 5bf7 fabe da6a ebda 3a49 04df aaad f485  [....j..:I......
+00003f60: d656 9bf8 31f6 2c66 122b 4466 4c88 6532  .V..1.,f.+DfL.e2
+00003f70: db71 4cea f90e a3f0 f4c0 a3cf 5f5b 3371  .qL........._[3q
+00003f80: afb2 a25e fd6f 9656 f54d fe60 0154 17ca  ...^.o.V.M.`.T..
+00003f90: 23b3 221b 66cb 48ec 0461 6452 e2c0 0a13  #.".f.H..adR....
+00003fa0: 2a3f 3309 33fd d0c6 13ea 461e 43d0 4974  *?3.3.....F.C.It
+00003fb0: 52a0 a1c8 4b1e e7d7 8b96 bf5f 0825 e196  R...K......_.%..
+00003fc0: b5a0 0b1b 5d29 c282 27d5 da81 e20c 5b18  ....])..'.....[.
+00003fd0: 8f2d 7b8c dd3b 4741 0e4f dfcb 1ded b7b8  .-{..;GA.O......
+00003fe0: aea5 9737 1d67 bfd4 6e1e c621 f55d 58f9  ...7.g..n..!.]X.
+00003ff0: 085a 7a14 62c8 2374 2368 e90c 1114 3212  .Zz.b.#t#h....2.
+00004000: fad6 f33b 6e26 dade 727f 2d92 1696 4ebb  ...;n&..r.-...N.
+00004010: eec0 97d4 f7b8 ee69 a576 b5d4 d322 cfb8  .......i.v..."..
+00004020: f16e 515e ed08 eebc 54c1 bd89 8722 1b99  .nQ^....T...."..
+00004030: 3ec3 bee9 4d82 0054 8fe0 4023 3fb0 6ce4  >...M..T..@#?.l.
+00004040: 4798 3cbf e05d 91c1 9aed d5fc c026 ee51  G.<..].......&.Q
+00004050: 95c6 a101 f126 1631 5908 8749 4861 c949  .....&.1Y..IHa.I
+00004060: e49b b09d 0b02 cf0f 3dc7 b6d7 95a6 9392  ........=.......
+00004070: 5690 ddb1 05e6 eb97 7f7e f9fa e5df 27a8  V........~....'.
+00004080: 2eea a4ff 17d5 abae a2c1 3b90 ad83 4316  ..........;...C.
+00004090: 9801 a2b1 4927 9e6b fab1 039b 6f9b 501a  ....I'.k....o.P.
+000040a0: 06cc 0f49 24bd d320 7adf 3b70 f338 ef34  ...I$.. z.;p.8.4
+000040b0: f50d 6f9b 3a57 7f20 236b b0cf 3291 9f4e  ..o.:W. #k..2..N
+000040c0: d875 2de6 604f abdc 7be4 2e5b 29fc 54ce  .u-.`O..{..[).T.
+000040d0: 1fce 45fb 3669 de2f 9549 4ad5 df43 75ab  ..E.6i./.IJ..Cu.
+000040e0: 91c6 eca1 7710 3977 fd8f f9d9 7f00 0000  ....w.9w........
+000040f0: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+00004100: 2100 202f 572a 8405 0000 2717 0000 2100  !. /W*....'...!.
+00004110: 0000 7070 742f 736c 6964 654c 6179 6f75  ..ppt/slideLayou
+00004120: 7473 2f73 6c69 6465 4c61 796f 7574 392e  ts/slideLayout9.
+00004130: 786d 6ccc 58dd 729b 3818 bddf 997d 0786  xml.X.r.8....}..
+00004140: bd56 8d7e 9132 4d3a 8061 673b 699b d9a4  .V.~.2M:.ag;i...
+00004150: 0f40 01c7 4cf9 5b90 5d67 3b9d e96b ed3e  .@..L.[.]g;..k.>
+00004160: 4e9f 6425 01b6 6992 d64d 9d9d dc80 2c3e  N.d%..i..M....,>
+00004170: 1dbe 4fe7 e848 f8f9 8b4d 5958 ebac edf2  ..O..H...MYX....
+00004180: ba3a b5e1 33c7 b6b2 2aa9 d3bc ba3e b5df  .:..3...*....>..
+00004190: 5e45 80db 5627 e32a 8d8b baca 4eed 9bac  ^E..V'.*....N...
+000041a0: b35f 9cfd facb f3e6 a42b d2f3 f8a6 5e49  ._.......+....^I
+000041b0: 4b61 54dd 497c 6a2f a56c 4e66 b32e 5966  KaT.I|j/.lNf..Yf
+000041c0: 65dc 3dab 9bac 52cf 1675 5bc6 52fd 6caf  e.=...R..u[.R.l.
+000041d0: 6769 1b7f 50d8 6531 438e c366 659c 57f6  gi..P.e1C..fe.W.
+000041e0: 30be 3d64 7cbd 58e4 4936 af93 5599 55b2  0.=d|.X.I6..U.U.
+000041f0: 0769 b322 962a ff6e 9937 dd88 d61c 82d6  .i.".*.n.7......
+00004200: b459 a760 cce8 694a f2a6 51d5 3679 72b5  .Y.`..iJ..Q.6yr.
+00004210: b12d 13d6 ae55 07b4 cf54 e5c9 6591 5a55  .-...U...T..e.ZU
+00004220: 5caa 8e8b 3c91 ab36 b33e e472 6905 71a3  \...<..6.>.ri.q.
+00004230: 914c 4cd7 5cb5 59a6 5bd5 faf7 b6b9 6c2e  .LL.\.Y.[.....l.
+00004240: 5a33 f4f5 faa2 b5f2 5443 0d10 f66c 7830  Z3......TC...lx0
+00004250: 8499 9fd5 da34 665f 0dbf 1e9b f1c9 66d1  .....4f_......f.
+00004260: 96fa ae66 c4da 9cda 8ab8 1b7d 9de9 be6c  ...f.......}...l
+00004270: 23ad a4ef 4c76 bdc9 f2cd 1db1 c932 bc23  #...Lv.......2.#
+00004280: 7a36 be60 b6f7 525d 559f dced 72d0 58ce  z6.`..R]U...r.X.
+00004290: 552e 8bcc d213 65f2 38ef e498 d1aa cd4f  U.....e.8......O
+000042a0: ed8f 5184 7c1a 4604 44aa 0588 e313 e087  ..Q.|.F.D.......
+000042b0: 4480 0861 1e22 370a 1066 9ff4 68c8 4e92  D..a."7..f..h.N.
+000042c0: 3633 dcfc 918e 1a83 ec16 af65 9eb4 7557  63.........e..uW
+000042d0: 2fe4 b3a4 2e07 818c 3a53 9442 3250 aab3  /.......:S.B2P..
+000042e0: fce8 5316 7202 e780 055e 0822 e246 0079  ..S.r....^.".F.y
+000042f0: d801 c49f aba4 5cc4 8517 7c1a 2640 e53c  ......\...|.&@.<
+00004300: de4d 15b3 a1de a1f0 9188 ae39 af93 f79d  .M.........9....
+00004310: 55d5 8a28 cd6b cfdb 36a2 2753 df9b e5a0  U..(.k..6.'S....
+00004320: 2ba9 e768 88eb 1f9a c66e 96ef a498 63e1  +..h.....n....c.
+00004330: 726e b823 d455 629d 928d 0546 08bb 3d89  rn.#.Ub....F..=.
+00004340: 9039 ce10 b14f 658f dc9c c88d 5fa7 377a  .9...Oe....._.7z
+00004350: f43b 7557 14c6 55b2 acd5 0a7c d763 169d  .;uW..U....|.c..
+00004360: bc94 3745 66da eb02 0e09 a5d9 e24f 15dc  ..7Ef........O..
+00004370: fdad deb6 43df 06e8 f6de c046 5fcc b856  ....C......F_..V
+00004380: 0d2a 626d 2959 05de 5ef6 ef90 6741 9127  .*bm)Y..^...gA.'
+00004390: ef2d 595b 599a 4beb 55dc c9ac b5cc dc28  .-Y[Y.K.U......(
+000043a0: cf51 201a b0a7 c0a0 6455 7a11 b7b1 ce60  .Q .....dUz....`
+000043b0: 0bf6 f262 48a2 31f5 8d75 9952 bf2d 583c  ...bH.1..u.R.-X<
+000043c0: 0a76 5cc2 1745 9c64 cbba 4855 12e8 89ca  .v\..E.d..HU....
+000043d0: 1763 cff1 19c3 00f9 3802 0e76 0870 2077  .c......8..v.p w
+000043e0: 800b 2982 fe1c 8b80 3b8f 2f5f 658b 3a9f  ..).....;./_e.:.
+000043f0: cd2e fa70 1153 c831 1c54 2cb8 4b10 9daa  ...p.S.1.T,.K...
+00004400: 9841 1769 6919 1513 ee62 d647 1ca2 e2fb  .A.ii....b.G....
+00004410: a46b 9571 7b6e fc2d af52 e5f7 ba69 46ad  .k.q{n.-.R...iF.
+00004420: 5eab 4dcd 8cfa 8eb2 4d13 eda0 86f5 7710  ^.M.....M.....w.
+00004430: 1ee2 fb78 1a64 c0c3 3b3c 0109 3918 4f47  ...x.d..;<..9.OG
+00004440: 6ef1 34c8 8047 7678 10bb da01 0e04 74f6  n.4..Gvx......t.
+00004450: 0135 ca00 48f7 0039 e2ba 8e07 006a 9401  .5..H..9.....j..
+00004460: 90ed 0011 e24c 873d 0050 a30c 80ee 1ea0  .....L.=.P......
+00004470: 4b0c 730f 00d4 2803 20df 016a b4c3 4999  K.s...(. ..j..I.
+00004480: 006a 9401 50ec 0132 ea3e 9014 8d72 b7bf  .j..P..2.>...r..
+00004490: 1ed7 14c9 7617 d7eb 71df 11f1 1375 443e  ....v...q....uD>
+000044a0: e701 42cc 030e 8108 b8ae cf01 f6a8 0f3c  ..B............<
+000044b0: 651d 9108 9960 823f be23 6aff b10d 6fcb  e....`.?.#j...o.
+000044c0: b858 0ce6 887e 6687 470e 7587 857e cf16  .X...~f.G.u..~..
+000044d0: 8f39 8454 45ff afe6 685c e588 e608 2766  .9.TE...h\....'f
+000044e0: f6f3 e608 27e6 7d04 7384 c736 c729 e011  ....'.}.s..6.)..
+000044f0: cc71 0a78 0473 9c02 1ec1 1ca7 8047 30c7  .q.x.s.......G0.
+00004500: 29e0 fde6 a8e1 55c0 f65b e7c7 0fa3 7ae5  ).....U..[....z.
+00004510: 99b3 6837 398c 3ec4 5be9 e8ad f358 4e4f  ..h79.>.[....XNO
+00004520: 9be4 897a ab23 3011 9198 03e5 4542 d9aa  ...z.#0.....EB..
+00004530: e701 0f11 0a02 ee79 44b8 8453 9f3d beb7  .......yD..S.=..
+00004540: a6f2 96b3 c29e fd7b add5 7c42 7fd3 00cd  .......{..|B....
+00004550: 0fa3 9185 fa96 37d5 528e 23e6 0721 2098  ......7.R.#..! .
+00004560: a919 c6c4 0582 610e bc80 a239 7143 c1a1  ......a....9qC..
+00004570: fa34 1c93 521c cabc cca2 fc5a 7d3b bc59  .4..R......Z};.Y
+00004580: 4943 e144 5a6a 17b6 ba52 0645 1657 5b05  IC.DZj...R.E.W[.
+00004590: ca33 e420 3473 e80c b93b 45a9 1c8e bf97  .3. 4s...;E.....
+000045a0: b351 6f51 5d6b 2def 2b8e 3e51 c521 ea53  .QoQ]k-.+.>Q.!.S
+000045b0: 2a42 0a22 9f40 e038 8280 4084 1c40 ca3c  *B.".@.8..@..@.<
+000045c0: a5b6 8862 011f 5f71 0bd9 f692 fb6b 15b7  ...b.._q.....k..
+000045d0: 6aea 46d5 7de7 6be7 4754 775c aadd 91ea  j.F.}.k.GTw\....
+000045e0: cb22 4f33 ebf5 aa7c f715 e1ec 8912 ce5c  ."O3...|.......\
+000045f0: e186 4859 8c10 d401 1e51 2737 3cf7 3008  ..HY.....Q'7<.0.
+00004600: 5c97 841c 059e 60e1 e313 de15 a99a b33b  \.....`........;
+00004610: 39ff ce21 ee41 4ec3 888f c5dc c180 07ea  9..!.AN.........
+00004620: 320f 889a 721c 7a4a e5dc f785 1708 46e9  2...r.zJ......F.
+00004630: d669 3a4d 69a5 b23b d460 be7c fee7 b72f  .i:Mi..;.`.|.../
+00004640: 9fff 3d82 bb98 dbf8 37e6 38eb a635 6847  ..=.....7.8..5hG
+00004650: 65cb 50c0 7de0 4312 0132 172e f022 a656  e.P.}.C..2...".V
+00004660: 2fc5 8404 3ef7 021c 6aed 3490 dcd6 8eea  /...>...j.4.....
+00004670: 3c4c 3b4d fd21 6b9b 3a37 fff7 4267 90cf  <L;M.!k.:7..Bg..
+00004680: 3a2e fa03 b143 9052 d140 53af 915d b69a  :....C.R.@S..]..
+00004690: f84b 5dbf ba17 edab b879 b336 2229 cdfe  .K]......y.6")..
+000046a0: 1e98 ae46 0bb3 0fdd 85e8 dac7 3fb8 cffe  ...F........?...
+000046b0: 0300 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
+000046c0: 0000 0021 0067 b1dc 2872 0400 00c0 0f00  ...!.g..(r......
+000046d0: 0022 0000 0070 7074 2f73 6c69 6465 4c61  ."...ppt/slideLa
+000046e0: 796f 7574 732f 736c 6964 654c 6179 6f75  youts/slideLayou
+000046f0: 7431 302e 786d 6ccc 57db 8edb 3610 7d2f  t10.xml.W...6.}/
+00004700: d07f 10d4 67ae 2ea4 64c9 8837 d08d 458b  ....g...d..7..E.
+00004710: 4d76 516f face 48f4 5a88 6ea5 68c7 6eb0  MvQo..H.Z.n.h.n.
+00004720: 407e abfd 9c7c 4987 94b4 f734 4ee1 2df6  @~...|I....4N.-.
+00004730: 45a4 28f2 7066 ce99 21f5 eaf5 aeae 8c2d  E.(.pf..!......-
+00004740: 177d d936 0bd3 39b1 4d83 3779 5b94 cdd5  .}.6..9.M.7y[...
+00004750: c27c 7749 5160 1abd 644d c1aa b6e1 0b73  .|wIQ`..dM.....s
+00004760: cf7b f3f5 e98f 3fbc eae6 7d55 9cb1 7dbb  .{....?...}U..}.
+00004770: 9106 6034 fd9c 2dcc b594 dddc b2fa 7ccd  ..`4..-.......|.
+00004780: 6bd6 9fb4 1d6f e0db aa15 3593 f02a aeac  k....o....5..*..
+00004790: 42b0 8f80 5d57 966b dbbe 55b3 b231 c7f5  B...]W.k..U..1..
+000047a0: e290 f5ed 6a55 e63c 6df3 4dcd 1b39 8008  ....jU.<m.M..9..
+000047b0: 5e31 09f6 f7eb b2eb 27b4 ee10 b44e f01e  ^1......'....N..
+000047c0: 60f4 eafb 26c9 7d07 de42 60e4 e5ce 34f4  `...&.}..B`...4.
+000047d0: 3cb1 8511 c73c 05d7 f365 5518 0dab 61e0  <....<...eU...a.
+000047e0: b294 1537 2040 c6ef 30b9 cc59 655c f29d  ...7 @..0..Ye\..
+000047f0: d4d3 faee 5270 ae7a cdf6 67d1 2dbb 0ba1  ....Rp.z..g.-...
+00004800: 57bf dd5e 08a3 2c14 da88 625a e387 719a  W..^..,...bZ..q.
+00004810: 7e6d b6ba 633d 587e 3575 d97c b712 b56a  ~m..c=X~5u.|...j
+00004820: 212a c66e 6102 797b f5b4 d418 1861 e4c3  !*.na.y{.....a..
+00004830: 607e 3b9a afcf 9f98 9baf b327 665b d306  `~;........'f[..
+00004840: d69d 4d95 5783 718f dd71 2777 86a0 a858  ..M.W.q..q'w...X
+00004850: 693b ce7a 3959 b411 e5c2 fc44 a91b 7b19  i;.z9Y.....D..{.
+00004860: 2588 420f 113b 2628 ce48 88a8 8b83 cc9d  %.B..;&(.H......
+00004870: d1c4 c5fe b55a edf8 f35c 70cd cf2f c5a4  .....Z...\p../..
+00004880: 33c7 7fc4 6d5d e6a2 eddb 953c c9db 7a14  3...m].....<..z.
+00004890: c9a4 35a0 d521 23ad caca 4f49 80b1 9f78  ..5..!#...OI...x
+000048a0: 198a ddc0 46d4 2736 c249 3443 38cc 08c6  ....F.'6.I4C8...
+000048b0: a997 faee ec7a 0c00 d83c b5da 0b6b f477  .....z...<...k.w
+000048c0: 747c 22a2 efce dafc 436f 342d 10a5 781d  t|".....Co4-..x.
+000048d0: 78bb 9931 90a9 da6e 3d6a 4baa 188d f386  x..1...n=jK.....
+000048e0: 8fba 731b e551 0572 17b7 c55e 6df2 1e5a  ..s..Q.r...^m..Z
+000048f0: 3dc8 e655 2f97 725f 71fd d2a9 8736 4300  =..U/.r_q....6C.
+00004900: 1115 53a9 cb1b f46e 3990 2b4f 93aa cc3f  ..S....n9.+O...?
+00004910: 18b2 3578 514a e30d eb25 1786 de1f 721b  ..5xQJ...%....r.
+00004920: 5094 8383 9b1a 8537 c505 13ec b7bb 60bf  P......7......`.
+00004930: 5e8c 01e9 b49d 9351 d624 87af 8b02 4fa2  ^......Q.$....O.
+00004940: b897 1fc6 45c5 72be 6eab 024c 715f a850  ....E.r.n..Lq_.P
+00004950: 4810 b9b0 a58f 52db 7151 1c60 8abc 2c4c  H.....R.qQ.`..,L
+00004960: 519a 45b3 cc8e 7084 bdff 4128 8a76 d368  Q.E...p...A(.v.h
+00004970: 4509 956a 2849 cabc dded e2ef 518f aaf5  E..j(I......Q...
+00004980: 80c2 9962 63d0 c763 2d75 8af9 6d75 531e  ...bc..c-u..muS.
+00004990: be5f 5b8a 412d adfe 9eb6 06fd 3cdc 45fb  ._[.A-......<.E.
+000049a0: f1ef bb2c 79de 4289 adf8 9657 0720 badf  ...,y.B....W. ..
+000049b0: 46bc 5c97 e270 40fc 6d40 da6e 845c 1f8c  F.\..p@.m@.n.\..
+000049c0: 480e 402c 574f 021e 3b43 c994 a129 93fc  H.@,WO..;C...)..
+000049d0: 5e62 e217 9a98 a197 6419 713d e446 8e83  ^b......d.q=.F..
+000049e0: dc98 6628 8b23 07d9 d8c6 7198 d1d4 a6d1  ..f(.#....q.....
+000049f0: f327 6601 89d8 ff09 9eb0 6a35 a5e4 7070  .'f.......j5..pp
+00004a00: 1ea5 a2af e08e a1bd f5a0 f0f8 7192 2182  ............q.!.
+00004a10: 7d88 3026 3314 fa38 4051 e2b9 2999 6561  }.0&3..8@Q..).ea
+00004a20: e024 d7d3 95a5 000e 6559 735a 5e6d 043f  .$......eYsZ^m.?
+00004a30: dfa8 9bc8 0385 8152 8cbe 9649 c559 7393  .......R...I.Ys.
+00004a40: e3f2 d4b5 5dd7 b23d cb9d ddaa 0d6c 38be  ....]..=.....l8.
+00004a50: debc 496f b46d 55b5 b8ab 38f2 4215 e7e8  ..Io.mU...8.B...
+00004a60: 60fb 14c5 3489 104d e218 3914 0e05 923a  `...4..M..9....:
+00004a70: 18e4 17d3 20f3 9e5f 712b 2906 c9fd b161  .... .._q+)....a
+00004a80: 0242 37a9 eebf 9c04 5f51 dd71 a9f6 27aa  .B7....._Q.q..'.
+00004a90: 9755 5970 e3ed a67e ff80 70ef 8512 1e79  .UYp...~..p....y
+00004aa0: 99ef 0689 8fa2 1067 288a 9c04 ea4c 4850  .......g(....LHP
+00004ab0: 02dc d320 9df9 34c3 cf4f 38fc 6341 cc9e  ... ..4..O8.cA..
+00004ac0: e45c 9f71 47ae 343e 8971 98da 1805 093c  .\.qG.4>.q.....<
+00004ad0: d284 40c8 7116 21c7 0be2 388c 92d0 f7bc  ..@.q.!...8.....
+00004ae0: 9b4a d32b 4a1b b0ee d002 f3e5 f35f 3f7d  .J.+J........_?}
+00004af0: f9fc f711 aa8b 6ea6 7fab 29ea ba37 6a07  ......n...)..7j.
+00004b00: acf5 dd24 8851 ec10 0a49 1ace 5044 7d0f  ...$.Q...I..PD}.
+00004b10: 510f 1392 c441 94e0 4c69 a773 c863 edc0  Q....A..Li.s.c..
+00004b20: e061 dae9 da8f 5c74 6da9 7f44 1d7b 94cf  .a....\tm..D.{..
+00004b30: 96a9 1bc8 cc25 c18c d88e be39 58da b6a9  .....%.....9X...
+00004b40: bdd1 c852 f90f 6d25 deb0 ee7c ab45 52eb  ...R..m%...|.ER.
+00004b50: 1b54 a287 3a25 cc61 eaed 14e5 fbf4 e77d  .T..:%.a.......}
+00004b60: fa0f 0000 00ff ff03 0050 4b03 0414 0006  .........PK.....
+00004b70: 0008 0000 0021 00ae 1646 bda6 0400 00a0  .....!...F......
+00004b80: 1000 0022 0000 0070 7074 2f73 6c69 6465  ..."...ppt/slide
+00004b90: 4c61 796f 7574 732f 736c 6964 654c 6179  Layouts/slideLay
+00004ba0: 6f75 7431 312e 786d 6ccc 58db 6edc 3610  out11.xml.X.n.6.
+00004bb0: 7d2f d07f 10d4 675a 122f ba18 5907 ba16  }/....gZ./..Y...
+00004bc0: 0d9c c4e8 3a7d 5724 ae57 886e a5b8 9b75  ....:}W$.W.n...u
+00004bd0: 8300 f9ad f673 f225 1d52 921d af9d 780d  .....s.%.R....x.
+00004be0: d881 5f96 1435 1c9e 9973 86a4 f6c5 cb5d  .._..5...s.....]
+00004bf0: 531b 5b2e 86aa 6b17 a673 649b 066f 8bae  S.[...k..sd..o..
+00004c00: acda 8b85 f9ee 3c43 be69 0c32 6fcb bcee  ......<C.i.2o...
+00004c10: 5abe 302f f960 be3c f9f5 9717 fdf1 5097  Z.0/.`.<......P.
+00004c20: a7f9 65b7 9106 f868 87e3 7c61 aea5 ec8f  ..e....h..|a....
+00004c30: 2d6b 28d6 bcc9 87a3 aee7 2dbc 5b75 a2c9  -k(.......-.[u..
+00004c40: 253c 8a0b ab14 f947 f0dd d416 b66d d76a  %<.....G.....m.j
+00004c50: f2aa 35a7 f9e2 90f9 dd6a 5515 3ce9 8a4d  ..5......jU.<..M
+00004c60: c35b 393a 11bc ce25 e01f d655 3fcc defa  .[9:...%...U?...
+00004c70: 43bc f582 0fe0 46cf be09 495e f610 2d24  C.....F...I^..-$
+00004c80: 469e 57b2 e661 5b9e ef4c 43db 8b2d bc71  F.W..a[..LC..-.q
+00004c90: cc13 4841 b1ac 4ba3 cd1b 18f8 0b4c ab22  ..HA..K......L."
+00004ca0: af0d 6d6f 40c6 8c73 be93 da6c e8cf 05e7  ..mo@..s...l....
+00004cb0: aad7 6e7f 17fd b23f 137a f69b ed99 30aa  ..n....?.z....0.
+00004cc0: 5279 9bbc 98d6 f462 32d3 8fed 5677 acbd  Ry.....b2...Vw..
+00004cd0: e917 7337 3fde ad44 a35a c88e b15b 9840  ..s7?..D.Z...[.@
+00004ce0: e2a5 fab5 d418 8030 8a71 b0b8 1e2d d66f  .......0.q...-.o
+00004cf0: efb0 2dd6 e91d d6d6 bc80 f5cd a22a aa11  ..-..........*..
+00004d00: dced 70f0 1cce 5e52 54d2 34a0 d341 ced0  ..p...^RT.4..A..
+00004d10: 36a2 5a98 9fb2 0c47 2ccd 28ca a087 a81d  6.Z....G,.(.....
+00004d20: 5114 a534 4019 267e 8abd 2cc6 c4fd ac66  Q..4@.&~..,....f
+00004d30: 3bee 7121 b826 ec8f 7216 9ee3 de22 bba9  ;.q!.&..r...."..
+00004d40: 0ad1 0ddd 4a1e 155d 33a9 6616 1ff0 ecd0  ....J..]3.f.....
+00004d50: 8967 05f7 9347 9cd0 4903 1ff9 4948 50e0  .g...G..I...IHP.
+00004d60: 0680 8362 8040 290d 63cf 27b1 9b7d 9e32  ...b.@).c.'..}.2
+00004d70: 0198 e756 4761 4d81 4f19 9819 19fa d3ae  ...VGaM.O.......
+00004d80: f830 186d 078c 2982 4702 af2c 4656 55db  .0.m..).G..,FVU.
+00004d90: af27 b149 9523 d3e8 4405 921c b537 cd1a  .'.I.#..D....7..
+00004da0: 4d75 e73a f977 32ef 7b98 06f6 c829 7199  Mu.:.w2.{....)q.
+00004db0: 83d9 4d11 6017 fbfa bd22 97f9 8ee3 137f  ..M.`...."......
+00004dc0: 9fe2 d175 7f2c 7751 575e aad9 efa1 056a  ...u.,wQW^.....j
+00004dd0: 15a2 85c9 73c5 eae8 b61e e452 5ed6 5c3f  ....s......R^.\?
+00004de0: f4ea 4783 1260 5ce7 6a07 e12d 7ab7 1c6d  ..G..`\.j..-z..m
+00004df0: e549 5c57 c507 4376 062f 2b69 bcce 07c9  .I\W..Cv./+i....
+00004e00: 85a1 a386 2d06 bc28 1463 72b5 17de 9667  ....-..(.cr....g
+00004e10: b9c8 fffc d6d9 abb3 096d afa1 ce10 35ea  .........m....5.
+00004e20: 1f6b 92dc d6a4 4aca 599d 177c ddd5 2540  .k....J.Y..|..%@
+00004e30: c1cf 549e 3808 8893 b918 258c d988 c5b1  ..T.8.....%.....
+00004e40: 0f38 1845 8e93 da09 8b3c 2708 eca7 97a7  .8.E.....<'.....
+00004e50: 12c1 9e3a 01de ee7a f203 544a 7cfc 0391  ...:...z..TJ|...
+00004e60: 7a1e a1e4 2945 da2b 496d ebab 6def e1a2  z...)E.+Im..m...
+00004e70: 5550 b566 871b a21d 85b9 bf8a 4ed0 8f57  UP.f........N..W
+00004e80: 59f2 a283 13a3 e65b 5e1f e011 dfef f17c  Y......[^......|
+00004e90: 5d89 c31d 92fb 1d66 dd46 c8f5 c11e e901  ]......f.F......
+00004ea0: 1eab d59d 0e1f bbf4 e95c fa49 2ef9 8d8a  .........\.I....
+00004eb0: 27cf b4e2 6dd7 8b03 1c46 087b 9e8f bc2c  '...m....F.{...,
+00004ec0: 25c8 755c 0fb9 c4b3 431f 6701 633f e140  %.u\....C.g.c?.@
+00004ed0: 2aa1 c287 7f20 92bc 5ecd b53e 5e08 be5b  *.... ..^..>^..[
+00004ee0: ecfa beb2 5f93 dfa9 c215 dc9d 74b4 cc27  ...._.......t..'
+00004ef0: 991b c529 a2c4 850c 13ea c119 4c7c 14c6  ...)........L|..
+00004f00: 0c27 d483 83d9 893f cf57 b212 3894 55c3  .'.....?.W..8.U.
+00004f10: b3ea 6223 f8db 8dba 61ed 290c 9462 0c8d  ..b#....a.)..b..
+00004f20: 8c6b 9eb7 5735 2e4f b08d b165 330b 7bd7  .k..W5.O...e3.{.
+00004f30: 6a03 0c8f af37 36eb 2deb 3ab5 5b7c ab38  j....76.-.:.[|.8
+00004f40: fa4c 1597 d941 ecb3 2046 3864 18a5 360b  .L...A.. F8d..6.
+00004f50: 11dc 136c 14c0 aa34 0870 9445 ced3 2b6e  ...l...4.p.E..+n
+00004f60: 25c5 28b9 bf37 b980 d4cd aabb e788 7988  %.(..7........y.
+00004f70: ea1e 976a 77a6 7a59 5725 37de 6c9a f77b  ...jw.zYW%7.l..{
+00004f80: 84b3 674a 781a a489 9b90 1031 3f0c 104e  ..gJx......1?..N
+00004f90: 6077 89b3 3801 eafd d883 1338 a0c1 4fd8  `w..8......8..O.
+00004fa0: 62e0 1b12 7276 27e7 fa8c 7be4 9dc6 a511  b...rv'...{.....
+00004fb0: 0912 9b20 3f86 9f24 a690 7292 86c8 617e  ... ?..$..r...a~
+00004fc0: 1405 611c b88c 5ded 3483 a2b4 0574 876e  ..a...].4....t.n
+00004fd0: 305f bffc fbdb d72f ff3d c2ee a29b f99b  0_...../.=......
+00004fe0: 71ce baee 4dda 01b4 2e8e fd08 450e cd10  q...M.......E...
+00004ff0: 4d02 0f85 99cb 50c6 08a5 71e4 8731 4995  M.....P...q..1I.
+00005000: 767a 87de d60e 0c1e a69d befb c845 df55  vz...........E.U
+00005010: fa43 dbb1 27f9 6c73 7503 6170 46b1 c073  .C..'.lsu.apF..s
+00005020: f5dd cdd2 d8e6 f64a 234b 153f b4b5 789d  .......J#K.?..x.
+00005030: f76f b75a 248d be41 c57a a857 c21c 4daf  .o.Z$..A.z.W..M.
+00005040: 4d54 ecf3 3f0b 27ff 0300 00ff ff03 0050  MT..?.'........P
+00005050: 4b03 0414 0006 0008 0000 0021 0017 3ced  K..........!..<.
+00005060: 6ad3 0000 00bf 0100 002a 0000 0070 7074  j........*...ppt
+00005070: 2f6e 6f74 6573 536c 6964 6573 2f5f 7265  /notesSlides/_re
+00005080: 6c73 2f6e 6f74 6573 536c 6964 6532 2e78  ls/notesSlide2.x
+00005090: 6d6c 2e72 656c 73ac 90c1 6ac3 300c 86ef  ml.rels...j.0...
+000050a0: 83bd 83d1 7d76 d2c2 18a3 4e2f a3d0 432f  ....}v....N/..C/
+000050b0: a57b 0063 2b89 5922 1b4b 1deb dbd7 b00d  .{.c+.Y".K......
+000050c0: 1ae8 6187 1df5 4bfa f4a1 cdf6 6b9e d427  ..a...K.....k..'
+000050d0: 168e 892c b4ba 0185 e453 8834 5878 3fed  ...,.....S.4Xx?.
+000050e0: 9e5e 40b1 380a 6e4a 8416 2ec8 b0ed 1e1f  .^@.8.nJ........
+000050f0: 3647 9c9c d425 1e63 6655 29c4 1646 91fc  6G...%.cfU)..F..
+00005100: 6a0c fb11 67c7 3a65 a4da e953 999d d4b2  j...g.:e...S....
+00005110: 0c26 3bff e106 34ab a679 36e5 9601 dd82  .&;...4..y6.....
+00005120: a9f6 c142 d987 15a8 d325 e35f d8a9 efa3  ...B.....%._....
+00005130: c7b7 e4cf 3392 dc39 6178 8a01 2bd0 9501  ....3..9ax..+...
+00005140: c582 d6df c94f 63ad 2b10 cc7d 8ff6 3f3d  .....Oc.+..}..?=
+00005150: 2809 f2c1 b160 59d8 dce4 8ba1 f6d7 cc2c  (....`Y........,
+00005160: dede 5d01 0000 ffff 0300 504b 0304 1400  ..].......PK....
+00005170: 0600 0800 0000 2100 c69e 7235 cf02 0000  ......!...r5....
+00005180: eb06 0000 1f00 0000 7070 742f 6e6f 7465  ........ppt/note
+00005190: 7353 6c69 6465 732f 6e6f 7465 7353 6c69  sSlides/notesSli
+000051a0: 6465 312e 786d 6cac 556d 6fda 3010 fe3e  de1.xml.Umo.0..>
+000051b0: 69ff c1ca f710 0229 4d50 a122 14b6 4e1d  i......)MP."..N.
+000051c0: 45a5 fb01 ae63 4834 c7f6 6c43 6153 fffb  E....cH4..lCaS..
+000051d0: ce4e 5268 4b5f 3e54 8a62 fbec bb7b 9e7b  .NRhK_>T.b...{.{
+000051e0: 9ccb d9f9 b664 6843 952e 041f 7861 abed  .....dhC....xa..
+000051f0: 21ca 89c8 0abe 1a78 bf6e a77e ec21 6d30  !......x.n.~.!m0
+00005200: cf30 139c 0ebc 1dd5 def9 f0eb 9733 d9e7  .0...........3..
+00005210: c250 8dc0 9feb 3e1e 78b9 31b2 1f04 9ae4  .P....>.x.1.....
+00005220: b4c4 ba25 24e5 b0b7 14aa c406 966a 1564  ...%$........j.d
+00005230: 0adf 43dc 9205 9d76 bb17 94b8 e05e edaf  ..C....v.....^..
+00005240: 3ee2 2f96 cb82 d00b 41d6 25e5 a60a a228  >./.....A.%....(
+00005250: c306 b0eb bc90 ba89 263f 124d 2aaa 218c  ........&?.M*.!.
+00005260: f37e 0269 08dc c882 6576 d4f2 5651 6a67  .~.i....ev..VQjg
+00005270: 7cf3 4dc9 859c 2bb7 3ddb cc15 2a32 a898  |.M...+.=...*2..
+00005280: 8738 2ea1 305e 506f d4c7 dc92 6fdc 2478  .8..0^Po....o.$x
+00005290: e6be 6aa6 b8bf 5daa d28e c00d 6d07 1e94  ..j...].....m...
+000052a0: 7f67 df81 b5d1 ad41 a432 92bd 95e4 d747  .g.....A.2.....G
+000052b0: ce92 7c72 e474 d024 080e 925a 5615 b897  ..|r.t.$...ZV...
+000052c0: 743a 0d9d 052b 328a 2e4b bca2 68ce 30a1  t:...+2..K..h.0.
+000052d0: b960 1955 287c e4d9 30d0 f24a 90df 1a71  .`.U(|..0..J...q
+000052e0: 010c ab82 881b 61ea d938 c77c 4547 5a52  ......a..8.|EGZR
+000052f0: e24c 5535 1edd ab12 d951 e6c8 ec24 64d6  .LU5.....Q...$d.
+00005300: 2cbb 2c57 f5c1 6ad7 4df6 e09b 9a56 345e  ,.,W..j.M....V4^
+00005310: 27d3 6dc8 ccdc 4d3d a4d1 799f c6fb 48ef  '.m...M=..y...H.
+00005320: 44b6 f320 d376 7ffc 75bc b26f b629 38d8  D.. .v..u..o.)8.
+00005330: 5cd6 d119 719f 69b3 303b 46dd 42da 9743  \...q.i.0;F.B..C
+00005340: a380 02c3 f61b a4dc ff31 f750 5628 b357  .........1.PV(.W
+00005350: db0c bf53 c644 0b59 858d d3b9 723b e65b  ...S.D.Y....r;.[
+00005360: 7bdc e685 46f0 6024 a5d9 fa46 08a6 112b  {...F.`$...F...+
+00005370: ee14 56bb d6b3 3894 6773 acf0 cd5b 2802  ..V...8.gs...[(.
+00005380: 8737 d8f3 fa80 22d1 d3eb 355b 9777 20c6  .7...."...5[.w .
+00005390: a130 ddcf 1006 ae10 8486 c6f5 77e0 fd59  .0..........w..Y
+000053a0: 6365 a8aa 753a f93c 9d96 2c73 9cfe c5c9  ce..u:.<..,s....
+000053b0: 3419 75db 899f 4c7a 277e da8b 267e 7a1a  4.u...Lz'~..&~z.
+000053c0: 877e 3b09 bbf1 4512 76c2 b8f7 e03d 4203  .~;...E.v....=B.
+000053d0: e21c c01d 5559 9766 cc28 e607 4287 7b69  ....UY.f.(..B.{i
+000053e0: 96b6 27bd 2ace 1b92 b8a1 6964 d055 aeb4  ..'.*.....id.U..
+000053f0: a967 68ad 0aa0 90a6 49af 338e 533f 0da3  .gh.....I.3.S?..
+00005400: a91f 5d24 a7fe 680a 64a6 27dd 281a a7f1  ..]$..h.d.'.(...
+00005410: 68dc 9d3c d8c6 1846 7da2 a8eb 9997 59d3  h..<...F}.....Y.
+00005420: 6dc3 e845 bf2d 0ba2 8416 4bd3 22a2 ac1b  m..E.-....K."...
+00005430: 7720 c53d 5552 14ae 7787 edfa 07b0 c10c  w .=UR..w.......
+00005440: fa4e d26d 8749 12c6 712d 1060 6b46 87d6  .N.m.I..q-.`kF..
+00005450: 2a5e f764 c2d4 4f2c af37 ee76 4032 5077  *^.d..O,.7.v@2Pw
+00005460: ec4c 127e 2ef5 e5d8 1fb1 1adb cf7f f81f  .L.~............
+00005470: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+00005480: 0000 2100 4aaf 7539 d200 0000 bf01 0000  ..!.J.u9........
+00005490: 2a00 0000 7070 742f 6e6f 7465 7353 6c69  *...ppt/notesSli
+000054a0: 6465 732f 5f72 656c 732f 6e6f 7465 7353  des/_rels/notesS
+000054b0: 6c69 6465 312e 786d 6c2e 7265 6c73 ac90  lide1.xml.rels..
+000054c0: b16a 0331 0c86 f742 dfc1 688f 7d97 2194  .j.1...B..h.}.!.
+000054d0: 125f 9652 c890 a5a4 0f60 6cdd 9dc9 9d6c  ._.R.....`l....l
+000054e0: 2c25 246f 5f43 4bc9 4186 0e1d f54b faf4  ,%$o_CK.A....K..
+000054f0: a1ed ee3a 4fea 8285 6322 0bad 6e40 21f9  ...:O...c"..n@!.
+00005500: 1422 0d16 3e8f efab 1750 2c8e 829b 12a1  ."..>....P,.....
+00005510: 851b 32ec bae7 a7ed 074e 4eea 128f 31b3  ..2......NN...1.
+00005520: aa14 620b a348 7e35 86fd 88b3 639d 3252  ..b..H~5....c.2R
+00005530: edf4 a9cc 4e6a 5906 939d 3fb9 01cd ba69  ....NjY...?....i
+00005540: 36a6 dc33 a05b 30d5 3e58 28fb b006 75bc  6..3.[0.>X(...u.
+00005550: 65fc 0b3b f57d f4f8 96fc 7946 9207 270c  e..;.}....yF..'.
+00005560: 4f31 6005 ba32 a058 d0fa 3bf9 69b4 ba02  O1`..2.X..;.i...
+00005570: c13c f668 ffd3 8392 201f 1c0b 9685 cd5d  .<.h.... ......]
+00005580: be18 fa35 338b b777 5f00 0000 ffff 0300  ...53..w_.......
+00005590: 504b 0304 1400 0600 0800 0000 2100 d5d1  PK..........!...
+000055a0: 92f1 bc00 0000 3701 0000 2d00 0000 7070  ......7...-...pp
+000055b0: 742f 736c 6964 654c 6179 6f75 7473 2f5f  t/slideLayouts/_
+000055c0: 7265 6c73 2f73 6c69 6465 4c61 796f 7574  rels/slideLayout
+000055d0: 3131 2e78 6d6c 2e72 656c 738c cfbd 0ac2  11.xml.rels.....
+000055e0: 3010 07f0 5df0 1dc2 ed26 ad83 8834 7511  0...]....&...4u.
+000055f0: c1c1 45f4 018e e4da 06db 24e4 a2e8 db9b  ..E.......$.....
+00005600: d182 83e3 7dfd fe5c b37f 4da3 7852 6217  ....}..\..M.xRb.
+00005610: bc86 5a56 20c8 9b60 9def 35dc aec7 d516  ..ZV ..`..5.....
+00005620: 0467 f416 c7e0 49c3 9b18 f6ed 72d1 5c68  .g....I.....r.\h
+00005630: c45c 8e78 7091 4551 3c6b 1872 8e3b a5d8  .\.xp.EQ<k.r.;..
+00005640: 0c34 21cb 10c9 9749 17d2 84b9 94a9 5711  .4!....I......W.
+00005650: cd1d 7b52 ebaa daa8 f46d 403b 33c5 c96a  ..{R.....m@;3..j
+00005660: 4827 5b83 b8be 23fd 6387 ae73 860e c13c  H'[...#.c..s...<
+00005670: 26f2 f947 84e2 d159 3a23 674a 85c5 d453  &..G...Y:#gJ...S
+00005680: d620 e577 7fb6 54cb 1201 aa6d d4ec ddf6  . .w..T....m....
+00005690: 0300 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
+000056a0: 0000 0021 00d5 d192 f1bc 0000 0037 0100  ...!.........7..
+000056b0: 002d 0000 0070 7074 2f73 6c69 6465 4c61  .-...ppt/slideLa
+000056c0: 796f 7574 732f 5f72 656c 732f 736c 6964  youts/_rels/slid
+000056d0: 654c 6179 6f75 7431 302e 786d 6c2e 7265  eLayout10.xml.re
+000056e0: 6c73 8ccf bd0a c230 1007 f05d f01d c2ed  ls.....0...]....
+000056f0: 26ad 8388 3475 11c1 c145 f401 8ee4 da06  &...4u...E......
+00005700: db24 e4a2 e8db 9bd1 8283 e37d fdfe 5cb3  .$.........}..\.
+00005710: 7f4d a378 5262 17bc 865a 5620 c89b 609d  .M.xRb...ZV ..`.
+00005720: ef35 dcae c7d5 1604 67f4 16c7 e049 c39b  .5......g....I..
+00005730: 18f6 ed72 d15c 68c4 5c8e 7870 9145 513c  ...r.\h.\.xp.EQ<
+00005740: 6b18 728e 3ba5 d80c 3421 cb10 c997 4917  k.r.;...4!....I.
+00005750: d284 b994 a957 11cd 1d7b 52eb aada a8f4  .....W...{R.....
+00005760: 6d40 3b33 c5c9 6a48 275b 83b8 be23 fd63  m@;3..jH'[...#.c
+00005770: 87ae 7386 0ec1 3c26 f2f9 4784 e2d1 593a  ..s...<&..G...Y:
+00005780: 2367 4a85 c5d4 53d6 20e5 777f b654 cb12  #gJ...S. .w..T..
+00005790: 01aa 6dd4 ecdd f603 0000 ffff 0300 504b  ..m...........PK
+000057a0: 0304 1400 0600 0800 0000 2100 d5d1 92f1  ..........!.....
+000057b0: bc00 0000 3701 0000 2c00 0000 7070 742f  ....7...,...ppt/
+000057c0: 736c 6964 654c 6179 6f75 7473 2f5f 7265  slideLayouts/_re
+000057d0: 6c73 2f73 6c69 6465 4c61 796f 7574 392e  ls/slideLayout9.
+000057e0: 786d 6c2e 7265 6c73 8ccf bd0a c230 1007  xml.rels.....0..
+000057f0: f05d f01d c2ed 26ad 8388 3475 11c1 c145  .]....&...4u...E
+00005800: f401 8ee4 da06 db24 e4a2 e8db 9bd1 8283  .......$........
+00005810: e37d fdfe 5cb3 7f4d a378 5262 17bc 865a  .}..\..M.xRb...Z
+00005820: 5620 c89b 609d ef35 dcae c7d5 1604 67f4  V ..`..5......g.
+00005830: 16c7 e049 c39b 18f6 ed72 d15c 68c4 5c8e  ...I.....r.\h.\.
+00005840: 7870 9145 513c 6b18 728e 3ba5 d80c 3421  xp.EQ<k.r.;...4!
+00005850: cb10 c997 4917 d284 b994 a957 11cd 1d7b  ....I......W...{
+00005860: 52eb aada a8f4 6d40 3b33 c5c9 6a48 275b  R.....m@;3..jH'[
+00005870: 83b8 be23 fd63 87ae 7386 0ec1 3c26 f2f9  ...#.c..s...<&..
+00005880: 4784 e2d1 593a 2367 4a85 c5d4 53d6 20e5  G...Y:#gJ...S. .
+00005890: 777f b654 cb12 01aa 6dd4 ecdd f603 0000  w..T....m.......
+000058a0: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+000058b0: 2100 d5d1 92f1 bc00 0000 3701 0000 2c00  !.........7...,.
+000058c0: 0000 7070 742f 736c 6964 654c 6179 6f75  ..ppt/slideLayou
+000058d0: 7473 2f5f 7265 6c73 2f73 6c69 6465 4c61  ts/_rels/slideLa
+000058e0: 796f 7574 382e 786d 6c2e 7265 6c73 8ccf  yout8.xml.rels..
+000058f0: bd0a c230 1007 f05d f01d c2ed 26ad 8388  ...0...]....&...
+00005900: 3475 11c1 c145 f401 8ee4 da06 db24 e4a2  4u...E.......$..
+00005910: e8db 9bd1 8283 e37d fdfe 5cb3 7f4d a378  .......}..\..M.x
+00005920: 5262 17bc 865a 5620 c89b 609d ef35 dcae  Rb...ZV ..`..5..
+00005930: c7d5 1604 67f4 16c7 e049 c39b 18f6 ed72  ....g....I.....r
+00005940: d15c 68c4 5c8e 7870 9145 513c 6b18 728e  .\h.\.xp.EQ<k.r.
+00005950: 3ba5 d80c 3421 cb10 c997 4917 d284 b994  ;...4!....I.....
+00005960: a957 11cd 1d7b 52eb aada a8f4 6d40 3b33  .W...{R.....m@;3
+00005970: c5c9 6a48 275b 83b8 be23 fd63 87ae 7386  ..jH'[...#.c..s.
+00005980: 0ec1 3c26 f2f9 4784 e2d1 593a 2367 4a85  ..<&..G...Y:#gJ.
+00005990: c5d4 53d6 20e5 777f b654 cb12 01aa 6dd4  ..S. .w..T....m.
+000059a0: ecdd f603 0000 ffff 0300 504b 0304 1400  ..........PK....
+000059b0: 0600 0800 0000 2100 39ca c7c6 ba02 0000  ......!.9.......
+000059c0: 8606 0000 1f00 0000 7070 742f 6e6f 7465  ........ppt/note
+000059d0: 7353 6c69 6465 732f 6e6f 7465 7353 6c69  sSlides/notesSli
+000059e0: 6465 322e 786d 6cac 54dd 4edb 3014 be9f  de2.xml.T.N.0...
+000059f0: b477 b072 9fa6 6942 4922 5ad4 9476 6262  .w.r..iBI"Z..vbb
+00005a00: 5051 f600 c671 9b68 8eed d96e 6937 f1ee  PQ...q.h...ni7..
+00005a10: 3b76 9216 0608 2e90 a2f8 d83e 7fdf 777c  ;v.........>..w|
+00005a20: ced9 f9ae 6668 4b95 ae04 1f79 61af ef21  ....fhK....ya..!
+00005a30: ca89 282a be1e 793f efe6 7ee2 216d 302f  ..(*..y?..~.!m0/
+00005a40: 3013 9c8e bc3d d5de f9f8 eb97 3399 7161  0....=......3.qa
+00005a50: a846 60cf 7586 475e 698c cc82 4093 92d6  .F`.u.G^i...@...
+00005a60: 58f7 84a4 1cee 5642 d5d8 c056 ad83 42e1  X.....VB...V..B.
+00005a70: 07f0 5bb3 60d0 ef0f 831a 57dc 6bed d547  ..[.`.....W.k..G
+00005a80: ecc5 6a55 117a 21c8 a6a6 dc34 4e14 65d8  ..jU.z!....4N.e.
+00005a90: 40ee baac a4ee bcc9 8f78 938a 6a70 e3ac  @........x..jp..
+00005aa0: 9fa5 3406 6c64 c90a bb6a 79a7 28b5 12df  ..4.ld...jy.(...
+00005ab0: 7e53 7229 17ca 5d5f 6f17 0a55 0530 e621  ~Sr)..]_o..U.0.!
+00005ac0: 8e6b 20c6 0bda 8b56 cd6d f9d6 09c1 7fe6  .k ....V.m......
+00005ad0: eb4e c4d9 6ea5 6abb 0236 b41b 7940 ffde  .N..n.j..6..y@..
+00005ae0: fe03 7b46 7706 91e6 901c 4f49 79f3 8a2e  ..{Fw.....OIy...
+00005af0: 2967 af68 075d 80e0 4950 8baa 49ee 259c  )g.h.]..IP..I.%.
+00005b00: 4107 67c9 aa82 a2cb 1aaf 295a 304c 6829  A.g.......)Z0Lh)
+00005b10: 5841 150a 0f38 3b04 5a5e 09f2 4b23 2e00  XA...8;.Z^..K#..
+00005b20: 6143 88b8 15a6 95a6 25e6 6b3a d192 1277  aC......%.k:...w
+00005b30: d4b0 7130 6f28 b2ab 2c91 d94b 88ac 5971  ..q0o(..,..K..Yq
+00005b40: 59af 5bc5 e6d6 09c7 e43b 4e1b 186f 8389  Y.[......;N..o..
+00005b50: 3a30 d7ee a53e 8531 781f c6fb 99de 8b62  :0...>.1x......b
+00005b60: ef41 a4dd 51fd ed7c 6566 7639 18d8 58d6  .A..Q..|efv9..X.
+00005b70: d01d e28c 69b3 347b 46dd 46da 9fcb 4601  ....i.4{F.F...F.
+00005b80: 0486 6d0f 52ee 7f5f 3435 36e3 bbb2 d208  ..m.R.._456.....
+00005b90: 3e8c 88e0 846d 6cd7 226d 4bd5 b3b5 36ae  >....ml."mK...6.
+00005ba0: e236 01e7 2b38 c6fc 005b f1f3 d25f 6fea  .6..+8...[..._o.
+00005bb0: 7b20 ea29 69d1 6790 06e5 05d7 3054 fe8c  { .)i.g.....0T..
+00005bc0: bcdf 1bac 0c55 2d87 279f c7e1 8a15 0ed3  .....U-.'.......
+00005bd0: df24 9da7 93a8 9ffa e96c 78e2 e7c3 78e6  .$.......lx...x.
+00005be0: e7a7 49e8 f7d3 304a 2ed2 7010 26c3 47ef  ..I...0J..p.&.G.
+00005bf0: 901a 00e7 90dc 6b15 40ba 3653 4631 3fb4  ......k.@.6SF1?.
+00005c00: 9c19 4747 d257 765e 40cb f262 8115 be7d  ..GG.Wv^@..b...}
+00005c10: 59be b74a e296 6ec8 40c7 5f69 d34a 68a3  Y..J..n.@._i.Jh.
+00005c20: 2a80 90e7 e970 304d 723f 0fe3 b91f 5fa4  *....p0Mr?...._.
+00005c30: a7fe 640e 60e6 2751 1c4f f364 328d 668f  ..d.`.'Q.O.d2.f.
+00005c40: 7668 8571 4614 75f3 ecb2 e826 6118 bf98  vh.qF.u....&a...
+00005c50: 8575 4594 d062 657a 44d4 ed50 0da4 78a0  .uE..bezD..P..x.
+00005c60: 4a8a cacd d5b0 df0e e72d 6623 2f8d e230  J........-f#/..0
+00005c70: 4cc2 c4f5 4ce0 52eb 5697 ac2d 783b 2e09  L...L.R.V..-x;..
+00005c80: 533f b0bc d9ba c701 b1a0 b853 7724 61ee  S?.........Sw$a.
+00005c90: b76f e3a8 624b 6c3b 73fc 0f00 00ff ff03  .o..bKl;s.......
+00005ca0: 0050 4b03 0414 0006 0008 0000 0021 0069  .PK..........!.i
+00005cb0: a25f 2115 0100 00c7 0700 002c 0000 0070  ._!........,...p
+00005cc0: 7074 2f73 6c69 6465 4d61 7374 6572 732f  pt/slideMasters/
+00005cd0: 5f72 656c 732f 736c 6964 654d 6173 7465  _rels/slideMaste
+00005ce0: 7231 2e78 6d6c 2e72 656c 73c4 d54d 6ac3  r1.xml.rels..Mj.
+00005cf0: 3010 05e0 7da1 7730 b38f 253b 8993 94c8  0...}.w0..%;....
+00005d00: d984 42a0 ab92 1e40 58e3 1f6a 4b46 524a  ..B....@X..jKFRJ
+00005d10: 7dfb 8a96 420c 6168 21a0 8dc0 92f5 e6e3  }...B.ah!.......
+00005d20: 6db4 3f7c 0e7d f281 d675 460b c852 0e09  m.?|.}...uF..R..
+00005d30: eaca a84e 3702 dece cf8b 2d24 ce4b ad64  ...N7.....-$.K.d
+00005d40: 6f34 0a98 d0c1 a17c 7cd8 bf62 2f7d b8e4  o4.....||..b/}..
+00005d50: da6e 7449 48d1 4e40 ebfd f8c4 98ab 5a1c  .ntIH.N@......Z.
+00005d60: a44b cd88 3a9c d4c6 0ed2 874f dbb0 5156  .K..:......O..QV
+00005d70: efb2 4196 735e 307b 9d01 e52c 3339 2901  ..A.s^0{...,39).
+00005d80: f6a4 c2fc f334 e25f b24d 5d77 151e 4d75  .....4._.M]w..Mu
+00005d90: 1950 fb1b 2398 eb3b 852f 7232 171f 62a5  .P..#..;./r2..b.
+00005da0: 6dd0 0b48 d3eb fdd9 4fdb 348c 0076 5bb6  m..H....O.4..v[.
+00005db0: 8c29 5b52 b24d 4cd9 8692 65f9 3d69 3edc  .)[R.ML...e.=i>.
+00005dc0: c519 ea7b e767 cd28 c75d 19ff 6d28 271b  ...{.g.(.]..m('.
+00005dd0: 8a29 233b 2b62 ca0a b2b3 b8a5 91ad ad63  .)#;+b.........c
+00005de0: d2d6 646b 3c6a 6b9c b2ad 62d2 5694 6c17  ..dk<jk...b.V.l.
+00005df0: 53b6 fb95 b1d9 f35b 7e01 0000 ffff 0300  S......[~.......
+00005e00: 504b 0304 1400 0600 0800 0000 2100 d5d1  PK..........!...
+00005e10: 92f1 bc00 0000 3701 0000 2c00 0000 7070  ......7...,...pp
+00005e20: 742f 736c 6964 654c 6179 6f75 7473 2f5f  t/slideLayouts/_
+00005e30: 7265 6c73 2f73 6c69 6465 4c61 796f 7574  rels/slideLayout
+00005e40: 372e 786d 6c2e 7265 6c73 8ccf bd0a c230  7.xml.rels.....0
+00005e50: 1007 f05d f01d c2ed 26ad 8388 3475 11c1  ...]....&...4u..
+00005e60: c145 f401 8ee4 da06 db24 e4a2 e8db 9bd1  .E.......$......
+00005e70: 8283 e37d fdfe 5cb3 7f4d a378 5262 17bc  ...}..\..M.xRb..
+00005e80: 865a 5620 c89b 609d ef35 dcae c7d5 1604  .ZV ..`..5......
+00005e90: 67f4 16c7 e049 c39b 18f6 ed72 d15c 68c4  g....I.....r.\h.
+00005ea0: 5c8e 7870 9145 513c 6b18 728e 3ba5 d80c  \.xp.EQ<k.r.;...
+00005eb0: 3421 cb10 c997 4917 d284 b994 a957 11cd  4!....I......W..
+00005ec0: 1d7b 52eb aada a8f4 6d40 3b33 c5c9 6a48  .{R.....m@;3..jH
+00005ed0: 275b 83b8 be23 fd63 87ae 7386 0ec1 3c26  '[...#.c..s...<&
+00005ee0: f2f9 4784 e2d1 593a 2367 4a85 c5d4 53d6  ..G...Y:#gJ...S.
+00005ef0: 20e5 777f b654 cb12 01aa 6dd4 ecdd f603   .w..T....m.....
+00005f00: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+00005f10: 0000 2100 d5d1 92f1 bc00 0000 3701 0000  ..!.........7...
+00005f20: 2c00 0000 7070 742f 736c 6964 654c 6179  ,...ppt/slideLay
+00005f30: 6f75 7473 2f5f 7265 6c73 2f73 6c69 6465  outs/_rels/slide
+00005f40: 4c61 796f 7574 362e 786d 6c2e 7265 6c73  Layout6.xml.rels
+00005f50: 8ccf bd0a c230 1007 f05d f01d c2ed 26ad  .....0...]....&.
+00005f60: 8388 3475 11c1 c145 f401 8ee4 da06 db24  ..4u...E.......$
+00005f70: e4a2 e8db 9bd1 8283 e37d fdfe 5cb3 7f4d  .........}..\..M
+00005f80: a378 5262 17bc 865a 5620 c89b 609d ef35  .xRb...ZV ..`..5
+00005f90: dcae c7d5 1604 67f4 16c7 e049 c39b 18f6  ......g....I....
+00005fa0: ed72 d15c 68c4 5c8e 7870 9145 513c 6b18  .r.\h.\.xp.EQ<k.
+00005fb0: 728e 3ba5 d80c 3421 cb10 c997 4917 d284  r.;...4!....I...
+00005fc0: b994 a957 11cd 1d7b 52eb aada a8f4 6d40  ...W...{R.....m@
+00005fd0: 3b33 c5c9 6a48 275b 83b8 be23 fd63 87ae  ;3..jH'[...#.c..
+00005fe0: 7386 0ec1 3c26 f2f9 4784 e2d1 593a 2367  s...<&..G...Y:#g
+00005ff0: 4a85 c5d4 53d6 20e5 777f b654 cb12 01aa  J...S. .w..T....
+00006000: 6dd4 ecdd f603 0000 ffff 0300 504b 0304  m...........PK..
+00006010: 1400 0600 0800 0000 2100 9b55 7ccd 1508  ........!..U|...
+00006020: 0000 6c36 0000 2100 0000 7070 742f 736c  ..l6..!...ppt/sl
+00006030: 6964 654d 6173 7465 7273 2f73 6c69 6465  ideMasters/slide
+00006040: 4d61 7374 6572 312e 786d 6cec 5afd 6ee3  Master1.xml.Z.n.
+00006050: 3612 ffbf c0bd 83a0 fbf3 a0b5 2891 fa30  6...........(..0
+00006060: d629 acaf 768b 741b 34e9 03c8 121d eb22  .)..v.t.4......"
+00006070: 4b2a 45a7 c916 05f6 59fa 16ed e3ec 93dc  K*E.....Y.......
+00006080: 9012 6d39 89bd c95d 7270 0223 8045 8f46  ..m9...]rp.#.E.F
+00006090: a3e1 fce6 3743 d279 ffed cdb2 d4ae 296b  ....7C.y......)k
+000060a0: 8bba 9ae8 e89d a96b b4ca eabc a82e 27fa  .......k......'.
+000060b0: 2f17 89e1 e95a cbd3 2a4f cbba a213 fd96  /....Z..*O......
+000060c0: b6fa b727 fff8 e67d 336e cbfc c7b4 e594  ...'...}3n......
+000060d0: 6960 a36a c7e9 445f 70de 8c47 a336 5bd0  i`.j..D_p..G.6[.
+000060e0: 65da beab 1b5a c1bd 79cd 9629 87af ec72  e....Z..y..)...r
+000060f0: 94b3 f437 b0bd 2c47 9669 3aa3 655a 547a  ...7..,G.i:.eZTz
+00006100: ff3c 7bcc f3f5 7c5e 6434 aab3 d592 56bc  .<{...|^d4....V.
+00006110: 33c2 6899 72f0 bf5d 144d abac 358f b1d6  3.h.r..].M..5...
+00006120: 30da 8219 f9f4 964b 2730 bfec bccc c575  0......K'0.....u
+00006130: 76d9 7dfe 4ce7 5a91 df40 944c 1381 463a  v.}.L.Z..@.L..F:
+00006140: 9696 6958 32ed 3a2d 27fa ec12 e9a3 93f7  ..iX2.:-'.......
+00006150: a35e b91f 8987 dbe6 8251 2a46 d5f5 77ac  .^.......Q*F..w.
+00006160: 396f ce98 7cc3 c7eb 3306 36c1 a4ae 55e9  9o..|...3.6...U.
+00006170: 12e2 2b0c c81b bd9a fc5a 5dcb c1e8 cee3  ..+......Z].....
+00006180: 976a 988e 6fe6 6c29 ae10 1e0d 3c04 146f  .j..o.l)....<..o
+00006190: c5e7 48c8 e80d d7b2 4e98 6da4 d9e2 a707  ..H.....N.m.....
+000061a0: 74b3 45fc 80f6 48bd 6034 78a9 9855 e7dc  t.E...H.`4x..U..
+000061b0: fde9 586a 3a17 052f a976 56a6 195d d465  ..Xj:../.vV..].e
+000061c0: 0eb9 d245 0e7c 3a6d b9f2 6ec5 8a89 fe7b  ...E.|:m..n....{
+000061d0: 9258 0189 136c 2430 32b0 1960 2388 b16f  .X...l$02..`#..o
+000061e0: 2496 edc5 969b 8496 edfc 219e 46ce 3863  $.........!.F.8c
+000061f0: 5482 f621 57c9 879c 7b80 2f8b 8cd5 6d3d  T..!W...{./...m=
+00006200: e7ef b27a d967 8e4a 40c0 1ae1 3efd 84c7  ...z.g.J@...>...
+00006210: bf47 7110 f9de d437 3006 1742 e29a 4682  .Gq....70..B..F.
+00006220: 82d8 98fa 08e1 d875 a269 80fe e883 013e  .......u.i.....>
+00006230: abab 9cc5 a89f 7b1f 0405 4adb 9cd6 d955  ......{...J....U
+00006240: ab55 3580 2630 ee30 5c6b 74c0 8a6b b3d0  .U5.&0.0\kt..k..
+00006250: f86d 03f1 e222 5ebd 5e77 530e 3611 7f10  .m..."^.^wS.6...
+00006260: 6ecf f620 7525 8eb6 4390 45b6 8147 2641  n.. u%..C.E..G&A
+00006270: c411 0a02 5164 5b84 38f6 16ae e9b8 612d  ....Qd[.8.....a-
+00006280: ff8e d64b 4d0c 263a a319 9740 a5d7 30c3  ...KM.&:...@..0.
+00006290: 4e55 a948 9f3a 4f9a 31bf 09ea fc56 68ce  NU.H.:O.1....Vh.
+000062a0: e00a f043 2d81 e717 35fb a46b e587 aa9d  ...C-...5..k....
+000062b0: e83e c218 decd e517 4c5c 0bbe b0e1 9dd9  .>......L\......
+000062c0: d61d 5e86 7529 f32f ad32 b033 d133 cea4  ..^.u)./.2.3.3..
+000062d0: 2f15 3077 bae2 f5bc e83d ea5e 296e 952d  /.0w.....=.^)n.-
+000062e0: 3fe7 b725 95f3 6ec4 8714 3370 a84c 4529  ?..%..n...3p.LE)
+000062f0: a395 f1cb 7917 167e 1296 4576 a5f1 5aa3  ....y..~..Ev..Z.
+00006300: 79c1 b5be 88c9 d043 ad03 2bc2 7687 b0b4  y......C..+.v...
+00006310: 42ab fc2c 65e9 cf43 633f 9cf5 016c 6438  B..,e..Cc?...ld8
+00006320: 5418 6464 f673 c35e 7343 e033 a486 75a0  T.dd.s.^sC.3..u.
+00006330: d4f0 2214 c54e 621a 24f6 3cc3 76cd c820  .."..Nb.$.<.v.. 
+00006340: 911d 19d8 71dc 2488 bc30 44e4 e5a9 21c0  ....q.$..0D...!.
+00006350: 160e 8984 fe5f 1882 3c8b 38fb 2982 6d82  ....._..<.8.).m.
+00006360: 6cdb 3b7c 8a3c 9915 8dc8 e16b f9ac 143e  l.;|.<.....k...>
+00006370: 9d25 2262 9224 ed16 4b3a 26dc 7d8b 046a  .%"b.$..K:&.}..j
+00006380: ff5b ce69 5657 b956 d26b 5a3e c2a2 f575  .[.iVW.V.kZ>...u
+00006390: 8b17 8b82 3dde a02c 84fb 0d26 f58a f1c5  ....=..,...&....
+000063a0: a32d e247 582c e60f 1a7c ee5a 8355 ad89  .-.GX,...|.Z.U..
+000063b0: 52be dd86 ed43 6dc3 566c da4e 6019 b66f  R....Cm.Vl.N`..o
+000063c0: c686 e999 53c3 0f2c 62d8 8ee9 4691 e75a  ....S..,b...F..Z
+000063d0: c40c 5fbe d6e4 1c56 bd9f 6026 6939 ef6b  .._....V..`&i9.k
+000063e0: 8e4c bcff b6e6 3836 745c 7267 3d66 b9d8  .L....86t\rg=f..
+000063f0: 960a a2e4 6cfa f62b 6aca 723a aac8 c8f1  ....l..+j.r:....
+00006400: 7589 040f d2f2 1276 13a5 7436 a773 91cd  u......v..t6.s..
+00006410: 229c 484c 5742 5297 459e 1465 f9c0 2a9a  ".HLWBR.E..e..*.
+00006420: df74 4b44 5e54 bc93 b8c4 34d5 3a74 addc  .tKD^T....4.:t..
+00006430: 7ddb d819 a937 c961 ef48 371e 3828 993a  }....7.a.H7.8(.:
+00006440: 2ff3 2ed9 8867 274e 10c6 06b6 1d48 701b  /....g'N.....Hp.
+00006450: bb86 efd8 9e31 0d89 1561 37f6 3d04 c9a6  .....1...a7.=...
+00006460: 7202 28c4 8b25 4d8a cb15 a33f ad3a 28b6  r.(..%M....?.:(.
+00006470: 080e 44d5 da25 0f4b 9a56 eb12 cb4f 2cd3  ..D..%.K.V...O,.
+00006480: b246 2619 59ee 86ec 73b1 b778 6eba 1345  .F&.Y...s..xn..E
+00006490: f7a4 ae45 b11e 121e 1f28 e131 4aa2 a94d  ...E.....(.1J..M
+000064a0: 6203 a21d 1800 746c f86e 9018 d89d 2601  b.....tl.n....&.
+000064b0: 095c 1c9a ff87 75f7 1cb2 59a6 e8af ab94  .\....u...Y.....
+000064c0: 41e8 7ad2 77ab e4a7 901e 9bb6 27d7 11bb  A.z.w.......'...
+000064d0: 588f 613b e1bd 65d6 abd5 fae1 f1fe 79c9  X.a;..e.......y.
+000064e0: e628 b29d 832f 54fb b85a ceee 508e 1c28  .(.../T..Z..P..(
+000064f0: e550 9078 d831 3dc3 4204 1b24 305d c38b  .P.x.1=.B..$0]..
+00006500: 62d3 307d 14bb 018e 1ce8 b52f 4fb9 b6cc  b.0}......./O...
+00006510: 2166 0fb1 4e2e a09e d66a 1d64 ee65 dd9b  !f..N....j.d.e..
+00006520: efb5 87ca b975 af75 7060 fb91 691b 5e08  .....u.up`..i.^.
+00006530: 1f51 8821 e5ed 786a 20e2 0581 3f0d 7d87  .Q.!..xj ...?.}.
+00006540: 9075 af6d 05a5 2ac8 8ec7 b6d8 2f9f fffa  .u.m..*...../...
+00006550: e797 cf7f 3f43 7f95 1775 5aa7 b25e 8e7a  ....?C...uZ..^.z
+00006560: ee82 b78e 1542 af0a 1086 3615 f9ae 314d  .....B....6...1M
+00006570: 1c62 24c4 c638 0cbc 6968 c782 bb0d c2f7  .b$..8..ih......
+00006580: b90b c2c7 71b7 a97f a3ac a90b 79c6 89cc  ....q.......y...
+00006590: 9ebe 1222 e421 d89e 5aa6 af78 d271 74e3  ...".!..Z..x.qt.
+000065a0: ad20 5e7f 7699 95ec c7b4 d166 9708 9663  . ^.v......f...c
+000065b0: 1c41 7c6f 6094 5fc1 6876 6909 9925 6496  .A|o`._.hvi..%d.
+000065c0: 90c1 28cd 325a 71d0 e807 4a62 29c9 5ac7  ..(.2Zq...Jb).Z.
+000065d0: 5612 5b49 b092 6025 214a 4294 c451 1228  V.[I..`%!JB..Q.(
+000065e0: 9e8b b2a8 ae20 18e2 a26b f3ba fcbe 13a8  ..... ...k......
+000065f0: 5177 120a 55e2 34bd ad57 fc43 de23 3190  Qw..U.4..W.C.#1.
+00006600: 7467 8d08 bbd8 b31d ec03 77c6 42c2 3ee4  tg........w.B.>.
+00006610: b200 edd6 2582 674a 57ae ecf7 e8a2 81ae  ....%.gJW.......
+00006620: 5c10 ecd1 b506 ba12 9e3d baf6 4057 56a3  \........=..@WV.
+00006630: 3dba 78a0 eb7c 4597 0c74 ddaf e83a 035d  =.x..|E..t...:.]
+00006640: 79de b147 d71d e8fa 5fd1 f586 5848 96ee  y..G...._...XH..
+00006650: 51de 024e b58e fbc0 f31b 595a 5a39 1687  Q..N......YZZ9..
+00006660: 753b b71d 1a54 a78b 7476 fea9 afb0 5d55  u;...T..tv....]U
+00006670: 9525 95a6 a755 c0ae e489 bbf8 d5a0 eabf  .%...U..........
+00006680: c2ad 0514 0868 9767 ab2a e3e2 beb4 5c9d  .....h.g.*....\.
+00006690: 3759 d7e0 b2b3 acaf 91be b9a9 9143 8540  7Y...........C.@
+000066a0: 9cf9 6fab ae4b e9fa ee6c f5b1 aeba 1399  ..o..K...l......
+000066b0: 41b5 ee9c bca2 4cfc 08f3 d8ca dd9b 1e6a  A.....L........j
+000066c0: c929 c922 3a87 75c8 44ff d7f2 df46 c9fb  .).":.u.D....F..
+000066d0: 5e98 deb9 41d3 fed0 bfbd 7323 6b7b db0f  ^...A.....s#k{..
+000066e0: 56f9 ede8 37b2 efdd 8362 99b2 5380 d8ea  V...7....b..S...
+000066f0: 16c3 4505 e51c 826a 28c1 e120 c5db beaa  ..E....j(.. ....
+00006700: 0efa de00 aca4 86ce b889 ce94 1529 78dd  .............)x.
+00006710: a455 ddc2 57d3 3203 5878 60b8 aa3f 606a  .U..W.2.Xx`..?`j
+00006720: 53f0 6c91 a4cb a214 8b0d 1064 8b94 b594  S.l........d....
+00006730: affb d56c 1582 448a 27fa 97cf 7f76 d241  ...l..D.'....v.A
+00006740: 3a58 7287 f012 e950 ed4a 876a 573a 54fb  :Xr....P.J.jW:T.
+00006750: d341 0ead 0de4 8e47 a4f3 af00 7272 4888  .A.....G....rrH.
+00006760: bf58 0178 46c4 05cc 3de2 f606 71d8 d0da  .X.xF...=...q...
+00006770: 22e6 47c8 9f08 b90c da81 432e 70ee 21c7  ".G.......C.p.!.
+00006780: 03c8 015e b99d 3a42 fe24 c8d1 6ba8 eb02  ...^..:B.$..k...
+00006790: e71e 7232 68e5 2671 258c 47c8 df1e e402  ..r2h.&q%.G.....
+000067a0: e71e 7267 0039 41f8 b52c df8e 903f 1172  ..rg.9A..,...?.r
+000067b0: 8173 0fb9 3b80 dc77 3bef 8f90 bf3d c805  .s..;..w;....=..
+000067c0: ce3d e4de 0672 1b5b 22e8 47c8 df22 e402  .=...r.[".G.."..
+000067d0: e71e 727f 00b9 e739 c7e5 db1b 855c e0dc  ..r....9.....\..
+000067e0: fdeb e9e6 5ca6 19d7 7c41 d9fa 9406 9e38  ....\...|A.....8
+000067f0: eb12 a39f ddfd c3f1 8dca f691 ce8b 24c9  ..............$.
+00006800: 6b8b f1c3 471f f207 9c63 7c76 1e14 a820  k...G....c|v... 
+00006810: 1ce3 b363 576d bb62 637d 0cd0 ae3d 28f2  ...cWm.bc}...=(.
+00006820: 2c4f 7a7f 0cd0 8e1d 9b6c e3c7 00ed dedf  ,Oz......l......
+00006830: a8ff 0338 0668 c76e 00dc 3d16 e97d 6b67  ...8.h.n..=..}kg
+00006840: 87b8 c722 bdbd d21c 2e2e e57f 54a8 1f6a  ..."........T..j
+00006850: bbdf 71bb 7f1d 3ff9 0f00 0000 ffff 0300  ..q...?.........
+00006860: 504b 0304 1400 0600 0800 0000 2100 d5d1  PK..........!...
+00006870: 92f1 bc00 0000 3701 0000 2c00 0000 7070  ......7...,...pp
+00006880: 742f 736c 6964 654c 6179 6f75 7473 2f5f  t/slideLayouts/_
+00006890: 7265 6c73 2f73 6c69 6465 4c61 796f 7574  rels/slideLayout
+000068a0: 352e 786d 6c2e 7265 6c73 8ccf bd0a c230  5.xml.rels.....0
+000068b0: 1007 f05d f01d c2ed 26ad 8388 3475 11c1  ...]....&...4u..
+000068c0: c145 f401 8ee4 da06 db24 e4a2 e8db 9bd1  .E.......$......
+000068d0: 8283 e37d fdfe 5cb3 7f4d a378 5262 17bc  ...}..\..M.xRb..
+000068e0: 865a 5620 c89b 609d ef35 dcae c7d5 1604  .ZV ..`..5......
+000068f0: 67f4 16c7 e049 c39b 18f6 ed72 d15c 68c4  g....I.....r.\h.
+00006900: 5c8e 7870 9145 513c 6b18 728e 3ba5 d80c  \.xp.EQ<k.r.;...
+00006910: 3421 cb10 c997 4917 d284 b994 a957 11cd  4!....I......W..
+00006920: 1d7b 52eb aada a8f4 6d40 3b33 c5c9 6a48  .{R.....m@;3..jH
+00006930: 275b 83b8 be23 fd63 87ae 7386 0ec1 3c26  '[...#.c..s...<&
+00006940: f2f9 4784 e2d1 593a 2367 4a85 c5d4 53d6  ..G...Y:#gJ...S.
+00006950: 20e5 777f b654 cb12 01aa 6dd4 ecdd f603   .w..T....m.....
+00006960: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+00006970: 0000 2100 d5d1 92f1 bc00 0000 3701 0000  ..!.........7...
+00006980: 2c00 0000 7070 742f 736c 6964 654c 6179  ,...ppt/slideLay
+00006990: 6f75 7473 2f5f 7265 6c73 2f73 6c69 6465  outs/_rels/slide
+000069a0: 4c61 796f 7574 312e 786d 6c2e 7265 6c73  Layout1.xml.rels
+000069b0: 8ccf bd0a c230 1007 f05d f01d c2ed 26ad  .....0...]....&.
+000069c0: 8388 3475 11c1 c145 f401 8ee4 da06 db24  ..4u...E.......$
+000069d0: e4a2 e8db 9bd1 8283 e37d fdfe 5cb3 7f4d  .........}..\..M
+000069e0: a378 5262 17bc 865a 5620 c89b 609d ef35  .xRb...ZV ..`..5
+000069f0: dcae c7d5 1604 67f4 16c7 e049 c39b 18f6  ......g....I....
+00006a00: ed72 d15c 68c4 5c8e 7870 9145 513c 6b18  .r.\h.\.xp.EQ<k.
+00006a10: 728e 3ba5 d80c 3421 cb10 c997 4917 d284  r.;...4!....I...
+00006a20: b994 a957 11cd 1d7b 52eb aada a8f4 6d40  ...W...{R.....m@
+00006a30: 3b33 c5c9 6a48 275b 83b8 be23 fd63 87ae  ;3..jH'[...#.c..
+00006a40: 7386 0ec1 3c26 f2f9 4784 e2d1 593a 2367  s...<&..G...Y:#g
+00006a50: 4a85 c5d4 53d6 20e5 777f b654 cb12 01aa  J...S. .w..T....
+00006a60: 6dd4 ecdd f603 0000 ffff 0300 504b 0304  m...........PK..
+00006a70: 1400 0600 0800 0000 2100 d5d1 92f1 bc00  ........!.......
+00006a80: 0000 3701 0000 2c00 0000 7070 742f 736c  ..7...,...ppt/sl
+00006a90: 6964 654c 6179 6f75 7473 2f5f 7265 6c73  ideLayouts/_rels
+00006aa0: 2f73 6c69 6465 4c61 796f 7574 322e 786d  /slideLayout2.xm
+00006ab0: 6c2e 7265 6c73 8ccf bd0a c230 1007 f05d  l.rels.....0...]
+00006ac0: f01d c2ed 26ad 8388 3475 11c1 c145 f401  ....&...4u...E..
+00006ad0: 8ee4 da06 db24 e4a2 e8db 9bd1 8283 e37d  .....$.........}
+00006ae0: fdfe 5cb3 7f4d a378 5262 17bc 865a 5620  ..\..M.xRb...ZV 
+00006af0: c89b 609d ef35 dcae c7d5 1604 67f4 16c7  ..`..5......g...
+00006b00: e049 c39b 18f6 ed72 d15c 68c4 5c8e 7870  .I.....r.\h.\.xp
+00006b10: 9145 513c 6b18 728e 3ba5 d80c 3421 cb10  .EQ<k.r.;...4!..
+00006b20: c997 4917 d284 b994 a957 11cd 1d7b 52eb  ..I......W...{R.
+00006b30: aada a8f4 6d40 3b33 c5c9 6a48 275b 83b8  ....m@;3..jH'[..
+00006b40: be23 fd63 87ae 7386 0ec1 3c26 f2f9 4784  .#.c..s...<&..G.
+00006b50: e2d1 593a 2367 4a85 c5d4 53d6 20e5 777f  ..Y:#gJ...S. .w.
+00006b60: b654 cb12 01aa 6dd4 ecdd f603 0000 ffff  .T....m.........
+00006b70: 0300 504b 0304 1400 0600 0800 0000 2100  ..PK..........!.
+00006b80: d5d1 92f1 bc00 0000 3701 0000 2c00 0000  ........7...,...
+00006b90: 7070 742f 736c 6964 654c 6179 6f75 7473  ppt/slideLayouts
+00006ba0: 2f5f 7265 6c73 2f73 6c69 6465 4c61 796f  /_rels/slideLayo
+00006bb0: 7574 332e 786d 6c2e 7265 6c73 8ccf bd0a  ut3.xml.rels....
+00006bc0: c230 1007 f05d f01d c2ed 26ad 8388 3475  .0...]....&...4u
+00006bd0: 11c1 c145 f401 8ee4 da06 db24 e4a2 e8db  ...E.......$....
+00006be0: 9bd1 8283 e37d fdfe 5cb3 7f4d a378 5262  .....}..\..M.xRb
+00006bf0: 17bc 865a 5620 c89b 609d ef35 dcae c7d5  ...ZV ..`..5....
+00006c00: 1604 67f4 16c7 e049 c39b 18f6 ed72 d15c  ..g....I.....r.\
+00006c10: 68c4 5c8e 7870 9145 513c 6b18 728e 3ba5  h.\.xp.EQ<k.r.;.
+00006c20: d80c 3421 cb10 c997 4917 d284 b994 a957  ..4!....I......W
+00006c30: 11cd 1d7b 52eb aada a8f4 6d40 3b33 c5c9  ...{R.....m@;3..
+00006c40: 6a48 275b 83b8 be23 fd63 87ae 7386 0ec1  jH'[...#.c..s...
+00006c50: 3c26 f2f9 4784 e2d1 593a 2367 4a85 c5d4  <&..G...Y:#gJ...
+00006c60: 53d6 20e5 777f b654 cb12 01aa 6dd4 ecdd  S. .w..T....m...
+00006c70: f603 0000 ffff 0300 504b 0304 1400 0600  ........PK......
+00006c80: 0800 0000 2100 d5d1 92f1 bc00 0000 3701  ....!.........7.
+00006c90: 0000 2c00 0000 7070 742f 736c 6964 654c  ..,...ppt/slideL
+00006ca0: 6179 6f75 7473 2f5f 7265 6c73 2f73 6c69  ayouts/_rels/sli
+00006cb0: 6465 4c61 796f 7574 342e 786d 6c2e 7265  deLayout4.xml.re
+00006cc0: 6c73 8ccf bd0a c230 1007 f05d f01d c2ed  ls.....0...]....
+00006cd0: 26ad 8388 3475 11c1 c145 f401 8ee4 da06  &...4u...E......
+00006ce0: db24 e4a2 e8db 9bd1 8283 e37d fdfe 5cb3  .$.........}..\.
+00006cf0: 7f4d a378 5262 17bc 865a 5620 c89b 609d  .M.xRb...ZV ..`.
+00006d00: ef35 dcae c7d5 1604 67f4 16c7 e049 c39b  .5......g....I..
+00006d10: 18f6 ed72 d15c 68c4 5c8e 7870 9145 513c  ...r.\h.\.xp.EQ<
+00006d20: 6b18 728e 3ba5 d80c 3421 cb10 c997 4917  k.r.;...4!....I.
+00006d30: d284 b994 a957 11cd 1d7b 52eb aada a8f4  .....W...{R.....
+00006d40: 6d40 3b33 c5c9 6a48 275b 83b8 be23 fd63  m@;3..jH'[...#.c
+00006d50: 87ae 7386 0ec1 3c26 f2f9 4784 e2d1 593a  ..s...<&..G...Y:
+00006d60: 2367 4a85 c5d4 53d6 20e5 777f b654 cb12  #gJ...S. .w..T..
+00006d70: 01aa 6dd4 ecdd f603 0000 ffff 0300 504b  ..m...........PK
+00006d80: 0304 1400 0600 0800 0000 2100 b4cf 5819  ..........!...X.
+00006d90: b900 0000 2401 0000 2c00 0000 7070 742f  ....$...,...ppt/
+00006da0: 6e6f 7465 734d 6173 7465 7273 2f5f 7265  notesMasters/_re
+00006db0: 6c73 2f6e 6f74 6573 4d61 7374 6572 312e  ls/notesMaster1.
+00006dc0: 786d 6c2e 7265 6c73 8ccf c10a c230 0c06  xml.rels.....0..
+00006dd0: e0bb e03b 94dc 6db7 1d44 64ed 2e22 ec2a  ...;..m..Dd..".*
+00006de0: f301 4a97 75c5 ad2d 6d15 f7f6 1676 71e0  ..J.u..-m....vq.
+00006df0: c14b 2009 ff17 5237 ef79 222f 0cd1 38cb  .K ...R7.y"/..8.
+00006e00: a1a4 0510 b4ca f5c6 6a0e f7ee 7a38 0189  ........j...z8..
+00006e10: 49da 5e4e ce22 8705 2334 62bf ab6f 38c9  I.^N."..#4b..o8.
+00006e20: 9443 7134 3e92 acd8 c861 4cc9 9f19 8b6a  .Cq4>....aL....j
+00006e30: c459 46ea 3cda bc19 5c98 65ca 6dd0 cc4b  .YF.<...\.e.m..K
+00006e40: f590 1a59 5514 4716 be0d 101b 93b4 3d87  ...YU.G.......=.
+00006e50: d0f6 2590 6ef1 f88f ed86 c128 bc38 f59c  ..%.n......(.8..
+00006e60: d1a6 1f27 58ca 59cc a00c 1a13 074a d7c9  ...'X.Y......J..
+00006e70: 5a2b 9a3d 60a2 669b dfc4 0700 00ff ff03  Z+.=`.f.........
+00006e80: 0050 4b03 0414 0006 0008 0000 0021 008f  .PK..........!..
+00006e90: 1de5 b0b6 0500 008c 1d00 0021 0000 0070  ...........!...p
+00006ea0: 7074 2f6e 6f74 6573 4d61 7374 6572 732f  pt/notesMasters/
+00006eb0: 6e6f 7465 734d 6173 7465 7231 2e78 6d6c  notesMaster1.xml
+00006ec0: ec58 db8e db36 107d 2fd0 7f10 d4c7 c2d1  .X...6.}/.......
+00006ed0: fd66 c41b d8de 75b2 c526 59c4 9b0f a025  .f....u..&Y....%
+00006ee0: da16 4c91 2a45 3bbb 2902 e4b7 dacf c997  ..L.*E;.).......
+00006ef0: 7448 91be ed76 e32c dca2 41fc 628d 86c3  tH...v.,..A.b...
+00006f00: 21e7 f0cc 68cc e72f 6e2b 62ad 306f 4a46  !...h../n+b.0oJF
+00006f10: 7bb6 f7cc b52d 4c73 5694 74d6 b3df df8c  {....-LsV.t.....
+00006f20: 3aa9 6d35 02d1 0211 4671 cfbe c38d fde2  :.m5....Fq......
+00006f30: ece7 9f9e d75d ca04 6e5e a346 606e 8117  .....]..n^.F`n..
+00006f40: da74 51cf 9e0b 5177 1da7 c9e7 b842 cd33  .tQ...Qw.....B.3
+00006f50: 5663 0a63 53c6 2b24 e095 cf9c 82a3 0fe0  Vc.cS.+$........
+00006f60: bd22 8eef bab1 53a1 92da 7a3e 3f64 3e9b  ."....S...z>?d>.
+00006f70: 4ecb 1c9f b37c 5961 2a5a 271c 1324 2082  N....|Ya*Z'..$ .
+00006f80: 665e d68d f156 1fe2 ade6 b801 376a f6ce  f^...V......7j..
+00006f90: 96ce 20c2 7c4c 0af9 9ccc dadf 7778 6a95  .. .|L......wxj.
+00006fa0: c52d e0e4 ba1e 58a0 aef2 8c87 845b 2b44  .-....X......[+D
+00006fb0: 7af6 64e6 d9ce d973 471b 6b49 4e6e ea1b  z.d....sG.kINn..
+00006fc0: 8eb1 94e8 ea25 afc7 f535 572b bc59 5d73  .....%...5W+.Y]s
+00006fd0: f009 2e6d 8ba2 0a10 960e d480 3653 af74  ...m........6S.t
+00006fe0: a504 676f facc 88a8 7b3b e595 7c02 3c16  ..go....{;..|.<.
+00006ff0: ec10 cef1 4efe 3a52 876f 8595 b7ca 7ca3  ....N.:R.o....|.
+00007000: cde7 6f1f b0cd e717 0f58 3b66 0167 6b51  ..o......X;f.gkQ
+00007010: 1955 bbb9 fbe1 f826 9c57 1815 4090 6b82  .U.....&.W..@.k.
+00007020: 723c 6744 ca0a 2365 6c36 dfd4 572c 5f34  r<gD..#el6..W,_4
+00007030: 1665 109c c4a2 8d75 6dd1 0220 9ff5 dc12  .e.....um.. ....
+00007040: 7735 f89d 171c 98f9 b167 ffbe 441c 28a8  w5.......g..D.(.
+00007050: a7b4 764a d86c f270 84fc 2cf1 5257 471e  ..vJ.l.p..,.RWG.
+00007060: 4669 92a6 3be1 a36e cd1b f112 b3ca 9242  Fi..;..n.......B
+00007070: cfe6 3817 8a09 6875 d588 d6d4 98a8 7db4  ..8...hu......}.
+00007080: abd7 5d71 3b60 c59d b49c c013 5082 a483  ..]q;`......P...
+00007090: f973 c63f da16 b9a4 4dcf cebc 3084 a585  .s.?....M...0...
+000070a0: 7a09 a3c4 8717 be3d 32d9 1911 64c8 c83a  z......=2...d..:
+000070b0: 02d2 88b1 b823 58c9 2be2 c1b2 1622 3348  .....#X.+...."3H
+000070c0: 6aa2 f657 e0e9 3b50 49c4 3c60 b98e 4a5b  j..W..;PI.<`..J[
+000070d0: b6f2 9687 5a81 428b 6bc4 919c 4690 ac07  ....Z.B.k...F...
+000070e0: 9876 7ebb d633 6b15 9d89 4a05 fa38 2302  .v~..3k...J..8#.
+000070f0: c388 7324 f00e 1ffc 63f0 a110 b6ce cd6f  ..s$....c......o
+00007100: 6642 90a6 61ec 053f 0a1f f853 f930 2585  fB..a..?...S.0%.
+00007110: 3ac9 3fd2 cccf 5ccf 1b74 e220 f43b e945  :.?...\..t. .;.E
+00007120: 9875 d2c0 1f75 bc30 0bdd fef9 79bf 1fc6  .u...u.0....y...
+00007130: 9f6c 7330 70dc a2ac f0a8 9c2d 397e bb6c  .ls0p......-9~.l
+00007140: e1e1 7ba4 b29a 4a0c 0946 741d 8038 f35d  ..{...J..Ft..8.]
+00007150: df77 dcc8 f113 b91d a136 3595 15f9 d8d4  .w.......65.....
+00007160: 0c0d 35c7 a42c b075 59a1 d92e 4383 af33  ..5..,.uY...C..3
+00007170: 14a4 774c 6869 3887 4de1 7e53 031b 0ea3  ..wLhi8.M.~S....
+00007180: 6f43 8acb 6aa6 29ac 12e2 9b28 1ca7 91a2  oC..j.)....(....
+00007190: 29b0 d4f3 c2c0 6d0f 74c3 e328 4ce3 d0f0  ).....m.t..(L...
+000071a0: 3870 d3d8 5b1f f993 888c e0eb 3f2a 0969  8p..[.......?*.i
+000071b0: a946 ad0f 9245 09f8 54d8 3080 518e 1ab7  .F...E..T.0.Q...
+000071c0: 9bef 2360 bad0 eb6e 5949 b2d1 ff2a 3b2c  ..#`...nYI...*;,
+000071d0: 4473 f0d3 b373 a13e 1a1b a2ab 977f a1f2  Ds...s.>........
+000071e0: 4586 5e6f 64c7 b443 acf0 18a5 4f42 b4fb  E.^od..C....OB..
+000071f0: 2d6c 69a4 58fb 541a 0184 6e14 3d4a a3d8  -li.X.T...n.=J..
+00007200: 75c3 d6e2 3baa 879b 4396 1511 eadd da42  u...;...C......B
+00007210: 01b2 5397 de8f 4d29 1a92 325f 5882 59b8  ..S...M)..2_X.Y.
+00007220: 2885 a59b 5e21 6169 a4d3 6653 a0da dad9  (...^!ai..fS....
+00007230: 2eb0 b38a 3ac9 c757 19e3 9cd1 c222 7885  ....:..W....."x.
+00007240: c901 1e55 9978 dce3 cdbc e487 3b54 8479  ...U.x......;T.y
+00007250: dce1 882d b998 1fec 51f1 fb2b 1ecb e983  ...-....Q..+....
+00007260: 0e8f 9d85 b1c9 c211 63f2 f4b6 d330 3a46  ........c....0:F
+00007270: 1a4e c55e 47da 66a1 82e0 099d 690a c9e8  .N.^G.f.....i...
+00007280: 7bfa 48fe b91f 49fe fff9 b7ae b893 efa4  {.H...I.........
+00007290: 554d 76fb 8137 cb6a b247 98f8 1884 816f  UMv..7.j.G.....o
+000072a0: 3eb8 7e88 338a 8f4f ee61 7f44 e61c a3a9  >.~.3..O.a.D....
+000072b0: 1d65 fdc0 cd3a d945 1c75 0671 78d1 1924  .e...:.E.u.qx..$
+000072c0: a9d7 7133 2f48 cf33 cff7 d24d 53db 4862  ..q3/H.3...MS.Hb
+000072d0: 5038 bc43 7bd9 2f9f fffc e5cb e7bf 8ed0  P8.C{./.........
+000072e0: c8aa 87b9 4c80 d385 c3d1 92b5 e425 0432  ....L........%.2
+000072f0: 1864 b13f 4c07 9d81 178e 3ae1 7996 74fa  .d.?L.....:.y.t.
+00007300: 2308 6914 0561 381c a4fd 6170 f149 de6f  #.i..a8...ap.I.o
+00007310: 7861 37e7 585d 7d5c 16e6 d2c4 0bef 5d9b  xa7.X]}\......].
+00007320: 5465 ce59 c3a6 e259 ce2a 7dff e2d4 ec03  Te.Y...Y.*}.....
+00007330: e635 2bd5 158c e7ea 7b1c d5e5 4571 1c24  .5+.....{...Eq.$
+00007340: 51ac 5b03 b535 f354 9b95 69a1 6f56 72c2  Q.[..5.T..i.oVr.
+00007350: 5fa3 da9a cc3c 487e 01bd b3b8 05a9 5880  _....<H~......X.
+00007360: 3499 f952 e74b 9d2f 7520 a13c c754 8085  4..R.K./u .<.T..
+00007370: 168c c637 9ab5 4d60 3481 d184 4613 1a4d  ...7..M`4...F..M
+00007380: 6434 91d1 c446 031f 8b39 29e9 02b0 900f  d4...F...9).....
+00007390: db9a 32f2 aa55 18a9 ad00 ea12 ec1e 272b  ..2..U........'+
+000073a0: c4af 5afe eab2 6601 336f d064 fc51 33be  ..Z...f.3o.d.Q3.
+000073b0: 65b9 32c1 e88a 0ef8 42fd 7390 b758 54bf  e.2.....B.s..XT.
+000073c0: c290 fc17 51d2 d9f5 92b6 7f23 1ea2 b8b5  ....Q......#....
+000073d0: c05c dedc 49f9 5ef3 bd77 3d05 e0de 6fbe  .\..I.^..w=...o.
+000073e0: 61d7 7255 45ec 2954 b89e fd6b 453b 44e8  a.rUE.)T...kE;D.
+000073f0: f281 f606 30d2 f744 cdde 40de 68df ed0e  ....0..D..@.h...
+00007400: 7733 4f89 fe06 1a95 e927 7c34 281a 9f60  w3O......'|4(..`
+00007410: 838f 01e1 848f 0445 e313 6ef0 f182 c48b  .......E..n.....
+00007420: 4f00 1954 3440 d116 40a9 9faa cffd 0920  O..T4@..@...... 
+00007430: 898a 0628 de00 e4fb 692c af49 4e00 2954  ...(....i,.IN.)T
+00007440: 3440 c916 4049 189c 6af4 1a15 0d50 ba01  4@..@I..j....P..
+00007450: 48a2 732a d26b 5434 40d9 1640 7194 9c8a  H.s*.kT4@..@q...
+00007460: f41a 95f6 8fdc 56bf 685e dbeb a4b3 bf01  ......V.h^......
+00007470: 0000 ffff 0300 504b 0304 0a00 0000 0000  ......PK........
+00007480: 0000 2100 669f 9372 be08 0000 be08 0000  ..!.f..r........
+00007490: 1700 0000 646f 6350 726f 7073 2f74 6875  ....docProps/thu
+000074a0: 6d62 6e61 696c 2e6a 7065 67ff d8ff e000  mbnail.jpeg.....
+000074b0: 104a 4649 4600 0101 0000 6000 6000 00ff  .JFIF.....`.`...
+000074c0: e100 8045 7869 6600 004d 4d00 2a00 0000  ...Exif..MM.*...
+000074d0: 0800 0401 1a00 0500 0000 0100 0000 3e01  ..............>.
+000074e0: 1b00 0500 0000 0100 0000 4601 2800 0300  ..........F.(...
+000074f0: 0000 0100 0200 0087 6900 0400 0000 0100  ........i.......
+00007500: 0000 4e00 0000 0000 0000 6000 0000 0100  ..N.......`.....
+00007510: 0000 6000 0000 0100 03a0 0100 0300 0000  ..`.............
+00007520: 0100 0100 00a0 0200 0400 0000 0100 0001  ................
+00007530: 00a0 0300 0400 0000 0100 0000 9000 0000  ................
+00007540: 00ff ed00 3850 686f 746f 7368 6f70 2033  ....8Photoshop 3
+00007550: 2e30 0038 4249 4d04 0400 0000 0000 0038  .0.8BIM........8
+00007560: 4249 4d04 2500 0000 0000 10d4 1d8c d98f  BIM.%...........
+00007570: 00b2 04e9 8009 98ec f842 7eff c000 1108  .........B~.....
+00007580: 0090 0100 0301 2200 0211 0103 1101 ffc4  ......".........
+00007590: 001f 0000 0105 0101 0101 0101 0000 0000  ................
+000075a0: 0000 0000 0102 0304 0506 0708 090a 0bff  ................
+000075b0: c400 b510 0002 0103 0302 0403 0505 0404  ................
+000075c0: 0000 017d 0102 0300 0411 0512 2131 4106  ...}........!1A.
+000075d0: 1351 6107 2271 1432 8191 a108 2342 b1c1  .Qa."q.2....#B..
+000075e0: 1552 d1f0 2433 6272 8209 0a16 1718 191a  .R..$3br........
+000075f0: 2526 2728 292a 3435 3637 3839 3a43 4445  %&'()*456789:CDE
+00007600: 4647 4849 4a53 5455 5657 5859 5a63 6465  FGHIJSTUVWXYZcde
+00007610: 6667 6869 6a73 7475 7677 7879 7a83 8485  fghijstuvwxyz...
+00007620: 8687 8889 8a92 9394 9596 9798 999a a2a3  ................
+00007630: a4a5 a6a7 a8a9 aab2 b3b4 b5b6 b7b8 b9ba  ................
+00007640: c2c3 c4c5 c6c7 c8c9 cad2 d3d4 d5d6 d7d8  ................
+00007650: d9da e1e2 e3e4 e5e6 e7e8 e9ea f1f2 f3f4  ................
+00007660: f5f6 f7f8 f9fa ffc4 001f 0100 0301 0101  ................
+00007670: 0101 0101 0101 0000 0000 0000 0102 0304  ................
+00007680: 0506 0708 090a 0bff c400 b511 0002 0102  ................
+00007690: 0404 0304 0705 0404 0001 0277 0001 0203  ...........w....
+000076a0: 1104 0521 3106 1241 5107 6171 1322 3281  ...!1..AQ.aq."2.
+000076b0: 0814 4291 a1b1 c109 2333 52f0 1562 72d1  ..B.....#3R..br.
+000076c0: 0a16 2434 e125 f117 1819 1a26 2728 292a  ..$4.%.....&'()*
+000076d0: 3536 3738 393a 4344 4546 4748 494a 5354  56789:CDEFGHIJST
+000076e0: 5556 5758 595a 6364 6566 6768 696a 7374  UVWXYZcdefghijst
+000076f0: 7576 7778 797a 8283 8485 8687 8889 8a92  uvwxyz..........
+00007700: 9394 9596 9798 999a a2a3 a4a5 a6a7 a8a9  ................
+00007710: aab2 b3b4 b5b6 b7b8 b9ba c2c3 c4c5 c6c7  ................
+00007720: c8c9 cad2 d3d4 d5d6 d7d8 d9da e2e3 e4e5  ................
+00007730: e6e7 e8e9 eaf2 f3f4 f5f6 f7f8 f9fa ffdb  ................
+00007740: 0043 0002 0202 0202 0203 0202 0305 0303  .C..............
+00007750: 0305 0605 0505 0506 0806 0606 0606 080a  ................
+00007760: 0808 0808 0808 0a0a 0a0a 0a0a 0a0a 0c0c  ................
+00007770: 0c0c 0c0c 0e0e 0e0e 0e0f 0f0f 0f0f 0f0f  ................
+00007780: 0f0f 0fff db00 4301 0202 0204 0404 0704  ......C.........
+00007790: 0407 100b 090b 1010 1010 1010 1010 1010  ................
+000077a0: 1010 1010 1010 1010 1010 1010 1010 1010  ................
+000077b0: 1010 1010 1010 1010 1010 1010 1010 1010  ................
+000077c0: 1010 1010 1010 1010 ffdd 0004 0010 ffda  ................
+000077d0: 000c 0301 0002 1103 1100 3f00 fdfc a28a  ..........?.....
+000077e0: 2800 a28a 2800 a28a 2800 a28a 2800 a28a  (...(...(...(...
+000077f0: 2800 a28a 2800 a28a 2800 a28a 2800 a28a  (...(...(...(...
+00007800: 2800 a28a 2800 a28a 2800 a28a 2800 a28a  (...(...(...(...
+00007810: 2800 a28a 2800 a28a 2800 a28a 2803 ffd0  (...(...(...(...
+00007820: fdfc a28a 2800 a28a 2800 a28a 2800 a28a  ....(...(...(...
+00007830: 2800 a28a 2800 a28a 2800 a28a 2800 a28a  (...(...(...(...
+00007840: 2800 a28a 2800 a28a 2800 a28a 2800 a28a  (...(...(...(...
+00007850: 2800 a28a 2800 a28a 2800 a28a 2800 a28a  (...(...(...(...
+00007860: 2803 ffd1 fdfc a28a 2800 a28a 2800 a28a  (.......(...(...
+00007870: 2800 a28a 2800 a28a 2800 a28a 2800 a28a  (...(...(...(...
+00007880: 2800 a28a 2800 a28a 2800 a28a 2800 a28a  (...(...(...(...
+00007890: 2800 a28a 2800 a28a 2800 a28a 2800 a28a  (...(...(...(...
+000078a0: 2800 a28a 2803 ffd2 fdfc a28a 2800 a28a  (...(.......(...
+000078b0: 2800 a28a 2800 a28a 2800 a28a 2800 a28a  (...(...(...(...
+000078c0: 2800 a2be 5db0 fda9 742b dbd4 9e4f 08eb  (...]...t+...O..
+000078d0: b69e 1aff 0084 824f 0c49 aecd 15ba d926  .......O.I.....&
+000078e0: a697 ad60 8367 9e6e 1a19 2e14 4627 588c  ...`.g.n....F'X.
+000078f0: 6199 5588 3bb6 a5c7 ed4f e1fb 5bfd 5649  a.U.;....O..[.VI
+00007900: bc25 aeaf 86fc 3fae 9f0e ea7a eb45 6cb6  .%....?....z.El.
+00007910: 36b7 bf69 5b45 6da6 7f3e 587c c740 f2c7  6..i[Em..>X|.@..
+00007920: 132c 7bbe 6c61 f680 7d47 457c 87a0 fed2  .,{.la..}GE|....
+00007930: 9e28 8e3f 8a3a c78c fc01 a9db 687f 0f75  .(.?.:......h..u
+00007940: 792d 4dcd 99b4 9dc5 9c50 59cb 233c 31dd  y-M......PY.#<1.
+00007950: 3caf 2469 3bdc 36c4 dbe4 a803 3282 87db  <.$i;.6.....2...
+00007960: 3c05 f16f c25f 121b 5abb f0b4 a6e3 46d2  <..o._..Z.....F.
+00007970: 6ec5 945a a6e8 fec5 7f32 a079 bec9 2062  n..Z.....2.y.. b
+00007980: 6548 59bc b77c 05f3 032a 93b4 d007 a851  eHY..|...*.....Q
+00007990: 5f28 e93f b476 a965 e26f 8b4b f10b c2f7  _(.?.v.e.o.K....
+000079a0: 3a17 84fe 1b4f ff00 215d f6d2 2f90 b616  :....O..!]../...
+000079b0: f758 78e2 b892 6796 6329 6884 7163 6144  .Xx...g.c)h.qcaD
+000079c0: 6c49 95ad d87f 695d 0749 9efa dfe2 7786  lI....i].I....w.
+000079d0: b57f 87e6 db45 bbf1 0427 555b 6916 e74e  .....E...'U[i..N
+000079e0: b0d9 f6a6 4367 3dc6 d9a1 1246 5e07 c49f  ....Cg=....F^...
+000079f0: 38da 1b9c 007d 2345 7cb1 a97e d037 17da  8....}#E|..~.7..
+00007a00: 6ead e1dd 5bc2 dad7 8135 cd4b c3da 9eaf  n...[....5.K....
+00007a10: a23e a62d 7fd2 a3b2 8434 9b0d b4f3 f953  .>.-.....4.....S
+00007a20: c3e6 46ed 0ca1 5c03 900e d6da 7c38 f8e9  ..F...\.....|8..
+00007a30: 797f 67e0 9f04 47a1 ea7e 29d7 a6f0 d681  y.g...G..~).....
+00007a40: aaeb 3790 3da4 696b 1eaa 8634 b891 6e27  ..7.=.ik...4..n'
+00007a50: 8649 7749 148d 2792 8fb4 0e79 2148 07d4  .IwI..'....y!H..
+00007a60: f451 4500 1451 4500 1451 4500 1451 4500  .QE..QE..QE..QE.
+00007a70: 1451 4500 1451 4500 7fff d3fd fca2 8a28  .QE..QE........(
+00007a80: 00a2 8a28 00a2 8a28 00a2 8a28 00a2 8a28  ...(...(...(...(
+00007a90: 00a2 8a28 03f3 f3e1 b7c2 3f8b de32 f0d4  ...(......?..2..
+00007aa0: fe16 f136 a763 a778 1478 ef56 d6de ddec  ...6.c.x.x.V....
+00007ab0: 678b 5768 ac7c 433d f416 c199 c446 19a6  g.Wh.|C=.....F..
+00007ac0: 8e39 7cfd a18c 4db1 54e4 4951 785f e10f  .9|...M.T.IQx_..
+00007ad0: c5bf 1fd8 f8ff 00c1 1aae a165 a578 0b5c  ...........e.x.\
+00007ae0: f1de a77d 7093 d94e 9aa9 b583 515b 8315  ...}p..N....Q[..
+00007af0: bb97 10bc 5746 3189 9972 88cd b43f ca57  ....WF1..r...?.W
+00007b00: f422 8a00 f972 fbe1 1fc5 8b3b df89 3a6f  ."...r.....;..:o
+00007b10: 837c 4ba7 695a 47c4 1be5 d412 f0db cafa  .|K.iZG.........
+00007b20: 9e9f 2cf0 5a59 dd08 fe6f 25f1 05bb bc0c  ..,.ZY...o%.....
+00007b30: 40db 2bae e055 4ee9 fe1e 7ecc 9e08 f06e  @.+..UN...~....n
+00007b40: 8173 f0df 5dd2 b4cf 13f8 1349 bb37 1e19  .s..]......I.7..
+00007b50: b1d4 ed12 f26d 261b 850d 716d e64e 1f7a  .....m&...qm.N.z
+00007b60: 09b7 3c4d f7c2 b6c6 242a 9afa 728a 00f9  ..<M....$*..r...
+00007b70: 43c5 ff00 b3df 88bc 57a8 7c52 d00e b169  C.......W.|R...i
+00007b80: 69e1 2f89 b6f0 4acc 90bf f68e 9fa8 dad9  i./...J.........
+00007b90: c167 0b45 f379 3242 bf66 8e5d ac01 ce57  .g.E.y2B.f.]...W
+00007ba0: a1c8 c9f1 27ec f7f1 0be3 20be 6f8e 3afe  ....'..... .o.:.
+00007bb0: 9919 4f0f 6a9a 0e9e ba0d b4d1 88e4 d5c4  ..O.j...........
+00007bc0: 227b f94d cbb9 2ebe 447e 5c23 e55f 9b73  "{.M....D~\#._.s
+00007bd0: be46 3ec5 a280 3e4d 97e0 c7c5 7f1d ead0  .F>...>M........
+00007be0: ebbf 1735 ed1e 5bad 0f45 d574 ad2d 348b  ...5..[..E.t.-4.
+00007bf0: 59e2 8e4b 9d5a 1582 6bdb 9f3a 4620 844c  Y..K.Z..k..:F .L
+00007c00: 2429 90bb dc97 6f97 185e 21fd 9cfc 77ad  $)....o..^!...w.
+00007c10: dbfc 3fd0 e1d4 342b 483c 156b a2c5 0eb9  ..?...4+H<.k....
+00007c20: 15a5 cc7a fdab 69a6 2373 1dac c928 430d  ...z..i.#s...(C.
+00007c30: d88f 6157 c285 76de 92f1 5f67 d140 0514  ..aW..v..._g.@..
+00007c40: 5140 0514 5140 0514 5140 0514 5140 0514  Q@..Q@..Q@..Q@..
+00007c50: 5140 0514 5140 1fff d4fd fca2 8a28 00a2  Q@..Q@.......(..
+00007c60: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
+00007c70: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
+00007c80: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
+00007c90: 8a28 00a2 8a28 00a2 8a28 03ff d5fd fca2  .(...(...(......
+00007ca0: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
+00007cb0: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
+00007cc0: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
+00007cd0: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 03ff  .(...(...(...(..
+00007ce0: d6fd fca2 8a28 00a2 8a28 00a2 8a28 00a2  .....(...(...(..
+00007cf0: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
+00007d00: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
+00007d10: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
+00007d20: 8a28 03ff d7fd fca2 8a28 00a2 8a28 00a2  .(.......(...(..
+00007d30: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
+00007d40: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
+00007d50: 8a28 00a2 8a28 00a2 8a28 00a2 8a28 00a2  .(...(...(...(..
+00007d60: 8a28 00a2 8a28 03ff d950 4b03 0414 0006  .(...(...PK.....
+00007d70: 0008 0000 0021 007b 43bc 5dc4 0600 00cf  .....!.{C.].....
+00007d80: 2000 0014 0000 0070 7074 2f74 6865 6d65   ......ppt/theme
+00007d90: 2f74 6865 6d65 312e 786d 6cec 59cd 8b1b  /theme1.xml.Y...
+00007da0: 3714 bf17 fa3f 0c73 77fc 35e3 8f10 27d8  7....?.sw.5...'.
+00007db0: 633b 9b64 3759 b29b 941c b5b6 3ca3 5833  c;.d7Y......<.X3
+00007dc0: 3292 bc1b 1302 2539 f552 28a4 a597 426f  2.....%9.R(...Bo
+00007dd0: 3d94 d240 030d bdf4 8f09 24b4 e91f d127  =..@......$....'
+00007de0: 8ded 19d9 9ae6 6b13 025d 2fd8 92e6 f79e  ......k..]/.....
+00007df0: 7e7a efe9 e9ad e6c2 a57b 3175 8e31 1784  ~z.......{1u.1..
+00007e00: 251d b77a aee2 3a38 19b1 3149 c28e 7beb  %..z..:8..1I..{.
+00007e10: 7058 6ab9 8e90 2819 23ca 12dc 7117 58b8  pXj...(.#...q.X.
+00007e20: 972e 7efe d905 745e 4638 c60e c827 e23c  ..~...t^F8...'.<
+00007e30: eab8 9194 b3f3 e5b2 18c1 3012 e7d8 0c27  ..........0....'
+00007e40: f06c c278 8c24 7479 581e 7374 027a 635a  .l.x.$tyX.st.zcZ
+00007e50: ae55 2a8d 728c 48e2 3a09 8a41 ed8d c984  .U*.r.H.:..A....
+00007e60: 8cb0 73a8 54ba 1757 ca07 14be 1229 d4c0  ..s.T..W.....)..
+00007e70: 88f2 03a5 1a1b 121a 3b9e 56d5 8f58 8880  ........;.V..X..
+00007e80: 72e7 18d1 8e0b f38c d9c9 21be 275d 8722  r.........!.']."
+00007e90: 21e1 41c7 ade8 8f5b be78 a1bc 16a2 b240  !.A....[.x.....@
+00007ea0: 3627 37d4 9fa5 dc52 603c ad69 391e 1ead  6'7....R`<.i9...
+00007eb0: 053d cff7 1add b57e 0da0 721b 3768 0e1a  .=.....~..r.7h..
+00007ec0: 83c6 5a9f 06a0 d108 569a 7231 7536 6b81  ..Z.....V.r1u6k.
+00007ed0: b7c4 e640 69d3 a2bb dfec d7ab 063e a7bf  ...@i........>..
+00007ee0: be85 effa eacf c06b 50da f4b6 f0c3 6190  .......kP.....a.
+00007ef0: d930 074a 9bfe 16de efb5 7b7d 53bf 06a5  .0.J......{}S...
+00007f00: cdc6 16be 59e9 f6bd a681 d7a0 8892 64ba  ....Y.........d.
+00007f10: 85ae f88d 7ab0 5aed 1a32 6174 c70a 6ffb  ....z.Z..2at..o.
+00007f20: deb0 595b c233 5439 175d a97c 228b 622d  ..Y[.3T9.].|".b-
+00007f30: 4677 191f 0240 3b17 4992 3872 31c3 1334  Fw...@;.I.8r1..4
+00007f40: 025c 8028 39e2 c4d9 2561 0481 3743 0913  .\.(9...%a..7C..
+00007f50: 305c a955 8695 3a7c ab3f 4fb7 b447 d179  0\.U..:|.?O..G.y
+00007f60: 8c72 d2e9 d048 6c0d 293e 8e18 7132 931d  .r...Hl.)>..q2..
+00007f70: f72a 6875 7390 17cf 9e3d 7ff8 f4f9 c3df  .*hus....=......
+00007f80: 9f3f 7af4 fce1 afcb b9b7 e576 5012 e6e5  .?z........vP...
+00007f90: 5efd f4cd 3f3f 7ce9 fcfd db8f af1e 7f6b  ^...??|........k
+00007fa0: c78b 3cfe e52f 5fbd fce3 cfff 522f 0d5a  ..<../_.....R/.Z
+00007fb0: df3d 79f9 f4c9 8bef bffe ebe7 c716 7897  .=y...........x.
+00007fc0: a3a3 3cfc 90c4 5838 d7f1 8973 93c5 b040  ..<...X8...s...@
+00007fd0: cb04 f888 bf9d c461 8448 5ea2 9b84 0225  .......a.H^....%
+00007fe0: 48c9 58d0 0319 19e8 eb0b 4491 05d7 c3a6  H.X.......D.....
+00007ff0: 1d6f 7348 1736 e0e5 f95d 83f0 41c4 e792  .osH.6...]..A...
+00008000: 5880 d7a2 d800 ee31 467b 8c5b d774 4dcd  X......1F{.[.tM.
+00008010: 95b7 c23c 09ed 93f3 791e 7713 a163 dbdc  ...<....y.w..c..
+00008020: c186 9707 f319 c43d b1a9 0c22 6cd0 dca7  .......=..."l...
+00008030: e072 14e2 044b 473d 6353 8c2d 6277 0831  .r...KG=cS.-bw.1
+00008040: ecba 4746 9c09 3691 ce1d e2f4 10b1 9ae4  ..GF..6.........
+00008050: 901c 19d1 9409 ed90 18fc b2b0 1104 7f1b  ................
+00008060: b6d9 bbed f418 b5a9 efe3 6313 097b 0351  ..........c..{.Q
+00008070: 9b4a 4c0d 335e 4673 8962 2b63 14d3 3c72  .JL.3^Fs.b+c..<r
+00008080: 17c9 c846 f260 c147 86c1 8504 4f87 9832  ...F.`.G....O..2
+00008090: 6730 c642 d864 6ef0 8541 f71a a419 bbdb  g0.B.dn..A......
+000080a0: f7e8 2236 915c 92a9 0db9 8b18 cb23 fb6c  .."6.\.......#.l
+000080b0: 1a44 289e 5939 9324 ca63 af88 2984 2872  .D(.Y9.$.c..).(r
+000080c0: f699 b492 60e6 0e51 7df0 034a 0add 7d9b  ....`..Q}..J..}.
+000080d0: 60c3 ddaf dfdb b720 0dd9 0344 3d99 73db  `...... ...D=.s.
+000080e0: 96c0 ccdc 8f0b 3a41 d8a6 bccb 6323 c576  ......:A....c#.v
+000080f0: 39b1 4647 6f1e 1aa1 bd8b 3145 2768 8cb1  9.FGo.....1E'h..
+00008100: 73eb 8a0d cf66 86cd 33d2 5723 c82a 3bd8  s....f..3.W#.*;.
+00008110: 669b abc8 8c55 d54f b080 5a49 1537 16c7  f....U.O..ZI.7..
+00008120: 1261 84ec 010e 5901 9fbd c546 e259 a024  .a....Y....F.Y.$
+00008130: 46bc 48f3 f5a9 1932 0338 ea62 6bbc d2d1  F.H....2.8.bk...
+00008140: d448 a584 ab4d 6b27 7143 c4c6 fa0a b5ee  .H...Mk'qC......
+00008150: 47c8 082b d517 f678 5d70 c37f 6fb2 c740  G..+...x]p..o..@
+00008160: e6ee 3bc8 e0b7 9681 c4fe c6b6 3944 d498  ..;.........9D..
+00008170: 200b 9843 0455 862d dd82 88e1 fe4c 446d   ..C.U.-.....LDm
+00008180: 272d 36b7 ca4d cc4d 9bb9 a1bc 51f4 c424  '-6..M.M....Q..$
+00008190: 796d 05b4 51fb f81f a7f6 f960 55cf e9d7  ym..Q......`U...
+000081a0: 3b45 2965 b3ca 29c2 6dd6 3601 e363 f2e9  ;E)e..).m.6..c..
+000081b0: 9736 7d34 4ff6 319c 2667 95cd 5965 f37f  .6}4O.1.&g..Ye..
+000081c0: ac6c 8af6 f359 3d73 56cf 9cd5 331f ad9e  .l...Y=sV...3...
+000081d0: c94a 187d 11b4 baee d15a e2c2 bb9f 09a1  .J.}.....Z......
+000081e0: f440 2e28 de15 baf8 11b0 f7c7 4318 d41d  .@.(........C...
+000081f0: 2db4 be6a 9a45 d05c 4e67 e042 8e74 dbe1  -..j.E.\Ng.B.t..
+00008200: 4c7e 4164 7410 a119 4c53 d533 8462 a93a  L~Adt...LS.3.b.:
+00008210: 14ce 8c09 289f f4b0 55b7 2ebf e6f1 1e1b  ....(...U.......
+00008220: a7a3 d5ea ea76 1304 90cc c6a1 fc5a 8d43  .....v.......Z.C
+00008230: b126 d3d1 4633 bbc6 5bab d7bd 505f b7ae  .&..F3..[...P_..
+00008240: 0828 d9b7 2191 9bcc 2451 b790 68ae 065f  .(..!...$Q..h.._
+00008250: 4342 afec 5458 b42d 2c5a 4a7d 210b fdb3  CB..TX.-,ZJ}!...
+00008260: f40a 1c4e 0e52 17e3 be97 3282 7083 901e  ...N.R....2.p...
+00008270: 2b3f a5f2 2bef 9eba a78b 8c69 2ebb 6659  +?..+......i..fY
+00008280: 5e5b 713d 1d4f 1b24 72e1 6692 c885 6104  ^[q=.O.$r.f...a.
+00008290: 87c7 e6f0 29fb ba9d b9d4 a0a7 4cb1 4da3  ....).......L.M.
+000082a0: d9fa 10be 5649 6423 37d0 c4ec 3927 b0e7  ....VId#7...9'..
+000082b0: ea3e a819 a159 c79d c03f 4ed0 8c67 a04f  .>...Y...?N..g.O
+000082c0: a84c 8568 9874 dc91 5c1a fa5d 32cb 8c0b  .L.h.t..\..]2...
+000082d0: d947 224a 61fa 51ba fe98 48cc 1d4a 6288  .G"Ja.Q...H..Jb.
+000082e0: f5bc 1b68 9271 abd6 9a6a 8d9f 28b9 76e5  ...h.q...j..(.v.
+000082f0: d3b3 9cfe c93b 194f 2678 240b 46b2 2e3c  .....;.O&x$.F..<
+00008300: 4b95 589f be27 5875 d81c 481f 44e3 13e7  K.X..'Xu..H.D...
+00008310: 88ce f94d 0486 f29b 5565 c031 1172 6dcd  ...M....Ue.1.rm.
+00008320: 31e1 b9e0 ceac b891 ae96 5bd1 78eb 926d  1.........[.x..m
+00008330: 5144 6711 5a9e 28f9 649e c275 7b4d 27b7  QDg.Z.(.d..u{M'.
+00008340: 0ecd 7473 5566 7fb9 98a3 5039 e9bd 4fdd  ..tsUf....P9..O.
+00008350: d70b 6d24 cd82 0344 9d9a f6fc f1e1 0ef9  ..m$...D........
+00008360: 1cab 2cef 1bac d2d4 bd99 ebda ab5c 5774  ..,..........\Wt
+00008370: 4abc ff81 90a3 964d 6650 538c 2dd4 8ace  J......MfPS.-...
+00008380: 8e53 2c08 72d3 ad43 b3e8 8c38 edd3 6033  .S,.r..C...8..`3
+00008390: 6ad5 01b1 aa2b 756f ebf5 363b ba0b 91df  j....+uo..6;....
+000083a0: 876a 754e a548 2fc8 ee41 f91d ac5e 4ca6  .juN.H/..A...^L.
+000083b0: 9940 8fae b2cb 3de9 cc39 e9b8 f72b 7ed7  .@....=..9...+~.
+000083c0: 0b6a 7e50 aab4 fc41 c9ab 7b95 52cb efd6  .j~P...A..{.R...
+000083d0: 4b5d dfaf 5707 7eb5 d2ef d51e 8051 6414  K]..W.~......Qd.
+000083e0: 57fd 74ee 21fc b34f 17cb b7f7 7a7c eb0d  W.t.!..O....z|..
+000083f0: 7ebc 2ab5 cf8d 585c 66ba 0e2e 6b61 fd06  ~.*...X\f...ka..
+00008400: bf5a 2b7e 83ef 10b0 ccfd 466d d8ae b77b  .Z+~......Fm...{
+00008410: 8d52 bbde 1d96 bc7e af55 6a07 8d5e a9df  .R.....~.Uj..^..
+00008420: 089a fd61 3ff0 5bed e103 d739 d660 af5b  ...a?.[....9.`.[
+00008430: 0fbc c6a0 556a 5483 a0e4 352a 8a7e ab5d  ....UjT...5*.~.]
+00008440: 6a7a b55a d76b 765b 03af fb60 696b 58f9  jz.Z.kv[...`ikX.
+00008450: ea77 655e cdeb e2bf 0000 00ff ff03 0050  .we^...........P
+00008460: 4b03 0414 0006 0008 0000 0021 007b 43bc  K..........!.{C.
+00008470: 5dc4 0600 00cf 2000 0014 0000 0070 7074  ]..... ......ppt
+00008480: 2f74 6865 6d65 2f74 6865 6d65 322e 786d  /theme/theme2.xm
+00008490: 6cec 59cd 8b1b 3714 bf17 fa3f 0c73 77fc  l.Y...7....?.sw.
+000084a0: 35e3 8f10 27d8 633b 9b64 3759 b29b 941c  5...'.c;.d7Y....
+000084b0: b5b6 3ca3 5833 3292 bc1b 1302 2539 f552  ..<.X32.....%9.R
+000084c0: 28a4 a597 426f 3d94 d240 030d bdf4 8f09  (...Bo=..@......
+000084d0: 24b4 e91f d127 8ded 19d9 9ae6 6b13 025d  $....'......k..]
+000084e0: 2fd8 92e6 f79e 7e7a efe9 e9ad e6c2 a57b  /.....~z.......{
+000084f0: 3175 8e31 1784 251d b77a aee2 3a38 19b1  1u.1..%..z..:8..
+00008500: 3149 c28e 7beb 7058 6ab9 8e90 2819 23ca  1I..{.pXj...(.#.
+00008510: 12dc 7117 58b8 972e 7efe d905 745e 4638  ..q.X...~...t^F8
+00008520: c60e c827 e23c eab8 9194 b3f3 e5b2 18c1  ...'.<..........
+00008530: 3012 e7d8 0c27 f06c c278 8c24 7479 581e  0....'.l.x.$tyX.
+00008540: 7374 027a 635a ae55 2a8d 728c 48e2 3a09  st.zcZ.U*.r.H.:.
+00008550: 8a41 ed8d c984 8cb0 73a8 54ba 1757 ca07  .A......s.T..W..
+00008560: 14be 1229 d4c0 88f2 03a5 1a1b 121a 3b9e  ...)..........;.
+00008570: 56d5 8f58 8880 72e7 18d1 8e0b f38c d9c9  V..X..r.........
+00008580: 21be 275d 8722 21e1 41c7 ade8 8f5b be78  !.']."!.A....[.x
+00008590: a1bc 16a2 b240 3627 37d4 9fa5 dc52 603c  .....@6'7....R`<
+000085a0: ad69 391e 1ead 053d cff7 1add b57e 0da0  .i9....=.....~..
+000085b0: 721b 3768 0e1a 83c6 5a9f 06a0 d108 569a  r.7h....Z.....V.
+000085c0: 7231 7536 6b81 b7c4 e640 69d3 a2bb dfec  r1u6k....@i.....
+000085d0: d7ab 063e a7bf be85 effa eacf c06b 50da  ...>.........kP.
+000085e0: f4b6 f0c3 6190 d930 074a 9bfe 16de efb5  ....a..0.J......
+000085f0: 7b7d 53bf 06a5 cdc6 16be 59e9 f6bd a681  {}S.......Y.....
+00008600: d7a0 8892 64ba 85ae f88d 7ab0 5aed 1a32  ....d.....z.Z..2
+00008610: 6174 c70a 6ffb deb0 595b c233 5439 175d  at..o...Y[.3T9.]
+00008620: a97c 228b 622d 4677 191f 0240 3b17 4992  .|".b-Fw...@;.I.
+00008630: 3872 31c3 1334 025c 8028 39e2 c4d9 2561  8r1..4.\.(9...%a
+00008640: 0481 3743 0913 305c a955 8695 3a7c ab3f  ..7C..0\.U..:|.?
+00008650: 4fb7 b447 d179 8c72 d2e9 d048 6c0d 293e  O..G.y.r...Hl.)>
+00008660: 8e18 7132 931d f72a 6875 7390 17cf 9e3d  ..q2...*hus....=
+00008670: 7ff8 f4f9 c3df 9f3f 7af4 fce1 afcb b9b7  .......?z.......
+00008680: e576 5012 e6e5 5efd f4cd 3f3f 7ce9 fcfd  .vP...^...??|...
+00008690: db8f af1e 7f6b c78b 3cfe e52f 5fbd fce3  .....k..<../_...
+000086a0: cfff 522f 0d5a df3d 79f9 f4c9 8bef bffe  ..R/.Z.=y.......
+000086b0: ebe7 c716 7897 a3a3 3cfc 90c4 5838 d7f1  ....x...<...X8..
+000086c0: 8973 93c5 b040 cb04 f888 bf9d c461 8448  .s...@.......a.H
+000086d0: 5ea2 9b84 0225 48c9 58d0 0319 19e8 eb0b  ^....%H.X.......
+000086e0: 4491 05d7 c3a6 1d6f 7348 1736 e0e5 f95d  D......osH.6...]
+000086f0: 83f0 41c4 e792 5880 d7a2 d800 ee31 467b  ..A...X......1F{
+00008700: 8c5b d774 4dcd 95b7 c23c 09ed 93f3 791e  .[.tM....<....y.
+00008710: 7713 a163 dbdc c186 9707 f319 c43d b1a9  w..c.........=..
+00008720: 0c22 6cd0 dca7 e072 14e2 044b 473d 6353  ."l....r...KG=cS
+00008730: 8c2d 6277 0831 ecba 4746 9c09 3691 ce1d  .-bw.1..GF..6...
+00008740: e2f4 10b1 9ae4 901c 19d1 9409 ed90 18fc  ................
+00008750: b2b0 1104 7f1b b6d9 bbed f418 b5a9 efe3  ................
+00008760: 6313 097b 0351 9b4a 4c0d 335e 4673 8962  c..{.Q.JL.3^Fs.b
+00008770: 2b63 14d3 3c72 17c9 c846 f260 c147 86c1  +c..<r...F.`.G..
+00008780: 8504 4f87 9832 6730 c642 d864 6ef0 8541  ..O..2g0.B.dn..A
+00008790: f71a a419 bbdb f7e8 2236 915c 92a9 0db9  ........"6.\....
+000087a0: 8b18 cb23 fb6c 1a44 289e 5939 9324 ca63  ...#.l.D(.Y9.$.c
+000087b0: af88 2984 2872 f699 b492 60e6 0e51 7df0  ..).(r....`..Q}.
+000087c0: 034a 0add 7d9b 60c3 ddaf dfdb b720 0dd9  .J..}.`...... ..
+000087d0: 0344 3d99 73db 96c0 ccdc 8f0b 3a41 d8a6  .D=.s.......:A..
+000087e0: bccb 6323 c576 39b1 4647 6f1e 1aa1 bd8b  ..c#.v9.FGo.....
+000087f0: 3145 2768 8cb1 73eb 8a0d cf66 86cd 33d2  1E'h..s....f..3.
+00008800: 5723 c82a 3bd8 669b abc8 8c55 d54f b080  W#.*;.f....U.O..
+00008810: 5a49 1537 16c7 1261 84ec 010e 5901 9fbd  ZI.7...a....Y...
+00008820: c546 e259 a024 46bc 48f3 f5a9 1932 0338  .F.Y.$F.H....2.8
+00008830: ea62 6bbc d2d1 d448 a584 ab4d 6b27 7143  .bk....H...Mk'qC
+00008840: c4c6 fa0a b5ee 47c8 082b d517 f678 5d70  ......G..+...x]p
+00008850: c37f 6fb2 c740 e6ee 3bc8 e0b7 9681 c4fe  ..o..@..;.......
+00008860: c6b6 3944 d498 200b 9843 0455 862d dd82  ..9D.. ..C.U.-..
+00008870: 88e1 fe4c 446d 272d 36b7 ca4d cc4d 9bb9  ...LDm'-6..M.M..
+00008880: a1bc 51f4 c424 796d 05b4 51fb f81f a7f6  ..Q..$ym..Q.....
+00008890: f960 55cf e9d7 3b45 2965 b3ca 29c2 6dd6  .`U...;E)e..).m.
+000088a0: 3601 e363 f2e9 9736 7d34 4ff6 319c 2667  6..c...6}4O.1.&g
+000088b0: 95cd 5965 f37f ac6c 8af6 f359 3d73 56cf  ..Ye...l...Y=sV.
+000088c0: 9cd5 331f ad9e c94a 187d 11b4 baee d15a  ..3....J.}.....Z
+000088d0: e2c2 bb9f 09a1 f440 2e28 de15 baf8 11b0  .......@.(......
+000088e0: f7c7 4318 d41d 2db4 be6a 9a45 d05c 4e67  ..C...-..j.E.\Ng
+000088f0: e042 8e74 dbe1 4c7e 4164 7410 a119 4c53  .B.t..L~Adt...LS
+00008900: d533 8462 a93a 14ce 8c09 289f f4b0 55b7  .3.b.:....(...U.
+00008910: 2ebf e6f1 1e1b a7a3 d5ea ea76 1304 90cc  ...........v....
+00008920: c6a1 fc5a 8d43 b126 d3d1 4633 bbc6 5bab  ...Z.C.&..F3..[.
+00008930: d7bd 505f b7ae 0828 d9b7 2191 9bcc 2451  ..P_...(..!...$Q
+00008940: b790 68ae 065f 4342 afec 5458 b42d 2c5a  ..h.._CB..TX.-,Z
+00008950: 4a7d 210b fdb3 f40a 1c4e 0e52 17e3 be97  J}!......N.R....
+00008960: 3282 7083 901e 2b3f a5f2 2bef 9eba a78b  2.p...+?..+.....
+00008970: 8c69 2ebb 6659 5e5b 713d 1d4f 1b24 72e1  .i..fY^[q=.O.$r.
+00008980: 6692 c885 6104 87c7 e6f0 29fb ba9d b9d4  f...a.....).....
+00008990: a0a7 4cb1 4da3 d9fa 10be 5649 6423 37d0  ..L.M.....VId#7.
+000089a0: c4ec 3927 b0e7 ea3e a819 a159 c79d c03f  ..9'...>...Y...?
+000089b0: 4ed0 8c67 a04f a84c 8568 9874 dc91 5c1a  N..g.O.L.h.t..\.
+000089c0: fa5d 32cb 8c0b d947 224a 61fa 51ba fe98  .]2....G"Ja.Q...
+000089d0: 48cc 1d4a 6288 f5bc 1b68 9271 abd6 9a6a  H..Jb....h.q...j
+000089e0: 8d9f 28b9 76e5 d3b3 9cfe c93b 194f 2678  ..(.v......;.O&x
+000089f0: 240b 46b2 2e3c 4b95 589f be27 5875 d81c  $.F..<K.X..'Xu..
+00008a00: 481f 44e3 13e7 88ce f94d 0486 f29b 5565  H.D......M....Ue
+00008a10: c031 1172 6dcd 31e1 b9e0 ceac b891 ae96  .1.rm.1.........
+00008a20: 5bd1 78eb 926d 5144 6711 5a9e 28f9 649e  [.x..mQDg.Z.(.d.
+00008a30: c275 7b4d 27b7 0ecd 7473 5566 7fb9 98a3  .u{M'...tsUf....
+00008a40: 5039 e9bd 4fdd d70b 6d24 cd82 0344 9d9a  P9..O...m$...D..
+00008a50: f6fc f1e1 0ef9 1cab 2cef 1bac d2d4 bd99  ........,.......
+00008a60: ebda ab5c 5774 4abc ff81 90a3 964d 6650  ...\WtJ......MfP
+00008a70: 538c 2dd4 8ace 8e53 2c08 72d3 ad43 b3e8  S.-....S,.r..C..
+00008a80: 8c38 edd3 6033 6ad5 01b1 aa2b 756f ebf5  .8..`3j....+uo..
+00008a90: 363b ba0b 91df 876a 754e a548 2fc8 ee41  6;.....juN.H/..A
+00008aa0: f91d ac5e 4ca6 9940 8fae b2cb 3de9 cc39  ...^L..@....=..9
+00008ab0: e9b8 f72b 7ed7 0b6a 7e50 aab4 fc41 c9ab  ...+~..j~P...A..
+00008ac0: 7b95 52cb efd6 4b5d dfaf 5707 7eb5 d2ef  {.R...K]..W.~...
+00008ad0: d51e 8051 6414 57fd 74ee 21fc b34f 17cb  ...Qd.W.t.!..O..
+00008ae0: b7f7 7a7c eb0d 7ebc 2ab5 cf8d 585c 66ba  ..z|..~.*...X\f.
+00008af0: 0e2e 6b61 fd06 bf5a 2b7e 83ef 10b0 ccfd  ..ka...Z+~......
+00008b00: 466d d8ae b77b 8d52 bbde 1d96 bc7e af55  Fm...{.R.....~.U
+00008b10: 6a07 8d5e a9df 089a fd61 3ff0 5bed e103  j..^.....a?.[...
+00008b20: d739 d660 af5b 0fbc c6a0 556a 5483 a0e4  .9.`.[....UjT...
+00008b30: 352a 8a7e ab5d 6a7a b55a d76b 765b 03af  5*.~.]jz.Z.kv[..
+00008b40: fb60 696b 58f9 ea77 655e cdeb e2bf 0000  .`ikX..we^......
+00008b50: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+00008b60: 0021 00ea 6f03 2d76 0100 0017 0300 0011  .!..o.-v........
+00008b70: 0000 0070 7074 2f76 6965 7750 726f 7073  ...ppt/viewProps
+00008b80: 2e78 6d6c 8c52 cb6e c230 10bc 57ea 3f58  .xml.R.n.0..W.?X
+00008b90: be97 2428 a525 2270 a9da 0b52 2b41 7b77  ..$(.%"p...R+A{w
+00008ba0: 9d4d 7095 d896 d740 e8d7 77f3 e055 3870  .Mp....@..w..U8p
+00008bb0: f3ec 6376 66d7 9359 5d95 6c03 0e95 d129  ..cvf..Y].l....)
+00008bc0: 8f06 2167 a0a5 c994 2e52 feb9 7c7d 78e6  ..!g.....R..|}x.
+00008bd0: 0cbd d099 288d 8694 ef00 f96c 7a7f 37b1  ....(......lz.7.
+00008be0: c946 c1f6 c331 22d0 9888 94af bcb7 4910  .F...1".......I.
+00008bf0: a05c 4125 7060 2c68 cae5 c655 c213 7445  .\A%p`,h...U..tE
+00008c00: 9039 b125 e2aa 0c86 6138 0a2a a134 effb  .9.%....a8.*.4..
+00008c10: dd2d fd26 cf95 8417 23d7 1568 df91 3828  .-.&....#..h..8(
+00008c20: 8527 f1b8 5216 f76c f616 36eb 0089 a6ed  .'..R..l..6.....
+00008c30: 3e93 3425 73ba 292c bf5a 8b0d a65a 6f1c  >.4%s.),.Z...Zo.
+00008c40: 6473 c83d c35f 5ad5 e328 8a78 709a 5b1a  ds.=._Z..(.xp.[.
+00008c50: dba6 c6f1 681c 37a9 e092 074b 95c1 11ca  ....h.7....K....
+00008c60: 4599 7588 a116 7669 de9c ca52 4e57 e8e0  E.u...vi...RNW..
+00008c70: fbf7 0f48 8f34 ae55 25fb da8d 700b 294a  ...H.4.U%...p.)J
+00008c80: d8c7 b101 d389 48b0 66cd 1987 1167 4413  ......H.f....gD.
+00008c90: 8561 2383 c2bb 2be1 e0d0 6713 e354 a134  .a#...+...g..T.4
+00008ca0: ab53 fe14 c79c eda8 e869 d417 f543 9bb2  .S.......i...C..
+00008cb0: 624d eae7 e8fb c441 7c47 766e 4d1b 0fb8  bM.....A|GvnM...
+00008cc0: 84da 9fb8 3dd9 c33f c59d b033 b5c7 d075  ....=..?...3...u
+00008cd0: a561 ab73 6fe5 c0dd 2efd 6274 417b 5d58  .a.so.....btA{]X
+00008ce0: 21e9 fb31 d9d8 a473 d3d7 96bb fdb3 63e9  !..1...s......c.
+00008cf0: fef4 f40f 0000 ffff 0300 504b 0304 1400  ..........PK....
+00008d00: 0600 0800 0000 2100 a364 236b 8d01 0000  ......!..d#k....
+00008d10: 3203 0000 1100 0000 7070 742f 7072 6573  2.......ppt/pres
+00008d20: 5072 6f70 732e 786d 6cac d251 6fdb 2010  Props.xml..Qo. .
+00008d30: 00e0 f749 fb0f 16ef 0430 368e ad38 951d  ...I.....06..8..
+00008d40: 1c69 d21e a6aa fd01 c8c6 099a 3108 48db  .i..........1.H.
+00008d50: a9ea 7f1f 73d2 2add 34a9 9af6 7420 74c7  ....s.*.4...t t.
+00008d60: 7770 9b9b 273d 250f d279 65e6 1a90 1506  wp..'=%..ye.....
+00008d70: 899c 7b33 a8f9 5083 fbbb 3d5c 83c4 0731  ..{3..P...=\...1
+00008d80: 0f62 32b3 acc1 0fe9 c1cd f6f3 a78d adac  .b2.............
+00008d90: 935e ce41 8498 facd 25b1 d0ec 2b51 8363  .^.A....%...+Q.c
+00008da0: 08b6 42c8 f747 a985 5f19 2be7 7836 1aa7  ..B..G.._.+.x6..
+00008db0: 4588 5b77 4083 138f f102 3da1 1463 86b4  E.[w@.....=..c..
+00008dc0: 5033 b8e4 bb8f e49b 7154 bde4 a63f e908  P3......qT...?..
+00008dd0: 3817 7172 5a24 fea8 ac7f ad66 3f52 edba  8.qrZ$.....f?R..
+00008de0: 8f77 a46d 6c52 3e85 af3e 5c56 c9c9 a91a  .w.mlR>..>\V....
+00008df0: 3c77 05db 7565 d640 86e9 0e66 244b 615b  <w..ue.@...f$Ka[
+00008e00: 762d 649c d002 6382 9bb4 78f9 954d b26a  v-d...c...x..M.j
+00008e10: 50be 176e f8a2 c541 7683 0a5c 04f1 8a23  P..n...Av..\...#
+00008e20: d91f 3cad 7a67 bc19 c3aa 37fa d227 b2e6  ..<.zg....7..'..
+00008e30: 513a 6bd4 d22a c197 f77a 1053 0d30 40db  Q:k..*...z.S.0@.
+00008e40: 0d5a 70ef 8d9c 9206 b3b4 8145 b96e 6046  .Zp........E.n`F
+00008e50: d312 362d e7b0 6d9b 75ce 588a 7382 df8c  ..6-..m.u.X.s...
+00008e60: 7214 a729 2c46 6ed5 7fe4 d1b4 60c5 df88  r..),Fn.....`...
+00008e70: 7b9e 77fb a6e1 1077 bb0e 6639 ed60 b9a6  {.w....w..f9.`..
+00008e80: 0466 ac4d 69db c540 b333 31af faa3 70e1  .f.Mi..@.31...p.
+00008e90: ce89 fe7b 9c9b 5b39 b6c2 cbe1 0d9a ff0b  ...{..[9........
+00008ea0: 34bd 8692 6be4 392e df8e 7e1f f3ed 4f00  4...k.9...~...O.
+00008eb0: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+00008ec0: 0000 2100 d8fd 8d8f ac00 0000 b600 0000  ..!.............
+00008ed0: 1300 0000 7070 742f 7461 626c 6553 7479  ....ppt/tableSty
+00008ee0: 6c65 732e 786d 6c0c cc49 0e82 3018 40e1  les.xml..I..0.@.
+00008ef0: bd89 7768 fe7d 2d43 5124 14c2 202b 77ea  ..wh.}-CQ$.. +w.
+00008f00: 012a 9421 e940 68a3 12e3 dd65 f9f2 922f  .*.!.@h....e.../
+00008f10: cd3f 4aa2 9758 ec64 3403 ffe0 0112 ba35  .?J..X.d4......5
+00008f20: dda4 0706 8f7b 8363 40d6 71dd 7169 b460  .....{.c@.q.qi.`
+00008f30: b00a 0b79 b6df a53c 714f 7973 ab14 57eb  ...y...<qOys..W.
+00008f40: d0a6 689b 7006 a373 7342 886d 47a1 b83d  ..h.p..ssB.mG..=
+00008f50: 9859 e8ed f566 51dc 6db9 0ca4 5bf8 7bd3  .Y...fQ.m...[.{.
+00008f60: 9524 81e7 1d89 e293 06d4 899e c137 aa82  .$...........7..
+00008f70: 20a2 b4c0 a7cb e588 6948 035c 7a34 c671   .......iH.\z4.q
+00008f80: 54d6 d5b9 a9fd 2a2c 7e40 b23f 0000 00ff  T.....*,~@.?....
+00008f90: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00008fa0: 00e0 bcff 0677 0100 00b0 0200 0011 0008  .....w..........
+00008fb0: 0164 6f63 5072 6f70 732f 636f 7265 2e78  .docProps/core.x
+00008fc0: 6d6c 20a2 0401 28a0 0001 0000 0000 0000  ml ...(.........
+00008fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00008fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00008ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009000: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009040: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009050: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009060: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009080: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009090: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000090a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000090b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000090c0: 0000 0000 0000 0000 0000 8c92 4f4b c330  ............OK.0
+000090d0: 1887 ef82 dfa1 e4de 25ed a84a e83a 50d9  ........%..J.:P.
+000090e0: c981 e044 f116 d277 5bb0 4d42 12f7 e7b6  ...D...w[.MB....
+000090f0: 9be8 c193 77c1 6f21 f86d 5486 dfc2 b65b  ....w.o!.mT....[
+00009100: bb89 3b78 4c7e cffb e4cd 9bc4 dd59 9e79  ..;xL~.......Y.y
+00009110: 1330 5628 d941 418b 200f 2457 a990 a30e  .0V(.AA. .$W....
+00009120: ba1c f4fc 23e4 59c7 64ca 3225 a183 e660  ....#.Y.d.2%...`
+00009130: 5137 d9df 8bb9 a65c 1938 374a 8371 02ac  Q7.....\.87J.q..
+00009140: 5798 a4a5 5c77 d0d8 394d 31b6 7c0c 39b3  W...\w..9M1.|.9.
+00009150: ad82 9045 3854 2667 ae58 9a11 d68c dfb2  ...E8T&g.X......
+00009160: 11e0 9090 039c 8363 2973 0c97 425f 3746  .......c)s..B_7F
+00009170: b456 a6bc 51ea 3b93 5582 9463 c820 07e9  .V..Q.;.U..c. ..
+00009180: 2c0e 5a01 deb0 0e4c 6e77 1654 c916 990b  ,.Z....Lnw.T....
+00009190: 37d7 b013 adc3 869e 59d1 80d3 e9b4 356d  7.......Y.....5m
+000091a0: 5768 d17f 80af fb67 17d5 557d 21cb 5971  Wh.....g..U}!.Yq
+000091b0: 4049 9c72 ea84 cb20 d1da cd7c a754 6663  @I.r... ...|.Tfc
+000091c0: dc6c 9631 37c0 9c32 c9f2 e5f5 fbfe e96b  .l.17..2.......k
+000091d0: f1f0 b158 7cbe 3f2e df9e 2bb0 8ecb 4967  ...X|.?...+...Ig
+000091e0: ccba 7ef1 2843 01e9 f17c 67c5 5faa 2c34  ..~.(C...|g._.,4
+000091f0: 3011 e5d3 2661 4534 cb78 3da7 d529 907a  0...&aE4.x=..).z
+00009200: c5fd e86a 1a75 72d5 3e39 1df4 5012 9230  ...j.ur.>9..P..0
+00009210: f449 e407 6440 221a 0594 0437 6583 bfea  .I..d@"....7e...
+00009220: 37c2 7cdd c03f 8ce1 e120 6853 d2a6 61b4  7.|..?... hS..a.
+00009230: 65ac 0549 d5f1 ef3f 96fc 0000 00ff ff03  e..I...?........
+00009240: 0050 4b03 0414 0006 0008 0000 0021 00c9  .PK..........!..
+00009250: b2e7 2828 0200 0051 0500 0010 0008 0164  ..((...Q.......d
+00009260: 6f63 5072 6f70 732f 6170 702e 786d 6c20  ocProps/app.xml 
+00009270: a204 0128 a000 0100 0000 0000 0000 0000  ...(............
+00009280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000092a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000092b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000092c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000092d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000092e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+000092f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009300: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009320: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009330: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009340: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009350: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009360: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00009370: 0000 0000 0000 00a4 5451 6fda 3010 7e9f  ........TQo.0.~.
+00009380: b4ff 60e5 1d0c aca2 1332 a92a 3ac4 4359  ..`......2.*:.CY
+00009390: 9108 edb3 6b5f 8835 c7b6 ec2b 83fd fa39  ....k_.5...+...9
+000093a0: 4993 4241 95ba e525 dfdd 7df9 7cf9 6c1f  I.BA...%..}.|.l.
+000093b0: bbd9 979a ecc0 0765 cd34 19f6 0709 0123  .......e.4.....#
+000093c0: ac54 663b 4d36 d9bc f73d 2101 b991 5c5b  .Tf;M6...=!...\[
+000093d0: 03d3 e400 21b9 49bf 7e61 2b6f 1d78 5410  ....!.I.~a+o.xT.
+000093e0: 4894 3061 9a14 886e 4269 1005 943c f463  H.0a...nBi...<.c
+000093f0: d9c4 4a6e 7dc9 3186 7e4b 6d9e 2b01 7756  ..Jn}.1.~Km.+.wV
+00009400: bc94 6090 8e06 8331 853d 8291 207b ae13  ..`....1.=.. {..
+00009410: 4c1a c5c9 0eff 5554 5a51 f517 1eb3 838b  L.....UTZQ......
+00009420: 7a29 cb2c 729d a912 d22b 46df 02f6 64bd  z).,r....+F...d.
+00009430: 0ce9 e81b a30d 62b7 ce69 2538 463b d2a5  ......b..i%8F;..
+00009440: 12de 069b 2359 72a1 0cda 5090 95fd 0d7e  ....#Yr...P....~
+00009450: 6563 c4e8 3137 fa01 21ae 5f47 f3ba bdf4  ec..17..!._G....
+00009460: 4949 08c2 0318 462f 94d9 8a7b bef5 dc15  II....F/...{....
+00009470: 21bd 8e8c b788 ad75 f569 1adb 7a45 eca7  !......u.i..zE..
+00009480: c5f8 1a31 da00 b650 5282 79ad 0e18 3d89  ...1...PR.y...=.
+00009490: d972 39d3 cad5 8516 b2b5 e01a 66d1 9534  .r9.........f..4
+000094a0: e73a 4094 ee12 6c01 bcda f115 573e 3277  .:@...l.....W>2w
+000094b0: 38d9 8140 eb49 507f e29e 8f13 f2cc 0354  8..@.IP........T
+000094c0: 5e4e 931d f78a 1b4c 1a5a 13d4 58bb 803e  ^N.....L.Z..X..>
+000094d0: 9d5b 8381 6c02 4846 bb64 0d8f b9c7 585d  .[..l.HF.d....X]
+000094e0: 55ff d980 0f89 8d56 160f 027c 427b f809  U......V...|B{..
+000094f0: edda 3e92 29d4 10fe bffd 3aa8 7d8c f8d4  ..>.).....:.}...
+00009500: e166 8987 3cee 395e 30fc fad8 f0ba 87c6  .f..<.9^0.......
+00009510: eea6 9ddb a8af 8fdb ebd0 8c6b f5ec d547  ...........k...G
+00009520: 3572 afb6 055e 643c d417 899c 19dc 21e7  5r...^d<......!.
+00009530: 70df 436b f589 391d fa51 3a3c 1061 cbea  p.Ck..9..Q:<.a..
+00009540: 1e92 5079 79b9 136b 847e a906 ce99 c7ad  ..Pyy..k.~......
+00009550: 5bef fc99 d9d2 7173 8885 0edd 2bf3 2b6c  [.....qs....+.+l
+00009560: 5c66 ef38 427b a24f 936c 5d70 0f32 4e86  \f.8B{.O.l]p.2N.
+00009570: eec4 7709 b688 de7a 5df1 6705 375b 902d  ..w....z].g.7[.-
+00009580: e7bc 50cd 84c7 6642 a6c3 717f 109f faee  ..P...fB..q.....
+00009590: b7b9 ea72 b7a3 2bfd 0b00 00ff ff03 0050  ...r..+........P
+000095a0: 4b01 022d 0014 0006 0008 0000 0021 00ef  K..-.........!..
+000095b0: 2890 b2e8 0100 0072 0f00 0013 0000 0000  (......r........
+000095c0: 0000 0000 0000 0000 0000 0000 005b 436f  .............[Co
+000095d0: 6e74 656e 745f 5479 7065 735d 2e78 6d6c  ntent_Types].xml
+000095e0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+000095f0: 68f8 74a1 0301 0000 e202 0000 0b00 0000  h.t.............
+00009600: 0000 0000 0000 0000 0000 2104 0000 5f72  ..........!..._r
+00009610: 656c 732f 2e72 656c 7350 4b01 022d 0014  els/.relsPK..-..
+00009620: 0006 0008 0000 0021 00a0 4e0f b6b7 0200  .......!..N.....
+00009630: 00fc 0600 0015 0000 0000 0000 0000 0000  ................
+00009640: 0000 0055 0700 0070 7074 2f73 6c69 6465  ...U...ppt/slide
+00009650: 732f 736c 6964 6531 2e78 6d6c 504b 0102  s/slide1.xmlPK..
+00009660: 2d00 1400 0600 0800 0000 2100 227d 323b  -.........!."}2;
+00009670: be02 0000 fd06 0000 1500 0000 0000 0000  ................
+00009680: 0000 0000 0000 3f0a 0000 7070 742f 736c  ......?...ppt/sl
+00009690: 6964 6573 2f73 6c69 6465 322e 786d 6c50  ides/slide2.xmlP
+000096a0: 4b01 022d 0014 0006 0008 0000 0021 0023  K..-.........!.#
+000096b0: f370 a4d6 0000 00ce 0100 0020 0000 0000  .p......... ....
+000096c0: 0000 0000 0000 0000 0030 0d00 0070 7074  .........0...ppt
+000096d0: 2f73 6c69 6465 732f 5f72 656c 732f 736c  /slides/_rels/sl
+000096e0: 6964 6533 2e78 6d6c 2e72 656c 7350 4b01  ide3.xml.relsPK.
+000096f0: 022d 0014 0006 0008 0000 0021 004b f53d  .-.........!.K.=
+00009700: ecbd 0000 0037 0100 0020 0000 0000 0000  .....7... ......
+00009710: 0000 0000 0000 0044 0e00 0070 7074 2f73  .......D...ppt/s
+00009720: 6c69 6465 732f 5f72 656c 732f 736c 6964  lides/_rels/slid
+00009730: 6532 2e78 6d6c 2e72 656c 7350 4b01 022d  e2.xml.relsPK..-
+00009740: 0014 0006 0008 0000 0021 00d8 0382 6bd6  .........!....k.
+00009750: 0000 00ce 0100 0020 0000 0000 0000 0000  ....... ........
+00009760: 0000 0000 003f 0f00 0070 7074 2f73 6c69  .....?...ppt/sli
+00009770: 6465 732f 5f72 656c 732f 736c 6964 6531  des/_rels/slide1
+00009780: 2e78 6d6c 2e72 656c 7350 4b01 022d 0014  .xml.relsPK..-..
+00009790: 0006 0008 0000 0021 009c 6339 c529 0100  .......!..c9.)..
+000097a0: 0071 0500 001f 0000 0000 0000 0000 0000  .q..............
+000097b0: 0000 0053 1000 0070 7074 2f5f 7265 6c73  ...S...ppt/_rels
+000097c0: 2f70 7265 7365 6e74 6174 696f 6e2e 786d  /presentation.xm
+000097d0: 6c2e 7265 6c73 504b 0102 2d00 1400 0600  l.relsPK..-.....
+000097e0: 0800 0000 2100 ad2b 3e30 af02 0000 b506  ....!..+>0......
+000097f0: 0000 1500 0000 0000 0000 0000 0000 0000  ................
+00009800: c112 0000 7070 742f 736c 6964 6573 2f73  ....ppt/slides/s
+00009810: 6c69 6465 332e 786d 6c50 4b01 022d 0014  lide3.xmlPK..-..
+00009820: 0006 0008 0000 0021 00d7 c1b4 c3b4 0200  .......!........
+00009830: 00d2 0d00 0014 0000 0000 0000 0000 0000  ................
+00009840: 0000 00a3 1500 0070 7074 2f70 7265 7365  .......ppt/prese
+00009850: 6e74 6174 696f 6e2e 786d 6c50 4b01 022d  ntation.xmlPK..-
+00009860: 0014 0006 0008 0000 0021 00a2 796c 2105  .........!..yl!.
+00009870: 0500 007e 1200 0021 0000 0000 0000 0000  ...~...!........
+00009880: 0000 0000 0089 1800 0070 7074 2f73 6c69  .........ppt/sli
+00009890: 6465 4c61 796f 7574 732f 736c 6964 654c  deLayouts/slideL
+000098a0: 6179 6f75 7431 2e78 6d6c 504b 0102 2d00  ayout1.xmlPK..-.
+000098b0: 1400 0600 0800 0000 2100 4a19 7e47 5404  ........!.J.~GT.
+000098c0: 0000 890f 0000 2100 0000 0000 0000 0000  ......!.........
+000098d0: 0000 0000 cd1d 0000 7070 742f 736c 6964  ........ppt/slid
+000098e0: 654c 6179 6f75 7473 2f73 6c69 6465 4c61  eLayouts/slideLa
+000098f0: 796f 7574 322e 786d 6c50 4b01 022d 0014  yout2.xmlPK..-..
+00009900: 0006 0008 0000 0021 00c3 d7f2 9b3e 0500  .......!.....>..
+00009910: 005e 1500 0021 0000 0000 0000 0000 0000  .^...!..........
+00009920: 0000 0060 2200 0070 7074 2f73 6c69 6465  ...`"..ppt/slide
+00009930: 4c61 796f 7574 732f 736c 6964 654c 6179  Layouts/slideLay
+00009940: 6f75 7433 2e78 6d6c 504b 0102 2d00 1400  out3.xmlPK..-...
+00009950: 0600 0800 0000 2100 abed 097a b504 0000  ......!....z....
+00009960: c313 0000 2100 0000 0000 0000 0000 0000  ....!...........
+00009970: 0000 dd27 0000 7070 742f 736c 6964 654c  ...'..ppt/slideL
+00009980: 6179 6f75 7473 2f73 6c69 6465 4c61 796f  ayouts/slideLayo
+00009990: 7574 342e 786d 6c50 4b01 022d 0014 0006  ut4.xmlPK..-....
+000099a0: 0008 0000 0021 006b 8a56 3713 0600 0055  .....!.k.V7....U
+000099b0: 1f00 0021 0000 0000 0000 0000 0000 0000  ...!............
+000099c0: 00d1 2c00 0070 7074 2f73 6c69 6465 4c61  ..,..ppt/slideLa
+000099d0: 796f 7574 732f 736c 6964 654c 6179 6f75  youts/slideLayou
+000099e0: 7435 2e78 6d6c 504b 0102 2d00 1400 0600  t5.xmlPK..-.....
+000099f0: 0800 0000 2100 300f 6131 db03 0000 140c  ....!.0.a1......
+00009a00: 0000 2100 0000 0000 0000 0000 0000 0000  ..!.............
+00009a10: 2333 0000 7070 742f 736c 6964 654c 6179  #3..ppt/slideLay
+00009a20: 6f75 7473 2f73 6c69 6465 4c61 796f 7574  outs/slideLayout
+00009a30: 362e 786d 6c50 4b01 022d 0014 0006 0008  6.xmlPK..-......
+00009a40: 0000 0021 0002 35ef b587 0300 00f6 0900  ...!..5.........
+00009a50: 0021 0000 0000 0000 0000 0000 0000 003d  .!.............=
+00009a60: 3700 0070 7074 2f73 6c69 6465 4c61 796f  7..ppt/slideLayo
+00009a70: 7574 732f 736c 6964 654c 6179 6f75 7437  uts/slideLayout7
+00009a80: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00009a90: 0000 2100 74a5 ee2e b205 0000 7817 0000  ..!.t.......x...
+00009aa0: 2100 0000 0000 0000 0000 0000 0000 033b  !..............;
+00009ab0: 0000 7070 742f 736c 6964 654c 6179 6f75  ..ppt/slideLayou
+00009ac0: 7473 2f73 6c69 6465 4c61 796f 7574 382e  ts/slideLayout8.
+00009ad0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
+00009ae0: 0021 0020 2f57 2a84 0500 0027 1700 0021  .!. /W*....'...!
+00009af0: 0000 0000 0000 0000 0000 0000 00f4 4000  ..............@.
+00009b00: 0070 7074 2f73 6c69 6465 4c61 796f 7574  .ppt/slideLayout
+00009b10: 732f 736c 6964 654c 6179 6f75 7439 2e78  s/slideLayout9.x
+00009b20: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
+00009b30: 2100 67b1 dc28 7204 0000 c00f 0000 2200  !.g..(r.......".
+00009b40: 0000 0000 0000 0000 0000 0000 b746 0000  .............F..
+00009b50: 7070 742f 736c 6964 654c 6179 6f75 7473  ppt/slideLayouts
+00009b60: 2f73 6c69 6465 4c61 796f 7574 3130 2e78  /slideLayout10.x
+00009b70: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
+00009b80: 2100 ae16 46bd a604 0000 a010 0000 2200  !...F.........".
+00009b90: 0000 0000 0000 0000 0000 0000 694b 0000  ............iK..
+00009ba0: 7070 742f 736c 6964 654c 6179 6f75 7473  ppt/slideLayouts
+00009bb0: 2f73 6c69 6465 4c61 796f 7574 3131 2e78  /slideLayout11.x
+00009bc0: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
+00009bd0: 2100 173c ed6a d300 0000 bf01 0000 2a00  !..<.j........*.
+00009be0: 0000 0000 0000 0000 0000 0000 4f50 0000  ............OP..
+00009bf0: 7070 742f 6e6f 7465 7353 6c69 6465 732f  ppt/notesSlides/
+00009c00: 5f72 656c 732f 6e6f 7465 7353 6c69 6465  _rels/notesSlide
+00009c10: 322e 786d 6c2e 7265 6c73 504b 0102 2d00  2.xml.relsPK..-.
+00009c20: 1400 0600 0800 0000 2100 c69e 7235 cf02  ........!...r5..
+00009c30: 0000 eb06 0000 1f00 0000 0000 0000 0000  ................
+00009c40: 0000 0000 6a51 0000 7070 742f 6e6f 7465  ....jQ..ppt/note
+00009c50: 7353 6c69 6465 732f 6e6f 7465 7353 6c69  sSlides/notesSli
+00009c60: 6465 312e 786d 6c50 4b01 022d 0014 0006  de1.xmlPK..-....
+00009c70: 0008 0000 0021 004a af75 39d2 0000 00bf  .....!.J.u9.....
+00009c80: 0100 002a 0000 0000 0000 0000 0000 0000  ...*............
+00009c90: 0076 5400 0070 7074 2f6e 6f74 6573 536c  .vT..ppt/notesSl
+00009ca0: 6964 6573 2f5f 7265 6c73 2f6e 6f74 6573  ides/_rels/notes
+00009cb0: 536c 6964 6531 2e78 6d6c 2e72 656c 7350  Slide1.xml.relsP
+00009cc0: 4b01 022d 0014 0006 0008 0000 0021 00d5  K..-.........!..
+00009cd0: d192 f1bc 0000 0037 0100 002d 0000 0000  .......7...-....
+00009ce0: 0000 0000 0000 0000 0090 5500 0070 7074  ..........U..ppt
+00009cf0: 2f73 6c69 6465 4c61 796f 7574 732f 5f72  /slideLayouts/_r
+00009d00: 656c 732f 736c 6964 654c 6179 6f75 7431  els/slideLayout1
+00009d10: 312e 786d 6c2e 7265 6c73 504b 0102 2d00  1.xml.relsPK..-.
+00009d20: 1400 0600 0800 0000 2100 d5d1 92f1 bc00  ........!.......
+00009d30: 0000 3701 0000 2d00 0000 0000 0000 0000  ..7...-.........
+00009d40: 0000 0000 9756 0000 7070 742f 736c 6964  .....V..ppt/slid
+00009d50: 654c 6179 6f75 7473 2f5f 7265 6c73 2f73  eLayouts/_rels/s
+00009d60: 6c69 6465 4c61 796f 7574 3130 2e78 6d6c  lideLayout10.xml
+00009d70: 2e72 656c 7350 4b01 022d 0014 0006 0008  .relsPK..-......
+00009d80: 0000 0021 00d5 d192 f1bc 0000 0037 0100  ...!.........7..
+00009d90: 002c 0000 0000 0000 0000 0000 0000 009e  .,..............
+00009da0: 5700 0070 7074 2f73 6c69 6465 4c61 796f  W..ppt/slideLayo
+00009db0: 7574 732f 5f72 656c 732f 736c 6964 654c  uts/_rels/slideL
+00009dc0: 6179 6f75 7439 2e78 6d6c 2e72 656c 7350  ayout9.xml.relsP
+00009dd0: 4b01 022d 0014 0006 0008 0000 0021 00d5  K..-.........!..
+00009de0: d192 f1bc 0000 0037 0100 002c 0000 0000  .......7...,....
+00009df0: 0000 0000 0000 0000 00a4 5800 0070 7074  ..........X..ppt
+00009e00: 2f73 6c69 6465 4c61 796f 7574 732f 5f72  /slideLayouts/_r
+00009e10: 656c 732f 736c 6964 654c 6179 6f75 7438  els/slideLayout8
+00009e20: 2e78 6d6c 2e72 656c 7350 4b01 022d 0014  .xml.relsPK..-..
+00009e30: 0006 0008 0000 0021 0039 cac7 c6ba 0200  .......!.9......
+00009e40: 0086 0600 001f 0000 0000 0000 0000 0000  ................
+00009e50: 0000 00aa 5900 0070 7074 2f6e 6f74 6573  ....Y..ppt/notes
+00009e60: 536c 6964 6573 2f6e 6f74 6573 536c 6964  Slides/notesSlid
+00009e70: 6532 2e78 6d6c 504b 0102 2d00 1400 0600  e2.xmlPK..-.....
+00009e80: 0800 0000 2100 69a2 5f21 1501 0000 c707  ....!.i._!......
+00009e90: 0000 2c00 0000 0000 0000 0000 0000 0000  ..,.............
+00009ea0: a15c 0000 7070 742f 736c 6964 654d 6173  .\..ppt/slideMas
+00009eb0: 7465 7273 2f5f 7265 6c73 2f73 6c69 6465  ters/_rels/slide
+00009ec0: 4d61 7374 6572 312e 786d 6c2e 7265 6c73  Master1.xml.rels
+00009ed0: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+00009ee0: d5d1 92f1 bc00 0000 3701 0000 2c00 0000  ........7...,...
+00009ef0: 0000 0000 0000 0000 0000 005e 0000 7070  ...........^..pp
+00009f00: 742f 736c 6964 654c 6179 6f75 7473 2f5f  t/slideLayouts/_
+00009f10: 7265 6c73 2f73 6c69 6465 4c61 796f 7574  rels/slideLayout
+00009f20: 372e 786d 6c2e 7265 6c73 504b 0102 2d00  7.xml.relsPK..-.
+00009f30: 1400 0600 0800 0000 2100 d5d1 92f1 bc00  ........!.......
+00009f40: 0000 3701 0000 2c00 0000 0000 0000 0000  ..7...,.........
+00009f50: 0000 0000 065f 0000 7070 742f 736c 6964  ....._..ppt/slid
+00009f60: 654c 6179 6f75 7473 2f5f 7265 6c73 2f73  eLayouts/_rels/s
+00009f70: 6c69 6465 4c61 796f 7574 362e 786d 6c2e  lideLayout6.xml.
+00009f80: 7265 6c73 504b 0102 2d00 1400 0600 0800  relsPK..-.......
+00009f90: 0000 2100 9b55 7ccd 1508 0000 6c36 0000  ..!..U|.....l6..
+00009fa0: 2100 0000 0000 0000 0000 0000 0000 0c60  !..............`
+00009fb0: 0000 7070 742f 736c 6964 654d 6173 7465  ..ppt/slideMaste
+00009fc0: 7273 2f73 6c69 6465 4d61 7374 6572 312e  rs/slideMaster1.
+00009fd0: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
+00009fe0: 0021 00d5 d192 f1bc 0000 0037 0100 002c  .!.........7...,
+00009ff0: 0000 0000 0000 0000 0000 0000 0060 6800  .............`h.
+0000a000: 0070 7074 2f73 6c69 6465 4c61 796f 7574  .ppt/slideLayout
+0000a010: 732f 5f72 656c 732f 736c 6964 654c 6179  s/_rels/slideLay
+0000a020: 6f75 7435 2e78 6d6c 2e72 656c 7350 4b01  out5.xml.relsPK.
+0000a030: 022d 0014 0006 0008 0000 0021 00d5 d192  .-.........!....
+0000a040: f1bc 0000 0037 0100 002c 0000 0000 0000  .....7...,......
+0000a050: 0000 0000 0000 0066 6900 0070 7074 2f73  .......fi..ppt/s
+0000a060: 6c69 6465 4c61 796f 7574 732f 5f72 656c  lideLayouts/_rel
+0000a070: 732f 736c 6964 654c 6179 6f75 7431 2e78  s/slideLayout1.x
+0000a080: 6d6c 2e72 656c 7350 4b01 022d 0014 0006  ml.relsPK..-....
+0000a090: 0008 0000 0021 00d5 d192 f1bc 0000 0037  .....!.........7
+0000a0a0: 0100 002c 0000 0000 0000 0000 0000 0000  ...,............
+0000a0b0: 006c 6a00 0070 7074 2f73 6c69 6465 4c61  .lj..ppt/slideLa
+0000a0c0: 796f 7574 732f 5f72 656c 732f 736c 6964  youts/_rels/slid
+0000a0d0: 654c 6179 6f75 7432 2e78 6d6c 2e72 656c  eLayout2.xml.rel
+0000a0e0: 7350 4b01 022d 0014 0006 0008 0000 0021  sPK..-.........!
+0000a0f0: 00d5 d192 f1bc 0000 0037 0100 002c 0000  .........7...,..
+0000a100: 0000 0000 0000 0000 0000 0072 6b00 0070  ...........rk..p
+0000a110: 7074 2f73 6c69 6465 4c61 796f 7574 732f  pt/slideLayouts/
+0000a120: 5f72 656c 732f 736c 6964 654c 6179 6f75  _rels/slideLayou
+0000a130: 7433 2e78 6d6c 2e72 656c 7350 4b01 022d  t3.xml.relsPK..-
+0000a140: 0014 0006 0008 0000 0021 00d5 d192 f1bc  .........!......
+0000a150: 0000 0037 0100 002c 0000 0000 0000 0000  ...7...,........
+0000a160: 0000 0000 0078 6c00 0070 7074 2f73 6c69  .....xl..ppt/sli
+0000a170: 6465 4c61 796f 7574 732f 5f72 656c 732f  deLayouts/_rels/
+0000a180: 736c 6964 654c 6179 6f75 7434 2e78 6d6c  slideLayout4.xml
+0000a190: 2e72 656c 7350 4b01 022d 0014 0006 0008  .relsPK..-......
+0000a1a0: 0000 0021 00b4 cf58 19b9 0000 0024 0100  ...!...X.....$..
+0000a1b0: 002c 0000 0000 0000 0000 0000 0000 007e  .,.............~
+0000a1c0: 6d00 0070 7074 2f6e 6f74 6573 4d61 7374  m..ppt/notesMast
+0000a1d0: 6572 732f 5f72 656c 732f 6e6f 7465 734d  ers/_rels/notesM
+0000a1e0: 6173 7465 7231 2e78 6d6c 2e72 656c 7350  aster1.xml.relsP
+0000a1f0: 4b01 022d 0014 0006 0008 0000 0021 008f  K..-.........!..
+0000a200: 1de5 b0b6 0500 008c 1d00 0021 0000 0000  ...........!....
+0000a210: 0000 0000 0000 0000 0081 6e00 0070 7074  ..........n..ppt
+0000a220: 2f6e 6f74 6573 4d61 7374 6572 732f 6e6f  /notesMasters/no
+0000a230: 7465 734d 6173 7465 7231 2e78 6d6c 504b  tesMaster1.xmlPK
+0000a240: 0102 2d00 0a00 0000 0000 0000 2100 669f  ..-.........!.f.
+0000a250: 9372 be08 0000 be08 0000 1700 0000 0000  .r..............
+0000a260: 0000 0000 0000 0000 7674 0000 646f 6350  ........vt..docP
+0000a270: 726f 7073 2f74 6875 6d62 6e61 696c 2e6a  rops/thumbnail.j
+0000a280: 7065 6750 4b01 022d 0014 0006 0008 0000  pegPK..-........
+0000a290: 0021 007b 43bc 5dc4 0600 00cf 2000 0014  .!.{C.]..... ...
+0000a2a0: 0000 0000 0000 0000 0000 0000 0069 7d00  .............i}.
+0000a2b0: 0070 7074 2f74 6865 6d65 2f74 6865 6d65  .ppt/theme/theme
+0000a2c0: 312e 786d 6c50 4b01 022d 0014 0006 0008  1.xmlPK..-......
+0000a2d0: 0000 0021 007b 43bc 5dc4 0600 00cf 2000  ...!.{C.]..... .
+0000a2e0: 0014 0000 0000 0000 0000 0000 0000 005f  ..............._
+0000a2f0: 8400 0070 7074 2f74 6865 6d65 2f74 6865  ...ppt/theme/the
+0000a300: 6d65 322e 786d 6c50 4b01 022d 0014 0006  me2.xmlPK..-....
+0000a310: 0008 0000 0021 00ea 6f03 2d76 0100 0017  .....!..o.-v....
+0000a320: 0300 0011 0000 0000 0000 0000 0000 0000  ................
+0000a330: 0055 8b00 0070 7074 2f76 6965 7750 726f  .U...ppt/viewPro
+0000a340: 7073 2e78 6d6c 504b 0102 2d00 1400 0600  ps.xmlPK..-.....
+0000a350: 0800 0000 2100 a364 236b 8d01 0000 3203  ....!..d#k....2.
+0000a360: 0000 1100 0000 0000 0000 0000 0000 0000  ................
+0000a370: fa8c 0000 7070 742f 7072 6573 5072 6f70  ....ppt/presProp
+0000a380: 732e 786d 6c50 4b01 022d 0014 0006 0008  s.xmlPK..-......
+0000a390: 0000 0021 00d8 fd8d 8fac 0000 00b6 0000  ...!............
+0000a3a0: 0013 0000 0000 0000 0000 0000 0000 00b6  ................
+0000a3b0: 8e00 0070 7074 2f74 6162 6c65 5374 796c  ...ppt/tableStyl
+0000a3c0: 6573 2e78 6d6c 504b 0102 2d00 1400 0600  es.xmlPK..-.....
+0000a3d0: 0800 0000 2100 e0bc ff06 7701 0000 b002  ....!.....w.....
+0000a3e0: 0000 1100 0000 0000 0000 0000 0000 0000  ................
+0000a3f0: 938f 0000 646f 6350 726f 7073 2f63 6f72  ....docProps/cor
+0000a400: 652e 786d 6c50 4b01 022d 0014 0006 0008  e.xmlPK..-......
+0000a410: 0000 0021 00c9 b2e7 2828 0200 0051 0500  ...!....((...Q..
+0000a420: 0010 0000 0000 0000 0000 0000 0000 0041  ...............A
+0000a430: 9200 0064 6f63 5072 6f70 732f 6170 702e  ...docProps/app.
+0000a440: 786d 6c50 4b05 0600 0000 0030 0030 00a4  xmlPK......0.0..
+0000a450: 0e00 009f 9500 0000 00                   .........
```

### Comparing `pptx-tools-0.1.1/pptx_tools/tts/azure_tts.py` & `pptx-tools-0.1.2/pptx_tools/tts/azure_tts.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.1/pptx_tools/tts/azure_tts_voice.py` & `pptx-tools-0.1.2/pptx_tools/tts/azure_tts_voice.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.1/pptx_tools/tts/google_tts.py` & `pptx-tools-0.1.2/pptx_tools/tts/google_tts.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,33 @@
+from distutils.version import LooseVersion
 from pathlib import Path
 
-from google.cloud import texttospeech
+from google.cloud.texttospeech import TextToSpeechClient
+import pkg_resources
 import pydub
 
 from .google_tts_voice import voice_name_to_language_code
 
 
+texttospeech_version = pkg_resources.get_distribution(
+    "google-cloud-texttospeech").version
+if LooseVersion(texttospeech_version) >= LooseVersion('2.0.0'):
+    from google.cloud.texttospeech import AudioConfig
+    from google.cloud.texttospeech import AudioEncoding
+    from google.cloud.texttospeech import SsmlVoiceGender
+    from google.cloud.texttospeech import SynthesisInput
+    from google.cloud.texttospeech import VoiceSelectionParams
+else:
+    from google.cloud.texttospeech_v1.gapic.enums import AudioEncoding
+    from google.cloud.texttospeech_v1.gapic.enums import SsmlVoiceGender
+    from google.cloud.texttospeech_v1.types import AudioConfig
+    from google.cloud.texttospeech_v1.types import SynthesisInput
+    from google.cloud.texttospeech_v1.types import VoiceSelectionParams
+
+
 lower2original = {k.lower(): k
                   for k in voice_name_to_language_code}
 
 
 def determine_voice_name(voice_name):
     voice_name = voice_name.lower()
     if len(voice_name) == 0:
@@ -41,31 +59,36 @@
 
     You can see which language is available here
     https://cloud.google.com/text-to-speech/docs/voices
     """
     audio_filepath = Path(audio_filepath)
     voice_name, language_code = determine_voice_name(voice_name)
 
-    client = texttospeech.TextToSpeechClient()
-    synthesis_input = texttospeech.SynthesisInput(
-        text=text)
-    voice = texttospeech.VoiceSelectionParams(
+    client = TextToSpeechClient()
+
+    synthesis_input = SynthesisInput(text=text)
+    voice = VoiceSelectionParams(
         language_code=language_code,
         name=voice_name,
-        ssml_gender=texttospeech.SsmlVoiceGender.FEMALE)
+        ssml_gender=SsmlVoiceGender.FEMALE)
 
     # Select the type of audio file you want returned
-    audio_config = texttospeech.AudioConfig(
-        audio_encoding=texttospeech.AudioEncoding.MP3,
+    audio_config = AudioConfig(
+        audio_encoding=AudioEncoding.MP3,
         sample_rate_hertz=sample_rate,
         speaking_rate=speaking_rate)
-    response = client.synthesize_speech(
-        input=synthesis_input,
-        voice=voice,
-        audio_config=audio_config)
+
+    if LooseVersion(texttospeech_version) >= LooseVersion('2.0.0'):
+        response = client.synthesize_speech(
+            input=synthesis_input,
+            voice=voice,
+            audio_config=audio_config)
+    else:
+        response = client.synthesize_speech(
+            synthesis_input, voice, audio_config)
 
     with open(str(audio_filepath.with_suffix('.mp3')), 'wb') as out:
         out.write(response.audio_content)
 
     if audio_filepath.suffix == '.wav':
         sound = pydub.AudioSegment.from_mp3(
             str(audio_filepath.with_suffix('.mp3')))
```

### Comparing `pptx-tools-0.1.1/pptx_tools/tts/google_tts_voice.py` & `pptx-tools-0.1.2/pptx_tools/tts/google_tts_voice.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.1/pptx_tools/utils.py` & `pptx-tools-0.1.2/pptx_tools/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 import langdetect
 from lxml import etree
 from pptx import Presentation
 from pptx.util import Inches
 
 from pptx_tools.audio_utils import get_wave_duration
 from pptx_tools.data import get_transparent_img_path
-from pptx_tools.tts import azure_text_to_speech
-from pptx_tools.tts import google_text_to_speech
 
 
 base_logger = logging.getLogger(__name__)
 
 
 def xpath(el, query):
     nsmap = {'p': 'http://schemas.openxmlformats.org/presentationml/2006/main'}
@@ -38,45 +36,53 @@
     """Synthesizes speech from the pptx."""
 
     if logger is None:
         logger = base_logger
     coloredlogs.install(level='DEBUG', logger=logger)
 
     if tts == 'google':
+        from pptx_tools.tts.google_tts import google_text_to_speech
         text_to_speech = google_text_to_speech
     elif tts == 'azure':
+        from pptx_tools.tts.azure_tts import azure_text_to_speech
         text_to_speech = azure_text_to_speech
     else:
         raise ValueError("Not supported tts {}".format(tts))
 
     output_path = Path(outdir)
     makedirs(output_path)
 
     presentation = Presentation(slide_path)
     total_time = 0.0
     for page, slide in enumerate(presentation.slides, start=1):
         if slide.has_notes_slide and slide.notes_slide.notes_text_frame.text:
             note_txt = slide.notes_slide.notes_text_frame.text
             note_txt = note_txt.replace('\n', ' ')
-            wave_path = output_path / f'{page}.wav'
+            wave_path = output_path / '{}.wav'.format(page)
 
             lang = langdetect.detect(note_txt)
-            if lang == 'en':
-                if tts == 'google':
-                    voice_name = 'en-US-Wavenet-A'
-                elif tts == 'azure':
-                    voice_name = 'en-US-BrandonNeural'
-            elif lang == 'ja':
-                if tts == 'google':
-                    voice_name = 'ja-JP-Wavenet-C'
-                elif tts == 'azure':
-                    voice_name = 'ja-JP-NanamiNeural'
-            else:
-                raise NotImplementedError(
-                    'Not supported language:{}'.format(lang))
+            if lang not in ['en', 'ja']:
+                logger.warning('Not supported language:{}'.format(lang))
+                lang = 'en'
+                logger.warning('Use english')
+            if voice_name is None:
+                if lang == 'en':
+                    if tts == 'google':
+                        voice_name = 'en-US-Wavenet-A'
+                    elif tts == 'azure':
+                        voice_name = 'en-US-BrandonNeural'
+                    else:
+                        raise RuntimeError('invalid tts')
+                elif lang == 'ja':
+                    if tts == 'google':
+                        voice_name = 'ja-JP-Wavenet-C'
+                    elif tts == 'azure':
+                        voice_name = 'ja-JP-NanamiNeural'
+                    else:
+                        raise RuntimeError('invalid tts')
             text_to_speech(wave_path, note_txt,
                            voice_name=voice_name)
             total_time += get_wave_duration(wave_path)
             try:
                 movie = slide.shapes.add_movie(
                     str(wave_path),
                     Inches(0), Inches(0), Inches(1.0), Inches(1.0),
```

### Comparing `pptx-tools-0.1.1/pptx_tools.egg-info/SOURCES.txt` & `pptx-tools-0.1.2/pptx_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.1/setup.py` & `pptx-tools-0.1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess
 import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "0.1.1"
+version = "0.1.2"
 
 
 if sys.argv[-1] == "release":
     # Release via github-actions.
     commands = [
         'git tag v{:s}'.format(version),
         'git push origin master --tag',
@@ -42,28 +42,27 @@
     for line in f:
         req = line.split('#')[0].strip()
         install_requires.append(req)
 
 setup(
     name="pptx-tools",
     version=version,
-    description="A python library",
+    description="A power point tools",
     author="iory",
     author_email="ab.ioryz@gmail.com",
     url="https://github.com/iory/pptx-tools",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.5",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: Implementation :: CPython",
     ],
     packages=find_packages(),
     package_data={'pptx_tools': listup_package_data()},
```

