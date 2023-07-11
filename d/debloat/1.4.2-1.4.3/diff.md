# Comparing `tmp/debloat-1.4.2.tar.gz` & `tmp/debloat-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debloat-1.4.2.tar", last modified: Tue Jul  4 13:48:47 2023, max compression
+gzip compressed data, was "debloat-1.4.3.tar", last modified: Tue Jul 11 18:43:41 2023, max compression
```

## Comparing `debloat-1.4.2.tar` & `debloat-1.4.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-04 13:48:47.762762 debloat-1.4.2/
--rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.4.2/LICENSE
--rw-rw-rw-   0        0        0     7405 2023-07-04 13:48:47.763262 debloat-1.4.2/PKG-INFO
--rw-rw-rw-   0        0        0     6851 2023-04-19 22:52:19.000000 debloat-1.4.2/README.md
--rw-rw-rw-   0        0        0      788 2023-07-04 17:12:52.000000 debloat-1.4.2/pyproject.toml
--rw-rw-rw-   0        0        0      166 2023-07-04 13:48:47.768263 debloat-1.4.2/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.4.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:48:47.714769 debloat-1.4.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-04 13:48:47.729256 debloat-1.4.2/src/debloat/
--rw-rw-rw-   0        0        0        0 2023-05-09 12:13:11.000000 debloat-1.4.2/src/debloat/__init__.py
--rw-rw-rw-   0        0        0      510 2023-03-27 10:51:40.000000 debloat-1.4.2/src/debloat/auxiliary.py
--rw-rw-rw-   0        0        0     3976 2023-07-04 17:04:54.000000 debloat-1.4.2/src/debloat/gui.py
--rw-rw-rw-   0        0        0     1679 2023-07-04 16:34:52.000000 debloat-1.4.2/src/debloat/main.py
--rw-rw-rw-   0        0        0    24361 2023-07-04 16:54:25.000000 debloat-1.4.2/src/debloat/processor.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:48:47.758763 debloat-1.4.2/src/debloat/tests/
--rw-rw-rw-   0        0        0        0 2023-05-24 09:41:28.000000 debloat-1.4.2/src/debloat/tests/__init__.py
--rw-rw-rw-   0        0        0     1027 2023-05-25 09:39:42.000000 debloat-1.4.2/src/debloat/tests/debloat_test.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:48:47.761762 debloat-1.4.2/src/debloat/utilities/
--rw-rw-rw-   0        0        0        0 2023-07-04 17:05:39.000000 debloat-1.4.2/src/debloat/utilities/__init__.py
--rw-rw-rw-   0        0        0      746 2023-07-04 12:21:17.000000 debloat-1.4.2/src/debloat/utilities/rsrc.py
-drwxrwxrwx   0        0        0        0 2023-07-04 13:48:47.756260 debloat-1.4.2/src/debloat.egg-info/
--rw-rw-rw-   0        0        0     7405 2023-07-04 13:48:47.000000 debloat-1.4.2/src/debloat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-04 13:48:47.000000 debloat-1.4.2/src/debloat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-04 13:48:47.000000 debloat-1.4.2/src/debloat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-07-04 13:48:47.000000 debloat-1.4.2/src/debloat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-07-04 13:48:47.000000 debloat-1.4.2/src/debloat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-04 13:48:47.000000 debloat-1.4.2/src/debloat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 18:43:41.433530 debloat-1.4.3/
+-rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.4.3/LICENSE
+-rw-rw-rw-   0        0        0     7905 2023-07-11 18:43:41.433530 debloat-1.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7353 2023-07-11 18:34:10.000000 debloat-1.4.3/README.md
+-rw-rw-rw-   0        0        0      788 2023-07-11 18:34:56.000000 debloat-1.4.3/pyproject.toml
+-rw-rw-rw-   0        0        0      166 2023-07-11 18:43:41.439031 debloat-1.4.3/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:43:41.376021 debloat-1.4.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 18:43:41.397524 debloat-1.4.3/src/debloat/
+-rw-rw-rw-   0        0        0        0 2023-05-09 12:13:11.000000 debloat-1.4.3/src/debloat/__init__.py
+-rw-rw-rw-   0        0        0      510 2023-03-27 10:51:40.000000 debloat-1.4.3/src/debloat/auxiliary.py
+-rw-rw-rw-   0        0        0     3976 2023-07-11 18:34:35.000000 debloat-1.4.3/src/debloat/gui.py
+-rw-rw-rw-   0        0        0     1679 2023-07-11 18:34:35.000000 debloat-1.4.3/src/debloat/main.py
+-rw-rw-rw-   0        0        0    24894 2023-07-11 18:42:12.000000 debloat-1.4.3/src/debloat/processor.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:43:41.429030 debloat-1.4.3/src/debloat/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-24 09:41:28.000000 debloat-1.4.3/src/debloat/tests/__init__.py
+-rw-rw-rw-   0        0        0     1027 2023-07-11 18:34:35.000000 debloat-1.4.3/src/debloat/tests/debloat_test.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:43:41.432030 debloat-1.4.3/src/debloat/utilities/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:05:39.000000 debloat-1.4.3/src/debloat/utilities/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-07-11 18:18:14.000000 debloat-1.4.3/src/debloat/utilities/rsrc.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:43:41.426530 debloat-1.4.3/src/debloat.egg-info/
+-rw-rw-rw-   0        0        0     7905 2023-07-11 18:43:41.000000 debloat-1.4.3/src/debloat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-11 18:43:41.000000 debloat-1.4.3/src/debloat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 18:43:41.000000 debloat-1.4.3/src/debloat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-07-11 18:43:41.000000 debloat-1.4.3/src/debloat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-07-11 18:43:41.000000 debloat-1.4.3/src/debloat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-11 18:43:41.000000 debloat-1.4.3/src/debloat.egg-info/top_level.txt
```

### Comparing `debloat-1.4.2/LICENSE` & `debloat-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `debloat-1.4.2/PKG-INFO` & `debloat-1.4.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debloat
-Version: 1.4.2
+Version: 1.4.3
 Summary: Debloat is an tool to remove excess garbage from bloated executables.
 Author-email: Squiblydoo <Squiblydoo@pm.me>
 Project-URL: Homepage, https://github.com/Squiblydoo/debloat
 Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -42,15 +42,16 @@
 `debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
 
 The gui can also be launched from the CLI using the command `debloat-gui`.
 
 ## Does it always work?
 Not yet.
 My unscientific guess is that it should work for every 7 of 8 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
