# Comparing `tmp/spwn-1.2.4.tar.gz` & `tmp/spwn-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spwn-1.2.4.tar", last modified: Tue Apr 18 14:32:45 2023, max compression
+gzip compressed data, was "spwn-1.2.5.tar", last modified: Tue Jul 11 18:41:59 2023, max compression
```

## Comparing `spwn-1.2.4.tar` & `spwn-1.2.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 14:32:45.111154 spwn-1.2.4/
--rw-r--r--   0 marco     (1000) marco     (1000)     1071 2023-04-12 12:46:15.000000 spwn-1.2.4/LICENSE
--rw-r--r--   0 marco     (1000) marco     (1000)     7372 2023-04-18 14:32:45.111154 spwn-1.2.4/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)     6916 2023-04-18 13:24:55.000000 spwn-1.2.4/README.md
--rw-r--r--   0 marco     (1000) marco     (1000)       38 2023-04-18 14:32:45.111154 spwn-1.2.4/setup.cfg
--rw-r--r--   0 marco     (1000) marco     (1000)      691 2023-04-18 13:43:37.000000 spwn-1.2.4/setup.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 14:32:45.111154 spwn-1.2.4/spwn/
--rw-r--r--   0 marco     (1000) marco     (1000)        0 2023-04-12 12:46:15.000000 spwn-1.2.4/spwn/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     3952 2023-04-17 13:18:21.000000 spwn-1.2.4/spwn/analyzer.py
--rw-r--r--   0 marco     (1000) marco     (1000)      296 2023-04-12 12:46:15.000000 spwn-1.2.4/spwn/binary.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2459 2023-04-18 12:27:58.000000 spwn-1.2.4/spwn/configgenerator.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1189 2023-04-18 12:31:23.000000 spwn-1.2.4/spwn/configmanager.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1966 2023-04-12 12:46:15.000000 spwn-1.2.4/spwn/customanalyzer.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4015 2023-04-12 12:46:15.000000 spwn-1.2.4/spwn/filemanager.py
--rw-r--r--   0 marco     (1000) marco     (1000)     1493 2023-04-12 12:46:15.000000 spwn-1.2.4/spwn/libc.py
--rw-r--r--   0 marco     (1000) marco     (1000)      112 2023-04-12 12:46:15.000000 spwn-1.2.4/spwn/loader.py
--rw-r--r--   0 marco     (1000) marco     (1000)     4250 2023-04-18 13:12:59.000000 spwn-1.2.4/spwn/scripter.py
--rw-r--r--   0 marco     (1000) marco     (1000)     6275 2023-04-18 13:22:39.000000 spwn-1.2.4/spwn/spwn.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2784 2023-04-12 12:46:15.000000 spwn-1.2.4/spwn/utils.py
-drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-04-18 14:32:45.111154 spwn-1.2.4/spwn.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)     7372 2023-04-18 14:32:45.000000 spwn-1.2.4/spwn.egg-info/PKG-INFO
--rw-r--r--   0 marco     (1000) marco     (1000)      406 2023-04-18 14:32:45.000000 spwn-1.2.4/spwn.egg-info/SOURCES.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        1 2023-04-18 14:32:45.000000 spwn-1.2.4/spwn.egg-info/dependency_links.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       40 2023-04-18 14:32:45.000000 spwn-1.2.4/spwn.egg-info/entry_points.txt
--rw-r--r--   0 marco     (1000) marco     (1000)       21 2023-04-18 14:32:45.000000 spwn-1.2.4/spwn.egg-info/requires.txt
--rw-r--r--   0 marco     (1000) marco     (1000)        5 2023-04-18 14:32:45.000000 spwn-1.2.4/spwn.egg-info/top_level.txt
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-07-11 18:41:59.106535 spwn-1.2.5/
+-rw-r--r--   0 marco     (1000) marco     (1000)     1071 2023-06-01 23:33:50.000000 spwn-1.2.5/LICENSE
+-rw-r--r--   0 marco     (1000) marco     (1000)     7374 2023-07-11 18:41:59.106535 spwn-1.2.5/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)     6918 2023-06-01 23:33:50.000000 spwn-1.2.5/README.md
+-rw-r--r--   0 marco     (1000) marco     (1000)       38 2023-07-11 18:41:59.106535 spwn-1.2.5/setup.cfg
+-rw-r--r--   0 marco     (1000) marco     (1000)      691 2023-07-11 18:38:35.000000 spwn-1.2.5/setup.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-07-11 18:41:59.106535 spwn-1.2.5/spwn/
+-rw-r--r--   0 marco     (1000) marco     (1000)        0 2023-06-01 23:33:50.000000 spwn-1.2.5/spwn/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     3921 2023-07-11 18:34:00.000000 spwn-1.2.5/spwn/analyzer.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      296 2023-06-01 23:33:50.000000 spwn-1.2.5/spwn/binary.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2463 2023-07-11 18:27:44.000000 spwn-1.2.5/spwn/configgenerator.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1189 2023-06-01 23:33:50.000000 spwn-1.2.5/spwn/configmanager.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1963 2023-06-01 23:33:50.000000 spwn-1.2.5/spwn/customanalyzer.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4426 2023-06-01 23:33:50.000000 spwn-1.2.5/spwn/filemanager.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     1493 2023-06-01 23:33:50.000000 spwn-1.2.5/spwn/libc.py
+-rw-r--r--   0 marco     (1000) marco     (1000)      112 2023-06-01 23:33:50.000000 spwn-1.2.5/spwn/loader.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     4250 2023-06-01 23:33:50.000000 spwn-1.2.5/spwn/scripter.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     6584 2023-06-01 23:33:50.000000 spwn-1.2.5/spwn/spwn.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2774 2023-06-01 23:33:50.000000 spwn-1.2.5/spwn/utils.py
+drwxr-xr-x   0 marco     (1000) marco     (1000)        0 2023-07-11 18:41:59.106535 spwn-1.2.5/spwn.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     7374 2023-07-11 18:41:59.000000 spwn-1.2.5/spwn.egg-info/PKG-INFO
+-rw-r--r--   0 marco     (1000) marco     (1000)      406 2023-07-11 18:41:59.000000 spwn-1.2.5/spwn.egg-info/SOURCES.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        1 2023-07-11 18:41:59.000000 spwn-1.2.5/spwn.egg-info/dependency_links.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       40 2023-07-11 18:41:59.000000 spwn-1.2.5/spwn.egg-info/entry_points.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)       21 2023-07-11 18:41:59.000000 spwn-1.2.5/spwn.egg-info/requires.txt
+-rw-r--r--   0 marco     (1000) marco     (1000)        5 2023-07-11 18:41:59.000000 spwn-1.2.5/spwn.egg-info/top_level.txt
```

### Comparing `spwn-1.2.4/LICENSE` & `spwn-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spwn-1.2.4/PKG-INFO` & `spwn-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spwn
-Version: 1.2.4
+Version: 1.2.5
 Summary: Automatic tool to quickly start a pwn CTF challenge
 Home-page: https://github.com/MarcoMeinardi/spwn
 Author: Chino
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
@@ -165,17 +165,17 @@
 ```python
 def main(files):
     print(f"The binary is {files.binary.name}")
 ```
 
 ### Decompiler
 For the decompilers commands, the syntax is the same of the pre and
