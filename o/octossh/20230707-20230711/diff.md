# Comparing `tmp/octossh-20230707.tar.gz` & `tmp/octossh-20230711.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octossh-20230707.tar", last modified: Fri Jul  7 15:47:48 2023, max compression
+gzip compressed data, was "octossh-20230711.tar", last modified: Tue Jul 11 19:34:56 2023, max compression
```

## Comparing `octossh-20230707.tar` & `octossh-20230711.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-07 15:47:48.880887 octossh-20230707/
--rw-rw-r--   0 l         (1000) l         (1000)     3395 2023-07-07 15:47:48.880887 octossh-20230707/PKG-INFO
--rw-rw-r--   0 l         (1000) l         (1000)     3068 2023-07-07 15:46:48.000000 octossh-20230707/README.md
--rw-rw-r--   0 l         (1000) l         (1000)      665 2023-07-07 15:12:59.000000 octossh-20230707/pyproject.toml
--rw-rw-r--   0 l         (1000) l         (1000)       38 2023-07-07 15:47:48.880887 octossh-20230707/setup.cfg
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-07 15:47:48.879887 octossh-20230707/src/
--rwxrwxr-x   0 l         (1000) l         (1000)    12705 2023-07-07 15:46:28.000000 octossh-20230707/src/ocsh.py
-drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-07 15:47:48.880887 octossh-20230707/src/octossh.egg-info/
--rw-rw-r--   0 l         (1000) l         (1000)     3395 2023-07-07 15:47:48.000000 octossh-20230707/src/octossh.egg-info/PKG-INFO
--rw-rw-r--   0 l         (1000) l         (1000)      248 2023-07-07 15:47:48.000000 octossh-20230707/src/octossh.egg-info/SOURCES.txt
--rw-rw-r--   0 l         (1000) l         (1000)        1 2023-07-07 15:47:48.000000 octossh-20230707/src/octossh.egg-info/dependency_links.txt
--rw-rw-r--   0 l         (1000) l         (1000)       35 2023-07-07 15:47:48.000000 octossh-20230707/src/octossh.egg-info/entry_points.txt
--rw-rw-r--   0 l         (1000) l         (1000)       54 2023-07-07 15:47:48.000000 octossh-20230707/src/octossh.egg-info/requires.txt
--rw-rw-r--   0 l         (1000) l         (1000)        5 2023-07-07 15:47:48.000000 octossh-20230707/src/octossh.egg-info/top_level.txt
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-11 19:34:56.009399 octossh-20230711/
+-rw-rw-r--   0 l         (1000) l         (1000)     3395 2023-07-11 19:34:56.009399 octossh-20230711/PKG-INFO
+-rw-rw-r--   0 l         (1000) l         (1000)     3068 2023-07-09 12:44:05.000000 octossh-20230711/README.md
+-rw-rw-r--   0 l         (1000) l         (1000)      665 2023-07-07 15:12:59.000000 octossh-20230711/pyproject.toml
+-rw-rw-r--   0 l         (1000) l         (1000)       38 2023-07-11 19:34:56.009399 octossh-20230711/setup.cfg
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-11 19:34:56.008399 octossh-20230711/src/
+-rwxrwxr-x   0 l         (1000) l         (1000)    13030 2023-07-11 19:34:29.000000 octossh-20230711/src/ocsh.py
+drwxrwxr-x   0 l         (1000) l         (1000)        0 2023-07-11 19:34:56.009399 octossh-20230711/src/octossh.egg-info/
+-rw-rw-r--   0 l         (1000) l         (1000)     3395 2023-07-11 19:34:56.000000 octossh-20230711/src/octossh.egg-info/PKG-INFO
+-rw-rw-r--   0 l         (1000) l         (1000)      248 2023-07-11 19:34:56.000000 octossh-20230711/src/octossh.egg-info/SOURCES.txt
+-rw-rw-r--   0 l         (1000) l         (1000)        1 2023-07-11 19:34:56.000000 octossh-20230711/src/octossh.egg-info/dependency_links.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       35 2023-07-11 19:34:56.000000 octossh-20230711/src/octossh.egg-info/entry_points.txt
+-rw-rw-r--   0 l         (1000) l         (1000)       54 2023-07-11 19:34:56.000000 octossh-20230711/src/octossh.egg-info/requires.txt
+-rw-rw-r--   0 l         (1000) l         (1000)        5 2023-07-11 19:34:56.000000 octossh-20230711/src/octossh.egg-info/top_level.txt
```

### Comparing `octossh-20230707/PKG-INFO` & `octossh-20230711/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octossh
-Version: 20230707
+Version: 20230711
 Summary: SSH password log-in and command automator
 Author-email: Laurent Ghigonis <ooookiwi@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/looran/octossh
 Keywords: ssh,bouncer,pass
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

### Comparing `octossh-20230707/README.md` & `octossh-20230711/README.md`

 * *Files identical despite different names*

### Comparing `octossh-20230707/pyproject.toml` & `octossh-20230711/pyproject.toml`

 * *Files identical despite different names*

### Comparing `octossh-20230707/src/ocsh.py` & `octossh-20230711/src/ocsh.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 # 2013, 2023 Laurent Ghigonis <ooookiwi@gmail.com>
 # 2013, Pierre-Olivier Vauboin
 
 DESCRIPTION = "octossh - SSH password log-in and command automator"
