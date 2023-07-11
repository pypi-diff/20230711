# Comparing `tmp/lvhao_lib-0.7.0.tar.gz` & `tmp/lvhao_lib-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lvhao_lib-0.7.0.tar", max compression
+gzip compressed data, was "lvhao_lib-0.7.1.tar", max compression
```

## Comparing `lvhao_lib-0.7.0.tar` & `lvhao_lib-0.7.1.tar`

### file list

```diff
@@ -1,10 +1,21 @@
--rw-r--r--   0        0        0        0 2023-07-10 04:36:58.117404 lvhao_lib-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-07-10 04:36:58.117367 lvhao_lib-0.7.0/lvhao_lib/__init__.py
--rw-r--r--   0        0        0  1368592 2023-07-06 23:47:26.000000 lvhao_lib-0.7.0/lvhao_lib/lib/linux_x86_64/libpnd.so
--rw-r--r--   0        0        0  1368592 2023-07-06 23:47:26.000000 lvhao_lib-0.7.0/lvhao_lib/lib/linux_x86_64/libpnd.so.1.0.0
--rw-r--r--   0        0        0  1004584 2023-07-06 23:48:36.000000 lvhao_lib-0.7.0/lvhao_lib/lib/mac_x86_64/libpnd.1.0.0.dylib
--rw-r--r--   0        0        0  1004584 2023-07-06 23:48:38.000000 lvhao_lib-0.7.0/lvhao_lib/lib/mac_x86_64/libpnd.dylib
--rw-r--r--   0        0        0   639488 2023-07-06 23:49:48.000000 lvhao_lib-0.7.0/lvhao_lib/lib/win_x64/pnd.dll
--rw-r--r--   0        0        0    10122 2023-07-06 23:49:48.000000 lvhao_lib-0.7.0/lvhao_lib/lib/win_x64/pnd.lib
--rw-r--r--   0        0        0      298 2023-07-10 04:38:18.996765 lvhao_lib-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      331 1970-01-01 00:00:00.000000 lvhao_lib-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-10 04:36:58.117404 lvhao_lib-0.7.1/README.md
+-rw-r--r--   0        0        0       68 2023-07-10 08:16:49.804310 lvhao_lib-0.7.1/lvhao_lib/__init__.py
+-rw-r--r--   0        0        0    24606 2023-07-10 11:00:09.937636 lvhao_lib-0.7.1/lvhao_lib/_pnd.c
+-rwxr-xr-x   0        0        0    51688 2023-07-11 07:00:41.209921 lvhao_lib-0.7.1/lvhao_lib/_pnd.cpython-310-darwin.so
+-rw-r--r--   0        0        0    15592 2023-07-11 07:00:39.284585 lvhao_lib-0.7.1/lvhao_lib/_pnd.o
+-rw-r--r--   0        0        0    19302 2023-07-10 10:59:34.217123 lvhao_lib-0.7.1/lvhao_lib/pnd/include/aios copy.h
+-rw-r--r--   0        0        0    19189 2023-07-10 11:00:56.944152 lvhao_lib-0.7.1/lvhao_lib/pnd/include/aios.h
+-rwxr-xr-x   0        0        0   938463 2023-07-10 07:33:38.000000 lvhao_lib-0.7.1/lvhao_lib/pnd/lib/darwin_arm64/libpnd.1.0.0.dylib
+-rwxr-xr-x   0        0        0   938463 2023-07-10 07:33:38.000000 lvhao_lib-0.7.1/lvhao_lib/pnd/lib/darwin_arm64/libpnd.dylib
+-rw-r--r--   0        0        0  1004584 2023-07-09 23:12:22.000000 lvhao_lib-0.7.1/lvhao_lib/pnd/lib/darwin_x86_64/libpnd.1.0.0.dylib
+-rw-r--r--   0        0        0  1004584 2023-07-09 23:12:22.000000 lvhao_lib-0.7.1/lvhao_lib/pnd/lib/darwin_x86_64/libpnd.dylib
+-rw-r--r--   0        0        0  1368592 2023-07-09 23:12:18.000000 lvhao_lib-0.7.1/lvhao_lib/pnd/lib/linux_x86_64/libpnd.so
+-rw-r--r--   0        0        0  1368592 2023-07-09 23:12:18.000000 lvhao_lib-0.7.1/lvhao_lib/pnd/lib/linux_x86_64/libpnd.so.1.0.0
+-rw-r--r--   0        0        0   639488 2023-07-09 23:14:04.000000 lvhao_lib-0.7.1/lvhao_lib/pnd/lib/win_x64/pnd.dll
+-rw-r--r--   0        0        0    10122 2023-07-09 23:14:04.000000 lvhao_lib-0.7.1/lvhao_lib/pnd/lib/win_x64/pnd.lib
+-rw-r--r--   0        0        0        0 2023-07-10 05:51:02.552786 lvhao_lib-0.7.1/lvhao_lib/src/__init__.py
+-rw-r--r--   0        0        0    11112 2023-07-11 05:28:58.441961 lvhao_lib-0.7.1/lvhao_lib/src/loader.py
+-rw-r--r--   0        0        0    13509 2023-07-11 05:26:18.004135 lvhao_lib-0.7.1/lvhao_lib/src/log/fourier_server_log.txt
+-rw-r--r--   0        0        0       32 2023-07-10 05:50:27.543156 lvhao_lib-0.7.1/lvhao_lib/src/lookup.py
+-rw-r--r--   0        0        0      475 2023-07-11 07:03:58.887132 lvhao_lib-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      369 1970-01-01 00:00:00.000000 lvhao_lib-0.7.1/PKG-INFO
```

### Comparing `lvhao_lib-0.7.0/lvhao_lib/lib/linux_x86_64/libpnd.so` & `lvhao_lib-0.7.1/lvhao_lib/pnd/lib/linux_x86_64/libpnd.so`

 * *Files identical despite different names*

### Comparing `lvhao_lib-0.7.0/lvhao_lib/lib/linux_x86_64/libpnd.so.1.0.0` & `lvhao_lib-0.7.1/lvhao_lib/pnd/lib/linux_x86_64/libpnd.so.1.0.0`

 * *Files identical despite different names*

### Comparing `lvhao_lib-0.7.0/lvhao_lib/lib/mac_x86_64/libpnd.1.0.0.dylib` & `lvhao_lib-0.7.1/lvhao_lib/pnd/lib/darwin_x86_64/libpnd.1.0.0.dylib`

 * *Files 0% similar despite different names*

#### strings -a -n 8 {}

```diff
@@ -9,15 +9,15 @@
 __thread_ptrs
 __thread_bss
 __common
 __LINKEDIT
 @rpath/libpnd.1.0.0.dylib
 /usr/lib/libc++.1.dylib
 /usr/lib/libSystem.B.dylib
