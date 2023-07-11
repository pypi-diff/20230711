# Comparing `tmp/auterion-cli-1.2.1.tar.gz` & `tmp/auterion-cli-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auterion-cli-1.2.1.tar", last modified: Mon Jul 10 07:53:08 2023, max compression
+gzip compressed data, was "auterion-cli-1.2.2.tar", last modified: Tue Jul 11 12:24:42 2023, max compression
```

## Comparing `auterion-cli-1.2.1.tar` & `auterion-cli-1.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:08.784307 auterion-cli-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-10 07:53:08.784307 auterion-cli-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-10 07:53:08.000000 auterion-cli-1.2.1/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:08.780306 auterion-cli-1.2.1/auterion_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-10 07:53:08.000000 auterion-cli-1.2.1/auterion_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-10 07:53:08.000000 auterion-cli-1.2.1/auterion_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:53:08.000000 auterion-cli-1.2.1/auterion_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-10 07:53:08.000000 auterion-cli-1.2.1/auterion_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 07:53:08.000000 auterion-cli-1.2.1/auterion_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-10 07:53:08.000000 auterion-cli-1.2.1/auterion_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 07:53:08.000000 auterion-cli-1.2.1/auterion_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:08.780306 auterion-cli-1.2.1/auterioncli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:08.780306 auterion-cli-1.2.1/auterioncli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/app_command.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:08.784307 auterion-cli-1.2.1/auterioncli/commands/app_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 07:53:08.784307 auterion-cli-1.2.1/auterioncli/commands/app_sdk/app-yml-spec/
--rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-10 07:53:00.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-07-10 07:53:00.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
--rw-r--r--   0 runner    (1001) docker     (123)    14696 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/app_build_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/app_init_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/app_install_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/slimify.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8807 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/app_sdk/update.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/command_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/container_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/device_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/info_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/report_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/commands/utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3690 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5302 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/auterioncli/meta_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 07:53:08.784307 auterion-cli-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-10 07:52:59.000000 auterion-cli-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:24:42.060939 auterion-cli-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-11 12:24:42.060939 auterion-cli-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 12:24:41.000000 auterion-cli-1.2.2/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:24:42.056939 auterion-cli-1.2.2/auterion_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-11 12:24:41.000000 auterion-cli-1.2.2/auterion_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-07-11 12:24:42.000000 auterion-cli-1.2.2/auterion_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:24:41.000000 auterion-cli-1.2.2/auterion_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 12:24:41.000000 auterion-cli-1.2.2/auterion_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:24:41.000000 auterion-cli-1.2.2/auterion_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-11 12:24:41.000000 auterion-cli-1.2.2/auterion_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 12:24:41.000000 auterion-cli-1.2.2/auterion_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:24:42.056939 auterion-cli-1.2.2/auterioncli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:24:42.056939 auterion-cli-1.2.2/auterioncli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9580 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/commands/app_command.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:24:42.060939 auterion-cli-1.2.2/auterioncli/commands/app_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/commands/app_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:24:42.060939 auterion-cli-1.2.2/auterioncli/commands/app_sdk/app-yml-spec/
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15218 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/commands/app_sdk/app_build_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/commands/app_sdk/app_init_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2130 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/commands/app_sdk/app_install_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/commands/app_sdk/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/commands/app_sdk/slimify.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8807 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/commands/app_sdk/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/commands/command_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/commands/container_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/commands/device_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/commands/info_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/commands/report_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/commands/utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3971 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/auterioncli/meta_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 12:24:42.060939 auterion-cli-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-07-11 12:24:34.000000 auterion-cli-1.2.2/setup.py
```

### Comparing `auterion-cli-1.2.1/README.md` & `auterion-cli-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.1/auterion_cli.egg-info/SOURCES.txt` & `auterion-cli-1.2.2/auterion_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.1/auterioncli/commands/app_command.py` & `auterion-cli-1.2.2/auterioncli/commands/app_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.1/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json` & `auterion-cli-1.2.2/auterioncli/commands/app_sdk/app-yml-spec/app-yml-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.1/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json` & `auterion-cli-1.2.2/auterioncli/commands/app_sdk/app-yml-spec/compose-spec.json`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.1/auterioncli/commands/app_sdk/app_build_command.py` & `auterion-cli-1.2.2/auterioncli/commands/app_sdk/app_build_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,33 +60,39 @@
         self._temp_dir = None
         self._config = config
 
     def setup_parser(self, parser):
         parser.add_argument('project_dir', help='Location of the project', nargs='?', default='.')
         parser.add_argument('--skip-docker-build', help='Do not execute docker build step. Just package.', action='store_true')
         parser.add_argument('--skip-packaging', help='Do not create an AuterionOS app, just build the docker images and leave them in local docker.', action='store_true')
+        parser.add_argument('-s', '--simulation', help='Override target-platform to build simulation', action='store_true', default=False)
 
     def run(self, args):
         check_not_running_on_skynode(self._config.get('this_device_type', 'unknown'))
         compose_cmd = ensure_docker()
         ensure_mender_artifact()
         check_not_running_in_docker()
 
         self._temp_dir = tempfile.mkdtemp()
         meta = self._load_metadata(args)
         self._verify_metadata(meta)
 
+        if args.simulation:
+            print('.. Overriding target-platform. Building for simulation.')
+            meta['target-platform'] = 'simulation'
+
         image_path = self._generate_image(compose_cmd, args, meta)
         if args.skip_packaging:
             return
 
         if re.match('^v\d+$', meta['auterion-app-base']):
             v = meta['auterion-app-base']
             base_image_name = 'auterion/app-base:' + meta['auterion-app-base']
-            slimify(image_path, base_image_name, self._config['persistent_dir'])
+            platform = self._extract_target_platform(meta)
+            slimify(image_path, base_image_name, platform, self._config['persistent_dir'])
             print('┌──────────────────────────────────────────────────────────────────────────────────────┐')
             print('│                                                                                      │')
             print('│  Your app requires app auterion app-base-%s to be installed on your device.          │' % v)
             print('│                                                                                      │')
             print('│  Get app-base-%s.auterionos from Auterion suite.                                     │' % v)
             print('│                                                                                      │')
             print('│  NOTE: The app base has to be installed on the skynode before you install your app.  │')
@@ -280,15 +286,18 @@
         slug = meta['app-author'] + '.' + meta['app-name']
 
         target_devices = self._extract_target_devices(meta)
         target_devices_args = []
         for d in target_devices:
             target_devices_args += ['-t', d]
 
-        out_file = os.path.join(args.project_dir, 'build', slug + '.auterionos')
+        if 'simulation' in target_devices:
+            out_file = os.path.join(args.project_dir, 'build', slug + '-simulation.auterionos')
+        else:
+            out_file = os.path.join(args.project_dir, 'build', slug + '.auterionos')
 
         meta_file = os.path.join(args.project_dir, 'auterion-app.yml')
 
         version_file = os.path.join(self._temp_dir, 'version')
         with open(version_file, 'w') as f:
             f.write(version)
```

