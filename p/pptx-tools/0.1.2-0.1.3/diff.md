# Comparing `tmp/pptx-tools-0.1.2.tar.gz` & `tmp/pptx-tools-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pptx-tools-0.1.2.tar", last modified: Tue Jul 11 05:23:47 2023, max compression
+gzip compressed data, was "pptx-tools-0.1.3.tar", last modified: Tue Jul 11 08:59:23 2023, max compression
```

## Comparing `pptx-tools-0.1.2.tar` & `pptx-tools-0.1.3.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/pptx_tools/
--rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/pptx_tools/apps/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1954 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/apps/slide_add_voice.py
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/audio_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/pptx_tools/data/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    42073 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/data/hello.pptx
--rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/data/transparent.png
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/pptx_tools/tts/
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/tts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/tts/azure_tts.py
--rw-r--r--   0 runner    (1001) docker     (122)    17546 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/tts/azure_tts_voice.py
--rw-r--r--   0 runner    (1001) docker     (122)     3357 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/tts/google_tts.py
--rw-r--r--   0 runner    (1001) docker     (122)    18411 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/tts/google_tts_voice.py
--rw-r--r--   0 runner    (1001) docker     (122)     3646 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/pptx_tools/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/pptx_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-07-11 05:23:47.000000 pptx-tools-0.1.2/pptx_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      764 2023-07-11 05:23:47.000000 pptx-tools-0.1.2/pptx_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 05:23:47.000000 pptx-tools-0.1.2/pptx_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-11 05:23:47.000000 pptx-tools-0.1.2/pptx_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 05:23:47.000000 pptx-tools-0.1.2/pptx_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)      186 2023-07-11 05:23:47.000000 pptx-tools-0.1.2/pptx_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-11 05:23:47.000000 pptx-tools-0.1.2/pptx_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      180 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:47.109816 pptx-tools-0.1.2/tests/pptx_tools/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/tests/pptx_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      712 2023-07-11 05:23:39.000000 pptx-tools-0.1.2/tests/pptx_tools/test_slide_add_voice.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1058 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      615 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:23.742346 pptx-tools-0.1.3/pptx_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)      131 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/pptx_tools/apps/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2112 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/apps/slide_add_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/audio_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/pptx_tools/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    42073 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/data/hello.pptx
+-rw-r--r--   0 runner    (1001) docker     (122)      404 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/data/transparent.png
+-rw-r--r--   0 runner    (1001) docker     (122)     2529 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/slide_transition.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/pptx_tools/tts/
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/tts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2287 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/tts/azure_tts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17546 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/tts/azure_tts_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3357 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/tts/google_tts.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18411 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/tts/google_tts_voice.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3973 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/pptx_tools/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/pptx_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1322 2023-07-11 08:59:23.000000 pptx-tools-0.1.3/pptx_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      795 2023-07-11 08:59:23.000000 pptx-tools-0.1.3/pptx_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 08:59:23.000000 pptx-tools-0.1.3/pptx_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       73 2023-07-11 08:59:23.000000 pptx-tools-0.1.3/pptx_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 08:59:23.000000 pptx-tools-0.1.3/pptx_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      191 2023-07-11 08:59:23.000000 pptx-tools-0.1.3/pptx_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-07-11 08:59:23.000000 pptx-tools-0.1.3/pptx_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      243 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:23.746346 pptx-tools-0.1.3/tests/pptx_tools/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/tests/pptx_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      712 2023-07-11 08:59:10.000000 pptx-tools-0.1.3/tests/pptx_tools/test_slide_add_voice.py
```

### Comparing `pptx-tools-0.1.2/LICENSE` & `pptx-tools-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.2/PKG-INFO` & `pptx-tools-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pptx-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: A power point tools
 Home-page: https://github.com/iory/pptx-tools
 Author: iory
 Author-email: ab.ioryz@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pptx-tools-0.1.2/README.md` & `pptx-tools-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.2/pptx_tools/apps/slide_add_voice.py` & `pptx-tools-0.1.3/pptx_tools/apps/slide_add_voice.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,16 @@
                         default='./presentations')
     parser.add_argument("--voice-name", type=str,
                         help='If not set, use default value.')
     parser.add_argument("--tts", choices=tts_engines,
                         default='google',
                         help='select the text-to-speech engine. '
                         'You can choose {}.'.format(tts_engines))
+    parser.add_argument("--slide-duration-offset", type=float,
+                        default=1.0)
     args = parser.parse_args()
     if args.voice_name is not None:
         if args.tts == 'google' and args.voice_name not in google_voice:
             print('Invalid voice_name. Avaliable voices are:')
             print([voice for voice in google_voice.keys()])
             print("You can check the sample audio here: "
                   "https://cloud.google.com/text-to-speech/docs/voices")