-/Users/runner/work/pnd-cpp/pnd-cpp/pnd/lib/mac_x86_64
+/Users/runner/work/pnd-cpp/pnd-cpp/pnd/lib/darwin_x86_64
 AWAVAUATSH
 [A\A]A^A_]
 AWAVAUATSPD
 UUUUUUUUH!
 33333333H
 [A\A]A^A_]
 AWAVAUATSPI
```

#### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 dynamically linked shared library, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL|WEAK_DEFINES|BINDS_TO_WEAK|NO_REEXPORTED_DYLIBS|HAS_TLV_DESCRIPTORS>*

```diff
@@ -101,30 +101,30 @@
 00000640: 10f1 0a00 385f 0000 0200 0000 1800 0000  ....8_..........
 00000650: c85a 0b00 1b0c 0000 2029 0c00 082b 0300  .Z...... )...+..
 00000660: 0b00 0000 5000 0000 0000 0000 1108 0000  ....P...........
 00000670: 1108 0000 bc02 0000 cd0a 0000 4e01 0000  ............N...
 00000680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000690: 0000 0000 0000 0000 781c 0c00 2903 0000  ........x...)...
 000006a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006b0: 1b00 0000 1800 0000 7eed d27f e09f 3766  ........~.....7f
-000006c0: 9622 28c4 39c8 4036 3200 0000 2000 0000  ."(.9.@62... ...
+000006b0: 1b00 0000 1800 0000 4dce b0e6 0edd 34d7  ........M.....4.
+000006c0: 9e9e 1cbf 325e a486 3200 0000 2000 0000  ....2^..2... ...
 000006d0: 0100 0000 0006 0c00 0001 0d00 0100 0000  ................
 000006e0: 0300 0000 0001 3403 2a00 0000 1000 0000  ......4.*.......
 000006f0: 0000 0000 0000 0000 0c00 0000 3000 0000  ............0...
 00000700: 1800 0000 0200 0000 0024 1405 0000 0100  .........$......
 00000710: 2f75 7372 2f6c 6962 2f6c 6962 632b 2b2e  /usr/lib/libc++.
 00000720: 312e 6479 6c69 6200 0c00 0000 3800 0000  1.dylib.....8...
 00000730: 1800 0000 0200 0000 0000 2705 0000 0100  ..........'.....
 00000740: 2f75 7372 2f6c 6962 2f6c 6962 5379 7374  /usr/lib/libSyst
 00000750: 656d 2e42 2e64 796c 6962 0000 0000 0000  em.B.dylib......
 00000760: 1c00 0080 4800 0000 0c00 0000 2f55 7365  ....H......./Use
 00000770: 7273 2f72 756e 6e65 722f 776f 726b 2f70  rs/runner/work/p
 00000780: 6e64 2d63 7070 2f70 6e64 2d63 7070 2f70  nd-cpp/pnd-cpp/p
