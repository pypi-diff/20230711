# Comparing `tmp/octossh-20230711.tar.gz` & `tmp/octossh-20230711.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octossh-20230711.tar", last modified: Tue Jul 11 19:34:56 2023, max compression
+gzip compressed data, was "octossh-20230711.post2.tar", last modified: Tue Jul 11 21:50:46 2023, max compression
```

## Comparing `octossh-20230711.tar` & `octossh-20230711.post2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-11 19:34:56.009399 octossh-20230711/
--rw-rw-r--   0 l         (1000) l         (1000)     3395 2023-07-11 19:34:56.009399 octossh-20230711/PKG-INFO
--rw-rw-r--   0 l         (1000) l         (1000)     3068 2023-07-09 12:44:05.000000 octossh-20230711/README.md
--rw-rw-r--   0 l         (1000) l         (1000)      665 2023-07-07 15:12:59.000000 octossh-20230711/pyproject.toml
--rw-rw-r--   0 l         (1000) l         (1000)       38 2023-07-11 19:34:56.009399 octossh-20230711/setup.cfg
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-11 19:34:56.008399 octossh-20230711/src/
--rwxrwxr-x   0 l         (1000) l         (1000)    13030 2023-07-11 19:34:29.000000 octossh-20230711/src/ocsh.py
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-11 19:34:56.009399 octossh-20230711/src/octossh.egg-info/
--rw-rw-r--   0 l         (1000) l         (1000)     3395 2023-07-11 19:34:56.000000 octossh-20230711/src/octossh.egg-info/PKG-INFO
--rw-rw-r--   0 l         (1000) l         (1000)      248 2023-07-11 19:34:56.000000 octossh-20230711/src/octossh.egg-info/SOURCES.txt
--rw-rw-r--   0 l         (1000) l         (1000)        1 2023-07-11 19:34:56.000000 octossh-20230711/src/octossh.egg-info/dependency_links.txt
--rw-rw-r--   0 l         (1000) l         (1000)       35 2023-07-11 19:34:56.000000 octossh-20230711/src/octossh.egg-info/entry_points.txt
--rw-rw-r--   0 l         (1000) l         (1000)       54 2023-07-11 19:34:56.000000 octossh-20230711/src/octossh.egg-info/requires.txt
--rw-rw-r--   0 l         (1000) l         (1000)        5 2023-07-11 19:34:56.000000 octossh-20230711/src/octossh.egg-info/top_level.txt
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-11 21:50:46.863648 octossh-20230711.post2/
+-rw-rw-r--   0 l         (1000) l         (1000)     3401 2023-07-11 21:50:46.863648 octossh-20230711.post2/PKG-INFO
+-rw-rw-r--   0 l         (1000) l         (1000)     3068 2023-07-09 12:44:05.000000 octossh-20230711.post2/README.md
+-rw-rw-r--   0 l         (1000) l         (1000)      665 2023-07-07 15:12:59.000000 octossh-20230711.post2/pyproject.toml
+-rw-rw-r--   0 l         (1000) l         (1000)       38 2023-07-11 21:50:46.863648 octossh-20230711.post2/setup.cfg
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-11 21:50:46.863648 octossh-20230711.post2/src/
+-rwxrwxr-x   0 l         (1000) l         (1000)    12915 2023-07-11 21:50:38.000000 octossh-20230711.post2/src/ocsh.py
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-11 21:50:46.863648 octossh-20230711.post2/src/octossh.egg-info/
+-rw-rw-r--   0 l         (1000) l         (1000)     3401 2023-07-11 21:50:46.000000 octossh-20230711.post2/src/octossh.egg-info/PKG-INFO
+-rw-rw-r--   0 l         (1000) l         (1000)      248 2023-07-11 21:50:46.000000 octossh-20230711.post2/src/octossh.egg-info/SOURCES.txt
+-rw-rw-r--   0 l         (1000) l         (1000)        1 2023-07-11 21:50:46.000000 octossh-20230711.post2/src/octossh.egg-info/dependency_links.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       35 2023-07-11 21:50:46.000000 octossh-20230711.post2/src/octossh.egg-info/entry_points.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       54 2023-07-11 21:50:46.000000 octossh-20230711.post2/src/octossh.egg-info/requires.txt
+-rw-rw-r--   0 l         (1000) l         (1000)        5 2023-07-11 21:50:46.000000 octossh-20230711.post2/src/octossh.egg-info/top_level.txt
```

### Comparing `octossh-20230711/PKG-INFO` & `octossh-20230711.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octossh
-Version: 20230711
+Version: 20230711.post2
 Summary: SSH password log-in and command automator
 Author-email: Laurent Ghigonis <ooookiwi@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/looran/octossh
 Keywords: ssh,bouncer,pass
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

### Comparing `octossh-20230711/README.md` & `octossh-20230711.post2/README.md`

 * *Files identical despite different names*