-VERSION = "20230707"
-SUMMARY = """octossh automates SSH password login and command execution through annotations on `ssh_config(5)` Hosts:
+VERSION = "20230711"
+SUMMARY = f"""octossh automates SSH password login and command execution through annotations on `ssh_config(5)` Hosts:
 * password authentication, reading password from pass[1]:
   * config:  `# ocsh pass <pass-name>`
   * command: `$ ocsh host`
 * post-login command execution:
   * config:  `# ocsh post <action> "<cmd>"`
   * command: `$ ocsh host[action]`
 * post-login command execution, reading additional password from pass[1]:
@@ -19,14 +19,15 @@
 [1] https://www.passwordstore.org/
 
 Compatibility with OpenSSH is kept as much as possible:
 * support usual SSH aliases, keys and command-line options
 * compatible with rsync, scp and other tools using SSH for transport, see example commands
 * autocompletion can be set-up with --ocsh-install-autocompletion
 
+v{VERSION}
 See also --ocsh-examples
 """
 EXAMPLES = """# connect to SSH alias 'host1' with automated password login
 # ssh_config(5)
 Host host1
    Hostname 10.0.0.1
    User minou
@@ -142,15 +143,15 @@
 } && complete -F _ocsh -o nospace ocsh
 """
 
     def __init__(self, conf, destination, jumphosts=None, args=None, ssh_options=None):
         if shutil.which('ssh') is None:
             raise self._err("you must install 'ssh'")
         self.conf = conf
-        self.prog = str(Path(__file__))
+        self.prog = str(Path(sys.argv[0]))
         if self.conf.conf_path:
             self.prog += " -F %s" % self.conf.conf_path
 
         ssh_cmd, ssh_target, post, password = self._get_target_cmd(destination)
 
         # construct imbricated proxycommand SSH commands for all target
         if jumphosts:
@@ -169,15 +170,15 @@
             #        ssh_options = None
             #    if len(cmd) > 0:
             #        cmd = "{} -o ProxyCommand=\"{} -W %h:%p\" {}".format(ssh_cmd, cmd.replace("\"", "\\\""), ssh_target)
             #    else:
             #        cmd = "{} {}".format(ssh_cmd, ssh_target)
 
         if args:
-            ssh_cmd = ssh_cmd + ' ' + ' '.join(args)
+            ssh_cmd = ssh_cmd + ' ' + args
 
         self.ssh_command = "{} {}".format(ssh_cmd, ssh_target)
         self.post = post
         self.password = password
 
     def run(self):
         debug("running: %s" % self.ssh_command)
@@ -252,27 +253,33 @@
     def _err(self, msg):
         error("error: %s" % msg)
         sys.exit(1)
 
 def main():
     parser = argparse.ArgumentParser(description=DESCRIPTION, epilog=SUMMARY, formatter_class=argparse.RawTextHelpFormatter)
     parser.add_argument('-F', '--ssh-config', default=Sshconf.CONFPATH_DEFAULT, help=argparse.SUPPRESS)
-    parser.add_argument('-J', '--jump-host', help=argparse.SUPPRESS)
+    parser.add_argument('-W', '--ssh-port-fw', help=argparse.SUPPRESS)
+    parser.add_argument('-J', '--ssh-jump-host', help=argparse.SUPPRESS)
     parser.add_argument('--ocsh-verbose', action='store_const', dest="loglevel", const=logging.DEBUG, default=logging.INFO, help="enable debug messages")
     parser.add_argument('--ocsh-pretend', action='store_true', help="do not actually perform the connection")
     parser.add_argument('--ocsh-examples', action='store_true', help="show example octossh configuration and commands")
     parser.add_argument('--ocsh-install-autocompletion', action='store_true', help="install bash autocompletion for the current user")
     parser.add_argument('destination', nargs='?', help='host[action]')
     parser.add_argument('args', nargs=argparse.REMAINDER, help='any OpenSSH options or remote command')
     args, ssh_options = parser.parse_known_args()
 
     if args.ocsh_examples:
         print("octossh examples:\n\n"+EXAMPLES)
         exit()
 
+    # XXX TODO create a custom parser that would pass ssh-* arguments more smoothly. Need our parser to know all SSH arguments.
+    ssh_args = ' '.join(args.args)
+    if args.ssh_port_fw:
+        ssh_args += "-W {}".format(args.ssh_port_fw)
+
     if args.ocsh_install_autocompletion:
         f = Path.home() / ".bash_completion"
         if f.exists():
             s = f.read_text()
             if "_ocsh" in s:
                 print("error: _ocsh autocompletion function already found in %s" % f)
                 sys.exit(1)
@@ -286,13 +293,13 @@
     if not args.destination:
         parser.print_usage()
         sys.exit(0)
 
     logging.basicConfig(level=args.loglevel, format='ocsh: %(message)s')
 
     c = Sshconf(Path(args.ssh_config))
-    o = Octossh(c, args.destination, args.jump_host, args.args, ssh_options)
+    o = Octossh(c, args.destination, args.ssh_jump_host, ssh_args, ssh_options)
     if not args.ocsh_pretend:
         o.run()
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `octossh-20230707/src/octossh.egg-info/PKG-INFO` & `octossh-20230711/src/octossh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octossh
-Version: 20230707
+Version: 20230711
 Summary: SSH password log-in and command automator
 Author-email: Laurent Ghigonis <ooookiwi@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/looran/octossh
 Keywords: ssh,bouncer,pass
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

