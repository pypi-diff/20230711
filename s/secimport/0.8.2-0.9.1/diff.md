# Comparing `tmp/secimport-0.8.2.tar.gz` & `tmp/secimport-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "secimport-0.8.2.tar", max compression
+gzip compressed data, was "secimport-0.9.1.tar", max compression
```

## Comparing `secimport-0.8.2.tar` & `secimport-0.9.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0     1069 2023-05-24 11:27:22.130038 secimport-0.8.2/LICENSE
--rw-r--r--   0        0        0     8790 2023-05-24 11:27:22.130038 secimport-0.8.2/README.md
--rw-r--r--   0        0        0     1719 2023-05-24 11:27:22.134038 secimport-0.8.2/pyproject.toml
--rw-r--r--   0        0        0      437 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/__init__.py
--rw-r--r--   0        0        0      362 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/actions/kill_on_processing.bt
--rw-r--r--   0        0        0      373 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/actions/kill_process.bt
--rw-r--r--   0        0        0      125 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/actions/log_file_system.bt
--rw-r--r--   0        0        0      110 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/actions/log_network.bt
--rw-r--r--   0        0        0       72 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/actions/log_python_module_entry.bt
--rw-r--r--   0        0        0       71 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/actions/log_python_module_exit.bt
--rw-r--r--   0        0        0      183 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/actions/log_syscall.bt
--rw-r--r--   0        0        0     8757 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/bpftrace_backend.py
--rw-r--r--   0        0        0    22157 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/default.template.bt
--rw-r--r--   0        0        0     1651 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/default.yaml.template.bt
--rw-r--r--   0        0        0       67 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/filters/file_system.bt
--rw-r--r--   0        0        0      176 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/filters/is_current_module_under_supervision.bt
--rw-r--r--   0        0        0       40 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/filters/networking.bt
--rw-r--r--   0        0        0      553 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/filters/processes.bt
--rwxr-xr-x   0        0        0    22668 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/generate_profile.bt
--rw-r--r--   0        0        0     1203 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/new_template.bt
--rw-r--r--   0        0        0      502 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/bpftrace_backend/probes/module_syscalls_allowlist_template.bt
--rw-r--r--   0        0        0        0 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/common/__init__.py
--rw-r--r--   0        0        0      112 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/common/instrumentation_backend.py
--rw-r--r--   0        0        0    18726 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/common/utils.py
--rw-r--r--   0        0        0        0 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/__init__.py
--rw-r--r--   0        0        0      415 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/actions/kill_on_processing.d
--rw-r--r--   0        0        0      662 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/actions/kill_process.d
--rw-r--r--   0        0        0      134 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/actions/log_file_system.d
--rw-r--r--   0        0        0      124 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/actions/log_network.d
--rw-r--r--   0        0        0      187 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/actions/log_python_module_entry.d
--rw-r--r--   0        0        0      188 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/actions/log_python_module_exit.d
--rw-r--r--   0        0        0       64 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/actions/log_syscall.d
--rwxr-xr-x   0        0        0     1606 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/default.allowlist.template.d
--rwxr-xr-x   0        0        0     1081 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/default.blocklist.template.d
--rwxr-xr-x   0        0        0     1753 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/default.template.d
--rwxr-xr-x   0        0        0     2587 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/default.yaml.template.d
--rw-r--r--   0        0        0     8813 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/dtrace_backend.py
--rw-r--r--   0        0        0      172 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/filters/file_system.d
--rw-r--r--   0        0        0      177 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/filters/is_current_module_under_supervision.d
--rw-r--r--   0        0        0       31 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/filters/networking.d
--rw-r--r--   0        0        0      436 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/filters/processes.d
--rw-r--r--   0        0        0      969 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/generate_profile.d
--rw-r--r--   0        0        0       30 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/headers/destructive.d
--rw-r--r--   0        0        0     1238 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d
--rwxr-xr-x   0        0        0     4389 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/backends/dtrace_backend/py_sandbox.d
--rw-r--r--   0        0        0    13379 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/cli.py
--rwxr-xr-x   0        0        0    22294 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/profiles/trace.bt
--rw-r--r--   0        0        0     3048 2023-05-24 11:27:22.134038 secimport-0.8.2/secimport/sandbox_helper.py
--rw-r--r--   0        0        0     9513 1970-01-01 00:00:00.000000 secimport-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-11 14:18:19.681406 secimport-0.9.1/LICENSE
+-rw-r--r--   0        0        0    13200 2023-07-11 14:18:19.681406 secimport-0.9.1/README.md
+-rw-r--r--   0        0        0     1719 2023-07-11 14:18:19.681406 secimport-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0      437 2023-07-11 14:18:19.681406 secimport-0.9.1/secimport/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/__init__.py
+-rw-r--r--   0        0        0      362 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/actions/kill_on_processing.bt
+-rw-r--r--   0        0        0      373 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/actions/kill_process.bt
+-rw-r--r--   0        0        0      125 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/actions/log_file_system.bt
+-rw-r--r--   0        0        0      110 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/actions/log_network.bt
+-rw-r--r--   0        0        0       72 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/actions/log_python_module_entry.bt
+-rw-r--r--   0        0        0       71 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/actions/log_python_module_exit.bt
+-rw-r--r--   0        0        0      183 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/actions/log_syscall.bt
+-rw-r--r--   0        0        0     8757 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/bpftrace_backend.py
+-rw-r--r--   0        0        0    22263 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/default.template.bt
+-rw-r--r--   0        0        0     1645 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/default.yaml.template.bt
+-rw-r--r--   0        0        0       67 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/filters/file_system.bt
+-rw-r--r--   0        0        0      176 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/filters/is_current_module_under_supervision.bt
+-rw-r--r--   0        0        0       40 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/filters/networking.bt
+-rw-r--r--   0        0        0      553 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/filters/processes.bt
+-rwxr-xr-x   0        0        0    22668 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/generate_profile.bt
+-rw-r--r--   0        0        0     1203 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/new_template.bt
+-rw-r--r--   0        0        0      502 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/bpftrace_backend/probes/module_syscalls_allowlist_template.bt
+-rw-r--r--   0        0        0        0 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/common/__init__.py
+-rw-r--r--   0        0        0      112 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/common/instrumentation_backend.py
+-rw-r--r--   0        0        0    10949 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/common/system_calls.py
+-rw-r--r--   0        0        0     8885 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/common/utils.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/__init__.py
+-rw-r--r--   0        0        0      415 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/actions/kill_on_processing.d
+-rw-r--r--   0        0        0      662 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/actions/kill_process.d
+-rw-r--r--   0        0        0      134 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/actions/log_file_system.d
+-rw-r--r--   0        0        0      124 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/actions/log_network.d
+-rw-r--r--   0        0        0      187 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/actions/log_python_module_entry.d
+-rw-r--r--   0        0        0      188 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/actions/log_python_module_exit.d
+-rw-r--r--   0        0        0       64 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/actions/log_syscall.d
+-rwxr-xr-x   0        0        0     1606 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/default.allowlist.template.d
+-rwxr-xr-x   0        0        0     1081 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/default.blocklist.template.d
+-rwxr-xr-x   0        0        0     1753 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/default.template.d
+-rwxr-xr-x   0        0        0     2587 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/default.yaml.template.d
+-rw-r--r--   0        0        0     8813 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/dtrace_backend.py
+-rw-r--r--   0        0        0      172 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/filters/file_system.d
+-rw-r--r--   0        0        0      177 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/filters/is_current_module_under_supervision.d
+-rw-r--r--   0        0        0       31 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/filters/networking.d
+-rw-r--r--   0        0        0      436 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/filters/processes.d
+-rw-r--r--   0        0        0      969 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/generate_profile.d
+-rw-r--r--   0        0        0       30 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/headers/destructive.d
+-rw-r--r--   0        0        0     1238 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d
+-rwxr-xr-x   0        0        0     4389 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/backends/dtrace_backend/py_sandbox.d
+-rw-r--r--   0        0        0    16216 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/cli.py
+-rwxr-xr-x   0        0        0    22294 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/profiles/trace.bt
+-rw-r--r--   0        0        0     3098 2023-07-11 14:18:19.685406 secimport-0.9.1/secimport/sandbox_helper.py
+-rw-r--r--   0        0        0    13923 1970-01-01 00:00:00.000000 secimport-0.9.1/PKG-INFO
```

### Comparing `secimport-0.8.2/LICENSE` & `secimport-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `secimport-0.8.2/pyproject.toml` & `secimport-0.9.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "secimport"
-version = "0.8.2"
+version = "0.9.1"
 description = "A sandbox/supervisor for python modules."
 authors = ["Avi Lumelsky"]
 license = "MIT"
 homepage = "https://github.com/avilum/secimport"
 readme = "README.md"
 packages = [
     { include = "secimport" },
```