-post analysis commands. I created an apposite config, rather than
+post analysis commands. I created a special config, rather than
 putting it in a pre analysis command, because I use IDA freeware
-and it can decompile only x86-64 binaries, so I have to use another
+and it can decompile only x86/x86_64 binaries, so I have to use another
 decompiler for other architectures (I have created this feature
 before the custom scripts thing, but since the decompiler is
 something that you will almost always launch, I left it to make
 it easier to use). If you want to use always the same decompiler,
 leave `idafree_command` empty and if you don't want to launch any
 decompiler, just leave both configs empty. If you wish to modify
 the conditions to select the decompiler, you can either modify
```

### Comparing `spwn-1.2.4/README.md` & `spwn-1.2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -151,17 +151,17 @@
 ```python
 def main(files):
     print(f"The binary is {files.binary.name}")
 ```
 
 ### Decompiler
 For the decompilers commands, the syntax is the same of the pre and
-post analysis commands. I created an apposite config, rather than
+post analysis commands. I created a special config, rather than
 putting it in a pre analysis command, because I use IDA freeware
-and it can decompile only x86-64 binaries, so I have to use another
+and it can decompile only x86/x86_64 binaries, so I have to use another
 decompiler for other architectures (I have created this feature
 before the custom scripts thing, but since the decompiler is
 something that you will almost always launch, I left it to make
 it easier to use). If you want to use always the same decompiler,
 leave `idafree_command` empty and if you don't want to launch any
 decompiler, just leave both configs empty. If you wish to modify
 the conditions to select the decompiler, you can either modify
