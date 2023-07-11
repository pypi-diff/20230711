# Comparing `tmp/debloat-1.4.3.tar.gz` & `tmp/debloat-1.4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "debloat-1.4.3.tar", last modified: Tue Jul 11 18:43:41 2023, max compression
+gzip compressed data, was "debloat-1.4.3.1.tar", last modified: Tue Jul 11 18:54:17 2023, max compression
```

## Comparing `debloat-1.4.3.tar` & `debloat-1.4.3.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 18:43:41.433530 debloat-1.4.3/
--rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.4.3/LICENSE
--rw-rw-rw-   0        0        0     7905 2023-07-11 18:43:41.433530 debloat-1.4.3/PKG-INFO
--rw-rw-rw-   0        0        0     7353 2023-07-11 18:34:10.000000 debloat-1.4.3/README.md
--rw-rw-rw-   0        0        0      788 2023-07-11 18:34:56.000000 debloat-1.4.3/pyproject.toml
--rw-rw-rw-   0        0        0      166 2023-07-11 18:43:41.439031 debloat-1.4.3/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.4.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:43:41.376021 debloat-1.4.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 18:43:41.397524 debloat-1.4.3/src/debloat/
--rw-rw-rw-   0        0        0        0 2023-05-09 12:13:11.000000 debloat-1.4.3/src/debloat/__init__.py
--rw-rw-rw-   0        0        0      510 2023-03-27 10:51:40.000000 debloat-1.4.3/src/debloat/auxiliary.py
--rw-rw-rw-   0        0        0     3976 2023-07-11 18:34:35.000000 debloat-1.4.3/src/debloat/gui.py
--rw-rw-rw-   0        0        0     1679 2023-07-11 18:34:35.000000 debloat-1.4.3/src/debloat/main.py
--rw-rw-rw-   0        0        0    24894 2023-07-11 18:42:12.000000 debloat-1.4.3/src/debloat/processor.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:43:41.429030 debloat-1.4.3/src/debloat/tests/
--rw-rw-rw-   0        0        0        0 2023-05-24 09:41:28.000000 debloat-1.4.3/src/debloat/tests/__init__.py
--rw-rw-rw-   0        0        0     1027 2023-07-11 18:34:35.000000 debloat-1.4.3/src/debloat/tests/debloat_test.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:43:41.432030 debloat-1.4.3/src/debloat/utilities/
--rw-rw-rw-   0        0        0        0 2023-07-04 17:05:39.000000 debloat-1.4.3/src/debloat/utilities/__init__.py
--rw-rw-rw-   0        0        0      746 2023-07-11 18:18:14.000000 debloat-1.4.3/src/debloat/utilities/rsrc.py
-drwxrwxrwx   0        0        0        0 2023-07-11 18:43:41.426530 debloat-1.4.3/src/debloat.egg-info/
--rw-rw-rw-   0        0        0     7905 2023-07-11 18:43:41.000000 debloat-1.4.3/src/debloat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      504 2023-07-11 18:43:41.000000 debloat-1.4.3/src/debloat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 18:43:41.000000 debloat-1.4.3/src/debloat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-07-11 18:43:41.000000 debloat-1.4.3/src/debloat.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-07-11 18:43:41.000000 debloat-1.4.3/src/debloat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-11 18:43:41.000000 debloat-1.4.3/src/debloat.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-11 18:54:17.142985 debloat-1.4.3.1/
+-rw-rw-rw-   0        0        0     1525 2023-03-27 10:23:04.000000 debloat-1.4.3.1/LICENSE
+-rw-rw-rw-   0        0        0     7907 2023-07-11 18:54:17.142985 debloat-1.4.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7353 2023-07-11 18:34:10.000000 debloat-1.4.3.1/README.md
+-rw-rw-rw-   0        0        0      790 2023-07-11 18:53:39.000000 debloat-1.4.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0      166 2023-07-11 18:54:17.144985 debloat-1.4.3.1/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-27 10:34:30.000000 debloat-1.4.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:54:17.092549 debloat-1.4.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-11 18:54:17.108479 debloat-1.4.3.1/src/debloat/
+-rw-rw-rw-   0        0        0        0 2023-05-09 12:13:11.000000 debloat-1.4.3.1/src/debloat/__init__.py
+-rw-rw-rw-   0        0        0      510 2023-03-27 10:51:40.000000 debloat-1.4.3.1/src/debloat/auxiliary.py
+-rw-rw-rw-   0        0        0     3987 2023-07-11 18:51:55.000000 debloat-1.4.3.1/src/debloat/gui.py
+-rw-rw-rw-   0        0        0     1702 2023-07-11 18:51:55.000000 debloat-1.4.3.1/src/debloat/main.py
+-rw-rw-rw-   0        0        0    24524 2023-07-11 18:52:22.000000 debloat-1.4.3.1/src/debloat/processor.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:54:17.138985 debloat-1.4.3.1/src/debloat/tests/
+-rw-rw-rw-   0        0        0        0 2023-05-24 09:41:28.000000 debloat-1.4.3.1/src/debloat/tests/__init__.py
+-rw-rw-rw-   0        0        0      579 2023-07-11 18:51:55.000000 debloat-1.4.3.1/src/debloat/tests/debloat_test.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:54:17.141485 debloat-1.4.3.1/src/debloat/utilities/
+-rw-rw-rw-   0        0        0        0 2023-07-04 17:05:39.000000 debloat-1.4.3.1/src/debloat/utilities/__init__.py
+-rw-rw-rw-   0        0        0      746 2023-07-11 18:18:14.000000 debloat-1.4.3.1/src/debloat/utilities/rsrc.py
+drwxrwxrwx   0        0        0        0 2023-07-11 18:54:17.136484 debloat-1.4.3.1/src/debloat.egg-info/
+-rw-rw-rw-   0        0        0     7907 2023-07-11 18:54:17.000000 debloat-1.4.3.1/src/debloat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      504 2023-07-11 18:54:17.000000 debloat-1.4.3.1/src/debloat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-11 18:54:17.000000 debloat-1.4.3.1/src/debloat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-07-11 18:54:17.000000 debloat-1.4.3.1/src/debloat.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-07-11 18:54:17.000000 debloat-1.4.3.1/src/debloat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-11 18:54:17.000000 debloat-1.4.3.1/src/debloat.egg-info/top_level.txt
```

### Comparing `debloat-1.4.3/LICENSE` & `debloat-1.4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `debloat-1.4.3/PKG-INFO` & `debloat-1.4.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debloat
-Version: 1.4.3
+Version: 1.4.3.1
 Summary: Debloat is an tool to remove excess garbage from bloated executables.
 Author-email: Squiblydoo <Squiblydoo@pm.me>
 Project-URL: Homepage, https://github.com/Squiblydoo/debloat
 Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `debloat-1.4.3/README.md` & `debloat-1.4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `debloat-1.4.3/pyproject.toml` & `debloat-1.4.3.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "debloat"
-version = "1.4.3"
+version = "1.4.3.1"
 authors = [
   { name="Squiblydoo", email="Squiblydoo@pm.me" },
 ]
 description = "Debloat is an tool to remove excess garbage from bloated executables."
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
```