-00000790: 6e64 2f6c 6962 2f6d 6163 5f78 3836 5f36  nd/lib/mac_x86_6
-000007a0: 3400 0000 0000 0000 2600 0000 1000 0000  4.......&.......
+00000790: 6e64 2f6c 6962 2f64 6172 7769 6e5f 7838  nd/lib/darwin_x8
+000007a0: 365f 3634 0000 0000 2600 0000 1000 0000  6_64....&.......
 000007b0: 4850 0b00 f008 0000 2900 0000 1000 0000  HP......).......
 000007c0: 3859 0b00 9001 0000 0000 0000 0000 0000  8Y..............
 000007d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000800: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `lvhao_lib-0.7.0/lvhao_lib/lib/mac_x86_64/libpnd.dylib` & `lvhao_lib-0.7.1/lvhao_lib/pnd/lib/darwin_x86_64/libpnd.dylib`

 * *Files 0% similar despite different names*

#### strings -a -n 8 {}

```diff
@@ -9,15 +9,15 @@
 __thread_ptrs
 __thread_bss
 __common
 __LINKEDIT
 @rpath/libpnd.1.0.0.dylib
 /usr/lib/libc++.1.dylib
 /usr/lib/libSystem.B.dylib
-/Users/runner/work/pnd-cpp/pnd-cpp/pnd/lib/mac_x86_64
+/Users/runner/work/pnd-cpp/pnd-cpp/pnd/lib/darwin_x86_64
 AWAVAUATSH
 [A\A]A^A_]
 AWAVAUATSPD
 UUUUUUUUH!
 33333333H
 [A\A]A^A_]
 AWAVAUATSPI
```

#### x86_64

 * *Format-specific differences are supported for this file format but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Mach-O 64-bit x86_64 dynamically linked shared library, flags:<NOUNDEFS|DYLDLINK|TWOLEVEL|WEAK_DEFINES|BINDS_TO_WEAK|NO_REEXPORTED_DYLIBS|HAS_TLV_DESCRIPTORS>*

