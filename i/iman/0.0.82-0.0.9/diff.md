# Comparing `tmp/iman-0.0.82.tar.gz` & `tmp/iman-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iman-0.0.82.tar", last modified: Tue Jul 11 05:51:14 2023, max compression
+gzip compressed data, was "dist\iman-0.0.9.tar", last modified: Wed Oct 26 09:01:02 2022, max compression
```

## Comparing `iman-0.0.82.tar` & `iman-0.0.9.tar`

### file list

```diff
@@ -1,72 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 05:51:14.000000 iman-0.0.82/
--rw-rw-rw-   0        0        0     6580 2023-07-11 05:51:14.000000 iman-0.0.82/PKG-INFO
--rw-rw-rw-   0        0        0     6206 2023-07-11 05:49:33.000000 iman-0.0.82/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-11 05:51:14.000000 iman-0.0.82/iman/
--rw-rw-rw-   0        0        0     2070 2022-12-25 10:45:05.000000 iman-0.0.82/iman/AUG.py
--rw-rw-rw-   0        0        0    17408 2023-02-15 06:58:32.000000 iman-0.0.82/iman/Audio.py
--rw-rw-rw-   0        0        0      124 2023-01-29 08:15:58.000000 iman-0.0.82/iman/Boors.py
-drwxrwxrwx   0        0        0        0 2023-07-11 05:51:14.000000 iman-0.0.82/iman/Features/
--rw-rw-rw-   0        0        0       42 2022-11-13 07:01:23.000000 iman-0.0.82/iman/Features/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-11 05:51:14.000000 iman-0.0.82/iman/Features/mfcc/
--rw-rw-rw-   0        0        0     2836 2022-11-13 07:05:02.000000 iman-0.0.82/iman/Features/mfcc/LS.py
--rw-rw-rw-   0        0        0      604 2022-12-12 11:32:38.000000 iman-0.0.82/iman/Features/mfcc/SB.py
--rw-rw-rw-   0        0        0        0 2022-11-13 06:42:54.000000 iman-0.0.82/iman/Features/mfcc/__init__.py
--rw-rw-rw-   0        0        0    11080 2021-12-01 10:31:39.000000 iman-0.0.82/iman/Features/mfcc/getmfcc_from_librosa.py
--rw-rw-rw-   0        0        0    41655 2022-12-12 11:33:13.000000 iman-0.0.82/iman/Features/mfcc/sb_mfcc_class.py
--rw-rw-rw-   0        0        0     1057 2022-12-25 10:05:56.000000 iman-0.0.82/iman/Image.py
--rw-rw-rw-   0        0        0      815 2022-12-20 06:25:42.000000 iman-0.0.82/iman/Report.py
--rw-rw-rw-   0        0        0     2640 2023-02-20 05:13:55.000000 iman-0.0.82/iman/Text.py
--rw-rw-rw-   0        0        0     4391 2023-01-31 04:41:51.000000 iman-0.0.82/iman/__init__.py
--rw-rw-rw-   0        0        0      686 2022-12-17 11:18:42.000000 iman-0.0.82/iman/examples.py
-drwxrwxrwx   0        0        0        0 2023-07-11 05:51:14.000000 iman-0.0.82/iman/examples_folder/
--rw-rw-rw-   0        0        0        0 2022-12-17 11:24:05.000000 iman-0.0.82/iman/examples_folder/__init__.py
--rw-rw-rw-   0        0        0      539 2023-01-01 11:18:41.000000 iman-0.0.82/iman/examples_folder/age.py
--rw-rw-rw-   0        0        0      100 2023-01-01 05:01:21.000000 iman-0.0.82/iman/examples_folder/ffmpeg.py
--rw-rw-rw-   0        0        0      490 2022-12-17 09:55:52.000000 iman-0.0.82/iman/examples_folder/flask.py
--rw-rw-rw-   0        0        0      262 2021-01-05 11:07:03.000000 iman-0.0.82/iman/examples_folder/gpu_allocate_tf.py
--rw-rw-rw-   0        0        0      299 2022-12-31 09:42:30.000000 iman-0.0.82/iman/examples_folder/graphviz_chart.py
--rw-rw-rw-   0        0        0      345 2022-12-17 11:09:10.000000 iman-0.0.82/iman/examples_folder/parallel.py
--rw-rw-rw-   0        0        0      217 2022-12-17 11:12:20.000000 iman-0.0.82/iman/examples_folder/post_by_python.py
--rw-rw-rw-   0        0        0      775 2019-12-03 03:31:26.000000 iman-0.0.82/iman/examples_folder/pyworldd.py
--rw-rw-rw-   0        0        0      406 2022-12-05 05:24:04.000000 iman-0.0.82/iman/examples_folder/queue_worker.py
--rw-rw-rw-   0        0        0     1607 2021-11-28 10:10:27.000000 iman-0.0.82/iman/examples_folder/save_docx.py
--rw-rw-rw-   0        0        0      478 2019-05-05 06:27:38.000000 iman-0.0.82/iman/examples_folder/stft_test.py
--rw-rw-rw-   0        0        0      276 2019-11-19 00:37:16.000000 iman-0.0.82/iman/examples_folder/threading_example.py
--rw-rw-rw-   0        0        0      454 2021-05-25 08:55:10.000000 iman-0.0.82/iman/examples_folder/wikipedia.py
--rw-rw-rw-   0        0        0    15323 2022-11-06 10:39:16.000000 iman-0.0.82/iman/gpu_info.py
--rw-rw-rw-   0        0        0     1862 2022-11-12 05:34:50.000000 iman-0.0.82/iman/info.py
--rw-rw-rw-   0        0        0      318 2022-11-08 10:24:41.000000 iman-0.0.82/iman/matlab.py
--rw-rw-rw-   0        0        0     3422 2022-12-26 10:35:15.000000 iman-0.0.82/iman/metrics.py
-drwxrwxrwx   0        0        0        0 2023-07-11 05:51:14.000000 iman-0.0.82/iman/num2fa/
--rw-rw-rw-   0        0        0     8938 2023-01-28 05:46:54.000000 iman-0.0.82/iman/num2fa/__init__.py
--rw-rw-rw-   0        0        0      506 2023-01-28 05:46:54.000000 iman-0.0.82/iman/num2fa/__main__.py
--rw-rw-rw-   0        0        0      237 2022-12-19 06:23:20.000000 iman-0.0.82/iman/par.py
-drwxrwxrwx   0        0        0        0 2023-07-11 05:51:14.000000 iman-0.0.82/iman/sad_tf/
--rw-rw-rw-   0        0        0       92 2022-12-19 05:24:00.000000 iman-0.0.82/iman/sad_tf/__init__.py
--rw-rw-rw-   0        0        0     4645 2022-12-11 08:36:07.000000 iman-0.0.82/iman/sad_tf/export_funcs.py
--rw-rw-rw-   0        0        0     2221 2023-07-05 11:06:11.000000 iman-0.0.82/iman/sad_tf/features.py
--rw-rw-rw-   0        0        0    18746 2023-07-11 04:57:53.000000 iman-0.0.82/iman/sad_tf/segmenter.py
--rw-rw-rw-   0        0        0    13783 2022-11-30 10:00:38.000000 iman-0.0.82/iman/sad_tf/sidekit_mfcc.py
--rw-rw-rw-   0        0        0      553 2022-01-12 05:39:10.000000 iman-0.0.82/iman/sad_tf/thread_returning.py
--rw-rw-rw-   0        0        0     7808 2022-01-12 05:39:09.000000 iman-0.0.82/iman/sad_tf/viterbi.py
--rw-rw-rw-   0        0        0     1755 2022-01-12 05:39:10.000000 iman-0.0.82/iman/sad_tf/viterbi_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-11 05:51:14.000000 iman-0.0.82/iman/sad_torch_mfcc/
--rw-rw-rw-   0        0        0      107 2022-12-26 10:21:43.000000 iman-0.0.82/iman/sad_torch_mfcc/__init__.py
--rw-rw-rw-   0        0        0     4645 2022-12-11 08:33:44.000000 iman-0.0.82/iman/sad_torch_mfcc/export_funcs.py
--rw-rw-rw-   0        0        0     2002 2023-07-05 11:08:54.000000 iman-0.0.82/iman/sad_torch_mfcc/features.py
--rw-rw-rw-   0        0        0     3098 2022-12-11 08:39:59.000000 iman-0.0.82/iman/sad_torch_mfcc/sad_model.py
--rw-rw-rw-   0        0        0    19230 2023-07-05 11:15:27.000000 iman-0.0.82/iman/sad_torch_mfcc/segmenter.py
--rw-rw-rw-   0        0        0      553 2022-01-12 05:39:10.000000 iman-0.0.82/iman/sad_torch_mfcc/thread_returning.py
--rw-rw-rw-   0        0        0     7808 2022-01-12 05:39:09.000000 iman-0.0.82/iman/sad_torch_mfcc/viterbi.py
--rw-rw-rw-   0        0        0     1755 2022-01-12 05:39:10.000000 iman-0.0.82/iman/sad_torch_mfcc/viterbi_utils.py
--rw-rw-rw-   0        0        0      422 2022-11-22 05:36:39.000000 iman-0.0.82/iman/tsne.py
--rw-rw-rw-   0        0        0     2234 2023-06-10 12:42:19.000000 iman-0.0.82/iman/web.py
--rw-rw-rw-   0        0        0     7159 2022-10-26 09:16:54.000000 iman-0.0.82/iman/xvector.py
-drwxrwxrwx   0        0        0        0 2023-07-11 05:51:14.000000 iman-0.0.82/iman.egg-info/
--rw-rw-rw-   0        0        0     6580 2023-07-11 05:51:13.000000 iman-0.0.82/iman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1596 2023-07-11 05:51:13.000000 iman-0.0.82/iman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 05:51:13.000000 iman-0.0.82/iman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-07-11 05:51:13.000000 iman-0.0.82/iman.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-07-11 05:51:13.000000 iman-0.0.82/iman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-11 05:51:14.000000 iman-0.0.82/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-07-11 05:49:04.000000 iman-0.0.82/setup.py
+drwxrwxrwx   0        0        0        0 2022-10-26 09:01:02.000000 iman-0.0.9/
+-rw-rw-rw-   0        0        0     1801 2022-10-26 09:01:02.000000 iman-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2022-10-26 09:01:02.000000 iman-0.0.9/iman/
+-rw-rw-rw-   0        0        0    11046 2022-10-25 11:17:35.000000 iman-0.0.9/iman/Audio.py
+-rw-rw-rw-   0        0        0     3963 2022-10-26 08:59:53.000000 iman-0.0.9/iman/__init__.py
+-rw-rw-rw-   0        0        0      843 2022-10-25 11:17:47.000000 iman-0.0.9/iman/info.py
+-rw-rw-rw-   0        0        0     2440 2022-10-26 08:38:23.000000 iman-0.0.9/iman/metrics.py
+-rw-rw-rw-   0        0        0      329 2022-10-25 11:18:01.000000 iman-0.0.9/iman/tsne.py
+-rw-rw-rw-   0        0        0     7143 2022-10-26 08:59:26.000000 iman-0.0.9/iman/xvector.py
+drwxrwxrwx   0        0        0        0 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/
+-rw-rw-rw-   0        0        0     1801 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2022-10-26 09:01:02.000000 iman-0.0.9/iman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-10-26 09:01:02.000000 iman-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     2204 2022-10-26 09:00:03.000000 iman-0.0.9/setup.py
```

### Comparing `iman-0.0.82/iman/Features/mfcc/getmfcc_from_librosa.py` & `iman-0.0.9/iman/Audio.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,65 +1,225 @@
 import numpy as np