### Comparing `auterion-cli-1.2.1/auterioncli/commands/app_sdk/app_init_command.py` & `auterion-cli-1.2.2/auterioncli/commands/app_sdk/app_init_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.1/auterioncli/commands/app_sdk/app_install_command.py` & `auterion-cli-1.2.2/auterioncli/commands/app_sdk/app_install_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.1/auterioncli/commands/app_sdk/environment.py` & `auterion-cli-1.2.2/auterioncli/commands/app_sdk/environment.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.1/auterioncli/commands/app_sdk/slimify.py` & `auterion-cli-1.2.2/auterioncli/commands/app_sdk/slimify.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,63 +39,66 @@
 
 
 def get_file_size_mb(path):
     file_stats = os.stat(path)
     return file_stats.st_size / (1024*1024)
 
 
-def get_base_image_layers(base_image, cache_dir):
-    cache_key = 'slimify_' + hashlib.sha1(base_image.encode()).hexdigest() + '.json'
+def get_base_image_layers(base_image, platform, cache_dir):
+    cache_key = 'slimify_' + hashlib.sha1((base_image + '_' + platform).encode()).hexdigest() + '.json'
     if cache_dir is not None:
         cache_file = os.path.join(cache_dir, cache_key)
         if os.path.exists(os.path.join(cache_dir, cache_key)):
-            print(f'.. Found cached base layer information for {base_image}')
+            print(f'.. Found cached base layer information for {base_image} {platform}')
             with open(cache_file, 'r') as f:
                 return json.load(f)
 
     try:
-        run_docker_command(['docker', 'pull', '--platform=linux/arm64', base_image], json_out=False)
+        run_docker_command(['docker', 'pull', f'--platform={platform}', base_image], json_out=False)
     except:
-        error(f'Failed to pull arm64 image for {base_image}. Aborting...')
+        error(f'Failed to pull {platform} image for {base_image}. Aborting...')
 
-    print(f'.. Pulled {base_image}')
+    print(f'.. Pulled {base_image} for {platform}')
     print('> Inspecting image')
     try:
         ret = run_docker_command(['docker', 'inspect', base_image])
     except:
         error(f'Failed to inspect image {base_image}. Aborting..')
 
+    architecture = platform.split('/')[1]
+    assert(ret[0]['Architecture'] == architecture)
     assert(ret[0]['Os'] == 'linux')
     layers = ret[0]['RootFS']['Layers']
     print(f'.. Base image has {len(layers)} layers')
 
     if cache_dir is not None:
         cache_file = os.path.join(cache_dir, cache_key)
         with open(cache_file, 'w') as f:
             json.dump(layers, f)
 
     return layers
 
 
-def slimify(save_image_path, base_image, cache_dir=None):
-    base_layers = get_base_image_layers(base_image, cache_dir)
+def slimify(save_image_path, base_image, platform, cache_dir=None):
+    architecture = platform.split('/')[1]
+    base_layers = get_base_image_layers(base_image, platform, cache_dir)
     with tarfile.open(save_image_path) as f:
         manifest_file = f.extractfile(f.getmember('manifest.json'))
         manifest = json.load(manifest_file)
         layer_entry_map = {}
         # we are not allowed to remove layers that appear multiple times in an image
         forbidden_layers = set()
 
         for image_information in manifest:
             seen_digests = set()
             image_layer_entries = image_information['Layers']
             config_name = image_information['Config']
             config_file = f.extractfile(f.getmember(config_name))
             config = json.load(config_file)