### Comparing `secimport-0.8.2/secimport/backends/bpftrace_backend/bpftrace_backend.py` & `secimport-0.9.1/secimport/backends/bpftrace_backend/bpftrace_backend.py`

 * *Files identical despite different names*

### Comparing `secimport-0.8.2/secimport/backends/bpftrace_backend/default.template.bt` & `secimport-0.9.1/secimport/backends/bpftrace_backend/default.template.bt`

 * *Files 1% similar despite different names*

```diff
@@ -678,16 +678,21 @@
 	@sysnum["pkey_free"] = 331;
 	@sysnum["statx"] = 332;
 	@sysnum["io_pgetevents"] = 333;
 	@sysnum["rseq"] = 334;
 
     // Defining the syscalls supervisions for all the modules
     // @syscalls_filters[@globals["current_module"], @sysname[args->id]]
+
+    // Syscall filters:
+    //  0 is undefined;
+    //  1 is allowed;
+    //  2 is blocked;
     ###SYSCALL_FILTER###
-    printf("STARTED\n");
+    printf("Sandbox Initialized.\n");
 }
 
 
 usdt:###INTERPRETER_PATH###:function__entry {
         @["depth"]++;
         @entrypoints[str(arg0)] = @["depth"];
         @globals["previous_module"] = @globals["current_module"];
```