### Comparing `debloat-1.4.3/src/debloat/gui.py` & `debloat-1.4.3.1/src/debloat/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
                                      text="Process file", \
                                      command=self.process)
         self.process_button.pack(pady=10)
 
         # Safe processing value and checkbox: Maybe not even needed?
         self.unsafe_processing = BooleanVar(value=False)
         self.unsafe_checkbox = Checkbutton(self,
-                                        text="Check to run unsafe processing",
+                                        text="Check to run last ditch effort processing",
                                          variable=self.unsafe_processing)
         self.unsafe_checkbox.pack()
 
         
 
         # Define Scrollbox for output of program.
         self.output_scrollbox = st.ScrolledText(self,
```

### Comparing `debloat-1.4.3/src/debloat/main.py` & `debloat-1.4.3.1/src/debloat/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,17 @@
     parser.add_argument("executable", 
                         help="Path to the executable to be debloated",
                         type=Path)
     parser.add_argument("--output", 
                         help="Output location", 
                         type=Path,
                         required=False)
-    parser.add_argument("-u", "--unsafe", 
+    parser.add_argument("-u", "--last-ditch-effort", dest="unsafe",
                         help="""
-    Disable safe processing. With unsafe processing, Debloat may remove the
+    Run last-ditch-effort processing. In this mode Debloat may remove the
     whole PE Overlay as a last resort if no smarter method works.
                             """,
                         action='store_true', default=False)
     args = parser.parse_args()
 
     file_path = args.executable
     out_path = args.output
```

### Comparing `debloat-1.4.3/src/debloat/processor.py` & `debloat-1.4.3.1/src/debloat/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 This file handles the processing of binaries and helper methods.
 
-Three methods are from https://github.com/binref/refinery 
-Copyright 2019 Jesko Hüttenhain used under the 3-Clause BSD License 
+Three methods rely heavily on parts of Binary Refinery
+https://github.com/binref/refinery 
+Copyright 2019 Jesko Hüttenhain under the 3-Clause BSD License 
 The methods are:
 refinery_strip()
 adjust_offsets()
 refinery_trim_resources()
 The RSRC Class is also from refinery.
 """
 import re
@@ -34,16 +35,15 @@
         return '%.1f KB' % (float(value) / 1024.0)
     elif value < 1024 * 1024 * 1024:
         return '%.1f MB' % (float(value) / 1024.0 / 1024.0)
     else:
         return '%.1f GB' % (float(value) / 1024.0 / 1024.0 / 1024.0)
 
 def write_patched_file(out_path: str,
-                        pe: pefile.PE, 
-                        end_of_real_data: int) -> Tuple[int, str]:
+                        pe: pefile.PE) -> Tuple[int, str]:
     '''Writes the patched file to disk.
     
     Keyword Arguments:
     out_path -- the path and file name to write
     pe -- the pefile that is being processed
     end_of_real_data -- an int indicating the size of bytes to write'''
     with open(out_path, 'wb') as writer:
@@ -319,61 +319,54 @@
             elif section.SizeOfRawData > biggest_section.SizeOfRawData:
                 biggest_section = section
                 biggest_uncompressed = section_compression_ratio
         # Handle specific bloated sections
         if biggest_section.Name.decode() == ".rsrc\x00\x00\x00":
             # Get biggest resource or resources and drop them from the 
             # Resource table
-            # TODO: recalculate PE header in situations where the 
-            # resource is not at the end of an executable.
-            # TODO: Handle other tomfoolery required when resource 
-            # is not at end of executable.
             log_message('''
 Bloat was located in the resource section. Removing bloat.. 
 ''')
-            
             bytes_removed = remove_resources(pe, pe_data)
             end_of_real_data =- bytes_removed
             return end_of_real_data, result
         elif biggest_section.Name.decode() == ".text\x00\x00\x00":
             # Data stored in the .text section is often a .NET Resource. The following checks
             # to confirm it is .NET and then drops the resources.
             if pe.OPTIONAL_HEADER.DATA_DIRECTORY[14].Size:
                 log_message('''
 Bloat was detected in the text section. Bloat is likely in a .NET Resource 
 This use case cannot be processed at this time. ''')
             return end_of_real_data, result
-                
-        # The use cases covered by this section are at the end of 
-        # the binary. In my experience, the bloated sections are 
-        # usually at the end unless they are bloat from .NET Resources.
         if biggest_uncompressed > 3000:
             log_message('''
-The compression ratio is indicative of a bloated section.
+The compression ratio of ''' + biggest_section.Name.decode() + ''' is indicative of a bloated section.
 ''', end="", flush=True)
             # Get the size of the section.
-            section_end = section.PointerToRawData + section.SizeOfRawData
-            original_section_size = section.SizeOfRawData
-            section_data = pe_data[section.PointerToRawData:section_end]
-            delta_last_non_junk = trim_junk(section_data, original_section_size)
-            pe_data[section.PointerToRawData + delta_last_non_junk:section_end] = []
+            biggest_section_end = biggest_section.PointerToRawData + biggest_section.SizeOfRawData
+            original_section_size = biggest_section.SizeOfRawData
+            biggest_section_data = pe_data[biggest_section.PointerToRawData:biggest_section_end]
+
+            delta_last_non_junk = trim_junk(pe, biggest_section_data, original_section_size)
+            # Remove the junk from the section.
+            pe_data[biggest_section.PointerToRawData + delta_last_non_junk:biggest_section_end] = []
             section_bytes_to_remove = original_section_size - delta_last_non_junk
             end_of_real_data =  end_of_real_data - section_bytes_to_remove
-            # This will update the last section header, SizeOfRawData, SizeOfImage.
-            pe.sections[pe.sections.index(biggest_section)].section_max_addr -= section_bytes_to_remove
-            pe.sections[pe.sections.index(biggest_section)].SizeOfRawData -= section_bytes_to_remove
-            #pe.sections[pe.sections.index(biggest_section)].Misc_VirtualSize -= section_bytes_to_remove
-            #pe.OPTIONAL_HEADER.SizeOfImage -= section_bytes_to_remove
+            # Adjust all offsets for the file.
+            adjust_offsets(pe, biggest_section.PointerToRawData, section_bytes_to_remove)
             log_message("Bloated section reduced.")
             return end_of_real_data, result
             
        
         
-def trim_junk(bloated_content: bytes, original_size_with_junk: int) -> int:
-    ''' Attempt multiple methods or removing junk from overlay.'''
+def trim_junk(pe: pefile.PE, bloated_content: bytes, 
+              original_size_with_junk: int) -> int:
+    '''Attempts multiple methods to trim junk from the end of a section.'''
+    alignment = pe.OPTIONAL_HEADER.FileAlignment
+
     backward_bloated_content = bloated_content[::-1]
     # Regex Explained:
     # Match raw bytes that are repeated more than 20 times at the end
     # of a binary. 
     delta_last_non_junk = original_size_with_junk
     # First Method: Trims 1 repeating byte.
     # Check against 200 bytes, if successful, calculate full match.
@@ -426,28 +419,35 @@
         # this suggests the attacker may have put a random series of
         # repeated bytes. These will be removed by loading the overlay
         # 200 bytes at a time and removing parts which repeat for more
         # than 20 bytes.
         if junk_to_remove < original_size_with_junk / 2:
             chunk_start = targeted_junk_match.end(0)
             chunk_end = chunk_start
+            unmatched_portion = 0
             while original_size_with_junk > chunk_end:
                 chunk_end = chunk_start + 200
                 repeated_junk_match = re.search(rb'(..)\1{20,}', 
                                                 binascii.hexlify(backward_bloated_content[chunk_start:chunk_end]))
                 if repeated_junk_match:
                     chunk_start += repeated_junk_match.end(0)
                     unmatched_portion = 200 - repeated_junk_match.end(0)
                 else:
                     chunk_start += unmatched_portion
                     break
             junk_to_remove = chunk_start 
         else:
             junk_to_remove = int(junk_to_remove / 2)
         delta_last_non_junk -= junk_to_remove
+    
+    # The returned size must account for the file alignment.
+    # We will make sure it is aligned by adding bytes.
+    not_aligned = delta_last_non_junk % alignment
+    delta_last_non_junk = delta_last_non_junk - not_aligned
+
     return delta_last_non_junk  
 
 def process_pe(pe: pefile.PE, out_path: str, unsafe_processing: bool,
                log_message: Callable[[str], None]) -> None:
     '''Prepare PE, perform checks, remote junk, write patched binary.'''
     beginning_file_size = len(pe.write())
     # We are using the variable "end_of_real_data" and are reassigning 
@@ -476,32 +476,30 @@
                 log_message('''
 The original file cannot be debloated. It must be unpacked with a tool such as UniExtract2.
                 ''')
         else:
             log_message("Packer not identified. Attempting dynamic trim...")
             last_section = find_last_section(pe)
             overlay = pe_data[last_section.PointerToRawData + last_section.SizeOfRawData:]
-            end_of_real_data = trim_junk(overlay, end_of_real_data)
+            end_of_real_data = trim_junk(pe, overlay, end_of_real_data)
             pe_data = pe_data[:end_of_real_data]
             if end_of_real_data == beginning_file_size:
                 if unsafe_processing is True:
                     log_message("""
-"Unsafe" switch detected. Running unsafe debloat technique:\n
-This is the last resort of removing the whole overlay: this works in some 
-cases, but can remove critical content. 
-If file is a Nullsoft executable, but was not detected, the original file can 
-be unpacked with the tool "UniExtract2".
+"Last ditch" switch detected. Running last ditch debloat technique:\n
+This is the last resort that removes the whole overlay: this works in cases where the overlay lacks a pattern.
+However, if the file does not run after this, it is in indicator that this method removed critical data.
                     """)
                     last_section = find_last_section(pe)
                     end_of_real_data = last_section.PointerToRawData + last_section.SizeOfRawData
                     pe_data = pe_data[:end_of_real_data] 
                 else:
                     log_message("""
 Overlay was unable to be trimmed. Try unpacking with UniExtract2 or re-running 
-Debloat with the "--unsafe" parameter."""
+Debloat with the "--last-ditch" parameter."""
                                 )
     # Handle bloated sections
     # TODO: break up into functions
     else:
         # In order to solve some use cases, we will find the biggest section 
         # within the binary.
         end_of_real_data, result = check_section_compression(pe, pe_data,
@@ -512,18 +510,17 @@
     if end_of_real_data == beginning_file_size:
         log_message("""No automated method for reducing the size worked. Please consider sharing the
 sample for additional analysis.
 Email: Squiblydoo@pm.me
 Twitter: @SquiblydooBlog.
                     """)
     else:
-        pe.__data__ =pe_data
+        pe.__data__ = pe_data
         final_filesize, new_pe_name = write_patched_file(out_path,
-                                                         pe, 
-                                                         end_of_real_data)
+                                                         pe)
         reduction_calculation = round(((beginning_file_size \
                                         - final_filesize) \
                                         / beginning_file_size) * 100, 2)
         log_message("Beginning File size: " \
                 + readable_size(beginning_file_size) + ".")
         log_message("File was reduced by " \
                     + str(reduction_calculation) + "%.")
```

### Comparing `debloat-1.4.3/src/debloat/utilities/rsrc.py` & `debloat-1.4.3.1/src/debloat/utilities/rsrc.py`

 * *Files identical despite different names*

### Comparing `debloat-1.4.3/src/debloat.egg-info/PKG-INFO` & `debloat-1.4.3.1/src/debloat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: debloat
-Version: 1.4.3
+Version: 1.4.3.1
 Summary: Debloat is an tool to remove excess garbage from bloated executables.
 Author-email: Squiblydoo <Squiblydoo@pm.me>
 Project-URL: Homepage, https://github.com/Squiblydoo/debloat
 Project-URL: Bug Tracker, https://github.com/Squiblydoo/debloat/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