-            assert(config['architecture'] == 'arm64')
+            assert(config['architecture'] == architecture)
             image_layers = config['rootfs']['diff_ids']
             for digest, file in zip(image_layers, image_layer_entries):
                 if digest in seen_digests:
                     forbidden_layers.add(digest)
                 seen_digests.add(digest)
                 layer_entry_map[digest] = (file, file in f.getnames())
```

### Comparing `auterion-cli-1.2.1/auterioncli/commands/app_sdk/update.py` & `auterion-cli-1.2.2/auterioncli/commands/app_sdk/update.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.1/auterioncli/commands/container_command.py` & `auterion-cli-1.2.2/auterioncli/commands/container_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.1/auterioncli/commands/device_command.py` & `auterion-cli-1.2.2/auterioncli/commands/device_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.1/auterioncli/commands/info_command.py` & `auterion-cli-1.2.2/auterioncli/commands/info_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.1/auterioncli/commands/report_command.py` & `auterion-cli-1.2.2/auterioncli/commands/report_command.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.1/auterioncli/commands/utils.py` & `auterion-cli-1.2.2/auterioncli/commands/utils.py`

 * *Files identical despite different names*

### Comparing `auterion-cli-1.2.1/auterioncli/main.py` & `auterion-cli-1.2.2/auterioncli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         "have_selected_device": have_selected_device,
         "this_device_type": this_device_type
     }
     commands = available_commands(config)
 
     main_parser = argparse.ArgumentParser()
     main_parser.add_argument('--version', help='Print version of this tool', action='store_true')
+    main_parser.add_argument('--no-update-check', help='Disable automatic update checks', action='store_true')
     command_subparsers = main_parser.add_subparsers(title="command", metavar='<command>', dest="root_command")
 
     for name, command in commands.items():
         parser = command_subparsers.add_parser(name, help=command.help())
         command.setup_parser(parser)
 
     args = main_parser.parse_args()
@@ -42,15 +43,17 @@
         print(get_version())
         exit(0)
 
     if args.root_command is None:
         main_parser.print_help()
         exit(1)
 
-    check_for_updates(config["persistent"])
+    # Do not check for updates on skynode, or if the user has explicitly disabled it
+    if not args.no_update_check and not config['this_device_type'] == 'skynode':
+        check_for_updates(config["persistent"])
 
     # warn user if no device is selected
     if commands[args.root_command].needs_device(args):
         device_present, serial_at_address = get_device_presence(config['device_address'])
         if not device_present:
             eprint(f"Error: No device reachable at {config['device_address']}.\n"
                    f"       Use 'device discover' command to show available devices.\n"
```

### Comparing `auterion-cli-1.2.1/auterioncli/meta_util.py` & `auterion-cli-1.2.2/auterioncli/meta_util.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
 
     # Check for updates at most once a day
     if current_time - last_update_check_time < 24 * 3600:
         return
 
     persistent_state['last_update_check_time'] = int(current_time)
 
-    print('Checking for updates...')
+    eprint('Checking for updates...')
     try:
         res = requests.get('https://pypi.org/pypi/auterion-cli/json', timeout=1)
     except requests.exceptions.Timeout:
         eprint("Warning: Update check timed out")
         return
     except:
         eprint("Warning: Update check failed")
@@ -125,17 +125,17 @@
     if res.ok:
         data = res.json()
         up_version = data.get('info', {}).get('version', None)
 
         our_version = get_version()
         try:
             if version.parse(up_version) > version.parse(our_version):
-                print("  ┌──────────────────────────────────────────────────────────────────────────────────────┐")
-                print("  │                                                                                      │")
-                print("  │  A new version of auterion-cli is available! {:>20} -> {:<16}│".format(
+                eprint("  ┌──────────────────────────────────────────────────────────────────────────────────────┐")
+                eprint("  │                                                                                      │")
+                eprint("  │  A new version of auterion-cli is available! {:>20} -> {:<16}│".format(
                     our_version, up_version))
-                print("  │                                                                                      │")
-                print("  │  Run `pip install --upgrade auterion-cli` to upgrade.                                │")
-                print("  │                                                                                      │")
-                print("  └──────────────────────────────────────────────────────────────────────────────────────┘")
+                eprint("  │                                                                                      │")
+                eprint("  │  Run `pip install --upgrade auterion-cli` to upgrade.                                │")
+                eprint("  │                                                                                      │")
+                eprint("  └──────────────────────────────────────────────────────────────────────────────────────┘")
         except version.InvalidVersion:
             eprint("Warning: Could not parse version")
```

### Comparing `auterion-cli-1.2.1/setup.py` & `auterion-cli-1.2.2/setup.py`

 * *Files identical despite different names*