### Comparing `secimport-0.8.2/secimport/backends/bpftrace_backend/default.yaml.template.bt` & `secimport-0.9.1/secimport/backends/bpftrace_backend/default.yaml.template.bt`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env bpftrace
 
 BEGIN {
-    ###SYSCALL_FILTER###
+###SYSCALL_FILTER###
 }
 
 
 usdt:###INTERPRETER_PATH###:function__entry {
         @stack[pid, tid]++;                     // depth (int)
         @latest_supervised_module =  str(arg0); // module name (string)
 }
 
-// usdt:###INTERPRETER_PATH###:function__return {
-//     @["depth"]--;
-// }
+usdt:###INTERPRETER_PATH###:function__return {
+     @stack[pid, tid]--;
+}
 
 tracepoint:raw_syscalls:sys_enter / @stack[pid, tid] && @syscalls_filters["general_requirements", args->id] != 1 && @syscalls_filters[@latest_supervised_module, args->id] != 1 /  {
     printf("\033[91m[SECURITY PROFILE VIOLATED]: %s called syscall %d at depth %d\033[0m\r\n", @latest_supervised_module, args->id, @stack[pid, tid]);
     if (str($1) == "STOP") {
         printf("\n^^^ STOPPING PROCESS %d DUE TO SYSCALL VIOLATION ^^^\n", pid);
         signal("SIGSTOP");
         printf("\t\tPROCESS %d STOPPED.\r\n", pid);
```

### Comparing `secimport-0.8.2/secimport/backends/bpftrace_backend/filters/processes.bt` & `secimport-0.9.1/secimport/backends/bpftrace_backend/filters/processes.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.8.2/secimport/backends/bpftrace_backend/generate_profile.bt` & `secimport-0.9.1/secimport/backends/bpftrace_backend/generate_profile.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.8.2/secimport/backends/bpftrace_backend/new_template.bt` & `secimport-0.9.1/secimport/backends/bpftrace_backend/new_template.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.8.2/secimport/backends/dtrace_backend/actions/kill_process.d` & `secimport-0.9.1/secimport/backends/dtrace_backend/actions/kill_process.d`

 * *Files identical despite different names*

### Comparing `secimport-0.8.2/secimport/backends/dtrace_backend/default.allowlist.template.d` & `secimport-0.9.1/secimport/backends/dtrace_backend/default.allowlist.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.8.2/secimport/backends/dtrace_backend/default.blocklist.template.d` & `secimport-0.9.1/secimport/backends/dtrace_backend/default.blocklist.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.8.2/secimport/backends/dtrace_backend/default.template.d` & `secimport-0.9.1/secimport/backends/dtrace_backend/default.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.8.2/secimport/backends/dtrace_backend/default.yaml.template.d` & `secimport-0.9.1/secimport/backends/dtrace_backend/default.yaml.template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.8.2/secimport/backends/dtrace_backend/dtrace_backend.py` & `secimport-0.9.1/secimport/backends/dtrace_backend/dtrace_backend.py`

 * *Files identical despite different names*

### Comparing `secimport-0.8.2/secimport/backends/dtrace_backend/generate_profile.d` & `secimport-0.9.1/secimport/backends/dtrace_backend/generate_profile.d`

 * *Files identical despite different names*

### Comparing `secimport-0.8.2/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d` & `secimport-0.9.1/secimport/backends/dtrace_backend/probes/module_syscalls_allowlist_template.d`

 * *Files identical despite different names*

### Comparing `secimport-0.8.2/secimport/backends/dtrace_backend/py_sandbox.d` & `secimport-0.9.1/secimport/backends/dtrace_backend/py_sandbox.d`

 * *Files identical despite different names*

### Comparing `secimport-0.8.2/secimport/cli.py` & `secimport-0.9.1/secimport/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,18 +24,24 @@
 
 def colored_print(color, *args):
     print(color, *args, COLORS.ENDC)
 
 
 class SecImportCLI:
     """
-    SecImport - A toolkit for Tracing and Securing Python Runtime using USDT probes and eBPF/DTrace: https://github.com/avilum/secimport/wiki/Command-Line-Usage
+    secimport is a comprehensive toolkit designed to enable the tracing, construction, and execution of secure Python runtimes. It leverages USDT probes and eBPF/DTrace technologies to enhance the overall security measures.\n
+    https://github.com/avilum/secimport/wiki/Command-Line-Usage
 
-    QUICK START:
-            >>> secimport interactive
+    WORKFLOW:
+            1. secimport trace / secimport shell
+            2. secimport build
+            3. secimport run
+
+    QUICKSTART:
+            $ secimport interactive
 
     EXAMPLES:
         1. trace:
             $  secimport trace
             $  secimport trace -h
             $  secimport trace_pid 123
             $  secimport trace_pid -h
@@ -51,16 +57,19 @@
             $  secimport run --sandbox_executable /path/to/my_sandbox.bt --sandbox_logfile my_log.log
             $  secimport run -h
     """
 
     @staticmethod
     def __create_profile_from_trace(
         trace_file: str = "trace.log",
-        output_json_file: str = "sandbox.json",
-        output_yaml_file: str = "sandbox.yaml",
+        output_json_file: str = "policy.json",
+        output_yaml_file: str = "policy.yaml",
+        output_syscalls_file: str = "syscalls.txt",
+        nsjail_sandbox_file: str = "nsjail-seccomp-sandbox.sh",
+        system_interpreter: str = sys.executable,
         destructive: bool = True,
     ) -> str:
         """Creates a yaml policy file from a given trace log. default: "trace.log".
 
         After running this command, the yaml output file can be compiled into sandbox code using the 'sandbox_from_profile' command.
         """
         print(COLORS.WARNING)
@@ -68,134 +77,169 @@
             raise FileNotFoundError(trace_file)
 
         parse_cmd = f"""cat {trace_file} | grep -Po "\@modules_syscalls\[\K(.+?)]" | tr -d ']' | sort > sandbox.log"""
         os.system(parse_cmd)
         modules_syscalls_file = Path("sandbox.log")
         if not modules_syscalls_file.exists():
             raise FileNotFoundError(trace_file)
+
         with open(modules_syscalls_file, "r") as f:
             lines = f.read().splitlines()
 
         modules_and_syscalls = defaultdict(list)
+        syscalls = set()
         for line in lines:
             parsed_items = line.split(",")
             if parsed_items == 1:
                 # General python import, interpreter dependency
                 modules_and_syscalls["general_requirements"].append(parsed_items[0])
             elif len(parsed_items) == 2:
                 # Module dependency
                 _module, _syscall = parsed_items
+                syscalls.add(_syscall)
                 if not _module or _module == "None":  # empty string and None
                     _module = "general_requirements"
                 modules_and_syscalls[_module].append(_syscall)
             else:
                 raise Exception("there are more than 2 items in one of the lines.")
 
+        # Creating a syscalls file
+        _syscalls = list(sorted(list(syscalls)))
+        syscalls_txt = ", ".join(_syscalls)
+        nsjail_sandbox_cmd = f"nsjail -Ml -Mo  --chroot / --port 8000 --user 99999 --group 99999 --seccomp_string 'ALLOW {{ {syscalls_txt} }} DEFAULT KILL' -- {system_interpreter} -i"
+        print(f"syscalls: {syscalls_txt}")
+        print(f"nsjail sandbox: {nsjail_sandbox_cmd}")
+
+        # Sandbox
+        with open(output_syscalls_file, "w") as f:
+            f.write(syscalls_txt)
+
+        # NSJail
+        with open(nsjail_sandbox_file, "w") as f:
+            f.write(nsjail_sandbox_cmd)
+        st = os.stat(nsjail_sandbox_file)
+        os.chmod(nsjail_sandbox_file, st.st_mode | stat.S_IEXEC)
+
         # JSON
         modules_json = json.dumps(modules_and_syscalls, indent=4)
         with open(output_json_file, "w") as f:
             f.write(modules_json)
-        print("CREATED JSON TEMPLATE: ", output_json_file)
 
         # Building the YAML template
         yaml_dict = {
             name: {
                 "destructive": destructive,
                 "syscall_allowlist": _syscalls,
             }
             for name, _syscalls in modules_and_syscalls.items()
         }
         yaml_dict = {"modules": yaml_dict}
         modules_yaml = yaml.safe_load(json.dumps(yaml_dict))
         modules_yaml = yaml.dump(modules_yaml)
         with open(output_yaml_file, "w") as f:
             f.write(modules_yaml)
-        print("CREATED YAML TEMPLATE: ", output_yaml_file)
+        print("Policy is ready: ", output_yaml_file, output_json_file)
 
         colored_print(COLORS.ENDC)
-        return output_yaml_file
+        return output_yaml_file, output_syscalls_file, nsjail_sandbox_file
 
     @staticmethod
-    def __create_sandbox_from_profile(
-        template_filename: str = "sandbox.yaml",
+    def compile_sandbox_from_profile(
+        template_filename: str = "policy.yaml", sandbox_filename_prefix: str = "sandbox"
     ) -> str:
-        """Generates a tailor-made sandbox code for a given yaml profile.
+        """Generates a tailor-made sandbox that will enforce a given yaml profile/policy in runtime.
 
         2 scripts will be created in the same directory: one for the dscript backend and one for the bpftrace backend.
         Returns: The file name of the bpftrace sandbox (preferred).
             _type_: str
         """
         print(COLORS.WARNING)
-        print("compiling template", template_filename)
         template_filename = Path(template_filename)
-        dtrace_sandbox_filename = Path(template_filename).with_suffix(".d")
+        dtrace_sandbox_filename = f"{sandbox_filename_prefix}.d"
         dtrace_rendered_profile = secimport.build_module_sandbox_from_yaml_template(
             template_path=template_filename,
             backend=secimport.InstrumentationBackend.DTRACE,
         )
+        if not dtrace_rendered_profile:
+            # empty file, error is already printed to the user
+            raise AssertionError(
+                f"The trace file '{template_filename}' has 0 modules. A valid policy should include at least 1 module."
+            )
+
         with open(dtrace_sandbox_filename, "w") as f:
             f.write(dtrace_rendered_profile)
+
         st = os.stat(dtrace_sandbox_filename)
         os.chmod(dtrace_sandbox_filename, st.st_mode | stat.S_IEXEC)
-        bpftrace_sandbox_filename = Path(template_filename).with_suffix(".bt")
+        print("DTRACE sandbox:", dtrace_sandbox_filename)
+
+        bpftrace_sandbox_filename = f"{sandbox_filename_prefix}.bt"
         bpftrace_rendered_profile = secimport.build_module_sandbox_from_yaml_template(
             template_path=template_filename,
             backend=secimport.InstrumentationBackend.EBPF,
         )
+
         with open(bpftrace_sandbox_filename, "w") as f:
             f.write(bpftrace_rendered_profile)
         st = os.stat(bpftrace_sandbox_filename)
         os.chmod(bpftrace_sandbox_filename, st.st_mode | stat.S_IEXEC)
-        print("\nDTRACE SANDBOX: ", dtrace_sandbox_filename)
-        print("BPFTRCE SANDBOX: ", bpftrace_sandbox_filename)
+
         colored_print(COLORS.ENDC)
         return bpftrace_sandbox_filename
 
     @staticmethod
+    def shell(*args, **kwargs):
+        """Alternative syntax for secimport "trace"."""
+        SecImportCLI.trace(*args, **kwargs)
+
+    @staticmethod
     def trace(
         entrypoint: str = None,
         python_interpreter: str = sys.executable,
         trace_log_file: str = "trace.log",
     ):
-        """Traces
+        """Traces a python process using an entrypoint or interactive interpreter. It might require sudo privilleges on some hosts.
         Args:
             entrypoint (str, optional): A python script path to trace. If not specified, a python interactive shell will be opened in the foregraound. This shell, or the given command, will be traced and logged to the "trace_log_file" argument.
             python_interpreter (str, optional): The path of the python executable interpreter to trace. Defaults to sys.executable.
             trace_log_file (str, optional): The log file to write the trace into. Defaults to "trace.log".
         """
-        colored_print(COLORS.OKGREEN, ">>> secimport trace")
         if entrypoint:
             # entrypoint_cmd = str(Path(entrypoint).absolute())
             entrypoint_cmd = f'bash -c "{python_interpreter} {entrypoint}"'
         else:
             entrypoint_cmd = python_interpreter
         cmd = [
             f"{SECIMPORT_ROOT}/profiles/trace.bt",
             "-c",
             f"{entrypoint_cmd}",
             "-o",
             f"{trace_log_file}",
         ]
-        colored_print(COLORS.HEADER, "\nTRACING:", cmd)
-        colored_print(COLORS.BOLD, "\n\t\t\tPress CTRL+D/CTRL+C to stop the trace;\n")
+        colored_print(COLORS.HEADER, "\nTracing using ", cmd)
+        colored_print(
+            COLORS.BOLD,
+            "Press CTRL+D or CTRL+C to stop the trace gracefully.\n",
+        )
         os.system(" ".join(cmd))
-        colored_print(COLORS.BOLD, "TRACING DONE;")
+        colored_print(
+            COLORS.BOLD, "The trace log is at", COLORS.OKGREEN, f"./{trace_log_file}"
+        )
 
     @staticmethod
     def trace_pid(
         pid: int,
         trace_log_file: str = "trace.log",
     ):
         """Traces a running process by pid. It might require sudo privilleges on some hosts.
 
         Args:
             pid (int): process pid to trace
             trace_log_file (str): The output file to write the trace into.
         """
-        colored_print(COLORS.OKGREEN, ">>> secimport trace_pid")
         assert isinstance(pid, int), f"pid must be an int, got: {pid}"
         cmd = [
             str(SECIMPORT_ROOT) + "/profiles/trace.bt",
             "-p",
             f"{pid}",
             "-o",
             f"{trace_log_file}",
@@ -203,59 +247,78 @@
         colored_print(COLORS.HEADER, "\nTRACING PID:")
         colored_print(COLORS.OKBLUE, pid)
         input("\t\t\tPress CTRL+D/CTRL+C to stop the trace;")
         os.system(" ".join(cmd))
         colored_print(COLORS.ENDC)
 
     @staticmethod
-    def build(trace_file: str = "trace.log") -> str:
-        colored_print(COLORS.OKGREEN, ">>> secimport build")
-        """Converts a trace log into an executable sandbox.
-        It uses `secimport create_profile_from_trace ...` and `secimport sandbox_from_profile...` under the hood.
+    def build(
+        trace_file: str = "trace.log",
+        output_json_file: str = "policy.json",
+        output_yaml_file: str = "policy.yaml",
+        output_syscalls_file: str = "syscalls.txt",
+        destructive: bool = False,
+    ) -> str:
+        """Compiles a trace log (trace.log). Creates the sandbox executable (instrumentation script) for each supported backend
+        It uses `create_profile_from_trace ...` and `sandbox_from_profile`.
 
         Raises:
             FileNotFoundError:
 
         Returns:
             _type_: str
         """
-        colored_print(COLORS.BOLD, "\nSECIMPORT COMPILING...")
-        output_yaml_file = SecImportCLI.__create_profile_from_trace(
-            trace_file=trace_file
+        (
+            output_yaml_file,
+            output_syscalls_file,
+            nsjail_sandbox_file,
+        ) = SecImportCLI.__create_profile_from_trace(
+            trace_file=trace_file,
+            output_json_file=output_json_file,
+            output_yaml_file=output_yaml_file,
+            output_syscalls_file=output_syscalls_file,
+            destructive=destructive,
         )
-        bpftrace_sandbox_filename = SecImportCLI.__create_sandbox_from_profile(
+
+        bpftrace_sandbox_filename = SecImportCLI.compile_sandbox_from_profile(
             template_filename=output_yaml_file
         )
-        colored_print(COLORS.BOLD, f"SANDBOX READY: {bpftrace_sandbox_filename}")
+        colored_print(COLORS.OKGREEN, f"syscalls: {COLORS.BOLD} {output_syscalls_file}")
+        colored_print(
+            COLORS.OKGREEN, f"nsjail sandbox: {COLORS.BOLD} {nsjail_sandbox_file}"
+        )
+        colored_print(
+            COLORS.OKGREEN,
+            f"secimport eBPF sandbox: {COLORS.BOLD} {bpftrace_sandbox_filename}",
+        )
 
     @staticmethod
     def run(
+        entrypoint: str = None,
         sandbox_executable: str = "./sandbox.bt",
         python_interpreter: str = sys.executable,
-        entrypoint: str = None,
         pid=None,
         stop_on_violation=False,
         kill_on_violation=False,
         sandbox_logfile: str = None,
     ):
         """Run a python process inside the sandbox.
 
         Args:
+            entrypoint (str, optional): A script entrypoint to trace explicitly. Defaults to None.
             sandbox_executable (str, optional): An executable sandbox file, generated by "secimport build". Defaults to "./sandbox.bt".
             python_interpreter (str, optional): The python interpreter to probe. Defaults to sys.executable.
-            entrypoint (str, optional): A script entrypoint to trace explicitly. Defaults to None.
             pid (_type_, optional): process id to trace. Defaults to None.
             stop_on_violation: (str, optional). If set to True, the sandbox will send SIGSTOP to the process and prevent the execution the syscall.
             kill_on_violation: (str, optional). If set to True, the sandbox will send SIGKILL to the process, and then the sandbox will exit.
             sandbox_logfile: (str, optional). Log the sandbox STDOUT to an explicit file, instead of the foreground STDOUT/STDERR.
         Raises:
             FileNotFoundError: _description_
             ValueError: _description_
         """
-        colored_print(COLORS.OKGREEN, ">>> secimport run")
         if not Path(sandbox_executable).exists:
             raise FileNotFoundError(
                 "The sandbox was not found. Try calling 'secimport trace/trace_pid' and then 'secimport compile_sandbox'"
             )
         sandbox_startup_cmd = [f"{sandbox_executable}", "--unsafe"]
         if pid is not None:
             sandbox_startup_cmd += [f" -p {pid}"]
@@ -293,32 +356,49 @@
             COLORS.BOLD,
             "SANDBOX EXITED;",
             f"Log file: {sandbox_logfile};" if sandbox_logfile else "",
         )
 
     @staticmethod
     def interactive():
+        colored_print(COLORS.BOLD, "Welcome to secimport!")
         colored_print(
             COLORS.OKBLUE,
-            "\nLet's create our first tailor-made sandbox with secimport!\n- A python shell will be opened\n- The behavior will be recorded.\n",
+            "1. A python code can be traced using",
+            COLORS.OKGREEN,
+            '"secimport trace"',
+            COLORS.OKBLUE,
+            "or using",
+            COLORS.OKGREEN,
+            '"secimport shell"',
+            COLORS.OKBLUE,
+            "\n 2. All the function calls and system calls will be recorded to",
+            COLORS.OKGREEN,
+            "./trace.log.\n",
         )
-        start = input("OK? (y): ") or "y"
+        start = input("Continue? (y): ") or "y"
         if start.lower() == "y":
             try:
                 SecImportCLI.trace()
             except KeyboardInterrupt:
                 ...
 
+            colored_print(
+                COLORS.OKBLUE,
+                '\nRunning "secimport build"; it compiles ./trace.log which is the trace log to ./sandbox.bt',
+            )
             SecImportCLI.build()
 
             colored_print(
                 COLORS.OKBLUE,
-                '\nNow, let\'s run the sandbox.\n- Run the same commands as before, they should run without any problem;.\n- Do something new in the shell; e.g:\t>>> __import__("os").system("ps")',
+                "\nNow, let's run the sandbox.\n1. Run the same commands as before. They should run without any problem.\n2. Do something new in the shell. For example, ",
+                COLORS.BOLD,
+                "run \"import os; os.system('ps'); and see how secimport detects it.\"",
             )
-            run = input("\n\tOK? (y): ") or "y"
+            run = input("\nContinue? (y): ") or "y"
 
             if run.lower() == "y":
                 SecImportCLI.run()
         else:
             colored_print(
                 COLORS.OKBLUE,
                 run,
```

### Comparing `secimport-0.8.2/secimport/profiles/trace.bt` & `secimport-0.9.1/secimport/profiles/trace.bt`

 * *Files identical despite different names*

### Comparing `secimport-0.8.2/secimport/sandbox_helper.py` & `secimport-0.9.1/secimport/sandbox_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,14 @@
 Import python modules with syscalls supervision.
 
 Copyright (c) 2022 Avi Lumelsky
 """
 
 from secimport.backends.common.instrumentation_backend import InstrumentationBackend
 from secimport.backends.common.utils import DEFAULT_BACKEND
-from secimport.backends.bpftrace_backend.bpftrace_backend import (
-    run_bpftrace_script_for_module,
-)
-from secimport.backends.dtrace_backend.dtrace_backend import (
-    run_dtrace_script_for_module,
-)
 
 
 def secure_import(
     module_name: str,
     allow_shells: bool = False,
     allow_networking: bool = False,
     use_sudo: bool = False,
@@ -39,26 +33,34 @@
         log_file_system (bool, optional): Whether to log filesystem calls - e.g read, open, write, etc.
         destructive (bool, optional): Whether to kill the process with -9 sigkill upon violation of any of the configurations above.
     Returns:
         _type_: A Python Module. The module is supervised by a dtrace process with destructive capabilities unless the 'destructive' argument is set to False.
     """
 
     if backend == InstrumentationBackend.EBPF:
+        from secimport.backends.bpftrace_backend.bpftrace_backend import (
+            run_bpftrace_script_for_module,
+        )
+
         assert run_bpftrace_script_for_module(
             module_name=module_name,
             allow_shells=allow_shells,
             allow_networking=allow_networking,
             use_sudo=use_sudo,
             log_python_calls=log_python_calls,
             log_syscalls=log_syscalls,
             log_network=log_network,
             log_file_system=log_file_system,
             destructive=destructive,
         )
     elif backend == InstrumentationBackend.DTRACE:
+        from secimport.backends.dtrace_backend.dtrace_backend import (
+            run_dtrace_script_for_module,
+        )
+
         assert run_dtrace_script_for_module(
             module_name=module_name,
             allow_shells=allow_shells,
             allow_networking=allow_networking,
             use_sudo=use_sudo,
             log_python_calls=log_python_calls,
             log_syscalls=log_syscalls,
```