-import six
-import scipy
-import scipy.fftpack as fft
+from scipy import signal
+import os
+import scipy.io.wavfile as wave
 from numpy.lib.stride_tricks import as_strided
+import six
 
-MAX_MEM_BLOCK = 2**8 * 2**10
 
-class LibrosaError(Exception):
-    '''The root librosa exception class'''
-    pass
+ALawDecompressTable =[
 
+     -5504, -5248, -6016, -5760, -4480, -4224, -4992, -4736,
 
-class ParameterError(LibrosaError):
-    '''Exception class for mal-formed inputs'''
-    pass
+     -7552, -7296, -8064, -7808, -6528, -6272, -7040, -6784,
 
+     -2752, -2624, -3008, -2880, -2240, -2112, -2496, -2368,
 
+     -3776, -3648, -4032, -3904, -3264, -3136, -3520, -3392,
 
-def pad_center(data, size, axis=-1, **kwargs):
+     -22016,-20992,-24064,-23040,-17920,-16896,-19968,-18944,
 
-    kwargs.setdefault('mode', 'constant')
+     -30208,-29184,-32256,-31232,-26112,-25088,-28160,-27136,
 
-    n = data.shape[axis]
+     -11008,-10496,-12032,-11520,-8960, -8448, -9984, -9472,
 
-    lpad = int((size - n) // 2)
+     -15104,-14592,-16128,-15616,-13056,-12544,-14080,-13568,
 
-    lengths = [(0, 0)] * data.ndim
-    lengths[axis] = (lpad, int(size - n - lpad))
+     -344,  -328,  -376,  -360,  -280,  -264,  -312,  -296,
 
-    if lpad < 0:
-        raise ParameterError(('Target size ({:d}) must be '
-                              'at least input size ({:d})').format(size, n))
+     -472,  -456,  -504,  -488,  -408,  -392,  -440,  -424,
 
-    return np.pad(data, lengths, **kwargs)
+     -88,   -72,   -120,  -104,  -24,   -8,    -56,   -40,
 
-def valid_audio(y, mono=True):
-    if not isinstance(y, np.ndarray):
-        raise ParameterError('data must be of type numpy.ndarray')
+     -216,  -200,  -248,  -232,  -152,  -136,  -184,  -168,
 
-    if not np.issubdtype(y.dtype, np.floating):
-        raise ParameterError('data must be floating-point')
+     -1376, -1312, -1504, -1440, -1120, -1056, -1248, -1184,
 
-    if mono and y.ndim != 1:
-        raise ParameterError('Invalid shape for monophonic audio: '
-                             'ndim={:d}, shape={}'.format(y.ndim, y.shape))
+     -1888, -1824, -2016, -1952, -1632, -1568, -1760, -1696,
 
-    elif y.ndim > 2 or y.ndim == 0:
-        raise ParameterError('Audio must have shape (samples,) or (channels, samples). '
-                             'Received shape={}'.format(y.shape))
+     -688,  -656,  -752,  -720,  -560,  -528,  -624,  -592,
 
-    if not np.isfinite(y).all():
-        raise ParameterError('Audio buffer is not finite everywhere')
+     -944,  -912,  -1008, -976,  -816,  -784,  -880,  -848,
 
-    return True
-	
-def frame(y, frame_length=2048, hop_length=512):
+      5504,  5248,  6016,  5760,  4480,  4224,  4992,  4736,
+
+      7552,  7296,  8064,  7808,  6528,  6272,  7040,  6784,
+
+      2752,  2624,  3008,  2880,  2240,  2112,  2496,  2368,
+
+      3776,  3648,  4032,  3904,  3264,  3136,  3520,  3392,
+
+      22016, 20992, 24064, 23040, 17920, 16896, 19968, 18944,
+
+      30208, 29184, 32256, 31232, 26112, 25088, 28160, 27136,
+
+      11008, 10496, 12032, 11520, 8960,  8448,  9984,  9472,
+
+      15104, 14592, 16128, 15616, 13056, 12544, 14080, 13568,
+
+      344,   328,   376,   360,   280,   264,   312,   296,
+
+      472,   456,   504,   488,   408,   392,   440,   424,
+
+      88,    72,   120,   104,    24,     8,    56,    40,
+
+      216,   200,   248,   232,   152,   136,   184,   168,
+
+      1376,  1312,  1504,  1440,  1120,  1056,  1248,  1184,
+
+      1888,  1824,  2016,  1952,  1632,  1568,  1760,  1696,
+
+      688,   656,   752,   720,   560,   528,   624,   592,
+
+      944,   912,  1008,   976,   816,   784,   880,   848]
+
+def Read_Alaw(filename):
+    with open(filename, "rb") as binaryfile :
+       myArr = bytearray(binaryfile.read())
+    g=[ALawDecompressTable[x]/32768 for x in myArr]
+    return np.array(g , dtype=np.float32)
+
+def Resample(data , fs, sr):
+    """Return Resampled Data.
+
+    Parameters
+    ----------
+    data : input audio data
+    fs : data sampling rate
+    sr : resample data to sr
+    
+    Output
+    ----------
+    data with sampling rate --> sr
+
+    """
+    if (fs!=sr):
+        nesbat = sr/fs
+        m = np.max(np.abs(data))
+        data = 0.5*(data/(m+1e-6))
+        data = signal.resample(data, int(len(data)*nesbat))
+    return (np.array(data , dtype=np.float32))    
+
+def Read(filename,sr):   # output sampling rate is sr
+   """Return Audio Data. (Just Mono Files)
+
+    Parameters
+    ----------
+    filename : input file path (PCM or alaw or [alaw_raw with .l or .r ext])
+    sr : desired sampling rate
+    
+    Output
+    ----------
+    data with sampling rate --> sr
+
+   """   
+   ext = os.path.basename(filename).split('.')[-1] 
+   if (ext.lower() == 'l' or ext.lower() == 'r' ):
+       return( Resample( Read_Alaw(filename) , 8000, sr) )
+   
+   File_Type_Header= np.fromfile(filename, dtype=np.byte, count=4, offset=8)
+   File_Type_Header = "".join(map(chr, File_Type_Header))   # Must be WAVE
+   if (File_Type_Header!="WAVE"):
+       return("no_wav")
+   Type_of_format = np.fromfile(filename, dtype=np.int8, count=1, offset=20)[0]  # 1 is PCM   6 is alaw
 
+   ch = np.fromfile(filename, dtype=np.int8, count=1, offset=22)[0]  
+   
+   if (ch!=1):
+       return("sterio file")
+   
+   fs = np.fromfile(filename, dtype=np.int32, count=1, offset=24)[0] # Hz
+   
+   if (Type_of_format!=1 and Type_of_format!=6 ):
+       return ("no_pcm_alaw")
+   
+   if (Type_of_format==6):   # if file is alaw
+        byte_length = np.fromfile(filename, dtype=np.int32, count=1, offset=40)[0]
+        data = np.fromfile(filename, dtype=np.byte, count=byte_length*4, offset=44)
+        data=np.array([ALawDecompressTable[x]/32768 for x in data], dtype=np.float32)
+        return (Resample(data,fs,sr))
+   
+   chunk_header = np.fromfile(filename, dtype=np.byte, count=4, offset=36)
+   chunk_header = "".join(map(chr, chunk_header))
+   if (chunk_header=="LIST"):
+     import librosa
+     data,_ = librosa.load(filename,sr)
+   elif(chunk_header=="data"):
+      byte_length = np.fromfile(filename, dtype=np.int32, count=1, offset=40)[0]
+      data = np.fromfile(filename, dtype=np.int16, count=byte_length // 2, offset=44)/32768
+      data = Resample(data,fs,sr)
+   else:
+       return ("Unknown chunk_header-->" + chunk_header)
+   return (data)
+
+def ReadMp3(filename,sr,mono=True):
+    import miniaudio
+    mp3file = miniaudio.read_file(filename,True)
+    sample_rate = mp3file.sample_rate
+    data =  np.array(mp3file.samples , dtype=np.float32)/32768
+    if (mp3file.nchannels==1):
+       if (sample_rate!=sr):
+            data = Resample(data ,sample_rate ,sr )
+    else:
+         ch1=np.array( [ data[i] for i in range(0,len(data),2)  ] , dtype=np.float32)
+         ch2=np.array([ data[i] for i in range(1,len(data),2)  ], dtype=np.float32)
+         if (mono):
+           cha = ch1+ch2
+         if (sample_rate!=sr):
+                if (mono):
+                  cha = Resample(cha ,sample_rate ,sr )
+                else:  
+                   ch1 = Resample(ch1 ,sample_rate ,sr )
+                   ch2 = Resample(ch2 ,sample_rate ,sr )
+         if (mono):          
+           data = cha
+         else:
+           data=  [ch1,ch2]       
+    return(data)
+
+
+def Write(filename, data ,fs):
+
+   """Write Audio Data.
+
+    Parameters
+    ----------
+    filename : Output file path (.wav)
+    data : Audio data
+    fs : sampling rate
+    
+    Output
+    ----------
+    Nothing
+
+   """
+   wave.write(filename, fs, np.int16(data*32768))
+
+def rmse(y=None, S=None, frame_length=2048, hop_length=512,
+         center=True, pad_mode='reflect'):
+    
+    if y is not None and S is not None:
+        raise ValueError('Either `y` or `S` should be input.')
+    if y is not None:
+        y = (y)
+        if center:
+            y = np.pad(y, int(frame_length // 2), mode=pad_mode)
+
+        x = frame(y,
+                       frame_length=frame_length,
+                       hop_length=hop_length)
+    elif S is not None:
+        x, _ = _spectrogram(y=y, S=S,
+                            n_fft=frame_length,
+                            hop_length=hop_length)
+    else:
+        raise ValueError('Either `y` or `S` must be input.')
+    return np.sqrt(np.mean(np.abs(x)**2, axis=0, keepdims=True))
+def frame(y, frame_length=2048, hop_length=512):
+   
     if not isinstance(y, np.ndarray):
         raise ParameterError('Input must be of type numpy.ndarray, '
                              'given type(y)={}'.format(type(y)))
 
     if y.ndim != 1:
         raise ParameterError('Input must be one-dimensional, '
                              'given y.ndim={}'.format(y.ndim))
@@ -77,26 +237,25 @@
     # Compute the number of frames that will fit. The end may get truncated.
     n_frames = 1 + int((len(y) - frame_length) / hop_length)
 
     # Vertical stride is one sample
     # Horizontal stride is `hop_length` samples
     y_frames = as_strided(y, shape=(frame_length, n_frames),
                           strides=(y.itemsize, hop_length * y.itemsize))
-    return y_frames
-	
+    return y_frames	
 def power_to_db(S, ref=1.0, amin=1e-10, top_db=80.0):
-  
+   
 
     S = np.asarray(S)
 
     if amin <= 0:
         raise ParameterError('amin must be strictly positive')
 
     if np.issubdtype(S.dtype, np.complexfloating):
-        print('power_to_db was called on complex input so phase '
+        warnings.warn('power_to_db was called on complex input so phase '
                       'information will be discarded. To suppress this warning, '
                       'call power_to_db(magphase(D, power=2)[0]) instead.')
         magnitude = np.abs(S)
     else:
         magnitude = S
 
     if six.callable(ref):
@@ -109,229 +268,64 @@
     log_spec -= 10.0 * np.log10(np.maximum(amin, ref_value))
 
     if top_db is not None:
         if top_db < 0:
             raise ParameterError('top_db must be non-negative')
         log_spec = np.maximum(log_spec, log_spec.max() - top_db)
 
-    return log_spec	
-
-
-def amplitude_to_db(S, ref=1.0, amin=1e-5, top_db=80.0):
-    S = np.asarray(S)
-
-    if np.issubdtype(S.dtype, np.complexfloating):
-        print('amplitude_to_db was called on complex input so phase '
-                      'information will be discarded. To suppress this warning, '
-                      'call amplitude_to_db(magphase(D)[0]) instead.')
-
-    magnitude = np.abs(S)
-
-    if six.callable(ref):
-        # User supplied a function to calculate reference power
-        ref_value = ref(magnitude)
-    else:
-        ref_value = np.abs(ref)
-
-    power = np.square(magnitude, out=magnitude)
-
-    return power_to_db(power, ref=ref_value**2, amin=amin**2,
-                       top_db=top_db)
-					   
-					   
-def STFT(y, n_fft=2048, hop_length=None, win_length=None, window='hann',
-         center=True, dtype=np.complex64, pad_mode='reflect'):
-    # By default, use the entire frame
-    if win_length is None:
-        win_length = n_fft
-
-    # Set the default hop, if it's not already specified
-    if hop_length is None:
-        hop_length = int(win_length // 4)
+    return log_spec
+def _signal_to_frame_nonsilent(y_mono, frame_length=2048, hop_length=512, top_db=60,
+                               ref=np.max):
 
-    fft_window = get_window(window, win_length, fftbins=True)
-
-    # Pad the window out to n_fft size
-    fft_window = pad_center(fft_window, n_fft)
-
-    # Reshape so that the window can be broadcast
-    fft_window = fft_window.reshape((-1, 1))
-
-    # Check audio is valid
-    valid_audio(y)
-
-    # Pad the time series so that frames are centered
-    if center:
-        y = np.pad(y, int(n_fft // 2), mode=pad_mode)
-
-    # Window the time series.
-    y_frames = frame(y, frame_length=n_fft, hop_length=hop_length)
-
-    # Pre-allocate the STFT matrix
-    stft_matrix = np.empty((int(1 + n_fft // 2), y_frames.shape[1]),
-                           dtype=dtype,
-                           order='F')
-
-    # how many columns can we fit within MAX_MEM_BLOCK?
-    n_columns = int(MAX_MEM_BLOCK / (stft_matrix.shape[0] *
-                                          stft_matrix.itemsize))
-
-    for bl_s in range(0, stft_matrix.shape[1], n_columns):
-        bl_t = min(bl_s + n_columns, stft_matrix.shape[1])
-
-        # RFFT and Conjugate here to match phase from DPWE code
-        stft_matrix[:, bl_s:bl_t] = fft.fft(fft_window *
-                                            y_frames[:, bl_s:bl_t],
-                                            axis=0)[:stft_matrix.shape[0]]
-
-    return stft_matrix
-
-
-def get_window(window, Nx, fftbins=True):
-    if six.callable(window):
-        return window(Nx)
-
-    elif (isinstance(window, (six.string_types, tuple)) or
-          np.isscalar(window)):
-        # TODO: if we add custom window functions in librosa, call them here
-
-        return scipy.signal.get_window(window, Nx, fftbins=fftbins)
-
-    elif isinstance(window, (np.ndarray, list)):
-        if len(window) == Nx:
-            return np.asarray(window)
-
-        raise ParameterError('Window size mismatch: '
-                             '{:d} != {:d}'.format(len(window), Nx))
-    else:
-        raise ParameterError('Invalid window specification: {}'.format(window))
-
-def hz_to_mel(frequencies, htk=False):
-
-    frequencies = np.asanyarray(frequencies)
-
-    if htk:
-        return 2595.0 * np.log10(1.0 + frequencies / 700.0)
-
-    # Fill in the linear part
-    f_min = 0.0
-    f_sp = 200.0 / 3
-
-    mels = (frequencies - f_min) / f_sp
-
-    # Fill in the log-scale part
-
-    min_log_hz = 1000.0                         # beginning of log region (Hz)
-    min_log_mel = (min_log_hz - f_min) / f_sp   # same (Mels)
-    logstep = np.log(6.4) / 27.0                # step size for log region
-
-    if frequencies.ndim:
-        # If we have array data, vectorize
-        log_t = (frequencies >= min_log_hz)
-        mels[log_t] = min_log_mel + np.log(frequencies[log_t]/min_log_hz) / logstep
-    elif frequencies >= min_log_hz:
-        # If we have scalar data, heck directly
-        mels = min_log_mel + np.log(frequencies / min_log_hz) / logstep
-
-    return mels
-
-def mel_to_hz(mels, htk=False):
+    # Convert to mono
    
-    mels = np.asanyarray(mels)
 
-    if htk:
-        return 700.0 * (10.0**(mels / 2595.0) - 1.0)
-
-    # Fill in the linear scale
-    f_min = 0.0
-    f_sp = 200.0 / 3
-    freqs = f_min + f_sp * mels
-
-    # And now the nonlinear scale
-    min_log_hz = 1000.0                         # beginning of log region (Hz)
-    min_log_mel = (min_log_hz - f_min) / f_sp   # same (Mels)
-    logstep = np.log(6.4) / 27.0                # step size for log region
-
-    if mels.ndim:
-        # If we have vector data, vectorize
-        log_t = (mels >= min_log_mel)
-        freqs[log_t] = min_log_hz * np.exp(logstep * (mels[log_t] - min_log_mel))
-    elif mels >= min_log_mel:
-        # If we have scalar data, check directly
-        freqs = min_log_hz * np.exp(logstep * (mels - min_log_mel))
-
-    return freqs
-
-
-def fft_frequencies(sr=22050, n_fft=2048):
-
-
-    return np.linspace(0,
-                       float(sr) / 2,
-                       int(1 + n_fft//2),
-                       endpoint=True)
-
-def mel_frequencies(n_mels=128, fmin=0.0, fmax=11025.0, htk=False):
-
-    # 'Center freqs' of mel bands - uniformly spaced between limits
-    min_mel = hz_to_mel(fmin, htk=htk)
-    max_mel = hz_to_mel(fmax, htk=htk)
-
-    mels = np.linspace(min_mel, max_mel, n_mels)
-
-    return mel_to_hz(mels, htk=htk)
-
-def MEL(sr, n_fft, n_mels=128, fmin=0.0, fmax=None, htk=False,
-        norm=1):
-
-    if fmax is None:
-        fmax = float(sr) / 2
-
-    if norm is not None and norm != 1 and norm != np.inf:
-        raise ParameterError('Unsupported norm: {}'.format(repr(norm)))
-
-    # Initialize the weights
-    n_mels = int(n_mels)
-    weights = np.zeros((n_mels, int(1 + n_fft // 2)))
-
-    # Center freqs of each FFT bin
-    fftfreqs = fft_frequencies(sr=sr, n_fft=n_fft)
-
-    # 'Center freqs' of mel bands - uniformly spaced between limits
-    mel_f = mel_frequencies(n_mels + 2, fmin=fmin, fmax=fmax, htk=htk)
-
-    fdiff = np.diff(mel_f)
-    ramps = np.subtract.outer(mel_f, fftfreqs)
-
-    for i in range(n_mels):
-        # lower and upper slopes for all bins
-        lower = -ramps[i] / fdiff[i]
-        upper = ramps[i+2] / fdiff[i+1]
-
-        # .. then intersect them with each other and zero
-        weights[i] = np.maximum(0, np.minimum(lower, upper))
-
-    if norm == 1:
-        # Slaney-style mel is scaled to be approx constant energy per channel
-        enorm = 2.0 / (mel_f[2:n_mels+2] - mel_f[:n_mels])
-        weights *= enorm[:, np.newaxis]
-
-    # Only check weights if f_mel[0] is positive
-    if not np.all((mel_f[:-2] == 0) | (weights.max(axis=1) > 0)):
-        # This means we have an empty channel somewhere
-        print('Empty filters detected in mel frequency basis. '
-                      'Some channels will produce empty responses. '
-                      'Try increasing your sampling rate (and fmax) or '
-                      'reducing n_mels.')
-
-    return weights
-
-def dct(n_filters, n_input):
-    basis = np.empty((n_filters, n_input))
-    basis[0, :] = 1.0 / np.sqrt(n_input)
+    # Compute the MSE for the signal
+    mse = rmse(y=y_mono,
+                       frame_length=frame_length,
+                       hop_length=hop_length)**2
+
+    return (power_to_db(mse.squeeze(),
+                             ref=ref,
+                             top_db=None) > - top_db)					 
+def split(y, top_db=40, ref=np.max, frame_length=200, hop_length=80):
+
+    non_silent = _signal_to_frame_nonsilent(y,
+                                            frame_length=frame_length,
+                                            hop_length=hop_length,
+                                            ref=ref,
+                                            top_db=top_db)
+
+    # Interval slicing, adapted from
+    # https://stackoverflow.com/questions/2619413/efficiently-finding-the-interval-with-non-zeros-in-scipy-numpy-in-python
+    # Find points where the sign flips
+    edges = np.flatnonzero(np.diff(non_silent.astype(int)))
+
+    # Pad back the sample lost in the diff
+    edges = [edges + 1]
+
+    # If the first frame had high energy, count it
+    if non_silent[0]:
+        edges.insert(0, [0])
+
+    # Likewise for the last frame
+    if non_silent[-1]:
+        edges.append([len(non_silent)])
+
+    # Convert from frames to samples
+    edges = frames_to_samples(np.concatenate(edges),
+                                   hop_length=hop_length)
+
+    # Clip to the signal duration
+    edges = np.minimum(edges, y.shape[-1])
+
+    # Stack the results back as an ndarray
+    return edges.reshape((-1, 2))
+def frames_to_samples(frames, hop_length=512, n_fft=None):
+  
 
-    samples = np.arange(1, 2*n_input, 2) * np.pi / (2.0 * n_input)
+    offset = 0
+    if n_fft is not None:
+        offset = int(n_fft // 2)
 
-    for i in range(1, n_filters):
-        basis[i, :] = np.cos(i*samples) * np.sqrt(2.0/n_input)
+    return (np.asanyarray(frames) * hop_length + offset).astype(int)
 
-    return basis
```

### Comparing `iman-0.0.82/iman/__init__.py` & `iman-0.0.9/iman/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,33 +1,16 @@
 import matplotlib.pyplot as plt
 import time
 from glob import glob as gf
 import os
 import numpy as np
-from joblib import load,dump
 
 def help():
-    from iman import web
-    x=web.dl(r'https://pypi.org/project/iman/')
-    idx = x.index('class="project-description"')
-    idy = x.index('</div>' , idx+1)
-    y= (x[idx+29:idy].strip().replace('<span class="docutils literal">','<').replace('</span>','>').replace('</section>','').replace('<h2>','').replace('</h2>','').replace('<p>','').replace('</p>','').replace('<section id=from-iman-import>',''))
-    
+   print('from iman import Audio:\n1-Read(filename,sr)\n2-Resample(data , fs, sr)\n3-Read_Alaw(filename)\n4-ReadMp3(filename,sr,mono=True)\n5-Write(filename, data ,fs)\n6-frame(y)\n7-split(y)\n\nfrom iman import *:\n1-plt\n2-now() (get time)\n3-F (format floating point)\n4-D (format int number)\n5-Write_List(MyList,Filename)\n6-Write_Dic(MyDic,Filename)\n7-Read(Filename) (read txt file)\n8-Read_Lines(Filename) (read txt file line by line and return list)\n9-Write(_str,Filename)\n10-gf(pattern) (Get files in a directory)\n11-gfa(directory , ext="*.*") (Get Files in a Directory and SubDirectories)\n12-ReadE(Filename) (Read Excel files)\n13-PM(dir)(creat directory)\n14-PB(fname)(get basename)\n15-PN(fname) (get file name)\n16-PE(fname)(get ext)\n17-PD(fname)(get directory)\n18-PS(fname)(get size)\n19-PJ(segments) (Join Path)\n20-clear() (clear cmd)\n21-os\n22-np\n23-RI(start_int , end_int , count=1) (random int)\n24-RF(start_float , end_float , count=1) (random float)\n25-RS(Arr) (shuffle)\n\nfrom iman import info:\n1-get() info about cpu and gpu (need torch)\n\n\nfrom iman import metrics:\n1-EER(lab,score)\n2-cosine_distance(v1,v2)\n3-roc(lab,score)\n4-wer(ref, hyp)\n5-cer(ref, hyp)\n6-wer_list(ref_list , hyp_list)\n7-cer_list(ref_list , hyp_list)\n\nfrom iman import tsne:\n1-plot(fea , label)\n\nfrom iman import xvector:\n1-xvec,lda_xvec,gender = get(filename , model(model_path , model_name , model_speaker_num))\n\n')
 
-    while(True):
-       try:
-        idx=0
-        idx = y.index('<section',idx+1)
-
-        idy = y.index('>' , idx+1)
-
-        y = y.replace(y[idx:idy+1] , '')
-       except:
-         break       
-    print(y)
    
 def clear():
     if os.name == 'nt':
         _ = os.system('cls')  
     else:
         _ = os.system('clear')
         
@@ -61,23 +44,20 @@
          return(fid.read())
 
 def Read_Lines(Filename):
     with open(Filename , 'r' , encoding='utf-8') as fid:
          return([x.strip() for x in fid if (x.strip()!="")])    
 
 def gfa(directory , ext="*.*"):
- fols = gf(directory)
- a=[]
- for _fol in fols: 
-   [a.append(x) for x in gf(os.path.join(_fol , ext))]
-   for root, dirs, files in os.walk(_fol):
+   a=[]
+   for root, dirs, files in os.walk(directory):
       for dirname in dirs:
-         _dir =os.path.join(root, dirname)         
-         [a.append(x) for x in gf(os.path.join(_dir , ext))]           
- return a         
+         _dir =os.path.join(root, dirname)  
+         [a.append(x) for x in gf(os.path.join(_dir , ext))]   
+   return a         
 
 def ReadE(Filename):
     import pandas as pd
     pp = pd.read_excel(Filename , engine='openpyxl')
     return pp
     
 def PB(filename):
@@ -89,18 +69,15 @@
 def PM(folname):
    return os.makedirs(folname , exist_ok=True)
        
 def PN(filename):
    return os.path.basename(os.path.splitext(filename)[0])  
 
 def PE(filename):
-   return os.path.splitext(filename)[1]   
-
-def PX(filename):
-   return os.path.exists(filename)    
+   return os.path.splitext(filename)[1]    
    
 def PJ(*_segments):
    x=""
    for p in _segments:
       x = os.path.join(x,p)
    return x   
    
@@ -111,49 +88,8 @@
    return np.random.randint(low=int(start_int), high=int(end_int), size=(count,))
    
 def RF(start_float , end_float , count=1):
   return np.random.uniform(start_float, end_float , count)
   
 def RS(Arr):
   np.random.shuffle(Arr)
-  return Arr
-  
-def RC(Arr , _size=1):
-   return np.random.choice(Arr , _size)
-
-
-def LJ(job_file_name):
-   return load(job_file_name)
-   
-def SJ(value , job_file_name):
-   dump(value , job_file_name)   
-   
-def LN(np_file_name):
-   return np.load(np_file_name) 
-   
-def SN(arr , np_file_name):
-   return np.save(np_file_name , arr)   
-   
-def cmd(command , redirect=True):
-  if (redirect):
-   return os.popen(command).read()   
-  else:
-    os.system(command)  
-    
-    
-def onehot(data, nb_classes):
-    """Convert an iterable of indices to one-hot encoded labels."""
-    targets = np.array(data).reshape(-1)
-    return np.eye(nb_classes)[targets]
-    
-    
-def exe(fname):
-    cmd('pyinstaller --onefile ' + fname , False)    
-    
-def FWL(wavfolder , sr): #Get Audio Lenth Exist in this folder    
-    files=gfa(wavfolder , '*.wav')
-    n=0
-    for filename in files:
-         n=n+PS(filename)
-    header=len(files)*44       
-    print((n-header)/(sr*2*60*60))
-    return  ((n-header)/(sr*2*60*60))       
+  return Arr
```

### Comparing `iman-0.0.82/iman/metrics.py` & `iman-0.0.9/iman/metrics.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import numpy as np
 from sklearn.metrics import roc_curve as rc
 from iman import *
 import Levenshtein as Lev
-import scipy.spatial as sp
 
 
 def help():
    print('\nneed <Levenshtein> and <sklearn>\n')
 
 
 def cosine_distance(v1,v2):
-  return sp.distance.cdist(v1, v2, 'cosine')
-  
+  dot_product = np.dot(v1, v2)
+  norm_a = np.linalg.norm(v1)
+  norm_b = np.linalg.norm(v2)
+  return dot_product / (norm_a * norm_b)
 
 def compute_eer(fpr,tpr,thresholds):
     fnr = 1-tpr
     abs_diffs = np.abs(fpr - fnr)
     min_index = np.argmin(abs_diffs)
     eer = np.mean((fpr[min_index], fnr[min_index]))
     return eer, thresholds[min_index]  ,min_index
@@ -69,51 +70,8 @@
        x.append(wer(ref_list[i] , hyp_list[i]))
     return np.mean(x)   
     
 def cer_list(ref_list , hyp_list):
     x=[]
     for i in range(len(ref_list)):
        x.append(cer(ref_list[i] , hyp_list[i]))
-    return np.mean(x)    
-    
-    
-def DER(ref_list , res_list , file_dur=-1 , sr=8000):
-    """ input--> [ [st1,en1] , [st2 , en2] , ....   ]
-        just for speech parts
-        Output--> Miss , FA , DER , miss_points, fa_points
-    """        
-    
-    if (file_dur==-1):
-        file_dur = max(ref_list[-1][1] , res_list[-1][1])
-    
-    ref = np.zeros((int(file_dur*sr)))
-    
-    for a,b in ref_list:
-        ref[int(sr * a) : int(sr*b)]=1
-              
-    res = np.zeros((int(file_dur*sr)))
-    
-    for a,b in res_list:
-        res[int(sr * a) : int(sr*b)]=1
-     
-    
-    _miss_points=[]
-    _y=np.where(ref==1)[0] 
-    for i in _y:
-        if (res[i]==0):
-            _miss_points.append(i)
-    x = len(_miss_points)
-    miss = x / file_dur 
-    
-
-    _fa_points=[]
-    _y=np.where(res==1)[0] 
-    for i in _y:
-        if (ref[i]==0):
-            _fa_points.append(i)
-    x1 = len(_fa_points)
-    fa = x1 / file_dur 
-    
-    _der =(x+x1)/file_dur
-    
-
-    return (miss , fa ,_der ,_miss_points,_fa_points)
+    return np.mean(x)
```

### Comparing `iman-0.0.82/iman/xvector.py` & `iman-0.0.9/iman/xvector.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,21 +193,21 @@
 def get_xvec(feat, modelxvec ,batch_size):
  
   xvec,gender = modelxvec.predict(feat, batch_size = batch_size,verbose=1,use_multiprocessing=True)
   return xvec,gender
 
 
 def model(model_path , model_name , model_speaker_num):
-    return [get_model(model_path , model_name , model_speaker_num) , model_path]
+    return get_model(model_path , model_name , model_speaker_num)
 
 def get(filename , _model):
    sample_rate=8000
    data =Audio.Read(filename , sample_rate)
    fea = get_fea_file(data , sample_rate)
-   xvec, a = get_xvec(np.reshape(fea , (1 , np.shape(fea)[0], np.shape(fea)[1])), _model[0], batch_size=1)
-   xvec_lda = apply_lda(xvec, PJ(_model[1], 'meanvec.npy'), PJ(_model[1], 'lda.job'))
+   xvec, a = get_xvec(np.reshape(fea , (1 , np.shape(fea)[0], np.shape(fea)[1])), _model, batch_size=1)
+   xvec_lda = apply_lda(xvec, PJ(model_path, 'meanvec.npy'), PJ(model_path, 'lda.job'))
    gender='male'
    if (a[0][0]>=a[0][1]):
        gender='female'
    return(np.squeeze(xvec),np.squeeze(xvec_lda),gender)
```