```diff
@@ -101,30 +101,30 @@
 00000640: 10f1 0a00 385f 0000 0200 0000 1800 0000  ....8_..........
 00000650: c85a 0b00 1b0c 0000 2029 0c00 082b 0300  .Z...... )...+..
 00000660: 0b00 0000 5000 0000 0000 0000 1108 0000  ....P...........
 00000670: 1108 0000 bc02 0000 cd0a 0000 4e01 0000  ............N...
 00000680: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000690: 0000 0000 0000 0000 781c 0c00 2903 0000  ........x...)...
 000006a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000006b0: 1b00 0000 1800 0000 7eed d27f e09f 3766  ........~.....7f
-000006c0: 9622 28c4 39c8 4036 3200 0000 2000 0000  ."(.9.@62... ...
+000006b0: 1b00 0000 1800 0000 4dce b0e6 0edd 34d7  ........M.....4.
+000006c0: 9e9e 1cbf 325e a486 3200 0000 2000 0000  ....2^..2... ...
 000006d0: 0100 0000 0006 0c00 0001 0d00 0100 0000  ................
 000006e0: 0300 0000 0001 3403 2a00 0000 1000 0000  ......4.*.......
 000006f0: 0000 0000 0000 0000 0c00 0000 3000 0000  ............0...
 00000700: 1800 0000 0200 0000 0024 1405 0000 0100  .........$......
 00000710: 2f75 7372 2f6c 6962 2f6c 6962 632b 2b2e  /usr/lib/libc++.
 00000720: 312e 6479 6c69 6200 0c00 0000 3800 0000  1.dylib.....8...
 00000730: 1800 0000 0200 0000 0000 2705 0000 0100  ..........'.....
 00000740: 2f75 7372 2f6c 6962 2f6c 6962 5379 7374  /usr/lib/libSyst
 00000750: 656d 2e42 2e64 796c 6962 0000 0000 0000  em.B.dylib......
 00000760: 1c00 0080 4800 0000 0c00 0000 2f55 7365  ....H......./Use
 00000770: 7273 2f72 756e 6e65 722f 776f 726b 2f70  rs/runner/work/p
 00000780: 6e64 2d63 7070 2f70 6e64 2d63 7070 2f70  nd-cpp/pnd-cpp/p
-00000790: 6e64 2f6c 6962 2f6d 6163 5f78 3836 5f36  nd/lib/mac_x86_6
-000007a0: 3400 0000 0000 0000 2600 0000 1000 0000  4.......&.......
+00000790: 6e64 2f6c 6962 2f64 6172 7769 6e5f 7838  nd/lib/darwin_x8
+000007a0: 365f 3634 0000 0000 2600 0000 1000 0000  6_64....&.......
 000007b0: 4850 0b00 f008 0000 2900 0000 1000 0000  HP......).......
 000007c0: 3859 0b00 9001 0000 0000 0000 0000 0000  8Y..............
 000007d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000007f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000800: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000810: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `lvhao_lib-0.7.0/lvhao_lib/lib/win_x64/pnd.dll` & `lvhao_lib-0.7.1/lvhao_lib/pnd/lib/win_x64/pnd.dll`

 * *Files 0% similar despite different names*

#### objdump

```diff
@@ -4,15 +4,15 @@
 start address 0x0000000180073f20
 
 Characteristics 0x2022
 	executable
 	large address aware
 	DLL
 
-Time/Date		Fri Jul  7 07:49:40 2023
+Time/Date		Mon Jul 10 07:14:02 2023
 Magic			020b	(PE32+)
 MajorLinkerVersion	14
 MinorLinkerVersion	35
 SizeOfCode		0000000000077c00
 SizeOfInitializedData	00000000002be200
 SizeOfUninitializedData	0000000000000000
 AddressOfEntryPoint	0000000000073f20
@@ -166167,20 +166167,17 @@
    18008095e:	add    %al,(%rax)
    180080960:	or     %bl,0x18007(%rax)
    180080966:	add    %al,(%rax)
    180080968:	adc    %bl,0x18007(%rax)
    18008096e:	add    %al,(%rax)
    180080970:	add    %al,(%rax)
    180080972:	add    %al,(%rax)
-   180080974:	xchg   %eax,%esp
-   180080975:	ret
-   180080976:	cmpsl  %es:(%rdi),%ds:(%rsi)
-   180080977:	add    %al,%fs:(%rax)
-   18008097a:	add    %al,(%rax)
-   18008097c:	or     $0x78000000,%eax
+   180080974:	mov    $0x64abaf,%edx
+   180080979:	add    %al,(%rax)
+   18008097b:	add    %cl,0x78000000(%rip)        # 0x1f8080981
    180080981:	add    (%rax),%eax
    180080983:	add    %dh,%ah
    180080985:	(bad)
    180080986:	or     %al,(%rax)
    180080988:	hlt
    180080989:	push   %rcx
    18008098a:	or     %al,(%rax)
```

### Comparing `lvhao_lib-0.7.0/lvhao_lib/lib/win_x64/pnd.lib` & `lvhao_lib-0.7.1/lvhao_lib/pnd/lib/win_x64/pnd.lib`

 * *Files identical despite different names*

