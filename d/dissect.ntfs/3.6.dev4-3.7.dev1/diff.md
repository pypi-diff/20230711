# Comparing `tmp/dissect.ntfs-3.6.dev4.tar.gz` & `tmp/dissect.ntfs-3.7.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.ntfs-3.6.dev4.tar", last modified: Tue Jun 27 07:49:07 2023, max compression
+gzip compressed data, was "dissect.ntfs-3.7.dev1.tar", last modified: Tue Jul 11 14:05:55 2023, max compression
```

## Comparing `dissect.ntfs-3.6.dev4.tar` & `dissect.ntfs-3.7.dev1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:07.263544 dissect.ntfs-3.6.dev4/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-27 07:49:07.263544 dissect.ntfs-3.6.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:07.243543 dissect.ntfs-3.6.dev4/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:07.251544 dissect.ntfs-3.6.dev4/dissect/ntfs/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17587 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/attr.py
--rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/c_ntfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/index.py
--rw-r--r--   0 runner    (1001) docker     (123)    17025 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/mft.py
--rw-r--r--   0 runner    (1001) docker     (123)     6726 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/ntfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/secure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/usnjrnl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9390 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/dissect/ntfs/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:07.247543 dissect.ntfs-3.6.dev4/dissect.ntfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-27 07:49:07.000000 dissect.ntfs-3.6.dev4/dissect.ntfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-06-27 07:49:07.000000 dissect.ntfs-3.6.dev4/dissect.ntfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-27 07:49:07.000000 dissect.ntfs-3.6.dev4/dissect.ntfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-27 07:49:07.000000 dissect.ntfs-3.6.dev4/dissect.ntfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-27 07:49:07.000000 dissect.ntfs-3.6.dev4/dissect.ntfs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-27 07:48:57.000000 dissect.ntfs-3.6.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-27 07:49:07.263544 dissect.ntfs-3.6.dev4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:07.259544 dissect.ntfs-3.6.dev4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-27 07:48:54.000000 dissect.ntfs-3.6.dev4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:07.259544 dissect.ntfs-3.6.dev4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/data/boot_2m.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/data/mft.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)   908628 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/data/ntfs.bin.gz
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/data/ntfs_fragmented_mft.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/data/sds.bin.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-27 07:49:07.263544 dissect.ntfs-3.6.dev4/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/test_attr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/test_mft.py
--rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/test_ntfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/test_secure.py
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/test_usnjrnl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-27 07:48:53.000000 dissect.ntfs-3.6.dev4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:05:55.049821 dissect.ntfs-3.7.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-11 14:05:55.049821 dissect.ntfs-3.7.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:05:55.033820 dissect.ntfs-3.7.dev1/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:05:55.041820 dissect.ntfs-3.7.dev1/dissect/ntfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/dissect/ntfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17840 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/dissect/ntfs/attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19726 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/dissect/ntfs/c_ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/dissect/ntfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/dissect/ntfs/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17228 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/dissect/ntfs/mft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6737 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/dissect/ntfs/ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7252 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/dissect/ntfs/secure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/dissect/ntfs/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/dissect/ntfs/usnjrnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9445 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/dissect/ntfs/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:05:55.037820 dissect.ntfs-3.7.dev1/dissect.ntfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-11 14:05:54.000000 dissect.ntfs-3.7.dev1/dissect.ntfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-11 14:05:55.000000 dissect.ntfs-3.7.dev1/dissect.ntfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:05:54.000000 dissect.ntfs-3.7.dev1/dissect.ntfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-11 14:05:54.000000 dissect.ntfs-3.7.dev1/dissect.ntfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 14:05:54.000000 dissect.ntfs-3.7.dev1/dissect.ntfs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-07-11 14:05:43.000000 dissect.ntfs-3.7.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:05:55.049821 dissect.ntfs-3.7.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:05:55.045820 dissect.ntfs-3.7.dev1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:05:55.049821 dissect.ntfs-3.7.dev1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tests/data/boot_2m.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tests/data/mft.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   908628 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tests/data/ntfs.bin.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tests/data/ntfs_fragmented_mft.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tests/data/sds.bin.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:05:55.049821 dissect.ntfs-3.7.dev1/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tests/test_attr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tests/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tests/test_mft.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tests/test_ntfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tests/test_secure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tests/test_usnjrnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2000 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-11 14:05:38.000000 dissect.ntfs-3.7.dev1/tox.ini
```

### Comparing `dissect.ntfs-3.6.dev4/LICENSE` & `dissect.ntfs-3.7.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/PKG-INFO` & `dissect.ntfs-3.7.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ntfs
-Version: 3.6.dev4
+Version: 3.7.dev1
 Summary: A Dissect module implementing a parser for the NTFS file system, used by the Windows operating system
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ntfs
 Project-URL: repository, https://github.com/fox-it/dissect.ntfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.ntfs-3.6.dev4/README.md` & `dissect.ntfs-3.7.dev1/README.md`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/dissect/ntfs/__init__.py` & `dissect.ntfs-3.7.dev1/dissect/ntfs/__init__.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/dissect/ntfs/attr.py` & `dissect.ntfs-3.7.dev1/dissect/ntfs/attr.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import io
 from datetime import datetime