-In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "-unsafe" switch. If you ever need this switch, consider sharing the sample for additional analysis.
+
+In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch-effort" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
 
 ## Use Cases (Images from [Malcat](https://malcat.fr/))
 ### Full support
 - [x] Bloat appended to the end of a Signed PE.<br>
 In the image below, the bloat has been appended to the end of the executable. <br>
 ![Screenshot 2023-02-11 at 3 32 36 PM](https://user-images.githubusercontent.com/77356206/218279963-00780b59-8227-47dd-a0af-41096f6ae17b.png)
 
@@ -76,17 +77,18 @@
 ## Why?
 There appear to be a limited number of tools to easily process bloated executables. The two tools I have seen the most are “foremost” which is intended for recovering binaries from a disk image and “pecheck”.
 
 [Foremost](https://www.kali.org/tools/foremost/) works best in instances where the junk bytes are null (0x00) and it struggles when the binary has a fake or real signature. Its use in removing bloat from files is not its original purpose.
 
 [Pecheck](https://github.com/DidierStevens/DidierStevensSuite/blob/master/pecheck.py) has been developed over 14+ years and has some confusing commandline options. The option to remove bloated content is not the primary function of the script. Pecheck has to be combined with another tool ([disitool](https://blog.didierstevens.com/programs/disitool/)) in order to handle signed executables. In my experience, there are other times where pecheck can get confused and return an executable twice the size of the original bloated executable. All these factors seem OK if you are handling a small number of binaries, but as the number of binaries and methods increase, a tool specific to removing bloat is needed.
 
-There are good solid manual methods to remove bloat from binaries, but these methods can be tedious and not all analysts have the skills to do this. This tool removes the burden of needing to know how to manually remove bloat. Additionally, it allows for better scale. The principles used in the script allow allow for better scale if automation is desired.\*
+[Binary Refinery](https://github.com/binref/refinery) is an amazing tool. It was written with the intention of being a [CyberChef](https://github.com/gchq/CyberChef) of the commandline. While both tools are amazing, they both have a shortcoming that requires the user to know what formulas should be applied. 
+
+There are good solid manual methods to remove bloat from binaries, but these methods can be tedious and not all analysts have the skills to do this. This tool removes the burden of needing to know how to manually remove bloat. Additionally, it allows for better scale. The principles used in the script allow allow for better scale if automation is desired.
 
-\* Note: If automation is desired, I recommend re-writing these concepts in C/C++ and not Python.
 
 ## How to build? 
 Follow the build commands appropriate to your platform. The main difference between build commands is the format of the icon.
 <br>
 MacOS<br>
 `pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns gui.py`
```

### Comparing `debloat-1.4.2/README.md` & `debloat-1.4.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 `debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
 
 The gui can also be launched from the CLI using the command `debloat-gui`.
 
 ## Does it always work?
 Not yet.
 My unscientific guess is that it should work for every 7 of 8 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
-In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "-unsafe" switch. If you ever need this switch, consider sharing the sample for additional analysis.
+
+In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch-effort" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
 
 ## Use Cases (Images from [Malcat](https://malcat.fr/))
 ### Full support
 - [x] Bloat appended to the end of a Signed PE.<br>
 In the image below, the bloat has been appended to the end of the executable. <br>
 ![Screenshot 2023-02-11 at 3 32 36 PM](https://user-images.githubusercontent.com/77356206/218279963-00780b59-8227-47dd-a0af-41096f6ae17b.png)
 
@@ -62,17 +63,18 @@
 ## Why?
 There appear to be a limited number of tools to easily process bloated executables. The two tools I have seen the most are “foremost” which is intended for recovering binaries from a disk image and “pecheck”.
 
 [Foremost](https://www.kali.org/tools/foremost/) works best in instances where the junk bytes are null (0x00) and it struggles when the binary has a fake or real signature. Its use in removing bloat from files is not its original purpose.
 
 [Pecheck](https://github.com/DidierStevens/DidierStevensSuite/blob/master/pecheck.py) has been developed over 14+ years and has some confusing commandline options. The option to remove bloated content is not the primary function of the script. Pecheck has to be combined with another tool ([disitool](https://blog.didierstevens.com/programs/disitool/)) in order to handle signed executables. In my experience, there are other times where pecheck can get confused and return an executable twice the size of the original bloated executable. All these factors seem OK if you are handling a small number of binaries, but as the number of binaries and methods increase, a tool specific to removing bloat is needed.
 
-There are good solid manual methods to remove bloat from binaries, but these methods can be tedious and not all analysts have the skills to do this. This tool removes the burden of needing to know how to manually remove bloat. Additionally, it allows for better scale. The principles used in the script allow allow for better scale if automation is desired.\*
+[Binary Refinery](https://github.com/binref/refinery) is an amazing tool. It was written with the intention of being a [CyberChef](https://github.com/gchq/CyberChef) of the commandline. While both tools are amazing, they both have a shortcoming that requires the user to know what formulas should be applied. 
+
+There are good solid manual methods to remove bloat from binaries, but these methods can be tedious and not all analysts have the skills to do this. This tool removes the burden of needing to know how to manually remove bloat. Additionally, it allows for better scale. The principles used in the script allow allow for better scale if automation is desired.
 
-\* Note: If automation is desired, I recommend re-writing these concepts in C/C++ and not Python.
 
 ## How to build? 
 Follow the build commands appropriate to your platform. The main difference between build commands is the format of the icon.
 <br>
 MacOS<br>
 `pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns gui.py`
 
@@ -84,8 +86,8 @@
 - I'm not sure why the same hook didn't work on Linux and pointing to the site-packages directory is not preferred. For some unknown reason, it would not find the binary if I pointed to the specific tkinterdnd2 or tkdnd directories.
 
 ## Where is this project going next?
 Batch processing: process all files in a directory and produce a report.
 
 Better support for using processing methods outside of debloat.
 
-Support for debloating without unzipping.
+Support for debloating without unzipping.
```

### Comparing `debloat-1.4.2/pyproject.toml` & `debloat-1.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "debloat"
-version = "1.4.2"
+version = "1.4.3"
 authors = [
   { name="Squiblydoo", email="Squiblydoo@pm.me" },
 ]
 description = "Debloat is an tool to remove excess garbage from bloated executables."
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
```

### Comparing `debloat-1.4.2/src/debloat/gui.py` & `debloat-1.4.3/src/debloat/gui.py`

 * *Files identical despite different names*

### Comparing `debloat-1.4.2/src/debloat/main.py` & `debloat-1.4.3/src/debloat/main.py`

 * *Files identical despite different names*

### Comparing `debloat-1.4.2/src/debloat/processor.py` & `debloat-1.4.3/src/debloat/processor.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,533 +1,533 @@
-"""
-This file handles the processing of binaries and helper methods.
-
-Three methods are from https://github.com/binref/refinery 
-Copyright 2019 Jesko Hüttenhain used under the 3-Clause BSD License 
-The methods are:
-refinery_strip()
-adjust_offsets()
-refinery_trim_resources()
-The RSRC Class is also from refinery.
-"""
-import re
-from typing import Tuple, Optional, Any, Callable
-import pefile
-import binascii
-import zlib
-from pefile import Structure, SectionStructure, DIRECTORY_ENTRY
-from typing import Generator, Iterable, Optional
-
-import debloat.utilities.rsrc as rsrc
-
-_KB = 1000
-_MB = _KB * _KB
-
-PACKER = {
-    1 : "Nullsoft"
-}
-
-def readable_size(value: int) -> str:
-    '''Return bytes in human readable format.'''
-    if value <= 1024:
-        return '%s bytes' % value
-    elif value < 1024 * 1024:
-        return '%.1f KB' % (float(value) / 1024.0)
-    elif value < 1024 * 1024 * 1024:
-        return '%.1f MB' % (float(value) / 1024.0 / 1024.0)
-    else:
-        return '%.1f GB' % (float(value) / 1024.0 / 1024.0 / 1024.0)
-
-def write_patched_file(out_path: str,
-                        pe: pefile.PE, 
-                        end_of_real_data: int) -> Tuple[int, str]:
-    '''Writes the patched file to disk.
-    
-    Keyword Arguments:
-    out_path -- the path and file name to write
-    pe -- the pefile that is being processed
-    end_of_real_data -- an int indicating the size of bytes to write'''
-    with open(out_path, 'wb') as writer:
-        writer.write(pe.write())
-        final_filesize = len(pe.write())
-        return final_filesize, out_path
-
-def handle_signature_abnormality(signature_address: int,
-                                signature_size: int, 
-                                beginning_file_size: int) -> bool:
-    '''Remove all bytes after a PE signature'''
-    # If the signature_address is 0, there was no original signature.
-    # We are setting the signature address to the filesize in order to
-    # skip the next check.
-    if signature_address == 0:
-        signature_address = beginning_file_size
-    # Check to see if there is data after the signature; if so, it is
-    #  junk data
-    if beginning_file_size > (signature_address + signature_size):
-        return True
-    return False
-
-def check_for_packer(pe: pefile.PE) -> int:
-    '''Check overlay bytes for known packers.'''
-    packer_header = pe.write()[pe.get_overlay_data_start_offset():pe.get_overlay_data_start_offset() + 30]
-    # TODO: Evalute any other packers that need special processing.
-
-    # NullSoft is not a packer, but an installer. We will detect this. It cannot be processed at this time
-    NULLSOFT_MAGICS = [
-        # https://nsis.sourceforge.io/Can_I_decompile_an_existing_installer
-        B'\xEF\xBE\xAD\xDE' B'Null' B'soft' B'Inst',   # v1.6
-        B'\xEF\xBE\xAD\xDE' B'Null' B'Soft' B'Inst',   # v1.3
-        B'\xED\xBE\xAD\xDE' B'Null' B'Soft' B'Inst',   # v1.1
-        B'\xEF\xBE\xAD\xDE' B'nsis' B'inst' B'all\0',  # v1.0
-    ]
-
-    for magic in range(len(NULLSOFT_MAGICS)):
-        packer_header_match = re.search(NULLSOFT_MAGICS[magic], packer_header)
-        if packer_header_match:
-             # Future: Handle NSIS installers
-            return 1 # Nullsoft
-    return 0
-
-def find_last_section(pe: pefile.PE) -> Optional[pefile.SectionStructure]:
-    '''Iterate through PE sections to identify the last one.'''
-    last_section = None
-    for section in pe.sections:
-        if last_section is None \
-                        or section.PointerToRawData > last_section.PointerToRawData:
-            last_section = section
-    return last_section
-
-def get_signature_info(pe: pefile.PE) -> Tuple[int, int]:
-    '''Remove PE signature and update header.''' 
-    signature_address = pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].VirtualAddress
-    signature_size = pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].Size
-    pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].VirtualAddress = 0
-    pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].Size = 0
-    
-    return signature_address, signature_size
-
-
-def adjust_offsets(pe: pefile.PE, gap_offset: int, gap_size: int):
-    base = pe.OPTIONAL_HEADER.ImageBase
-    alignment = pe.OPTIONAL_HEADER.FileAlignment
-    rva_offset = pe.get_rva_from_offset(gap_offset)
-    tva_offset = rva_offset + base
-
-    section = pe.get_section_by_offset(gap_offset)
-    new_section_size = section.SizeOfRawData - gap_size
-    if new_section_size % alignment != 0:
-        raise RuntimeError(
-            F'trimming 0x{gap_size:X} bytes from section {(section.Name)} of size 0x{section.SizeOfRawData:X} '
-            F'violates required section alignment of 0x{alignment:X} bytes')
-    inside_section_offset = gap_offset - section.PointerToRawData
-    if inside_section_offset > new_section_size:
-        overlap = inside_section_offset - new_section_size
-        raise RuntimeError(F'trimming from section {(section.Name)}; data extends {overlap} beyond section')
-
-    rva_lbound = section.VirtualAddress
-    rva_ubound = section.VirtualAddress + section.Misc_VirtualSize - 1
-    tva_lbound = rva_lbound + base
-    tva_ubound = rva_ubound + base
-
-    def adjust_attributes_of_structure(
-        structure: Structure,
-        threshold: int,
-        lbound: Optional[int],
-        ubound: Optional[int],
-        attributes: Iterable[str]
-    ):
-        for attribute in attributes:
-            old_value = getattr(structure, attribute, 0)
-            if old_value <= threshold:
-                continue
-            if lbound is not None and old_value < lbound:
-                continue
-            if ubound is not None and old_value > ubound:
-                continue
-            new_value = old_value - gap_size
-            if new_value < 0:
-                raise RuntimeError(F'adjusting attribute {attribute} of {structure.name} would result in negative value: {new_value}')
-            setattr(structure, attribute, new_value)
-
-    it: Iterable[Structure] = iter(pe.__structures__)
-
-    for structure in it:
-        old_offset = structure.get_file_offset()
-        new_offset = old_offset - gap_offset
-
-        if old_offset > gap_offset:
-            if isinstance(structure, SectionStructure) and new_offset % alignment != 0:
-                raise RuntimeError(
-                    F'section {(structure.Name)} would be moved to offset 0x{new_offset:X}, '
-                    F'violating section alignment value 0x{alignment:X}.')
-            if old_offset < gap_offset + gap_size:
-                raise RuntimeError(
-                    F'structure starts inside removed region: {structure}')
-            structure.set_file_offset(new_offset)
-
-        adjust_attributes_of_structure(structure, rva_offset, rva_lbound, rva_ubound, (
-            'OffsetToData',
-            'AddressOfData',
-            'VirtualAddress',
-            'AddressOfNames',
-            'AddressOfNameOrdinals',
-            'AddressOfFunctions',
-            'AddressOfEntryPoint',
-            'AddressOfRawData',
-            'BaseOfCode',
-            'BaseOfData',
-        ))
-        adjust_attributes_of_structure(structure, tva_offset, tva_lbound, tva_ubound, (
-            'StartAddressOfRawData',
-            'EndAddressOfRawData',
-            'AddressOfIndex',
-            'AddressOfCallBacks',
-        ))
-        adjust_attributes_of_structure(structure, gap_offset, None, None, (
-            'OffsetModuleName',
-            'PointerToRawData',
-        ))
-        
-        for attribute in (
-            'CvHeaderOffset',
-            'OffsetIn2Qwords',
-            'OffsetInQwords',
-            'Offset',
-            'OffsetLow',
-            'OffsetHigh'
-        ):
-            if not hasattr(structure, attribute):
-                continue
-
-    section.SizeOfRawData = new_section_size
-    return pe
-    
-
-def refinery_strip(pe: pefile.PE, data: memoryview, block_size=_MB) -> int:
-    threshold = 1
-    alignment = pe.OPTIONAL_HEADER.FileAlignment
-    data_overhang = len(data) % alignment
-    result = data_overhang
-
-    if not data:
-        return 0
-    
-    if 0 < threshold < 1:
-        def compression_ratio(offset: int):
-            ratio = len(zlib.compress(data[:offset], level=1))
-            return ratio
-        upper = len(data)
-        lower = result
-        if compression_ratio(upper) <= threshold:
-            while block_size < upper - lower:
-                pivot = (lower + upper) // 2
-                ratio = compression_ratio(pivot)
-                if ratio > threshold:
-                    lower = pivot + 1
-                    continue
-                upper = pivot
-                if abs(ratio - threshold) < 1e-10:
-                    break
-        result = upper
-
-    match = re.search(B'(?s).(?=\\x%02x+$)' % data[result - 1], data[:result])
-    if match is not None:
-        cutoff = match.start() - 1
-        length = result - cutoff
-        if length > block_size:
-            result = cutoff
-
-    result = max(result, data_overhang)
-
-    result = result + (data_overhang - result) % alignment
-
-    while result > len(data):
-        result -= alignment
-
-    return result
-
-
-def refinery_trim_resources(pe: pefile.PE, pe_data: bytearray) -> int:
-    size_limit = 50000
-    size_removed = 0
-
-    def find_bloated_resources(pe: pefile.PE, directory, level: int = 0, *path) -> Generator[Structure, None, None]:
-        for entry in directory.entries:
-            name = getattr(entry, 'name')
-            numeric_id = getattr(entry, 'id')
-            if not name:
-                if level == 0 and numeric_id in iter(rsrc.RSRC):
-                    name = rsrc.RSRC(entry.id)
-                elif numeric_id is not None:
-                    name = str(numeric_id)
-            name = name and str(name) or '?'
-            if entry.struct.DataIsDirectory:
-                yield from find_bloated_resources(pe, entry.directory, level + 1, *path, name)
-                continue
-            struct: Structure = entry.data.struct
-            name = '/'.join((*path, name))
-            if struct.Size <= size_limit:
-                continue
-            yield name, struct
-    
-    RSRC_INDEX = DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_RESOURCE']
-    pe.parse_data_directories(directories=[RSRC_INDEX])
-
-    try:
-        resources = pe.DIRECTORY_ENTRY_RESOURCE
-    except AttributeError:
-        return 0
-    for name, resource in find_bloated_resources(pe, resources):
-        offset = pe.get_offset_from_rva(resource.OffsetToData)
-        old_size = resource.Size
-        new_size = refinery_strip(pe, memoryview(pe_data)[offset:offset + old_size])
-        gap_size = old_size - new_size
-        gap_offset = offset + new_size
-        if gap_size <= 0:
-            continue
-        resource.Size = new_size
-        adjust_offsets(pe, gap_offset, gap_size)
-        size_removed += gap_size
-        pe_data[gap_offset:gap_offset + gap_size] = []
-
-    pe.OPTIONAL_HEADER.DATA_DIRECTORY[RSRC_INDEX].Size -= size_removed
-    return size_removed
-        
-    
-
-def remove_resources(pe: pefile.PE, pe_data: bytearray) -> Tuple[bytearray, int]:
-    trimmed = refinery_trim_resources(pe, pe_data)
-    return trimmed
-
-def check_section_compression(pe: pefile.PE, pe_data: bytearray, end_of_real_data, 
-                          log_message: Callable[[str], None]) -> Tuple[pefile.PE, int, str]:
-        biggest_section = None
-        biggest_uncompressed = int
-        result = ""
-        for section in pe.sections:
-            section_name = section.Name.decode()
-            compressed_section_size = len(zlib.compress(
-                pe.write()[section.PointerToRawData: 
-                           (section.PointerToRawData + section.SizeOfRawData)]))
-            uncompressed_section_size = section.SizeOfRawData
-            section_compression_ratio = uncompressed_section_size / compressed_section_size * 100
-            log_message("Section: "  + section_name, end="\t", flush=True)
-            log_message(" Compression Ratio: " + str(round(section_compression_ratio, 2)) +"%", end="\t",flush=True) 
-            log_message("Size of section: " + readable_size(section.SizeOfRawData) +".",flush=True)
-            if biggest_section == None:
-                biggest_section = section
-                biggest_uncompressed = section_compression_ratio
-            elif section.SizeOfRawData > biggest_section.SizeOfRawData:
-                biggest_section = section
-                biggest_uncompressed = section_compression_ratio
-        # Handle specific bloated sections
-        if biggest_section.Name.decode() == ".rsrc\x00\x00\x00":
-            # Get biggest resource or resources and drop them from the 
-            # Resource table
-            # TODO: recalculate PE header in situations where the 
-            # resource is not at the end of an executable.
-            # TODO: Handle other tomfoolery required when resource 
-            # is not at end of executable.
-            log_message('''
-Bloat was located in the resource section. Removing bloat.. 
-''')
-            
-            bytes_removed = remove_resources(pe, pe_data)
-            end_of_real_data =- bytes_removed
-            return end_of_real_data, result
-        elif biggest_section.Name.decode() == ".text\x00\x00\x00":
-            # Data stored in the .text section is often a .NET Resource. The following checks
-            # to confirm it is .NET and then drops the resources.
-            if pe.OPTIONAL_HEADER.DATA_DIRECTORY[14].Size:
-                log_message('''
-Bloat was detected in the text section. Bloat is likely in a .NET Resource 
-This use case cannot be processed at this time. ''')
-            return end_of_real_data, result
-                
-        # The use cases covered by this section are at the end of 
-        # the binary. In my experience, the bloated sections are 
-        # usually at the end unless they are bloat from .NET Resources.
-        if biggest_uncompressed > 3000:
-            log_message('''
-The compression ratio is indicative of a bloated section.
-''', end="", flush=True)
-            # Get the size of the section.
-            section_end = section.PointerToRawData + section.SizeOfRawData
-            original_section_size = section.SizeOfRawData
-            section_data = pe_data[section.PointerToRawData:section_end]
-            delta_last_non_junk = trim_junk(section_data, original_section_size)
-            pe_data[section.PointerToRawData + delta_last_non_junk:section_end] = []
-            section_bytes_to_remove = original_section_size - delta_last_non_junk
-            end_of_real_data =  end_of_real_data - section_bytes_to_remove
-            # This will update the last section header, SizeOfRawData, SizeOfImage.
-            pe.sections[pe.sections.index(biggest_section)].section_max_addr -= section_bytes_to_remove
-            pe.sections[pe.sections.index(biggest_section)].SizeOfRawData -= section_bytes_to_remove
-            #pe.sections[pe.sections.index(biggest_section)].Misc_VirtualSize -= section_bytes_to_remove
-            #pe.OPTIONAL_HEADER.SizeOfImage -= section_bytes_to_remove
-            log_message("Bloated section reduced.")
-            return end_of_real_data, result
-            
-       
-        
-def trim_junk(bloated_content: bytes, original_size_with_junk: int) -> int:
-    ''' Attempt multiple methods or removing junk from overlay.'''
-    backward_bloated_content = bloated_content[::-1]
-    # Regex Explained:
-    # Match raw bytes that are repeated more than 20 times at the end
-    # of a binary. 
-    delta_last_non_junk = original_size_with_junk
-    # First Method: Trims 1 repeating byte.
-    # Check against 200 bytes, if successful, calculate full match.
-    junk_match = re.search(rb'^(..)\1{20,}', backward_bloated_content[:600])
-    # Second Method: If "not junk_match" check for junk larger than 1 repeating byte
-    chunk_start = 0
-    if not junk_match:
-        # Brute force check: check to see if there are 1-20 bytes
-        # being repeated and feed the number into the regex
-        for i in range(300):
-            # Regex Explained:
-            # Starting at the end of the PE, check for repeated bytes.
-            # This indicates junk bytes in the overlay. Match that set
-            # of repeated bytes 1 or more times. 
-            junk_regex = rb"^(..{" + bytes(str(i), "utf-8") + rb"})\1{2,}"
-            multibyte_junk_regex = re.search(junk_regex, backward_bloated_content[:1000])
-            if multibyte_junk_regex:
-                # Having found the pattern, we can make the regex efficient
-                # by targeting the pattern using the "targeted_regex"
-                targeted_regex = rb"(" + binascii.hexlify(multibyte_junk_regex.group(1)) + rb")\1{1,}"
-                chunk_end = chunk_start
-                while original_size_with_junk > chunk_end:
-                    chunk_end = chunk_start + 1000
-                    targeted_multibyte_junk_regex = re.search(targeted_regex, 
-                                                              binascii.hexlify(backward_bloated_content[chunk_start:chunk_end]))
-                    if targeted_multibyte_junk_regex:
-                        chunk_start += targeted_multibyte_junk_regex.end(0)
-                        unmatched_portion = 1000 - targeted_multibyte_junk_regex.end(0)
-                    else:
-                        # If the targeted_multibyte_junk_regex does not
-                        # return anything, that indicates the previous loop
-                        # had content which did not match. We'll use that
-                        # to help ensure we do not remove too much of the file. 
-                        chunk_start += unmatched_portion 
-                        break
-                break
-                # It was determined that data cannot be removed any more
-                # from the chunk_start. But the value of chunk_start
-                # now tells us how much data we can safely remove.
-        junk_to_remove = chunk_start  
-        #junk_to_remove = int(junk_to_remove)
-        delta_last_non_junk -= junk_to_remove
-    # Third Method: check for a series of one repeated byte. 
-    # Junk was identified. A new size is assigned and returned.
-    else:
-        targeted_regex = rb""+ binascii.hexlify(junk_match.string) + rb"{1,}"
-        targeted_junk_match = re.search(targeted_regex, binascii.hexlify(backward_bloated_content))
-        junk_to_remove = targeted_junk_match.end(0)
-        # If the trimming did not remove more than half of the bytes then
-        # this suggests the attacker may have put a random series of
-        # repeated bytes. These will be removed by loading the overlay
-        # 200 bytes at a time and removing parts which repeat for more
-        # than 20 bytes.
-        if junk_to_remove < original_size_with_junk / 2:
-            chunk_start = targeted_junk_match.end(0)
-            chunk_end = chunk_start
-            while original_size_with_junk > chunk_end:
-                chunk_end = chunk_start + 200
-                repeated_junk_match = re.search(rb'(..)\1{20,}', 
-                                                binascii.hexlify(backward_bloated_content[chunk_start:chunk_end]))
-                if repeated_junk_match:
-                    chunk_start += repeated_junk_match.end(0)
-                    unmatched_portion = 200 - repeated_junk_match.end(0)
-                else:
-                    chunk_start += unmatched_portion
-                    break
-            junk_to_remove = chunk_start 
-        else:
-            junk_to_remove = int(junk_to_remove / 2)
-        delta_last_non_junk -= junk_to_remove
-    return delta_last_non_junk  
-
-def process_pe(pe: pefile.PE, out_path: str, unsafe_processing: bool,
-               log_message: Callable[[str], None]) -> None:
-    '''Prepare PE, perform checks, remote junk, write patched binary.'''
-    beginning_file_size = len(pe.write())
-    # We are using the variable "end_of_real_data" and are reassigning 
-    # the value based on our analysis.We are assigning it now in case 
-    # we are unable to reduce the binary size for any reason.
-    end_of_real_data = beginning_file_size
-    pe_data = bytearray(pe.__data__)
-    # Remove Signature and modify size of Optional Header Security entry.
-    signature_address, signature_size = get_signature_info(pe)
-    pe_data[signature_address:signature_address + signature_size] = []
-    signature_abnormality = handle_signature_abnormality(signature_address, 
-                                                        signature_size, 
-                                                        beginning_file_size)
-    if signature_abnormality:
-        log_message('''
-We detected data after the signature. This is abnormal. Removing signature and extra data...''')
-        end_of_real_data = signature_address
-        pe_data = pe_data[:end_of_real_data]
-    # Handle Overlays: this includes packers and overlays which are completely junk
-    elif pe.get_overlay_data_start_offset() and signature_size < len(pe.get_overlay()):
-        log_message("An overlay was detected. Checking for known packer.")
-        packer_idenfitied = check_for_packer(pe)
-        if packer_idenfitied:
-            log_message("Packer identified: " + PACKER[packer_idenfitied])
-            if PACKER[1]:
-                log_message('''
-The original file cannot be debloated. It must be unpacked with a tool such as UniExtract2.
-                ''')
-        else:
-            log_message("Packer not identified. Attempting dynamic trim...")
-            last_section = find_last_section(pe)
-            overlay = pe_data[last_section.PointerToRawData + last_section.SizeOfRawData:]
-            end_of_real_data = trim_junk(overlay, end_of_real_data)
-            pe_data = pe_data[:end_of_real_data]
-            if end_of_real_data == beginning_file_size:
-                if unsafe_processing is True:
-                    log_message("""
-"Unsafe" switch detected. Running unsafe debloat technique:\n
-This is the last resort of removing the whole overlay: this works in some 
-cases, but can remove critical content. 
-If file is a Nullsoft executable, but was not detected, the original file can 
-be unpacked with the tool "UniExtract2".
-                    """)
-                    last_section = find_last_section(pe)
-                    end_of_real_data = last_section.PointerToRawData + last_section.SizeOfRawData
-                    pe_data = pe_data[:end_of_real_data] 
-                else:
-                    log_message("""
-Overlay was unable to be trimmed. Try unpacking with UniExtract2 or re-running 
-Debloat with the "--unsafe" parameter."""
-                                )
-    # Handle bloated sections
-    # TODO: break up into functions
-    else:
-        # In order to solve some use cases, we will find the biggest section 
-        # within the binary.
-        end_of_real_data, result = check_section_compression(pe, pe_data,
-                                                             end_of_real_data, 
-                                                             log_message=log_message)
-        log_message(result)
-    # All processing is done. Report results.
-    if end_of_real_data == beginning_file_size:
-        log_message("""No automated method for reducing the size worked. Please consider sharing the
-sample for additional analysis.
-Email: Squiblydoo@pm.me
-Twitter: @SquiblydooBlog.
-                    """)
-    else:
-        pe.__data__ =pe_data
-        final_filesize, new_pe_name = write_patched_file(out_path,
-                                                         pe, 
-                                                         end_of_real_data)
-        reduction_calculation = round(((beginning_file_size \
-                                        - final_filesize) \
-                                        / beginning_file_size) * 100, 2)
-        log_message("Beginning File size: " \
-                + readable_size(beginning_file_size) + ".")
-        log_message("File was reduced by " \
-                    + str(reduction_calculation) + "%.")
-        log_message("Final file size: " \
-                    + readable_size(final_filesize) + ".")
-        log_message("Processing complete.\nFile written to '" \
-                    + str(new_pe_name) + "'.")
+"""
+This file handles the processing of binaries and helper methods.
+
+Three methods are from https://github.com/binref/refinery 
+Copyright 2019 Jesko Hüttenhain used under the 3-Clause BSD License 
+The methods are:
+refinery_strip()
+adjust_offsets()
+refinery_trim_resources()
+The RSRC Class is also from refinery.
+"""
+import re
+from typing import Tuple, Optional, Any, Callable
+import pefile
+import binascii
+import zlib
+from pefile import Structure, SectionStructure, DIRECTORY_ENTRY
+from typing import Generator, Iterable, Optional
+
+import debloat.utilities.rsrc as rsrc
+
+_KB = 1000
+_MB = _KB * _KB
+
+PACKER = {
+    1 : "Nullsoft"
+}
+
+def readable_size(value: int) -> str:
+    '''Return bytes in human readable format.'''
+    if value <= 1024:
+        return '%s bytes' % value
+    elif value < 1024 * 1024:
+        return '%.1f KB' % (float(value) / 1024.0)
+    elif value < 1024 * 1024 * 1024:
+        return '%.1f MB' % (float(value) / 1024.0 / 1024.0)
+    else:
+        return '%.1f GB' % (float(value) / 1024.0 / 1024.0 / 1024.0)
+
+def write_patched_file(out_path: str,
+                        pe: pefile.PE, 
+                        end_of_real_data: int) -> Tuple[int, str]:
+    '''Writes the patched file to disk.
+    
+    Keyword Arguments:
+    out_path -- the path and file name to write
+    pe -- the pefile that is being processed
+    end_of_real_data -- an int indicating the size of bytes to write'''
+    with open(out_path, 'wb') as writer:
+        writer.write(pe.write())
+        final_filesize = len(pe.write())
+        return final_filesize, out_path
+
+def handle_signature_abnormality(signature_address: int,
+                                signature_size: int, 
+                                beginning_file_size: int) -> bool:
+    '''Remove all bytes after a PE signature'''
+    # If the signature_address is 0, there was no original signature.
+    # We are setting the signature address to the filesize in order to
+    # skip the next check.
+    if signature_address == 0:
+        signature_address = beginning_file_size
+    # Check to see if there is data after the signature; if so, it is
+    #  junk data
+    if beginning_file_size > (signature_address + signature_size):
+        return True
+    return False
+
+def check_for_packer(pe: pefile.PE) -> int:
+    '''Check overlay bytes for known packers.'''
+    packer_header = pe.write()[pe.get_overlay_data_start_offset():pe.get_overlay_data_start_offset() + 30]
+    # TODO: Evalute any other packers that need special processing.
+
+    # NullSoft is not a packer, but an installer. We will detect this. It cannot be processed at this time
+    NULLSOFT_MAGICS = [
+        # https://nsis.sourceforge.io/Can_I_decompile_an_existing_installer
+        B'\xEF\xBE\xAD\xDE' B'Null' B'soft' B'Inst',   # v1.6
+        B'\xEF\xBE\xAD\xDE' B'Null' B'Soft' B'Inst',   # v1.3
+        B'\xED\xBE\xAD\xDE' B'Null' B'Soft' B'Inst',   # v1.1
+        B'\xEF\xBE\xAD\xDE' B'nsis' B'inst' B'all\0',  # v1.0
+    ]
+
+    for magic in range(len(NULLSOFT_MAGICS)):
+        packer_header_match = re.search(NULLSOFT_MAGICS[magic], packer_header)
+        if packer_header_match:
+             # Future: Handle NSIS installers
+            return 1 # Nullsoft
+    return 0
+
+def find_last_section(pe: pefile.PE) -> Optional[pefile.SectionStructure]:
+    '''Iterate through PE sections to identify the last one.'''
+    last_section = None
+    for section in pe.sections:
+        if last_section is None \
+                        or section.PointerToRawData > last_section.PointerToRawData:
+            last_section = section
+    return last_section
+
+def get_signature_info(pe: pefile.PE) -> Tuple[int, int]:
+    '''Remove PE signature and update header.''' 
+    signature_address = pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].VirtualAddress
+    signature_size = pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].Size
+    pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].VirtualAddress = 0
+    pe.OPTIONAL_HEADER.DATA_DIRECTORY[pefile.DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_SECURITY']].Size = 0
+    
+    return signature_address, signature_size
+
+
+def adjust_offsets(pe: pefile.PE, gap_offset: int, gap_size: int):
+    base = pe.OPTIONAL_HEADER.ImageBase
+    alignment = pe.OPTIONAL_HEADER.FileAlignment
+    rva_offset = pe.get_rva_from_offset(gap_offset)
+    tva_offset = rva_offset + base
+
+    section = pe.get_section_by_offset(gap_offset)
+    new_section_size = section.SizeOfRawData - gap_size
+    if new_section_size % alignment != 0:
+        raise RuntimeError(
+            F'trimming 0x{gap_size:X} bytes from section {(section.Name)} of size 0x{section.SizeOfRawData:X} '
+            F'violates required section alignment of 0x{alignment:X} bytes')
+    inside_section_offset = gap_offset - section.PointerToRawData
+    if inside_section_offset > new_section_size:
+        overlap = inside_section_offset - new_section_size
+        raise RuntimeError(F'trimming from section {(section.Name)}; data extends {overlap} beyond section')
+
+    rva_lbound = section.VirtualAddress
+    rva_ubound = section.VirtualAddress + section.Misc_VirtualSize - 1
+    tva_lbound = rva_lbound + base
+    tva_ubound = rva_ubound + base
+
+    def adjust_attributes_of_structure(
+        structure: Structure,
+        threshold: int,
+        lbound: Optional[int],
+        ubound: Optional[int],
+        attributes: Iterable[str]
+    ):
+        for attribute in attributes:
+            old_value = getattr(structure, attribute, 0)
+            if old_value <= threshold:
+                continue
+            if lbound is not None and old_value < lbound:
+                continue
+            if ubound is not None and old_value > ubound:
+                continue
+            new_value = old_value - gap_size
+            if new_value < 0:
+                raise RuntimeError(F'adjusting attribute {attribute} of {structure.name} would result in negative value: {new_value}')
+            setattr(structure, attribute, new_value)
+
+    it: Iterable[Structure] = iter(pe.__structures__)
+
+    for structure in it:
+        old_offset = structure.get_file_offset()
+        new_offset = old_offset - gap_offset
+
+        if old_offset > gap_offset:
+            if isinstance(structure, SectionStructure) and new_offset % alignment != 0:
+                raise RuntimeError(
+                    F'section {(structure.Name)} would be moved to offset 0x{new_offset:X}, '
+                    F'violating section alignment value 0x{alignment:X}.')
+            if old_offset < gap_offset + gap_size:
+                raise RuntimeError(
+                    F'structure starts inside removed region: {structure}')
+            structure.set_file_offset(new_offset)
+
+        adjust_attributes_of_structure(structure, rva_offset, rva_lbound, rva_ubound, (
+            'OffsetToData',
+            'AddressOfData',
+            'VirtualAddress',
+            'AddressOfNames',
+            'AddressOfNameOrdinals',
+            'AddressOfFunctions',
+            'AddressOfEntryPoint',
+            'AddressOfRawData',
+            'BaseOfCode',
+            'BaseOfData',
+        ))
+        adjust_attributes_of_structure(structure, tva_offset, tva_lbound, tva_ubound, (
+            'StartAddressOfRawData',
+            'EndAddressOfRawData',
+            'AddressOfIndex',
+            'AddressOfCallBacks',
+        ))
+        adjust_attributes_of_structure(structure, gap_offset, None, None, (
+            'OffsetModuleName',
+            'PointerToRawData',
+        ))
+        
+        for attribute in (
+            'CvHeaderOffset',
+            'OffsetIn2Qwords',
+            'OffsetInQwords',
+            'Offset',
+            'OffsetLow',
+            'OffsetHigh'
+        ):
+            if not hasattr(structure, attribute):
+                continue
+
+    section.SizeOfRawData = new_section_size
+    return pe
+    
+
+def refinery_strip(pe: pefile.PE, data: memoryview, block_size=_MB) -> int:
+    threshold = 1
+    alignment = pe.OPTIONAL_HEADER.FileAlignment
+    data_overhang = len(data) % alignment
+    result = data_overhang
+
+    if not data:
+        return 0
+    
+    if 0 < threshold < 1:
+        def compression_ratio(offset: int):
+            ratio = len(zlib.compress(data[:offset], level=1))
+            return ratio
+        upper = len(data)
+        lower = result
+        if compression_ratio(upper) <= threshold:
+            while block_size < upper - lower:
+                pivot = (lower + upper) // 2
+                ratio = compression_ratio(pivot)
+                if ratio > threshold:
+                    lower = pivot + 1
+                    continue
+                upper = pivot
+                if abs(ratio - threshold) < 1e-10:
+                    break
+        result = upper
+
+    match = re.search(B'(?s).(?=\\x%02x+$)' % data[result - 1], data[:result])
+    if match is not None:
+        cutoff = match.start() - 1
+        length = result - cutoff
+        if length > block_size:
+            result = cutoff
+
+    result = max(result, data_overhang)
+
+    result = result + (data_overhang - result) % alignment
+
+    while result > len(data):
+        result -= alignment
+
+    return result
+
+
+def refinery_trim_resources(pe: pefile.PE, pe_data: bytearray) -> int:
+    size_limit = 50000
+    size_removed = 0
+
+    def find_bloated_resources(pe: pefile.PE, directory, level: int = 0, *path) -> Generator[Structure, None, None]:
+        for entry in directory.entries:
+            name = getattr(entry, 'name')
+            numeric_id = getattr(entry, 'id')
+            if not name:
+                if level == 0 and numeric_id in iter(rsrc.RSRC):
+                    name = rsrc.RSRC(entry.id)
+                elif numeric_id is not None:
+                    name = str(numeric_id)
+            name = name and str(name) or '?'
+            if entry.struct.DataIsDirectory:
+                yield from find_bloated_resources(pe, entry.directory, level + 1, *path, name)
+                continue
+            struct: Structure = entry.data.struct
+            name = '/'.join((*path, name))
+            if struct.Size <= size_limit:
+                continue
+            yield name, struct
+    
+    RSRC_INDEX = DIRECTORY_ENTRY['IMAGE_DIRECTORY_ENTRY_RESOURCE']
+    pe.parse_data_directories(directories=[RSRC_INDEX])
+
+    try:
+        resources = pe.DIRECTORY_ENTRY_RESOURCE
+    except AttributeError:
+        return 0
+    for name, resource in find_bloated_resources(pe, resources):
+        offset = pe.get_offset_from_rva(resource.OffsetToData)
+        old_size = resource.Size
+        new_size = refinery_strip(pe, memoryview(pe_data)[offset:offset + old_size])
+        gap_size = old_size - new_size
+        gap_offset = offset + new_size
+        if gap_size <= 0:
+            continue
+        resource.Size = new_size
+        adjust_offsets(pe, gap_offset, gap_size)
+        size_removed += gap_size
+        pe_data[gap_offset:gap_offset + gap_size] = []
+
+    pe.OPTIONAL_HEADER.DATA_DIRECTORY[RSRC_INDEX].Size -= size_removed
+    return size_removed
+        
+    
+
+def remove_resources(pe: pefile.PE, pe_data: bytearray) -> Tuple[bytearray, int]:
+    trimmed = refinery_trim_resources(pe, pe_data)
+    return trimmed
+
+def check_section_compression(pe: pefile.PE, pe_data: bytearray, end_of_real_data, 
+                          log_message: Callable[[str], None]) -> Tuple[pefile.PE, int, str]:
+        biggest_section = None
+        biggest_uncompressed = int
+        result = ""
+        for section in pe.sections:
+            section_name = section.Name.decode()
+            compressed_section_size = len(zlib.compress(
+                pe.write()[section.PointerToRawData: 
+                           (section.PointerToRawData + section.SizeOfRawData)]))
+            uncompressed_section_size = section.SizeOfRawData
+            section_compression_ratio = uncompressed_section_size / compressed_section_size * 100
+            log_message("Section: "  + section_name, end="\t", flush=True)
+            log_message(" Compression Ratio: " + str(round(section_compression_ratio, 2)) +"%", end="\t",flush=True) 
+            log_message("Size of section: " + readable_size(section.SizeOfRawData) +".",flush=True)
+            if biggest_section == None:
+                biggest_section = section
+                biggest_uncompressed = section_compression_ratio
+            elif section.SizeOfRawData > biggest_section.SizeOfRawData:
+                biggest_section = section
+                biggest_uncompressed = section_compression_ratio
+        # Handle specific bloated sections
+        if biggest_section.Name.decode() == ".rsrc\x00\x00\x00":
+            # Get biggest resource or resources and drop them from the 
+            # Resource table
+            # TODO: recalculate PE header in situations where the 
+            # resource is not at the end of an executable.
+            # TODO: Handle other tomfoolery required when resource 
+            # is not at end of executable.
+            log_message('''
+Bloat was located in the resource section. Removing bloat.. 
+''')
+            
+            bytes_removed = remove_resources(pe, pe_data)
+            end_of_real_data =- bytes_removed
+            return end_of_real_data, result
+        elif biggest_section.Name.decode() == ".text\x00\x00\x00":
+            # Data stored in the .text section is often a .NET Resource. The following checks
+            # to confirm it is .NET and then drops the resources.
+            if pe.OPTIONAL_HEADER.DATA_DIRECTORY[14].Size:
+                log_message('''
+Bloat was detected in the text section. Bloat is likely in a .NET Resource 
+This use case cannot be processed at this time. ''')
+            return end_of_real_data, result
+                
+        # The use cases covered by this section are at the end of 
+        # the binary. In my experience, the bloated sections are 
+        # usually at the end unless they are bloat from .NET Resources.
+        if biggest_uncompressed > 3000:
+            log_message('''
+The compression ratio is indicative of a bloated section.
+''', end="", flush=True)
+            # Get the size of the section.
+            section_end = section.PointerToRawData + section.SizeOfRawData
+            original_section_size = section.SizeOfRawData
+            section_data = pe_data[section.PointerToRawData:section_end]
+            delta_last_non_junk = trim_junk(section_data, original_section_size)
+            pe_data[section.PointerToRawData + delta_last_non_junk:section_end] = []
+            section_bytes_to_remove = original_section_size - delta_last_non_junk
+            end_of_real_data =  end_of_real_data - section_bytes_to_remove
+            # This will update the last section header, SizeOfRawData, SizeOfImage.
+            pe.sections[pe.sections.index(biggest_section)].section_max_addr -= section_bytes_to_remove
+            pe.sections[pe.sections.index(biggest_section)].SizeOfRawData -= section_bytes_to_remove
+            #pe.sections[pe.sections.index(biggest_section)].Misc_VirtualSize -= section_bytes_to_remove
+            #pe.OPTIONAL_HEADER.SizeOfImage -= section_bytes_to_remove
+            log_message("Bloated section reduced.")
+            return end_of_real_data, result
+            
+       
+        
+def trim_junk(bloated_content: bytes, original_size_with_junk: int) -> int:
+    ''' Attempt multiple methods or removing junk from overlay.'''
+    backward_bloated_content = bloated_content[::-1]
+    # Regex Explained:
+    # Match raw bytes that are repeated more than 20 times at the end
+    # of a binary. 
+    delta_last_non_junk = original_size_with_junk
+    # First Method: Trims 1 repeating byte.
+    # Check against 200 bytes, if successful, calculate full match.
+    junk_match = re.search(rb'^(..)\1{20,}', backward_bloated_content[:600])
+    # Second Method: If "not junk_match" check for junk larger than 1 repeating byte
+    chunk_start = 0
+    if not junk_match:
+        # Brute force check: check to see if there are 1-20 bytes
+        # being repeated and feed the number into the regex
+        for i in range(300):
+            # Regex Explained:
+            # Starting at the end of the PE, check for repeated bytes.
+            # This indicates junk bytes in the overlay. Match that set
+            # of repeated bytes 1 or more times. 
+            junk_regex = rb"^(..{" + bytes(str(i), "utf-8") + rb"})\1{2,}"
+            multibyte_junk_regex = re.search(junk_regex, backward_bloated_content[:1000])
+            if multibyte_junk_regex:
+                # Having found the pattern, we can make the regex efficient
+                # by targeting the pattern using the "targeted_regex"
+                targeted_regex = rb"(" + binascii.hexlify(multibyte_junk_regex.group(1)) + rb")\1{1,}"
+                chunk_end = chunk_start
+                while original_size_with_junk > chunk_end:
+                    chunk_end = chunk_start + 1000
+                    targeted_multibyte_junk_regex = re.search(targeted_regex, 
+                                                              binascii.hexlify(backward_bloated_content[chunk_start:chunk_end]))
+                    if targeted_multibyte_junk_regex:
+                        chunk_start += targeted_multibyte_junk_regex.end(0)
+                        unmatched_portion = 1000 - targeted_multibyte_junk_regex.end(0)
+                    else:
+                        # If the targeted_multibyte_junk_regex does not
+                        # return anything, that indicates the previous loop
+                        # had content which did not match. We'll use that
+                        # to help ensure we do not remove too much of the file. 
+                        chunk_start += unmatched_portion 
+                        break
+                break
+                # It was determined that data cannot be removed any more
+                # from the chunk_start. But the value of chunk_start
+                # now tells us how much data we can safely remove.
+        junk_to_remove = chunk_start  
+        #junk_to_remove = int(junk_to_remove)
+        delta_last_non_junk -= junk_to_remove
+    # Third Method: check for a series of one repeated byte. 
+    # Junk was identified. A new size is assigned and returned.
+    else:
+        targeted_regex = rb""+ binascii.hexlify(junk_match.string) + rb"{1,}"
+        targeted_junk_match = re.search(targeted_regex, binascii.hexlify(backward_bloated_content))
+        junk_to_remove = targeted_junk_match.end(0)
+        # If the trimming did not remove more than half of the bytes then
+        # this suggests the attacker may have put a random series of
+        # repeated bytes. These will be removed by loading the overlay
+        # 200 bytes at a time and removing parts which repeat for more
+        # than 20 bytes.
+        if junk_to_remove < original_size_with_junk / 2:
+            chunk_start = targeted_junk_match.end(0)
+            chunk_end = chunk_start
+            while original_size_with_junk > chunk_end:
+                chunk_end = chunk_start + 200
+                repeated_junk_match = re.search(rb'(..)\1{20,}', 
+                                                binascii.hexlify(backward_bloated_content[chunk_start:chunk_end]))
+                if repeated_junk_match:
+                    chunk_start += repeated_junk_match.end(0)
+                    unmatched_portion = 200 - repeated_junk_match.end(0)
+                else:
+                    chunk_start += unmatched_portion
+                    break
+            junk_to_remove = chunk_start 
+        else:
+            junk_to_remove = int(junk_to_remove / 2)
+        delta_last_non_junk -= junk_to_remove
+    return delta_last_non_junk  
+
+def process_pe(pe: pefile.PE, out_path: str, unsafe_processing: bool,
+               log_message: Callable[[str], None]) -> None:
+    '''Prepare PE, perform checks, remote junk, write patched binary.'''
+    beginning_file_size = len(pe.write())
+    # We are using the variable "end_of_real_data" and are reassigning 
+    # the value based on our analysis.We are assigning it now in case 
+    # we are unable to reduce the binary size for any reason.
+    end_of_real_data = beginning_file_size
+    pe_data = bytearray(pe.__data__)
+    # Remove Signature and modify size of Optional Header Security entry.
+    signature_address, signature_size = get_signature_info(pe)
+    pe_data[signature_address:signature_address + signature_size] = []
+    signature_abnormality = handle_signature_abnormality(signature_address, 
+                                                        signature_size, 
+                                                        beginning_file_size)
+    if signature_abnormality:
+        log_message('''
+We detected data after the signature. This is abnormal. Removing signature and extra data...''')
+        end_of_real_data = signature_address
+        pe_data = pe_data[:end_of_real_data]
+    # Handle Overlays: this includes packers and overlays which are completely junk
+    elif pe.get_overlay_data_start_offset() and signature_size < len(pe.get_overlay()):
+        log_message("An overlay was detected. Checking for known packer.")
+        packer_idenfitied = check_for_packer(pe)
+        if packer_idenfitied:
+            log_message("Packer identified: " + PACKER[packer_idenfitied])
+            if PACKER[1]:
+                log_message('''
+The original file cannot be debloated. It must be unpacked with a tool such as UniExtract2.
+                ''')
+        else:
+            log_message("Packer not identified. Attempting dynamic trim...")
+            last_section = find_last_section(pe)
+            overlay = pe_data[last_section.PointerToRawData + last_section.SizeOfRawData:]
+            end_of_real_data = trim_junk(overlay, end_of_real_data)
+            pe_data = pe_data[:end_of_real_data]
+            if end_of_real_data == beginning_file_size:
+                if unsafe_processing is True:
+                    log_message("""
+"Unsafe" switch detected. Running unsafe debloat technique:\n
+This is the last resort of removing the whole overlay: this works in some 
+cases, but can remove critical content. 
+If file is a Nullsoft executable, but was not detected, the original file can 
+be unpacked with the tool "UniExtract2".
+                    """)
+                    last_section = find_last_section(pe)
+                    end_of_real_data = last_section.PointerToRawData + last_section.SizeOfRawData
+                    pe_data = pe_data[:end_of_real_data] 
+                else:
+                    log_message("""
+Overlay was unable to be trimmed. Try unpacking with UniExtract2 or re-running 
+Debloat with the "--unsafe" parameter."""
+                                )
+    # Handle bloated sections
+    # TODO: break up into functions
+    else:
+        # In order to solve some use cases, we will find the biggest section 
+        # within the binary.
+        end_of_real_data, result = check_section_compression(pe, pe_data,
+                                                             end_of_real_data, 
+                                                             log_message=log_message)
+        log_message(result)
+    # All processing is done. Report results.
+    if end_of_real_data == beginning_file_size:
+        log_message("""No automated method for reducing the size worked. Please consider sharing the
+sample for additional analysis.
+Email: Squiblydoo@pm.me
+Twitter: @SquiblydooBlog.
+                    """)
+    else:
+        pe.__data__ =pe_data
+        final_filesize, new_pe_name = write_patched_file(out_path,
+                                                         pe, 
+                                                         end_of_real_data)
+        reduction_calculation = round(((beginning_file_size \
+                                        - final_filesize) \
+                                        / beginning_file_size) * 100, 2)
+        log_message("Beginning File size: " \
+                + readable_size(beginning_file_size) + ".")
+        log_message("File was reduced by " \
+                    + str(reduction_calculation) + "%.")
+        log_message("Final file size: " \
+                    + readable_size(final_filesize) + ".")
+        log_message("Processing complete.\nFile written to '" \
+                    + str(new_pe_name) + "'.")
```

### Comparing `debloat-1.4.2/src/debloat/tests/debloat_test.py` & `debloat-1.4.3/src/debloat/tests/debloat_test.py`

 * *Files identical despite different names*

### Comparing `debloat-1.4.2/src/debloat/utilities/rsrc.py` & `debloat-1.4.3/src/debloat/utilities/rsrc.py`

 * *Files identical despite different names*

### Comparing `debloat-1.4.2/src/debloat.egg-info/PKG-INFO` & `debloat-1.4.3/src/debloat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debloat
-Version: 1.4.2
+Version: 1.4.3
 Summary: Debloat is an tool to remove excess garbage from bloated executables.
 Author-email: Squiblydoo <Squiblydoo@pm.me>
 Project-URL: Homepage, https://github.com/Squiblydoo/debloat
 Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
@@ -42,15 +42,16 @@
 `debloat` can take two arguments. The first argument is required: the file to debloat. The second argument is optional: the output location. When no output is provided, it will be written to the same directory as the original file.
 
 The gui can also be launched from the CLI using the command `debloat-gui`.
 
 ## Does it always work?
 Not yet.
 My unscientific guess is that it should work for every 7 of 8 binaries. There are specific usecases I know where it does not work and I am working to implement solutions for those usecases. 
-In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "-unsafe" switch. If you ever need this switch, consider sharing the sample for additional analysis.
+
+In previous versions, `debloat` could accidentally remove too much of the binary. That is no longer the case unless you use the "--last-ditch-effort" switch. If you ever need this switch, consider sharing the sample for additional analysis. This option has now been added to the GUI. Functionally, what the function does is it will remove the whole overlay, if there is one. In some cases this is necessary as no pattern for the junk was found---this is most commonly the case in samples that do not compress well.
 
 ## Use Cases (Images from [Malcat](https://malcat.fr/))
 ### Full support
 - [x] Bloat appended to the end of a Signed PE.<br>
 In the image below, the bloat has been appended to the end of the executable. <br>
 ![Screenshot 2023-02-11 at 3 32 36 PM](https://user-images.githubusercontent.com/77356206/218279963-00780b59-8227-47dd-a0af-41096f6ae17b.png)
 
@@ -76,17 +77,18 @@
 ## Why?
 There appear to be a limited number of tools to easily process bloated executables. The two tools I have seen the most are “foremost” which is intended for recovering binaries from a disk image and “pecheck”.
 
 [Foremost](https://www.kali.org/tools/foremost/) works best in instances where the junk bytes are null (0x00) and it struggles when the binary has a fake or real signature. Its use in removing bloat from files is not its original purpose.
 
 [Pecheck](https://github.com/DidierStevens/DidierStevensSuite/blob/master/pecheck.py) has been developed over 14+ years and has some confusing commandline options. The option to remove bloated content is not the primary function of the script. Pecheck has to be combined with another tool ([disitool](https://blog.didierstevens.com/programs/disitool/)) in order to handle signed executables. In my experience, there are other times where pecheck can get confused and return an executable twice the size of the original bloated executable. All these factors seem OK if you are handling a small number of binaries, but as the number of binaries and methods increase, a tool specific to removing bloat is needed.
 
-There are good solid manual methods to remove bloat from binaries, but these methods can be tedious and not all analysts have the skills to do this. This tool removes the burden of needing to know how to manually remove bloat. Additionally, it allows for better scale. The principles used in the script allow allow for better scale if automation is desired.\*
+[Binary Refinery](https://github.com/binref/refinery) is an amazing tool. It was written with the intention of being a [CyberChef](https://github.com/gchq/CyberChef) of the commandline. While both tools are amazing, they both have a shortcoming that requires the user to know what formulas should be applied. 
+
+There are good solid manual methods to remove bloat from binaries, but these methods can be tedious and not all analysts have the skills to do this. This tool removes the burden of needing to know how to manually remove bloat. Additionally, it allows for better scale. The principles used in the script allow allow for better scale if automation is desired.
 
-\* Note: If automation is desired, I recommend re-writing these concepts in C/C++ and not Python.
 
 ## How to build? 
 Follow the build commands appropriate to your platform. The main difference between build commands is the format of the icon.
 <br>
 MacOS<br>
 `pyinstaller --onefile --noconsole --additional-hooks-dir=./hook --icon=debloat.icns gui.py`
```