### Comparing `octossh-20230711/pyproject.toml` & `octossh-20230711.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `octossh-20230711/src/ocsh.py` & `octossh-20230711.post2/src/ocsh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 # 2013, 2023 Laurent Ghigonis <ooookiwi@gmail.com>
 # 2013, Pierre-Olivier Vauboin
 
 DESCRIPTION = "octossh - SSH password log-in and command automator"
-VERSION = "20230711"
+VERSION = "20230711-2"
 SUMMARY = f"""octossh automates SSH password login and command execution through annotations on `ssh_config(5)` Hosts:
 * password authentication, reading password from pass[1]:
   * config:  `# ocsh pass <pass-name>`
   * command: `$ ocsh host`
 * post-login command execution:
   * config:  `# ocsh post <action> "<cmd>"`
   * command: `$ ocsh host[action]`
@@ -147,15 +147,15 @@
         if shutil.which('ssh') is None:
             raise self._err("you must install 'ssh'")
         self.conf = conf
         self.prog = str(Path(sys.argv[0]))
         if self.conf.conf_path:
             self.prog += " -F %s" % self.conf.conf_path
 
-        ssh_cmd, ssh_target, post, password = self._get_target_cmd(destination)
+        ssh_cmd, ssh_target, post, passname = self._get_target_cmd(destination)
 
         # construct imbricated proxycommand SSH commands for all target
         if jumphosts:
             self._err("-J support not implemented")
             # XXX TODO implement jump host properly
             jump_list = jumphosts.split(',')
             cmd = ""
@@ -174,21 +174,25 @@
             #        cmd = "{} {}".format(ssh_cmd, ssh_target)
 
         if args:
             ssh_cmd = ssh_cmd + ' ' + args
 
         self.ssh_command = "{} {}".format(ssh_cmd, ssh_target)
         self.post = post
-        self.password = password
+        self.passname = passname
 
     def run(self):
-        debug("running: %s" % self.ssh_command)
         ssh_command = self.ssh_command
-        if self.password:
-            ssh_command = ssh_command.replace("_PASSWORD_", self.password)
+        if self.passname:
+            if shutil.which('pass') is None:
+                raise self._err("you must install 'pass', see https://www.passwordstore.org/")
+            if shutil.which('sshpass') is None:
+                raise self._err("you must install 'sshpass'")
+            ssh_command = "sshpass -p \"$(pass {})\" {} ".format(self.passname, ssh_command)
+        debug("running: %s" % ssh_command)
 
         if len(self.post.keys()) > 0:
             if not os.isatty(sys.stdout.fileno()):
                 raise self._err("cannot use post actions in non-interactive shell")
             p = pexpect.spawn(ssh_command)
             for action in self.post.keys():
                 cmd, passname = self.post[action]
@@ -227,32 +231,27 @@
                     else:
                         raise self._err("invalid action '%s' for host '%s'" % (action, usr['host']))
                 
         # construct command to reach target
         ssh_cmd = "ssh -v"
         if self.conf.conf_path:
             ssh_cmd += " -F %s" % self.conf.conf_path
-        password = None
+        passname = None
         if 'pass' in conf:
-            if shutil.which('pass') is None:
-                raise self._err("you must install 'pass', see https://www.passwordstore.org/")
-            if shutil.which('sshpass') is None:
-                raise self._err("you must install 'sshpass'")
-            password = subprocess.run(["pass", conf['pass']], capture_output=True).stdout.decode().strip()
-            ssh_cmd = "sshpass -p '_PASSWORD_' " + ssh_cmd
+            passname = conf['pass']
         if 'ProxyJump' in conf:
             # if ProxyJump in ssh_config(5), replace with ocsh
             ssh_cmd += ' -o ProxyCommand="{} -W %h:%p {}" -o ProxyJump=None'.format(self.prog, conf['ProxyJump'])
         elif 'ProxyCommand' in conf:
             # if ProxyCommand in ssh_config(5) uses ssh, replace with ocsh
             pcmd = conf['ProxyCommand'].split(' ')
             if pcmd[0].endswith('ssh'):
                 ssh_cmd += ' -o ProxyCommand="{} {}"'.format(self.prog, ' '.join(pcmd[1:]))
 
-        return ssh_cmd, target, post, password
+        return ssh_cmd, target, post, passname
 
     def _err(self, msg):
         error("error: %s" % msg)
         sys.exit(1)
 
 def main():
     parser = argparse.ArgumentParser(description=DESCRIPTION, epilog=SUMMARY, formatter_class=argparse.RawTextHelpFormatter)
```

### Comparing `octossh-20230711/src/octossh.egg-info/PKG-INFO` & `octossh-20230711.post2/src/octossh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octossh
-Version: 20230711
+Version: 20230711.post2
 Summary: SSH password log-in and command automator
 Author-email: Laurent Ghigonis <ooookiwi@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/looran/octossh
 Keywords: ssh,bouncer,pass
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