@@ -37,13 +39,14 @@
         elif args.tts == 'azure' and args.voice_name not in azure_voice:
             print('Invalid voice_name. Avaliable voices are:')
             print([voice for voice in azure_voice.keys()])
             sys.exit(0)
     output_dir = Path(make_fancy_output_dir(
         args.out, no_save=True))
     output_slide_path = add_synthesize_audio(
-        args.input, output_dir, voice_name=args.voice_name)
+        args.input, output_dir, voice_name=args.voice_name,
+        slide_duration_offset=args.slide_duration_offset)
     termcolor.cprint('=> Saved to {}'.format(output_slide_path), 'green')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `pptx-tools-0.1.2/pptx_tools/data/hello.pptx` & `pptx-tools-0.1.3/pptx_tools/data/hello.pptx`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.2/pptx_tools/tts/azure_tts.py` & `pptx-tools-0.1.3/pptx_tools/tts/azure_tts.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.2/pptx_tools/tts/azure_tts_voice.py` & `pptx-tools-0.1.3/pptx_tools/tts/azure_tts_voice.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.2/pptx_tools/tts/google_tts.py` & `pptx-tools-0.1.3/pptx_tools/tts/google_tts.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.2/pptx_tools/tts/google_tts_voice.py` & `pptx-tools-0.1.3/pptx_tools/tts/google_tts_voice.py`

 * *Files identical despite different names*

### Comparing `pptx-tools-0.1.2/pptx_tools/utils.py` & `pptx-tools-0.1.3/pptx_tools/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 
 import coloredlogs
 from eos import makedirs
 import langdetect
 from lxml import etree
 from pptx import Presentation
 from pptx.util import Inches
+from tqdm import tqdm
 
 from pptx_tools.audio_utils import get_wave_duration
 from pptx_tools.data import get_transparent_img_path
+from pptx_tools.slide_transition import set_slide_duration
 
 
 base_logger = logging.getLogger(__name__)
 
 
 def xpath(el, query):
     nsmap = {'p': 'http://schemas.openxmlformats.org/presentationml/2006/main'}
@@ -28,15 +30,16 @@
     )[0]
     cond = xpath(el_cnt.getparent().getparent(), './/p:cond')[0]
     cond.set('delay', '0')
 
 
 def add_synthesize_audio(slide_path, outdir, logger=None,
                          voice_name=None,
-                         tts='google'):
+                         tts='google',
+                         slide_duration_offset=1.0):
     """Synthesizes speech from the pptx."""
 
     if logger is None:
         logger = base_logger
     coloredlogs.install(level='DEBUG', logger=logger)
 
     if tts == 'google':
@@ -49,15 +52,16 @@
         raise ValueError("Not supported tts {}".format(tts))
 
     output_path = Path(outdir)
     makedirs(output_path)
 
     presentation = Presentation(slide_path)
     total_time = 0.0
-    for page, slide in enumerate(presentation.slides, start=1):
+    for page, slide in tqdm(enumerate(presentation.slides, start=1),
+                            total=len(presentation.slides)):
         if slide.has_notes_slide and slide.notes_slide.notes_text_frame.text:
             note_txt = slide.notes_slide.notes_text_frame.text
             note_txt = note_txt.replace('\n', ' ')
             wave_path = output_path / '{}.wav'.format(page)
 
             lang = langdetect.detect(note_txt)
             if lang not in ['en', 'ja']:
@@ -77,15 +81,17 @@
                         voice_name = 'ja-JP-Wavenet-C'
                     elif tts == 'azure':
                         voice_name = 'ja-JP-NanamiNeural'
                     else:
                         raise RuntimeError('invalid tts')
             text_to_speech(wave_path, note_txt,
                            voice_name=voice_name)
-            total_time += get_wave_duration(wave_path)
+            duration = get_wave_duration(wave_path)
+            set_slide_duration(slide, duration + slide_duration_offset)
+            total_time += duration + slide_duration_offset
             try:
                 movie = slide.shapes.add_movie(
                     str(wave_path),
                     Inches(0), Inches(0), Inches(1.0), Inches(1.0),
                     poster_frame_image=str(get_transparent_img_path()),
                     mime_type='video/unknown')
             except AttributeError:
```

### Comparing `pptx-tools-0.1.2/pptx_tools.egg-info/PKG-INFO` & `pptx-tools-0.1.3/pptx_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pptx-tools
-Version: 0.1.2
+Version: 0.1.3
 Summary: A power point tools
 Home-page: https://github.com/iory/pptx-tools
 Author: iory
 Author-email: ab.ioryz@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `pptx-tools-0.1.2/pptx_tools.egg-info/SOURCES.txt` & `pptx-tools-0.1.3/pptx_tools.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 MANIFEST.in
 README.md
 requirements.txt
 setup.cfg
 setup.py
 pptx_tools/__init__.py
 pptx_tools/audio_utils.py
+pptx_tools/slide_transition.py
 pptx_tools/utils.py
 pptx_tools.egg-info/PKG-INFO
 pptx_tools.egg-info/SOURCES.txt
 pptx_tools.egg-info/dependency_links.txt
 pptx_tools.egg-info/entry_points.txt
 pptx_tools.egg-info/not-zip-safe
 pptx_tools.egg-info/requires.txt
```

### Comparing `pptx-tools-0.1.2/setup.py` & `pptx-tools-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import subprocess
 import sys
 
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "0.1.2"
+version = "0.1.3"
 
 
 if sys.argv[-1] == "release":
     # Release via github-actions.
     commands = [
         'git tag v{:s}'.format(version),
         'git push origin master --tag',
```

### Comparing `pptx-tools-0.1.2/tests/pptx_tools/test_slide_add_voice.py` & `pptx-tools-0.1.3/tests/pptx_tools/test_slide_add_voice.py`

 * *Files identical despite different names*