-from typing import TYPE_CHECKING, Any, BinaryIO, Iterator, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, BinaryIO, Iterator, Optional
 
 from dissect.util.stream import RangeStream, RunlistStream
 from dissect.util.ts import wintimestamp
 
 from dissect.ntfs.c_ntfs import (
     ATTRIBUTE_TYPE_CODE,
     IO_REPARSE_TAG,
@@ -20,15 +20,15 @@
 if TYPE_CHECKING:
     from dissect.ntfs.mft import MftRecord
 
 
 class Attribute:
     """Parse and interact with MFT attributes.
 
-    Wrapper for an AttributeHeader and AttributeRecord combination.
+    Wrapper for an :class:`AttributeHeader` and :class:`AttributeRecord` combination.
 
     Args:
         record: The MFT record this attribute belongs to.
         header: The AttributeHeader for this Attribute.
     """
 
     __slots__ = ("record", "header", "attribute")
@@ -82,15 +82,15 @@
         return self.header.resident
 
     @property
     def name(self) -> str:
         """Return the name of this attribute."""
         return self.header.name
 
-    def dataruns(self) -> List[Tuple[int, int]]:
+    def dataruns(self) -> list[tuple[int, int]]:
         """Return the dataruns of this attribute, if non-resident.
 
         Raises:
             TypeError: If attribute is resident.
         """
         return self.header.dataruns()
 
@@ -190,15 +190,15 @@
         return self.header.Form.Nonresident.HighestVcn if not self.resident else None
 
     @property
     def compression_unit(self) -> Optional[int]:
         """Return the compression unit if non-resident, else None."""
         return self.header.Form.Nonresident.CompressionUnit if not self.resident else None
 
-    def dataruns(self) -> List[Tuple[int, int]]:
+    def dataruns(self) -> list[tuple[int, int]]:
         """Return the dataruns of this attribute, if non-resident.
 
         Raises:
             TypeError: If attribute is resident.
         """
         if self.resident:
             raise TypeError("Resident attributes don't have dataruns")
@@ -277,26 +277,26 @@
 
     @classmethod
     def from_fh(
         cls, fh: BinaryIO, attr_type: ATTRIBUTE_TYPE_CODE, record: Optional[MftRecord] = None
     ) -> AttributeRecord:
         """Parse an attribute from a file-like object.
 
-        Selects a more specific AttributeRecord class if one is available for the given attribute type.
+        Selects a more specific :class:`AttributeRecord` class if one is available for the given attribute type.
 
         Args:
             fh: The file-like object to parse an attribute from.
             attr_type: The attribute type to parse.
             record: The MFT record this attribute belongs to.
         """
         return ATTRIBUTE_CLASS_MAP.get(attr_type, cls)(fh, record)
 
 
 class AttributeList(AttributeRecord):
-    """Specific AttributeRecord parser for $ATTRIBUTE_LIST."""
+    """Specific :class:`AttributeRecord` parser for ``$ATTRIBUTE_LIST``."""
 
     __slots__ = ("entries",)
 
     def __init__(self, fh: BinaryIO, record: Optional[MftRecord] = None):
         super().__init__(fh, record)
 
         offset = 0
@@ -316,15 +316,15 @@
             self.entries.append(entry)
             offset += entry.RecordLength
 
     def __repr__(self) -> str:
         return "<$ATTRIBUTE_LIST>"
 
     def attributes(self) -> Iterator[Attribute]:
-        """Iterate all entries within this $ATTRIBUTE_LIST and yield all embedded attributes."""
+        """Iterate all entries within this ``$ATTRIBUTE_LIST`` and yield all embedded attributes."""
         if not self.record:
             raise MftNotAvailableError("Can't iterate $ATTRIBUTE_LIST attributes without a bounded MFT record")
 
         seen = {self.record.segment}
 
         for entry in self.entries:
             segment = segment_reference(entry.SegmentReference)
@@ -335,163 +335,163 @@
             record = self.record.ntfs.mft(segment)
 
             for attr_list in record.attributes.values():
                 yield from attr_list
 
 
 class StandardInformation(AttributeRecord):
-    """Specific AttributeRecord parser for $STANDARD_INFORMATION."""
+    """Specific :class:`AttributeRecord` parser for ``$STANDARD_INFORMATION``."""
 
     __slots__ = ("attr",)
 
     def __init__(self, fh: BinaryIO, record: Optional[MftRecord] = None):
         super().__init__(fh, record)
         # Data can be less than the _STANDARD_INFORMATION structure size, so pad remaining fields with null bytes
         data = fh.read().ljust(len(c_ntfs._STANDARD_INFORMATION), b"\x00")
         self.attr = c_ntfs._STANDARD_INFORMATION(data)
 
     def __repr__(self) -> str:
         return "<$STANDARD_INFORMATION>"
 
     @property
     def creation_time(self) -> datetime:
-        """Return the $STANDARD_INFORMATION CreationTime."""
+        """Return the ``$STANDARD_INFORMATION`` ``CreationTime``."""
         return wintimestamp(self.attr.CreationTime)
 
     @property
     def creation_time_ns(self) -> int:
-        """Return the $STANDARD_INFORMATION CreationTime in nanoseconds."""
+        """Return the ``$STANDARD_INFORMATION`` ``CreationTime`` in nanoseconds."""
         return ts_to_ns(self.attr.CreationTime)
 
     @property
     def last_modification_time(self) -> datetime:
-        """Return the $STANDARD_INFORMATION LastModificationTime."""
+        """Return the ``$STANDARD_INFORMATION`` ``LastModificationTime``."""
         return wintimestamp(self.attr.LastModificationTime)
 
     @property
     def last_modification_time_ns(self) -> int:
-        """Return the $STANDARD_INFORMATION LastModificationTime in nanoseconds."""
+        """Return the ``$STANDARD_INFORMATION`` ``LastModificationTime`` in nanoseconds."""
         return ts_to_ns(self.attr.LastModificationTime)
 
     @property
     def last_change_time(self) -> datetime:
-        """Return the $STANDARD_INFORMATION LastChangeTime."""
+        """Return the ``$STANDARD_INFORMATION`` ``LastChangeTime``."""
         return wintimestamp(self.attr.LastChangeTime)
 
     @property
     def last_change_time_ns(self) -> int:
-        """Return the $STANDARD_INFORMATION LastChangeTime in nanoseconds."""
+        """Return the ``$STANDARD_INFORMATION`` ``LastChangeTime`` in nanoseconds."""
         return ts_to_ns(self.attr.LastChangeTime)
 
     @property
     def last_access_time(self) -> datetime:
-        """Return the $STANDARD_INFORMATION LastAccessTime."""
+        """Return the ``$STANDARD_INFORMATION`` ``LastAccessTime``."""
         return wintimestamp(self.attr.LastAccessTime)
 
     @property
     def last_access_time_ns(self) -> int:
-        """Return the $STANDARD_INFORMATION LastAccessTime in nanoseconds."""
+        """Return the ``$STANDARD_INFORMATION`` ``LastAccessTime`` in nanoseconds."""
         return ts_to_ns(self.attr.LastAccessTime)
 
     @property
     def file_attributes(self) -> int:
-        """Return the $STANDARD_INFORMATION FileAttributes."""
+        """Return the ``$STANDARD_INFORMATION`` ``FileAttributes``."""
         return self.attr.FileAttributes
 
     @property
     def owner_id(self) -> int:
-        """Return the $STANDARD_INFORMATION OwnerId."""
+        """Return the ``$STANDARD_INFORMATION`` ``OwnerId``."""
         return self.attr.OwnerId
 
     @property
     def security_id(self) -> int:
-        """Return the $STANDARD_INFORMATION SecurityId."""
+        """Return the ``$STANDARD_INFORMATION`` ``SecurityId``."""
         return self.attr.SecurityId
 
 
 class FileName(AttributeRecord):
-    """Specific AttributeRecord parser for $FILE_NAME."""
+    """Specific :class:`AttributeRecord` parser for ``$FILE_NAME``."""
 
     __slots__ = ("attr",)
 
     def __init__(self, fh: BinaryIO, record: Optional[MftRecord] = None):
         super().__init__(fh, record)
         data = fh.read().ljust(len(c_ntfs.STANDARD_INFORMATION_EX), b"\x00")
         self.attr = c_ntfs._FILE_NAME(data)
 
     def __repr__(self) -> str:
         return f"<$FILE_NAME {self.file_name}>"
 
     @property
     def creation_time(self) -> datetime:
-        """Return the $FILE_NAME file CreationTime."""
+        """Return the ``$FILE_NAME``file ``CreationTime``."""
         return wintimestamp(self.attr.CreationTime)
 
     @property
     def creation_time_ns(self) -> int:
-        """Return the $FILE_NAME file CreationTime in nanoseconds."""
+        """Return the ``$FILE_NAME`` file ``CreationTime`` in nanoseconds."""
         return ts_to_ns(self.attr.CreationTime)
 
     @property
     def last_modification_time(self) -> datetime:
-        """Return the $FILE_NAME file LastModificationTime."""
+        """Return the ``$FILE_NAME`` file ``LastModificationTime``."""
         return wintimestamp(self.attr.LastModificationTime)
 
     @property
     def last_modification_time_ns(self) -> int:
-        """Return the $FILE_NAME file LastModificationTime in nanoseconds."""
+        """Return the ``$FILE_NAME`` file ``LastModificationTime`` in nanoseconds."""
         return ts_to_ns(self.attr.LastModificationTime)
 
     @property
     def last_change_time(self) -> datetime:
-        """Return the $FILE_NAME file LastChangeTime."""
+        """Return the ``$FILE_NAME`` file ``LastChangeTime``."""
         return wintimestamp(self.attr.LastChangeTime)
 
     @property
     def last_change_time_ns(self) -> int:
-        """Return the $FILE_NAME file LastChangeTime in nanoseconds."""
+        """Return the ``$FILE_NAME`` file ``LastChangeTime`` in nanoseconds."""
         return ts_to_ns(self.attr.LastChangeTime)
 
     @property
     def last_access_time(self) -> datetime:
-        """Return the $FILE_NAME file LastAccessTime."""
+        """Return the ``$FILE_NAME`` file ``LastAccessTime``."""
         return wintimestamp(self.attr.LastAccessTime)
 
     @property
     def last_access_time_ns(self) -> int:
-        """Return the $FILE_NAME file LastAccessTime in nanoseconds."""
+        """Return the ``$FILE_NAME`` file ``LastAccessTime`` in nanoseconds."""
         return ts_to_ns(self.attr.LastAccessTime)
 
     @property
     def file_size(self) -> int:
-        """Return the $FILE_NAME file FileSize."""
+        """Return the ``$FILE_NAME`` file ``FileSize``."""
         return self.attr.FileSize
 
     @property
     def file_attributes(self) -> int:
-        """Return the $FILE_NAME file FileAttributes."""
+        """Return the ``$FILE_NAME`` file ``FileAttributes``."""
         return self.attr.FileAttributes
 
     @property
     def flags(self) -> int:
-        """Return the $FILE_NAME flags, which can be either FILE_NAME_NTFS or FILE_NAME_DOS."""
+        """Return the ``$FILE_NAME`` flags, which can be either ``FILE_NAME_NTFS`` or ``FILE_NAME_DOS``."""
         return self.attr.Flags
 
     @property
     def file_name(self) -> str:
-        """Return the file name string stored in this $FILE_NAME attribute."""
+        """Return the file name string stored in this ``$FILE_NAME`` attribute."""
         return self.attr.FileName
 
     def full_path(self) -> str:
         """Use the parent directory reference to try to generate a full path from this file name."""
         return get_full_path(self.record.ntfs.mft, self.file_name, self.attr.ParentDirectory)
 
 
 class ReparsePoint(AttributeRecord):
-    """Specific AttributeRecord parser for $REPARSE_POINT."""
+    """Specific :class:`AttributeRecord` parser for ``$REPARSE_POINT``."""
 
     __slots__ = ("attr", "tag_header", "buffer")
 
     def __init__(self, fh: BinaryIO, record: Optional[MftRecord] = None):
         super().__init__(fh, record)
         self.attr = c_ntfs._REPARSE_DATA_BUFFER(fh)
         data = io.BytesIO(fh.read(self.attr.ReparseDataLength))
```

### Comparing `dissect.ntfs-3.6.dev4/dissect/ntfs/c_ntfs.py` & `dissect.ntfs-3.7.dev1/dissect/ntfs/c_ntfs.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/dissect/ntfs/index.py` & `dissect.ntfs-3.7.dev1/dissect/ntfs/index.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import io
 from enum import Enum, auto
 from functools import cached_property, lru_cache
-from typing import TYPE_CHECKING, Any, BinaryIO, Callable, Iterator, List, Optional
+from typing import TYPE_CHECKING, Any, BinaryIO, Callable, Iterator, Optional
 
 from dissect.ntfs.attr import AttributeRecord
 from dissect.ntfs.c_ntfs import (
     ATTRIBUTE_TYPE_CODE,
     COLLATION,
     INDEX_ENTRY_END,
     INDEX_ENTRY_NODE,
@@ -60,15 +60,15 @@
             self._index_stream = None
 
     def __iter__(self) -> Iterator[IndexEntry]:
         return self.entries()
 
     @lru_cache(128)
     def index_buffer(self, vcn: int) -> IndexBuffer:
-        """Return the IndexBuffer at the specified cluster number.
+        """Return the :class:`IndexBuffer` at the specified cluster number.
 
         Args:
             vcn: The virtual cluster number within the index allocation to read.
 
         Raises:
             FileNotFoundError: If this index has no index allocation.
         """
@@ -118,15 +118,15 @@
 
         if exact and (entry.is_end or cmp(entry, search_value) != Match.Equal):
             raise KeyError(f"Value not found: {value}")
 
         return entry
 
     def entries(self) -> Iterator[IndexEntry]:
-        """Yield all IndexEntry's in this Index."""
+        """Yield all :class:`IndexEntry`'s in this :class:`Index`."""
 
         for entry in self.root.entries():
             if entry.is_end:
                 break
 
             yield entry
 
@@ -144,18 +144,18 @@
                 except EOFError:
                     break
 
                 vcn += 1
 
 
 class IndexRoot:
-    """Represents the $INDEX_ROOT.
+    """Represents the ``$INDEX_ROOT``.
 
     Args:
-        index: The Index class instance this IndexRoot belongs to.
+        index: The :class:`Index`` class instance this :class:`IndexRoot` belongs to.
         fh: The file-like object to parse an index root on.
     """
 
     def __init__(self, index: Index, fh: BinaryIO):
         self.index = index
         self.fh = fh
 
@@ -178,30 +178,30 @@
 
     @property
     def clusters_per_index_buffer(self) -> int:
         """Return the size of an index buffer in the index allocation in clusters."""
         return self.header.ClustersPerIndexBuffer
 
     def entries(self) -> Iterator[IndexEntry]:
-        """Yield all IndexEntry's in this IndexRoot."""
+        """Yield all :class:`IndexEntry`'s in this :class:`IndexRoot`."""
         yield from _iter_entries(
             self.index,
             self.fh,
             # Offset starts from the _INDEX_HEADER
             len(c_ntfs._INDEX_ROOT),
             self.header.IndexHeader.TotalSizeOfEntries,
         )
 
 
 class IndexBuffer:
-    """Represent an index buffer in $INDEX_ALLOCATION.
+    """Represent an index buffer in ``$INDEX_ALLOCATION``.
 
     Args:
-        index: The Index class instance this IndexRoot belongs to.
-        fh: The file-like object of $INDEX_ALLOCATION.
+        index: The :class:`Index` class instance this :class:`IndexRoot` belongs to.
+        fh: The file-like object of ``$INDEX_ALLOCATION``.
         offset: The offset in bytes to the index buffer on the file-like object we want to read.
         size: The size of the index buffer in bytes.
 
     Raises:
         EOFError: If there's not enough data available to read an index buffer.
         BrokenIndexError: If the index buffer doesn't start with the expected magic value.
     """
@@ -220,44 +220,44 @@
         if buf[:4] != b"INDX":
             raise BrokenIndexError("Broken INDX header")
 
         self.data = apply_fixup(buf)
         self.header = c_ntfs._INDEX_ALLOCATION_BUFFER(self.data)
 
     def entries(self) -> Iterator[IndexEntry]:
-        """Yield all IndexEntry's in this IndexBuffer."""
+        """Yield all :class:`IndexEntry`'s in this :class:`IndexBuffer`."""
         yield from _iter_entries(
             self.index,
             io.BytesIO(self.data),
             # Offset starts from the _INDEX_HEADER
             self.header.IndexHeader.FirstEntryOffset + 0x18,
             self.header.IndexHeader.TotalSizeOfEntries,
         )
 
 
 class IndexEntry:
     """Parse and interact with index entries.
 
     Args:
-        index: The Index class instance this IndexEntry belongs to.
+        index: The :class:`Index` class instance this :class:`IndexEntry` belongs to.
         fh: The file-like object to parse an index entry on.
         offset: The offset in the file-like object to parse an index entry at.
     """
 
     def __init__(self, index: Index, fh: BinaryIO, offset: int):
         self.index = index
         self.fh = fh
         self.offset = offset
 
         fh.seek(offset)
         self.header = c_ntfs._INDEX_ENTRY(fh)
         self.buf = fh.read(self.header.Length - len(c_ntfs._INDEX_ENTRY))
 
     def dereference(self) -> MftRecord:
-        """Dereference this IndexEntry to the MFT record it points to.
+        """Dereference this :class:`IndexEntry` to the MFT record it points to.
 
         Note that the file reference is a union with the data part so only access this if you know the entry has
         a file reference and not a data part.
 
         Raises:
             MftNotAvailableError: If no MFT is available.
         """
@@ -280,15 +280,15 @@
         data and not a file reference.
         """
         offset = self.header.DataOffset - len(c_ntfs._INDEX_ENTRY)
         return self.buf[offset : offset + self.header.DataLength]
 
     @cached_property
     def attribute(self) -> Optional[AttributeRecord]:
-        """Return the AttributeRecord of the attribute contained in this entry."""
+        """Return the :class:`dissect.ntfs.attr.AttributeRecord` of the attribute contained in this entry."""
         if self.key_length and self.index.root.attribute_type:
             return AttributeRecord.from_fh(
                 io.BytesIO(self.buf),
                 self.index.root.attribute_type,
                 record=self.index.record,
             )
         return None
@@ -333,15 +333,15 @@
 
         if entry.is_end:
             break
 
         offset += entry.length
 
 
-def _bsearch(entries: List[IndexEntry], value: Any, cmp: Callable[[IndexEntry, Any], Match]) -> IndexEntry:
+def _bsearch(entries: list[IndexEntry], value: Any, cmp: Callable[[IndexEntry, Any], Match]) -> IndexEntry:
     min_idx = 0
     max_idx = len(entries) - 1
 
     while min_idx != max_idx:
         test_idx = min_idx + (max_idx - min_idx) // 2
         test_entry = entries[test_idx]
```

### Comparing `dissect.ntfs-3.6.dev4/dissect/ntfs/mft.py` & `dissect.ntfs-3.7.dev1/dissect/ntfs/mft.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,14 @@
 from __future__ import annotations
 
 import ntpath
 from functools import cached_property, lru_cache
 from io import BytesIO
 from operator import itemgetter
-from typing import (
-    TYPE_CHECKING,
-    Any,
-    BinaryIO,
-    Dict,
-    Iterator,
-    List,
-    Optional,
-    Tuple,
-    Union,
-)
+from typing import TYPE_CHECKING, Any, BinaryIO, Iterator, Optional, Union
 
 from dissect.cstruct import Instance
 
 from dissect.ntfs.attr import Attribute, AttributeHeader
 from dissect.ntfs.c_ntfs import (
     ATTRIBUTE_TYPE_CODE,
     DEFAULT_RECORD_SIZE,
@@ -42,15 +32,15 @@
 from dissect.ntfs.util import AttributeCollection, AttributeMap, apply_fixup
 
 if TYPE_CHECKING:
     from dissect.ntfs.ntfs import NTFS
 
 
 class Mft:
-    """Interact with the $MFT (Master File Table).
+    """Interact with the ``$MFT`` (Master File Table).
 
     Args:
         fh: A file-like object of the $MFT file.
         ntfs: An optional NTFS class instance.
     """
 
     def __init__(self, fh: BinaryIO, ntfs: Optional[NTFS] = None):
@@ -100,17 +90,17 @@
         return node
 
     @lru_cache(4096)
     def get(self, ref: Union[int, str, Instance], root: Optional[MftRecord] = None) -> MftRecord:
         """Retrieve an MFT record using a variety of methods.
 
         Supported references are:
-        - _MFT_SEGMENT_REFERENCE cstruct instance
-        - integer segment number
-        - string file path
+            - ``_MFT_SEGMENT_REFERENCE`` cstruct instance
+            - integer segment number
+            - string file path
 
         Args:
             ref: Reference to retrieve the record by.
             root: Optional root record to start resolving from. Useful for relative path lookups.
 
         Raises:
             TypeError: If the reference is of an unsupported type.
@@ -142,15 +132,15 @@
             except EOFError:
                 break
 
 
 class MftRecord:
     """MFT record parsing and interaction.
 
-    Use the from_fh or from_bytes class methods to instantiate.
+    Use the :func:`~MftRecord.from_fh` or :func:`~MftRecord.from_bytes` class methods to instantiate.
     """
 
     def __init__(self):
         self.ntfs: Optional[NTFS] = None
         self.segment: Optional[int] = None
         self.offset: Optional[int] = None
         self.data: Optional[bytes] = None
@@ -202,15 +192,15 @@
             raise BrokenMftError(f"Invalid MFT record Signature: {data[:4]}")
 
         obj.data = apply_fixup(data)
         obj.header = c_ntfs._FILE_RECORD_SEGMENT_HEADER(obj.data)
         return obj
 
     def get(self, path: str) -> MftRecord:
-        """Retrieve a MftRecord relative to this one.
+        """Retrieve a :class:`MftRecord` relative to this one.
 
         Args:
             path: The path to lookup.
 
         Raises:
             MftNotAvailableError: If no MFT is available.
         """
@@ -218,15 +208,15 @@
             raise MftNotAvailableError()
         return self.ntfs.mft.get(path, root=self)
 
     @cached_property
     def attributes(self) -> AttributeMap:
         """Parse and return the attributes in this MFT record.
 
-        $ATTRIBUTE_LIST's are only parsed if there's an MFT available on the NTFS object.
+        ``$ATTRIBUTE_LIST``'s are only parsed if there's an MFT available on the NTFS object.
 
         Raises:
             BrokenMftError: If an error occurred parsing the attributes.
         """
         fh = BytesIO(self.data)
         offset = self.header.FirstAttributeOffset
         attrs = AttributeMap()
@@ -259,46 +249,46 @@
             for attr in attr_list.attributes():
                 attrs.add(attr)
 
         return attrs
 
     @cached_property
     def resident(self) -> bool:
-        """Return whether this record's default $DATA attribute is resident."""
+        """Return whether this record's default ``$DATA`` attribute is resident."""
         return any(attr.header.resident for attr in self.attributes[ATTRIBUTE_TYPE_CODE.DATA])
 
     @cached_property
     def filename(self) -> Optional[str]:
-        """Return the first file name, or None if this record has no file names."""
+        """Return the first file name, or ``None`` if this record has no file names."""
         filenames = self.filenames()
         return filenames[0] if filenames else None
 
-    def filenames(self, ignore_dos: bool = False) -> List[str]:
+    def filenames(self, ignore_dos: bool = False) -> list[str]:
         """Return all file names of this record.
 
         Args:
             ignore_dos: Ignore DOS file name entries.
         """
         result = []
         for attr in self.attributes[ATTRIBUTE_TYPE_CODE.FILE_NAME]:
             if ignore_dos and attr.flags == FILE_NAME_DOS:
                 continue
             result.append((attr.flags, attr.file_name))
         return [item[1] for item in sorted(result, key=itemgetter(0))]
 
-    def full_path(self, ignore_dos: bool = False):
-        """Return the first full path, or None if this record has no file names.
+    def full_path(self, ignore_dos: bool = False) -> Optional[str]:
+        """Return the first full path, or ``None`` if this record has no file names.
 
         Args:
             ignore_dos: Ignore DOS file name entries.
         """
         paths = self.full_paths(ignore_dos)
         return paths[0] if paths else None
 
-    def full_paths(self, ignore_dos: bool = False):
+    def full_paths(self, ignore_dos: bool = False) -> list[str]:
         """Return all full paths of this record.
 
         Args:
             ignore_dos: Ignore DOS file name entries.
         """
         result = []
 
@@ -345,15 +335,15 @@
             raise NotAReparsePointError(f"{self!r} is not a reparse point")
         return self.attributes[ATTRIBUTE_TYPE_CODE.REPARSE_POINT].substitute_name
 
     @cached_property
     def reparse_point_record(self) -> MftRecord:
         """Resolve a reparse point and return the target record.
 
-        Note: absolute links (such as directory junctions) will _always_ fail in the context of a single filesystem.
+        Note: absolute links (such as directory junctions) will *always* fail in the context of a single filesystem.
         Absolute links include the drive letter, of which we have no knowledge here.
         """
         if not self.is_reparse_point():
             raise NotAReparsePointError(f"{self!r} is not a reparse point")
 
         if not self.ntfs or not self.ntfs.mft:
             raise MftNotAvailableError()
@@ -365,23 +355,23 @@
             target_name = ntpath.join(ntpath.dirname(self.full_path()), target_name)
 
         return self.ntfs.mft.get(target_name)
 
     def _get_stream_attributes(
         self, name: str, attr_type: ATTRIBUTE_TYPE_CODE = ATTRIBUTE_TYPE_CODE.DATA
     ) -> AttributeCollection[Attribute]:
-        """Return the AttributeCollection of all attributes with the given name and attribute type.
+        """Return the :class:`~dissect.ntfs.util.AttributeCollection` of all attributes with the given name and attribute type.
 
         Args:
             name: The attribute name, often an empty string.
             attr_type: The attribute type to find.
 
         Raises:
             FileNotFoundError: If there are no attributes with the given name and type.
-        """
+        """  # noqa: E501
         attrs = self.attributes.find(name, attr_type)
         if not attrs:
             raise FileNotFoundError(f"No such stream on record {self}: ({name!r}, {attr_type})")
         return attrs
 
     def open(
         self,
@@ -417,15 +407,15 @@
         Raises:
             FileNotFoundError: If there are no attributes with the given name and type.
         """
         return self._get_stream_attributes(name, attr_type).size(allocated)
 
     def dataruns(
         self, name: str = "", attr_type: ATTRIBUTE_TYPE_CODE = ATTRIBUTE_TYPE_CODE.DATA
-    ) -> List[Tuple[int, int]]:
+    ) -> list[tuple[int, int]]:
         """Return the dataruns of the given stream name and type.
 
         Args:
             name: The stream name, an empty string for the "default" data stream.
             attr_type: The attribute type to get the dataruns of.
 
         Raises:
@@ -437,46 +427,46 @@
         """Return whether or not this record has attributes with the given name and type."""
         return bool(self.attributes.find(name, attr_type))
 
     def index(self, name: str) -> Index:
         """Open an index on this record.
 
         Args:
-            name: The index name to open. For example, "$I30".
+            name: The index name to open. For example, ``"$I30"``.
         """
         return Index(self, name)
 
     def iterdir(self, dereference: bool = False, ignore_dos: bool = False) -> Iterator[Union[IndexEntry, MftRecord]]:
         """Yield directory entries of this record.
 
         Args:
-            dereference: Determines whether to resolve the IndexEntry's to MftRecord's. This impacts performance.
+            dereference: Determines whether to resolve the :class:`~dissect.ntfs.index.IndexEntry`'s to :class:`MftRecord`'s. This impacts performance.
             ignore_dos: Ignore DOS file name entries.
 
         Raises:
             NotADirectoryError: If this record is not a directory.
-        """
+        """  # noqa: E501
         if not self.is_dir():
             raise NotADirectoryError(f"{self!r} is not a directory")
 
         for entry in self.index("$I30").entries():
             if ignore_dos and entry.attribute.flags == FILE_NAME_DOS:
                 continue
             yield entry.dereference() if dereference else entry
 
-    def listdir(self, dereference: bool = False, ignore_dos: bool = False) -> Dict[str, Union[IndexEntry, MftRecord]]:
+    def listdir(self, dereference: bool = False, ignore_dos: bool = False) -> dict[str, Union[IndexEntry, MftRecord]]:
         """Return a dictionary of the directory entries of this record.
 
         Args:
-            dereference: Determines whether to resolve the IndexEntry's to MftRecord's. This impacts performance.
+            dereference: Determines whether to resolve the :class:`~dissect.ntfs.index.IndexEntry`'s to :class:`MftRecord`'s. This impacts performance.
             ignore_dos: Ignore DOS file name entries.
 
         Raises:
             NotADirectoryError: If this record is not a directory.
-        """
+        """  # noqa: E501
         result = {}
         for entry in self.iterdir(dereference, ignore_dos):
             filenames = entry.filenames(ignore_dos) if dereference else [entry.attribute.file_name]
             for filename in filenames:
                 result[filename] = entry
 
         return result
```

### Comparing `dissect.ntfs-3.6.dev4/dissect/ntfs/ntfs.py` & `dissect.ntfs-3.7.dev1/dissect/ntfs/ntfs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from functools import cached_property
-from typing import BinaryIO, Iterator, List, Optional, Tuple
+from typing import BinaryIO, Iterator, Optional
 
 from dissect.ntfs.c_ntfs import (
     ATTRIBUTE_TYPE_CODE,
     DEFAULT_CLUSTER_SIZE,
     DEFAULT_INDEX_SIZE,
     DEFAULT_RECORD_SIZE,
     DEFAULT_SECTOR_SIZE,
@@ -19,23 +19,23 @@
 
 
 class NTFS:
     """Implementation for Microsoft NTFS.
 
     This implementation supports parsing NTFS from either a full NTFS volume or from separate files.
     If you have a file-like object of an NTFS volume, simply pass it as the fh argument. If you have separate
-    file-like objects for things like $BOOT or $MFT, pass those as the boot and mft arguments.
+    file-like objects for things like ``$BOOT`` or ``$MFT``, pass those as the boot and mft arguments.
     The separate arguments take precedence over parsing from the volume file-like object.
 
     Args:
         fh: A file-like object for the volume to use for parsing NTFS. This is where "data on disk" is read from.
-        boot: A file-like object for the $BOOT file.
-        mft: A file-like object for the $MFT file.
-        usnjrnl: A file-like object for the $Extend/$Usnjrnl:$J file.
-        sds: A file-like object for the $Secure:$SDS file.
+        boot: A file-like object for the ``$BOOT`` file.
+        mft: A file-like object for the ``$MFT`` file.
+        usnjrnl: A file-like object for the ``$Extend/$Usnjrnl:$J`` file.
+        sds: A file-like object for the ``$Secure:$SDS`` file.
     """
 
     def __init__(
         self,
         fh: Optional[BinaryIO] = None,
         boot: Optional[BinaryIO] = None,
         mft: Optional[BinaryIO] = None,
@@ -142,11 +142,11 @@
             volume_file = self.mft.get(FILE_NUMBER_VOLUME)
             volume_name = volume_file.attributes[ATTRIBUTE_TYPE_CODE.VOLUME_NAME].data()
             return volume_name.decode("utf-16-le")
         except (AttributeError, FileNotFoundError):
             return None
 
 
-def _get_dataruns_from_attribute_list(record: MftRecord) -> Iterator[List[Tuple[int, int]]]:
+def _get_dataruns_from_attribute_list(record: MftRecord) -> Iterator[list[tuple[int, int]]]:
     for attr in record.attributes[ATTRIBUTE_TYPE_CODE.ATTRIBUTE_LIST].attributes():
         if attr.type == ATTRIBUTE_TYPE_CODE.DATA:
             yield attr.dataruns()
```

### Comparing `dissect.ntfs-3.6.dev4/dissect/ntfs/secure.py` & `dissect.ntfs-3.7.dev1/dissect/ntfs/secure.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from dissect.util.sid import read_sid
 
 from dissect.ntfs.c_ntfs import ACE_TYPE, c_ntfs
 from dissect.ntfs.mft import MftRecord
 
 
 class Secure:
-    """Lookup security descriptors from the $Secure file, or optionally just a file-like object of the $SDS.
+    """Lookup security descriptors from the ``$Secure`` file, or optionally just a file-like object of the ``$SDS``.
 
-    Only one the record or sds arguments needs to be provided.
+    Only one the ``record`` or ``sds`` arguments needs to be provided.
 
     Args:
-        record: The MFT record of the $Secure file, used when opening from a full NTFS volume.
-        sds: A file-like object of the $SDS stream, used when opening from separate system files.
+        record: The MFT record of the ``$Secure`` file, used when opening from a full NTFS volume.
+        sds: A file-like object of the ``$SDS`` stream, used when opening from separate system files.
     """
 
     def __init__(self, record: MftRecord = None, sds: BinaryIO = None):
         self.record = record
         self.sds = None
         self.sii = None
 
@@ -64,15 +64,15 @@
             offset += entry.Length
             # Align to 16 bytes with some bit magic
             offset += -(offset) & 0xF
 
     def lookup(self, security_id: int) -> SecurityDescriptor:
         """Lookup a security descriptor by the security ID.
 
-        An index is used if available ($SII), otherwise we iterate all entries until we find the correct one.
+        An index is used if available (``$SII``), otherwise we iterate all entries until we find the correct one.
 
         Args:
             security_id: The security ID to lookup.
 
         Raises:
             KeyError: If the security ID can't be found.
         """
```

### Comparing `dissect.ntfs-3.6.dev4/dissect/ntfs/stream.py` & `dissect.ntfs-3.7.dev1/dissect/ntfs/stream.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import io
-from typing import BinaryIO, List, Tuple
+from typing import BinaryIO
 
 from dissect.util import lznt1
 from dissect.util.stream import RunlistStream
 
 
 class CompressedRunlistStream(RunlistStream):
-    """Specialized RunlistStream for reading NTFS compressed streams.
+    """Specialized :class:`~dissect.util.stream.RunlistStream` for reading NTFS compressed streams.
 
     Args:
         fh: The source file-like object.
         runlist: The runlist for this stream in block units.
         size: The size of the stream. This can be smaller than the total sum of blocks (to account for slack space).
         compression_unit: The compression unit of for this stream.
     """
 
     def __init__(
-        self, fh: BinaryIO, runlist: List[Tuple[int, int]], size: int, cluster_size: int, compression_unit: int
+        self, fh: BinaryIO, runlist: list[tuple[int, int]], size: int, cluster_size: int, compression_unit: int
     ):
         # RunlistStream has block_size but we want to make cluster_size available to be more in line with NTFS naming
         self.cluster_size = cluster_size
         self.compression_unit = compression_unit
         self.compression_unit_size = cluster_size << compression_unit
 
         self._cu_blocks = []
 
         # First use the compression_unit_size to set the alignment of AlignedStream
         super().__init__(fh, runlist, size, self.compression_unit_size)
         # This also sets the block_size of RunlistStream, so reset that to the correct cluster_size
         self.block_size = cluster_size
 
     @property
-    def runlist(self) -> List[Tuple[int, int]]:
+    def runlist(self) -> list[tuple[int, int]]:
         return self._runlist
 
     @runlist.setter
-    def runlist(self, runlist: List[Tuple[int, int]]) -> None:
+    def runlist(self, runlist: list[tuple[int, int]]) -> None:
         self._runlist = runlist
 
         runs = []
         block_num = 0
         current = 2**self.compression_unit
 
         # Build a list of aligned CU blocks
```

### Comparing `dissect.ntfs-3.6.dev4/dissect/ntfs/usnjrnl.py` & `dissect.ntfs-3.7.dev1/dissect/ntfs/usnjrnl.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from dissect.ntfs.util import ts_to_ns
 
 if TYPE_CHECKING:
     from dissect.ntfs.ntfs import NTFS
 
 
 class UsnJrnl:
-    """Parse the USN journal from a file-like object of the $UsnJrnl:$J stream.
+    """Parse the USN journal from a file-like object of the ``$UsnJrnl:$J`` stream.
 
     Args:
         fh: A file-like object of the $UsnJrnl:$J stream.
-        ntfs: An optional NTFS class instance, used for resolving file paths.
+        ntfs: An optional :class:`~dissect.ntfs.ntfs.NTFS` class instance, used for resolving file paths.
     """
 
     def __init__(self, fh: BinaryIO, ntfs: Optional[NTFS] = None):
         self.fh = fh
         self.ntfs = ntfs
 
     def records(self) -> Iterator[UsnRecord]:
@@ -63,15 +63,15 @@
                 offset += -(offset) & (8 - 1)
 
 
 class UsnRecord:
     """Parse a USN record from a file-like object and offset.
 
     Args:
-        usnjrnl: The ``UsnJrnl`` class this record is parsed from.
+        usnjrnl: The :class:`UsnJrnl` class this record is parsed from.
         fh: The file-like object to parse a USN record from.
         offset: The offset to parse a USN record at.
     """
 
     def __init__(self, usnjrnl: UsnJrnl, fh: BinaryIO, offset: int):
         self.usnjrnl = usnjrnl
         self.offset = offset
```

### Comparing `dissect.ntfs-3.6.dev4/dissect/ntfs/util.py` & `dissect.ntfs-3.7.dev1/dissect/ntfs/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import struct
 from collections import UserDict
-from typing import TYPE_CHECKING, Any, BinaryIO, List, Optional, Set, Tuple, Union
+from typing import TYPE_CHECKING, Any, BinaryIO, Optional, Union
 
 from dissect.cstruct import EnumInstance, Instance
 from dissect.util.stream import RunlistStream
 
 from dissect.ntfs.c_ntfs import (
     ATTRIBUTE_FLAG_COMPRESSION_MASK,
     ATTRIBUTE_TYPE_CODE,
@@ -24,22 +24,22 @@
     from dissect.ntfs.ntfs import NTFS
 
 
 class AttributeMap(UserDict):
     """Utility dictionary-like object for interacting with a collection of attributes.
 
     Allows convenient accessing of attributes added to this collection. For example:
-    - Get attributes by name, e.g. attributes.DATA to get all $DATA attributes.
-    - Get attributes by type code enum or integer, e.g. attributes[0x80] or attributes[ATTRIBUTE_TYPE_CODE.DATA].
-    - Check attribute membership by enum or integer, e.g. 0x80 in attributes or ATTRIBUTE_TYPE_CODE.DATA in attributes.
-    - Find all attributes with a given name and type, e.g. attributes.find("$I30", ATTRIBUTE_TYPE_CODE.INDEX_ROOT).
+    - Get attributes by name, e.g. ``attributes.DATA`` to get all ``$DATA`` attributes.
+    - Get attributes by type code enum or integer, e.g. ``attributes[0x80]`` or ``attributes[ATTRIBUTE_TYPE_CODE.DATA]``.
+    - Check attribute membership by enum or integer, e.g. ``0x80 in attributes`` or ``ATTRIBUTE_TYPE_CODE.DATA in attributes``.
+    - Find all attributes with a given name and type, e.g. ``attributes.find("$I30", ATTRIBUTE_TYPE_CODE.INDEX_ROOT)``.
 
     Note that any data retrieval from an ``AttributeMap`` will always succeed and return an
     :class:`~dissect.ntfs.util.AttributeCollection`, either empty or containing one or more attributes.
-    """
+    """  # noqa: E501
 
     def __getattr__(self, attr: str) -> AttributeCollection:
         if attr in ATTRIBUTE_TYPE_CODE:
             return self[ATTRIBUTE_TYPE_CODE[attr]]
 
         return super().__getattribute__(attr)
 
@@ -52,15 +52,15 @@
         if isinstance(key, EnumInstance):
             key = key.value
         return super().__contains__(key)
 
     def add(self, attr: Attribute) -> None:
         """Add an attribute to the collection.
 
-        Note that this is the only intended way to modify the ``AttributeMap``!
+        Note that this is the only intended way to modify the :class:`AttributeMap`!
 
         Args:
             attr: The attribute to add.
         """
         key = attr.header.type.value
         if key not in self:
             self[key] = AttributeCollection()
@@ -81,19 +81,19 @@
 
 
 class AttributeCollection(list):
     """Utility list-like object for interacting with a list of attributes.
 
     Allows convenient access to attribute properties for a list of one or more attributes.
 
-    For example, if we have only one attribute we want to access the "size", we want to be able
-    to do attribute_list.size instead of attribute_list[0].size.
+    For example, if we have only one attribute we want to access the ``size``, we want to be able
+    to do ``attribute_list.size`` instead of ``attribute_list[0].size``.
 
     Additionally, we can also provide functionality here that we want to perform on a group of
-    attributes, like open() and size().
+    attributes, like ``open()`` and ``size()``.
     """
 
     def __getattr__(self, attr: str) -> Any:
         if len(self) == 0:
             raise AttributeError("Attribute not found")
 
         if hasattr(self[0], attr):
@@ -150,40 +150,40 @@
         """
         if self.header.resident:
             return self.header.size
 
         attrs = self._get_stream_attrs()
         return attrs[0].header.allocated_size if allocated else attrs[0].header.size
 
-    def dataruns(self) -> List[Tuple[int, int]]:
+    def dataruns(self) -> list[tuple[int, int]]:
         """Get the dataruns for this list of attributes.
 
         Raises:
             TypeError: If attribute is resident.
         """
         if self.header.resident:
             raise TypeError("Attribute is resident and has no dataruns")
 
         return self._get_dataruns()
 
-    def _get_stream_attrs(self) -> List[Attribute]:
+    def _get_stream_attrs(self) -> list[Attribute]:
         return sorted((attr for attr in self if not attr.header.resident), key=lambda attr: attr.header.lowest_vcn)
 
-    def _get_dataruns(self, attrs: Optional[List[Attribute]] = None) -> List[Tuple[int, int]]:
+    def _get_dataruns(self, attrs: Optional[list[Attribute]] = None) -> list[tuple[int, int]]:
         attrs = attrs or self._get_stream_attrs()
 
         runs = []
         for attr in self._get_stream_attrs():
             runs += attr.header.dataruns()
 
         return runs
 
 
 def apply_fixup(data: bytes) -> bytes:
-    """Parse and apply fixup data from MULTI_SECTOR_HEADER to the given bytes.
+    """Parse and apply fixup data from ``MULTI_SECTOR_HEADER`` to the given bytes.
 
     Args:
         data: The bytes to fixup
 
     Returns:
         The fixed up bytes.
     """
@@ -221,24 +221,24 @@
     return bytes(data)
 
 
 def ensure_volume(ntfs: NTFS) -> None:
     """Check if a volume is available for reading.
 
     A volume in this context refers to a disk or other file that contains the raw NTFS data, not contained
-    in system files like the $MFT.
+    in system files like the ``$MFT``.
 
     Raises:
         VolumeNotAvailableError: If a volume is not available.
     """
     if not ntfs or not ntfs.fh:
         raise VolumeNotAvailableError()
 
 
-def get_full_path(mft: Mft, name: str, parent: Instance, seen: Set[str] = None) -> str:
+def get_full_path(mft: Mft, name: str, parent: Instance, seen: set[str] = None) -> str:
     """Walk up parent file references to construct a full path.
 
     Args:
         mft: The MFT object to use for looking up file references.
         name: The file name to use.
         parent: The parent reference to start backtracking from.
```

### Comparing `dissect.ntfs-3.6.dev4/dissect.ntfs.egg-info/PKG-INFO` & `dissect.ntfs-3.7.dev1/dissect.ntfs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.ntfs
-Version: 3.6.dev4
+Version: 3.7.dev1
 Summary: A Dissect module implementing a parser for the NTFS file system, used by the Windows operating system
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.ntfs
 Project-URL: repository, https://github.com/fox-it/dissect.ntfs
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.ntfs-3.6.dev4/dissect.ntfs.egg-info/SOURCES.txt` & `dissect.ntfs-3.7.dev1/dissect.ntfs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/pyproject.toml` & `dissect.ntfs-3.7.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/tests/conftest.py` & `dissect.ntfs-3.7.dev1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/tests/data/boot_2m.bin.gz` & `dissect.ntfs-3.7.dev1/tests/data/boot_2m.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/tests/data/mft.bin.gz` & `dissect.ntfs-3.7.dev1/tests/data/mft.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/tests/data/ntfs.bin.gz` & `dissect.ntfs-3.7.dev1/tests/data/ntfs.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/tests/data/ntfs_fragmented_mft.csv.gz` & `dissect.ntfs-3.7.dev1/tests/data/ntfs_fragmented_mft.csv.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/tests/data/sds.bin.gz` & `dissect.ntfs-3.7.dev1/tests/data/sds.bin.gz`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/tests/docs/Makefile` & `dissect.ntfs-3.7.dev1/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/tests/docs/conf.py` & `dissect.ntfs-3.7.dev1/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/tests/test_attr.py` & `dissect.ntfs-3.7.dev1/tests/test_attr.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/tests/test_index.py` & `dissect.ntfs-3.7.dev1/tests/test_index.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/tests/test_mft.py` & `dissect.ntfs-3.7.dev1/tests/test_mft.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/tests/test_ntfs.py` & `dissect.ntfs-3.7.dev1/tests/test_ntfs.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/tests/test_secure.py` & `dissect.ntfs-3.7.dev1/tests/test_secure.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/tests/test_usnjrnl.py` & `dissect.ntfs-3.7.dev1/tests/test_usnjrnl.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/tests/test_util.py` & `dissect.ntfs-3.7.dev1/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dissect.ntfs-3.6.dev4/tox.ini` & `dissect.ntfs-3.7.dev1/tox.ini`

 * *Files identical despite different names*