```

### Comparing `spwn-1.2.4/setup.py` & `spwn-1.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md") as f:
 	long_description = f.read()
 
 setuptools.setup(
 	name="spwn",
-	version="1.2.4",
+	version="1.2.5",
 	author="Chino",
 	description="Automatic tool to quickly start a pwn CTF challenge",
 	long_description=long_description,
 	long_description_content_type="text/markdown",
 	classifiers=[
 		"Environment :: Console",
 		"Operating System :: POSIX :: Linux",
```

### Comparing `spwn-1.2.4/spwn/analyzer.py` & `spwn-1.2.5/spwn/analyzer.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 			print("[!] yara found something")
 			for match in matches:
 				addresses = [instance.offset for string_match in match.strings for instance in string_match.instances]
 				print(f'[*] {match.rule} at {", ".join(map(hex, addresses))}')
 			print()
 
 	def open_decompiler(self) -> None:
-		if self.configs.idafree_command and self.files.binary.pwnfile.arch == "amd64" and self.files.binary.pwnfile.bits == 64:
+		if self.configs.idafree_command and self.files.binary.pwnfile.arch in ["amd64", "i386"]:
 			subprocess.Popen(self.configs.idafree_command.format(binary=self.files.binary.name), shell=True, start_new_session=True)
 		elif self.configs.decompiler_command:
 			subprocess.Popen(self.configs.decompiler_command.format(binary=self.files.binary.name), shell=True, start_new_session=True)
 
 	def check_and_print_seccomp(self) -> None:
 		for function in self.files.binary.pwnfile.sym:
 			if "seccomp" in function or "prctl" in function:
```

### Comparing `spwn-1.2.4/spwn/configgenerator.py` & `spwn-1.2.5/spwn/configgenerator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import requests
 import json
 
 
 default_configs = {
-	"debug_dir": "debug",
+	"debug_dir": "debug_dir",
 	"script_file": "a.py",
 	"pwn_process": "r",
 	"tab": "\t",
 	"template_file": "~/.config/spwn/template.py",
 	"custom_template_prefix": "template_",
 	"suppress_warnings": False,
 	"yara_rules": "~/.config/spwn/findcrypt3.rules",
```

### Comparing `spwn-1.2.4/spwn/configmanager.py` & `spwn-1.2.5/spwn/configmanager.py`

 * *Files identical despite different names*

### Comparing `spwn-1.2.4/spwn/customanalyzer.py` & `spwn-1.2.5/spwn/customanalyzer.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 	def run_command(self, command: str, timeout: int | bool | None) -> None:
 		command = command.format(binary=self.files.binary.name, debug_binary=self.files.binary.debug_name)
 		if timeout is not False:
 			print(f"[*] {command}")
 			if timeout:
 				try:
-					# Use `exec command``, otherwise, because of `shell=True`, the process wouldn't be killed on timeout
+					# Use `exec command`, otherwise, because of `shell=True`, the process won't get killed on timeout
 					p = subprocess.run(f"exec {command}", shell=True, timeout=timeout, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding="latin-1")
 					print(p.stdout)
 				except subprocess.TimeoutExpired:
 					print("[!] Timeout")
 			else:
 				p = subprocess.run(command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding="latin-1")
 				print(p.stdout)
```

### Comparing `spwn-1.2.4/spwn/filemanager.py` & `spwn-1.2.5/spwn/filemanager.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	def __init__(self, configs: ConfigManager):
 		self.configs = configs
 		self.binary = None
 		self.libc = None
 		self.loader = None
 		self.other_binaries = []
 
-	def auto_recognize(self) -> None:
+	def auto_recognize(self, maybe_has_debug: bool) -> None:
 		binaries = []
 		libcs = []
 		loaders = []
 		other_libraries = []
 		files = list(filter(lambda x: pwn.platform.architecture(x)[1] == "ELF", os.listdir()))
 		self.other_binaries = files
 		if not files:
@@ -45,33 +45,40 @@
 		elif len(binaries) > 1:
 			self.binary = utils.ask_list_delete("Select binary", binaries, can_skip=False)
 			self.binary = Binary(self.binary)
 			other_libraries.extend(binaries)
 		else:
 			self.ask_all(files)
 			return
+		del files[files.index(self.binary.name)]
 
 		# Libc
-		del files[files.index(self.binary.name)]
 		if len(libcs) == 1:
 			self.libc = Libc(libcs[0])
 		else:
 			libcs.extend(other_libraries)
 			if not libcs:
 				return
 
 			self.libc = utils.ask_list_delete("Select libc", libcs, can_skip=True)
 			if self.libc is None:
 				return
 			self.libc = Libc(self.libc)
 
 			other_libraries = libcs
+		del files[files.index(self.libc.name)]
+
+		if maybe_has_debug:
+			if os.path.exists(self.configs.debug_dir):
+				if os.path.exists(os.path.join(self.configs.debug_dir, self.binary.name)):
+					self.binary.debug_name = os.path.join(self.configs.debug_dir, self.binary.name)
+				if os.path.exists(os.path.join(self.configs.debug_dir, "libc.so.6")):
+					self.libc.debug_name = os.path.join(self.configs.debug_dir, self.libc.name)
 
 		# Loader
-		del files[files.index(self.libc.name)]
 		if len(loaders) == 1:
 			self.loader = Loader(loaders[0])
 		else:
 			if not loaders:
 				return
 			self.loader = utils.ask_list_delete("Select loader", loaders, can_skip=True)
 			if self.loader:
```

### Comparing `spwn-1.2.4/spwn/libc.py` & `spwn-1.2.5/spwn/libc.py`

 * *Files identical despite different names*

### Comparing `spwn-1.2.4/spwn/scripter.py` & `spwn-1.2.5/spwn/scripter.py`

 * *Files identical despite different names*

### Comparing `spwn-1.2.4/spwn/spwn.py` & `spwn-1.2.5/spwn/spwn.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import argparse
 import os
 import shutil
 import sys
 
-sys.argv.append("NOTERM")  # HACK to prevent pwntools to messup the terminal, the added arg will be removed by pwnlib
+sys.argv = ["NOTERM"] + sys.argv  # HACK to prevent pwntools to messup the terminal, the added arg will be removed by pwnlib
 
 from spwn.filemanager import FileManager
 from spwn.analyzer import Analyzer
 from spwn.scripter import Scripter
 from spwn.configmanager import ConfigManager
 from spwn.customanalyzer import CustomAnalyzer
 from spwn.configgenerator import ConfigGenerator
 
 
 CONFIG_PATH = os.path.expanduser("~/.config/spwn/config.json")
 
 
 class Spwn:
-	def __init__(self, create_interactions: bool = False, interactions_only: bool = False, no_decompiler: bool = True):
+	def __init__(self, create_interactions: bool, no_decompiler: bool, script_only: bool, interactions_only: bool):
 		if not interactions_only:
-			self.create_interactions = create_interactions
+			self.create_interactions = create_interactions or script_only
 			self.no_decompiler = no_decompiler
+			self.script_only = script_only
 			self.check_dependencies()
 			self.files = FileManager(configs)
-			self.files.auto_recognize()
+			self.files.auto_recognize(self.script_only)
 
 			print("[*] Binary:", self.files.binary.name)
 			if self.files.libc: print("[*] Libc:  ", self.files.libc.name)
 			else: print("[!] No libc")
 			if self.files.loader: print("[*] Loader:", self.files.loader.name)
 			else: print("[!] No loader")
 			if self.files.other_binaries: print("[*] Other: ", self.files.other_binaries)
@@ -35,46 +36,47 @@
 		else:
 			self.files = None
 
 		self.run()
 
 	def run(self) -> None:
 		if self.files:
-			analyzer = Analyzer(configs, self.files)
-			custom_analyzer = CustomAnalyzer(configs, self.files)
-			analyzer.pre_analysis(open_decompiler=not self.no_decompiler)
-			custom_analyzer.pre_analysis()
-			print()
-
-			if self.files.libc:
-				self.create_debug_dir()
-				self.populate_debug_dir()
-				self.files.libc.maybe_unstrip()
-
-				if self.files.loader is None:
-					self.files.get_loader()
-				if self.files.loader is not None:
-					self.files.loader.set_executable()
-
-				self.files.patchelf()
-
-			self.files.binary.set_executable()
-			analyzer.post_analysis()
-			custom_analyzer.post_analysis()
+			if not self.script_only:
+				analyzer = Analyzer(configs, self.files)
+				custom_analyzer = CustomAnalyzer(configs, self.files)
+				analyzer.pre_analysis(open_decompiler=not self.no_decompiler)
+				custom_analyzer.pre_analysis()
+				print()
+
+				if self.files.libc:
+					self.create_debug_dir()
+					self.populate_debug_dir()
+					self.files.libc.maybe_unstrip()
+
+					if self.files.loader is None:
+						self.files.get_loader()
+					if self.files.loader is not None:
+						self.files.loader.set_executable()
+
+					self.files.patchelf()
+
+				self.files.binary.set_executable()
+				analyzer.post_analysis()
+				custom_analyzer.post_analysis()
 
 			self.scripter = Scripter(configs, self.files, create_interactions=self.create_interactions)
 			self.scripter.create_script()
 			self.create_script_file()
 			self.scripter.save_script()
 		else:
 			self.scripter = Scripter(configs)
 			self.scripter.create_menu_interaction_functions()
 			self.scripter.dump_interactions()
 
-	def check_dependencies(self):
+	def check_dependencies(self) -> None:
 		deps = ["patchelf", "file"]
 		semi_deps = {
 			"eu-unstrip": "elfutils",
 			"seccomp-tools": "seccomp-tools",
 			"cwe_checker": "cwe_checker (https://github.com/fkie-cad/cwe_checker)"
 		}
 
@@ -154,14 +156,21 @@
 		"-i", "--inter",
 		action="store_true",
 		default=False,
 		help="Interactively create interaction functions"
 	)
 
 	parser.add_argument(
+		"-so", "--sonly",
+		action="store_true",
+		default=False,
+		help="Create the interaction script without analyzing the binary"
+	)
+
+	parser.add_argument(
 		"-io", "--ionly",
 		action="store_true",
 		default=False,
 		help="Create the interaction functions, without doing any analysis"
 	)
 
 	parser.add_argument(
@@ -185,16 +194,18 @@
 	)
 
 	args = parser.parse_args(sys.argv[1:])
 	others = set(args.others)
 
 	possible_arguments = {
 		"ionly": "ionly",
+		"so": "sonly",
+		"sonly": "sonly",
 		"io": "ionly",
-		"interactive": "inter",
+		"interactions": "inter",
 		"inter": "inter",
 		"i": "inter",
 		"nodecomp": "nodecomp",
 		"nd": "nodecomp"
 	}
 
 	for arg in possible_arguments:
@@ -206,11 +217,8 @@
 	if args.config or "config" in others:
 		print("[*] Setup completed")
 	else:
 		global configs
 		template = others.pop() if others else None
 		configs = ConfigManager(CONFIG_PATH, template)
 
-		if args.ionly:
-			Spwn(interactions_only=True)
-		else:
-			Spwn(create_interactions=args.inter, no_decompiler=args.nodecomp)
+		Spwn(create_interactions=args.inter, no_decompiler=args.nodecomp, script_only=args.sonly, interactions_only=args.ionly)
```

### Comparing `spwn-1.2.4/spwn/utils.py` & `spwn-1.2.5/spwn/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,21 +59,21 @@
 	ans = options[resp]
 	del options[resp]
 
 	return ans
 
 
 def ask_string(msg: str, can_skip: bool) -> str | None:
-	resp = input(f"{msg} > ")[:-1]
+	resp = input(f"{msg} > ")
 	if resp: return resp
 	elif can_skip: return None
 
 	while True:
 		print("[!] Canno be empty")
-		resp = input("> ")[:-1]
+		resp = input("> ")
 		if resp:
 			return resp
 
 
 def download_package(package_url: str, tempdir: str) -> bool:
 	try:
 		r = requests.get(package_url)
```

### Comparing `spwn-1.2.4/spwn.egg-info/PKG-INFO` & `spwn-1.2.5/spwn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spwn
-Version: 1.2.4
+Version: 1.2.5
 Summary: Automatic tool to quickly start a pwn CTF challenge
 Home-page: https://github.com/MarcoMeinardi/spwn
 Author: Chino
 Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
@@ -165,17 +165,17 @@
 ```python
 def main(files):
     print(f"The binary is {files.binary.name}")
 ```
 
 ### Decompiler
 For the decompilers commands, the syntax is the same of the pre and
-post analysis commands. I created an apposite config, rather than
+post analysis commands. I created a special config, rather than
 putting it in a pre analysis command, because I use IDA freeware
-and it can decompile only x86-64 binaries, so I have to use another
+and it can decompile only x86/x86_64 binaries, so I have to use another
 decompiler for other architectures (I have created this feature
 before the custom scripts thing, but since the decompiler is
 something that you will almost always launch, I left it to make
 it easier to use). If you want to use always the same decompiler,
 leave `idafree_command` empty and if you don't want to launch any
 decompiler, just leave both configs empty. If you wish to modify
 the conditions to select the decompiler, you can either modify
```

