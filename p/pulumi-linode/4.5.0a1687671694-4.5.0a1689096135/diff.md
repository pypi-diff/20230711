# Comparing `tmp/pulumi_linode-4.5.0a1687671694.tar.gz` & `tmp/pulumi_linode-4.5.0a1689096135.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_linode-4.5.0a1687671694.tar", last modified: Sun Jun 25 05:50:39 2023, max compression
+gzip compressed data, was "pulumi_linode-4.5.0a1689096135.tar", last modified: Tue Jul 11 17:27:04 2023, max compression
```

## Comparing `pulumi_linode-4.5.0a1687671694.tar` & `pulumi_linode-4.5.0a1689096135.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:50:39.545437 pulumi_linode-4.5.0a1687671694/
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-25 05:50:39.545437 pulumi_linode-4.5.0a1687671694/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:50:39.545437 pulumi_linode-4.5.0a1687671694/pulumi_linode/
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   178907 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/account_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:50:39.545437 pulumi_linode-4.5.0a1687671694/pulumi_linode/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/database_access_controls.py
--rw-r--r--   0 runner    (1001) docker     (123)    44527 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/database_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)    50181 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/database_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)    41355 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    34477 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    31367 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/firewall_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_account_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_account_logins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4710 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_account_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_database_backups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_database_engines.py
--rw-r--r--   0 runner    (1001) docker     (123)    14416 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_database_mysql.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_database_mysql_backups.py
--rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_database_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_domain_zonefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     7737 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7794 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_instance_backups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3564 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_instance_networking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6955 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6541 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_instances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_ipv6_range.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_kernel.py
--rw-r--r--   0 runner    (1001) docker     (123)     4624 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_linode_object_storage_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_lke_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_lke_versions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_networking_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_node_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)    12788 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_node_balancer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6773 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_node_balancer_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_object_storage_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     5227 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_stack_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     7994 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_stack_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    15422 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_vlans.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    31230 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/image.py
--rw-r--r--   0 runner    (1001) docker     (123)   106257 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    34385 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/instance_disk.py
--rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/instance_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/instance_shared_ips.py
--rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/ipv6_range.py
--rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/lke_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    22675 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/node_balancer.py
--rw-r--r--   0 runner    (1001) docker     (123)    57583 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/node_balancer_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    21834 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/node_balancer_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    30548 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/object_storage_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/object_storage_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    49713 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/object_storage_object.py
--rw-r--r--   0 runner    (1001) docker     (123)   258855 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    19421 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/rdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    31276 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/stack_script.py
--rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/token.py
--rw-r--r--   0 runner    (1001) docker     (123)    41796 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    24901 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-25 05:50:39.545437 pulumi_linode-4.5.0a1687671694/pulumi_linode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/pulumi_linode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-25 05:50:39.545437 pulumi_linode-4.5.0a1687671694/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-25 05:50:39.000000 pulumi_linode-4.5.0a1687671694/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:27:04.614489 pulumi_linode-4.5.0a1689096135/
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-11 17:27:04.614489 pulumi_linode-4.5.0a1689096135/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:27:04.614489 pulumi_linode-4.5.0a1689096135/pulumi_linode/
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   178907 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16532 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/account_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:27:04.614489 pulumi_linode-4.5.0a1689096135/pulumi_linode/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12684 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/database_access_controls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44527 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/database_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50181 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/database_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41355 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34477 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31367 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/firewall_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7643 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4954 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_account_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_account_logins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_account_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_database_backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8238 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_database_engines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_database_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_database_mysql_backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16008 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_database_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9608 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_domain_zonefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_instance_backups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_instance_networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7105 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6616 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_instances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_ipv6_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5598 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_linode_object_storage_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_lke_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_lke_versions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7190 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_networking_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_node_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13058 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_node_balancer_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6893 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_node_balancer_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4871 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_object_storage_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5317 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_stack_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8084 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_stack_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15647 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_vlans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6953 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31230 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)   106257 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34385 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/instance_disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19005 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/instance_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/instance_shared_ips.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15118 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/ipv6_range.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26054 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/lke_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22675 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/node_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57583 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/node_balancer_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21834 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/node_balancer_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30548 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/object_storage_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14371 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/object_storage_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49713 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/object_storage_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)   258855 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19421 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/rdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9506 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31276 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/stack_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41796 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24901 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:27:04.614489 pulumi_linode-4.5.0a1689096135/pulumi_linode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/pulumi_linode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:27:04.614489 pulumi_linode-4.5.0a1689096135/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-07-11 17:27:04.000000 pulumi_linode-4.5.0a1689096135/setup.py
```

### Comparing `pulumi_linode-4.5.0a1687671694/PKG-INFO` & `pulumi_linode-4.5.0a1689096135/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_linode
-Version: 4.5.0a1687671694
+Version: 4.5.0a1689096135
 Summary: A Pulumi package for creating and managing linode cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-linode
 Keywords: pulumi linode
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_linode-4.5.0a1687671694/README.md` & `pulumi_linode-4.5.0a1689096135/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/__init__.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/_inputs.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/_utilities.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/account_settings.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/account_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/config/vars.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/database_access_controls.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/database_access_controls.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/database_mysql.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/database_mysql.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/database_postgresql.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/database_postgresql.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/domain.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/domain_record.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/firewall.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/firewall_device.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/firewall_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_account.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_account.py`

 * *Files 7% similar despite different names*

```diff
@@ -202,20 +202,20 @@
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getAccount:getAccount', __args__, opts=opts, typ=GetAccountResult).value
 
     return AwaitableGetAccountResult(
-        address1=__ret__.address1,
-        address2=__ret__.address2,
-        balance=__ret__.balance,
-        city=__ret__.city,
-        company=__ret__.company,
-        country=__ret__.country,
-        email=__ret__.email,
-        first_name=__ret__.first_name,
-        id=__ret__.id,
-        last_name=__ret__.last_name,
-        phone=__ret__.phone,
-        state=__ret__.state,
-        zip=__ret__.zip)
+        address1=pulumi.get(__ret__, 'address1'),
+        address2=pulumi.get(__ret__, 'address2'),
+        balance=pulumi.get(__ret__, 'balance'),
+        city=pulumi.get(__ret__, 'city'),
+        company=pulumi.get(__ret__, 'company'),
+        country=pulumi.get(__ret__, 'country'),
+        email=pulumi.get(__ret__, 'email'),
+        first_name=pulumi.get(__ret__, 'first_name'),
+        id=pulumi.get(__ret__, 'id'),
+        last_name=pulumi.get(__ret__, 'last_name'),
+        phone=pulumi.get(__ret__, 'phone'),
+        state=pulumi.get(__ret__, 'state'),
+        zip=pulumi.get(__ret__, 'zip'))
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_account_login.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_account_login.py`

 * *Files 8% similar despite different names*

```diff
@@ -122,20 +122,20 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getAccountLogin:getAccountLogin', __args__, opts=opts, typ=GetAccountLoginResult).value
 
     return AwaitableGetAccountLoginResult(
-        datetime=__ret__.datetime,
-        id=__ret__.id,
-        ip=__ret__.ip,
-        restricted=__ret__.restricted,
-        status=__ret__.status,
-        username=__ret__.username)
+        datetime=pulumi.get(__ret__, 'datetime'),
+        id=pulumi.get(__ret__, 'id'),
+        ip=pulumi.get(__ret__, 'ip'),
+        restricted=pulumi.get(__ret__, 'restricted'),
+        status=pulumi.get(__ret__, 'status'),
+        username=pulumi.get(__ret__, 'username'))
 
 
 @_utilities.lift_output_func(get_account_login)
 def get_account_login_output(id: Optional[pulumi.Input[int]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAccountLoginResult]:
     """
     Provides details about a specific Linode account login.
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_account_logins.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_account_logins.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,17 +101,17 @@
     __args__ = dict()
     __args__['filters'] = filters
     __args__['logins'] = logins
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getAccountLogins:getAccountLogins', __args__, opts=opts, typ=GetAccountLoginsResult).value
 
     return AwaitableGetAccountLoginsResult(
-        filters=__ret__.filters,
-        id=__ret__.id,
-        logins=__ret__.logins)
+        filters=pulumi.get(__ret__, 'filters'),
+        id=pulumi.get(__ret__, 'id'),
+        logins=pulumi.get(__ret__, 'logins'))
 
 
 @_utilities.lift_output_func(get_account_logins)
 def get_account_logins_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetAccountLoginsFilterArgs']]]]] = None,
                               logins: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetAccountLoginsLoginArgs']]]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAccountLoginsResult]:
     """
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_account_settings.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_account_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,13 +116,13 @@
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getAccountSettings:getAccountSettings', __args__, opts=opts, typ=GetAccountSettingsResult).value
 
     return AwaitableGetAccountSettingsResult(
-        backups_enabled=__ret__.backups_enabled,
-        id=__ret__.id,
-        longview_subscription=__ret__.longview_subscription,
-        managed=__ret__.managed,
-        network_helper=__ret__.network_helper,
-        object_storage=__ret__.object_storage)
+        backups_enabled=pulumi.get(__ret__, 'backups_enabled'),
+        id=pulumi.get(__ret__, 'id'),
+        longview_subscription=pulumi.get(__ret__, 'longview_subscription'),
+        managed=pulumi.get(__ret__, 'managed'),
+        network_helper=pulumi.get(__ret__, 'network_helper'),
+        object_storage=pulumi.get(__ret__, 'object_storage'))
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_database_backups.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_database_backups.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,22 +163,22 @@
     __args__['latest'] = latest
     __args__['order'] = order
     __args__['orderBy'] = order_by
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDatabaseBackups:getDatabaseBackups', __args__, opts=opts, typ=GetDatabaseBackupsResult).value
 
     return AwaitableGetDatabaseBackupsResult(
-        backups=__ret__.backups,
-        database_id=__ret__.database_id,
-        database_type=__ret__.database_type,
-        filters=__ret__.filters,
-        id=__ret__.id,
-        latest=__ret__.latest,
-        order=__ret__.order,
-        order_by=__ret__.order_by)
+        backups=pulumi.get(__ret__, 'backups'),
+        database_id=pulumi.get(__ret__, 'database_id'),
+        database_type=pulumi.get(__ret__, 'database_type'),
+        filters=pulumi.get(__ret__, 'filters'),
+        id=pulumi.get(__ret__, 'id'),
+        latest=pulumi.get(__ret__, 'latest'),
+        order=pulumi.get(__ret__, 'order'),
+        order_by=pulumi.get(__ret__, 'order_by'))
 
 
 @_utilities.lift_output_func(get_database_backups)
 def get_database_backups_output(backups: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetDatabaseBackupsBackupArgs']]]]] = None,
                                 database_id: Optional[pulumi.Input[int]] = None,
                                 database_type: Optional[pulumi.Input[str]] = None,
                                 filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetDatabaseBackupsFilterArgs']]]]] = None,
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_database_engines.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_database_engines.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,20 +156,20 @@
     __args__['latest'] = latest
     __args__['order'] = order
     __args__['orderBy'] = order_by
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDatabaseEngines:getDatabaseEngines', __args__, opts=opts, typ=GetDatabaseEnginesResult).value
 
     return AwaitableGetDatabaseEnginesResult(
-        engines=__ret__.engines,
-        filters=__ret__.filters,
-        id=__ret__.id,
-        latest=__ret__.latest,
-        order=__ret__.order,
-        order_by=__ret__.order_by)
+        engines=pulumi.get(__ret__, 'engines'),
+        filters=pulumi.get(__ret__, 'filters'),
+        id=pulumi.get(__ret__, 'id'),
+        latest=pulumi.get(__ret__, 'latest'),
+        order=pulumi.get(__ret__, 'order'),
+        order_by=pulumi.get(__ret__, 'order_by'))
 
 
 @_utilities.lift_output_func(get_database_engines)
 def get_database_engines_output(engines: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetDatabaseEnginesEngineArgs']]]]] = None,
                                 filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetDatabaseEnginesFilterArgs']]]]] = None,
                                 latest: Optional[pulumi.Input[Optional[bool]]] = None,
                                 order: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_database_mysql.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_database_mysql.py`

 * *Files 5% similar despite different names*

```diff
@@ -325,36 +325,36 @@
     __args__ = dict()
     __args__['databaseId'] = database_id
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDatabaseMysql:getDatabaseMysql', __args__, opts=opts, typ=GetDatabaseMysqlResult).value
 
     return AwaitableGetDatabaseMysqlResult(
-        allow_lists=__ret__.allow_lists,
-        ca_cert=__ret__.ca_cert,
-        cluster_size=__ret__.cluster_size,
-        created=__ret__.created,
-        database_id=__ret__.database_id,
-        encrypted=__ret__.encrypted,
-        engine=__ret__.engine,
-        engine_id=__ret__.engine_id,
-        host_primary=__ret__.host_primary,
-        host_secondary=__ret__.host_secondary,
-        id=__ret__.id,
-        label=__ret__.label,
-        region=__ret__.region,
-        replication_type=__ret__.replication_type,
-        root_password=__ret__.root_password,
-        root_username=__ret__.root_username,
-        ssl_connection=__ret__.ssl_connection,
-        status=__ret__.status,
-        type=__ret__.type,
-        updated=__ret__.updated,
-        updates=__ret__.updates,
-        version=__ret__.version)
+        allow_lists=pulumi.get(__ret__, 'allow_lists'),
+        ca_cert=pulumi.get(__ret__, 'ca_cert'),
+        cluster_size=pulumi.get(__ret__, 'cluster_size'),
+        created=pulumi.get(__ret__, 'created'),
+        database_id=pulumi.get(__ret__, 'database_id'),
+        encrypted=pulumi.get(__ret__, 'encrypted'),
+        engine=pulumi.get(__ret__, 'engine'),
+        engine_id=pulumi.get(__ret__, 'engine_id'),
+        host_primary=pulumi.get(__ret__, 'host_primary'),
+        host_secondary=pulumi.get(__ret__, 'host_secondary'),
+        id=pulumi.get(__ret__, 'id'),
+        label=pulumi.get(__ret__, 'label'),
+        region=pulumi.get(__ret__, 'region'),
+        replication_type=pulumi.get(__ret__, 'replication_type'),
+        root_password=pulumi.get(__ret__, 'root_password'),
+        root_username=pulumi.get(__ret__, 'root_username'),
+        ssl_connection=pulumi.get(__ret__, 'ssl_connection'),
+        status=pulumi.get(__ret__, 'status'),
+        type=pulumi.get(__ret__, 'type'),
+        updated=pulumi.get(__ret__, 'updated'),
+        updates=pulumi.get(__ret__, 'updates'),
+        version=pulumi.get(__ret__, 'version'))
 
 
 @_utilities.lift_output_func(get_database_mysql)
 def get_database_mysql_output(database_id: Optional[pulumi.Input[Optional[int]]] = None,
                               id: Optional[pulumi.Input[Optional[int]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabaseMysqlResult]:
     """
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_database_mysql_backups.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_database_mysql_backups.py`

 * *Files 6% similar despite different names*

```diff
@@ -149,21 +149,21 @@
     __args__['latest'] = latest
     __args__['order'] = order
     __args__['orderBy'] = order_by
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDatabaseMysqlBackups:getDatabaseMysqlBackups', __args__, opts=opts, typ=GetDatabaseMysqlBackupsResult).value
 
     return AwaitableGetDatabaseMysqlBackupsResult(
-        backups=__ret__.backups,
-        database_id=__ret__.database_id,
-        filters=__ret__.filters,
-        id=__ret__.id,
-        latest=__ret__.latest,
-        order=__ret__.order,
-        order_by=__ret__.order_by)
+        backups=pulumi.get(__ret__, 'backups'),
+        database_id=pulumi.get(__ret__, 'database_id'),
+        filters=pulumi.get(__ret__, 'filters'),
+        id=pulumi.get(__ret__, 'id'),
+        latest=pulumi.get(__ret__, 'latest'),
+        order=pulumi.get(__ret__, 'order'),
+        order_by=pulumi.get(__ret__, 'order_by'))
 
 
 @_utilities.lift_output_func(get_database_mysql_backups)
 def get_database_mysql_backups_output(database_id: Optional[pulumi.Input[int]] = None,
                                       filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetDatabaseMysqlBackupsFilterArgs']]]]] = None,
                                       latest: Optional[pulumi.Input[Optional[bool]]] = None,
                                       order: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_database_postgresql.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_database_postgresql.py`

 * *Files 4% similar despite different names*

```diff
@@ -346,38 +346,38 @@
     __args__ = dict()
     __args__['databaseId'] = database_id
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDatabasePostgresql:getDatabasePostgresql', __args__, opts=opts, typ=GetDatabasePostgresqlResult).value
 
     return AwaitableGetDatabasePostgresqlResult(
-        allow_lists=__ret__.allow_lists,
-        ca_cert=__ret__.ca_cert,
-        cluster_size=__ret__.cluster_size,
-        created=__ret__.created,
-        database_id=__ret__.database_id,
-        encrypted=__ret__.encrypted,
-        engine=__ret__.engine,
-        engine_id=__ret__.engine_id,
-        host_primary=__ret__.host_primary,
-        host_secondary=__ret__.host_secondary,
-        id=__ret__.id,
-        label=__ret__.label,
-        port=__ret__.port,
-        region=__ret__.region,
-        replication_commit_type=__ret__.replication_commit_type,
-        replication_type=__ret__.replication_type,
-        root_password=__ret__.root_password,
-        root_username=__ret__.root_username,
-        ssl_connection=__ret__.ssl_connection,
-        status=__ret__.status,
-        type=__ret__.type,
-        updated=__ret__.updated,
-        updates=__ret__.updates,
-        version=__ret__.version)
+        allow_lists=pulumi.get(__ret__, 'allow_lists'),
+        ca_cert=pulumi.get(__ret__, 'ca_cert'),
+        cluster_size=pulumi.get(__ret__, 'cluster_size'),
+        created=pulumi.get(__ret__, 'created'),
+        database_id=pulumi.get(__ret__, 'database_id'),
+        encrypted=pulumi.get(__ret__, 'encrypted'),
+        engine=pulumi.get(__ret__, 'engine'),
+        engine_id=pulumi.get(__ret__, 'engine_id'),
+        host_primary=pulumi.get(__ret__, 'host_primary'),
+        host_secondary=pulumi.get(__ret__, 'host_secondary'),
+        id=pulumi.get(__ret__, 'id'),
+        label=pulumi.get(__ret__, 'label'),
+        port=pulumi.get(__ret__, 'port'),
+        region=pulumi.get(__ret__, 'region'),
+        replication_commit_type=pulumi.get(__ret__, 'replication_commit_type'),
+        replication_type=pulumi.get(__ret__, 'replication_type'),
+        root_password=pulumi.get(__ret__, 'root_password'),
+        root_username=pulumi.get(__ret__, 'root_username'),
+        ssl_connection=pulumi.get(__ret__, 'ssl_connection'),
+        status=pulumi.get(__ret__, 'status'),
+        type=pulumi.get(__ret__, 'type'),
+        updated=pulumi.get(__ret__, 'updated'),
+        updates=pulumi.get(__ret__, 'updates'),
+        version=pulumi.get(__ret__, 'version'))
 
 
 @_utilities.lift_output_func(get_database_postgresql)
 def get_database_postgresql_output(database_id: Optional[pulumi.Input[Optional[int]]] = None,
                                    id: Optional[pulumi.Input[Optional[int]]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDatabasePostgresqlResult]:
     """
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_databases.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_databases.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,19 +124,19 @@
     __args__['filters'] = filters
     __args__['order'] = order
     __args__['orderBy'] = order_by
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDatabases:getDatabases', __args__, opts=opts, typ=GetDatabasesResult).value
 
     return AwaitableGetDatabasesResult(
-        databases=__ret__.databases,
-        filters=__ret__.filters,
-        id=__ret__.id,
-        order=__ret__.order,
-        order_by=__ret__.order_by)
+        databases=pulumi.get(__ret__, 'databases'),
+        filters=pulumi.get(__ret__, 'filters'),
+        id=pulumi.get(__ret__, 'id'),
+        order=pulumi.get(__ret__, 'order'),
+        order_by=pulumi.get(__ret__, 'order_by'))
 
 
 @_utilities.lift_output_func(get_databases)
 def get_databases_output(databases: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetDatabasesDatabaseArgs']]]]] = None,
                          filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetDatabasesFilterArgs']]]]] = None,
                          order: Optional[pulumi.Input[Optional[str]]] = None,
                          order_by: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_domain.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_domain.py`

 * *Files 8% similar despite different names*

```diff
@@ -225,28 +225,28 @@
     __args__ = dict()
     __args__['domain'] = domain
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDomain:getDomain', __args__, opts=opts, typ=GetDomainResult).value
 
     return AwaitableGetDomainResult(
-        axfr_ips=__ret__.axfr_ips,
-        description=__ret__.description,
-        domain=__ret__.domain,
-        expire_sec=__ret__.expire_sec,
-        group=__ret__.group,
-        id=__ret__.id,
-        master_ips=__ret__.master_ips,
-        refresh_sec=__ret__.refresh_sec,
-        retry_sec=__ret__.retry_sec,
-        soa_email=__ret__.soa_email,
-        status=__ret__.status,
-        tags=__ret__.tags,
-        ttl_sec=__ret__.ttl_sec,
-        type=__ret__.type)
+        axfr_ips=pulumi.get(__ret__, 'axfr_ips'),
+        description=pulumi.get(__ret__, 'description'),
+        domain=pulumi.get(__ret__, 'domain'),
+        expire_sec=pulumi.get(__ret__, 'expire_sec'),
+        group=pulumi.get(__ret__, 'group'),
+        id=pulumi.get(__ret__, 'id'),
+        master_ips=pulumi.get(__ret__, 'master_ips'),
+        refresh_sec=pulumi.get(__ret__, 'refresh_sec'),
+        retry_sec=pulumi.get(__ret__, 'retry_sec'),
+        soa_email=pulumi.get(__ret__, 'soa_email'),
+        status=pulumi.get(__ret__, 'status'),
+        tags=pulumi.get(__ret__, 'tags'),
+        ttl_sec=pulumi.get(__ret__, 'ttl_sec'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_domain)
 def get_domain_output(domain: Optional[pulumi.Input[Optional[str]]] = None,
                       id: Optional[pulumi.Input[Optional[int]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDomainResult]:
     """
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_domain_record.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_domain_record.py`

 * *Files 4% similar despite different names*

```diff
@@ -206,26 +206,26 @@
     __args__['domainId'] = domain_id
     __args__['id'] = id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDomainRecord:getDomainRecord', __args__, opts=opts, typ=GetDomainRecordResult).value
 
     return AwaitableGetDomainRecordResult(
-        domain_id=__ret__.domain_id,
-        id=__ret__.id,
-        name=__ret__.name,
-        port=__ret__.port,
-        priority=__ret__.priority,
-        protocol=__ret__.protocol,
-        service=__ret__.service,
-        tag=__ret__.tag,
-        target=__ret__.target,
-        ttl_sec=__ret__.ttl_sec,
-        type=__ret__.type,
-        weight=__ret__.weight)
+        domain_id=pulumi.get(__ret__, 'domain_id'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        port=pulumi.get(__ret__, 'port'),
+        priority=pulumi.get(__ret__, 'priority'),
+        protocol=pulumi.get(__ret__, 'protocol'),
+        service=pulumi.get(__ret__, 'service'),
+        tag=pulumi.get(__ret__, 'tag'),
+        target=pulumi.get(__ret__, 'target'),
+        ttl_sec=pulumi.get(__ret__, 'ttl_sec'),
+        type=pulumi.get(__ret__, 'type'),
+        weight=pulumi.get(__ret__, 'weight'))
 
 
 @_utilities.lift_output_func(get_domain_record)
 def get_domain_record_output(domain_id: Optional[pulumi.Input[int]] = None,
                              id: Optional[pulumi.Input[Optional[int]]] = None,
                              name: Optional[pulumi.Input[Optional[str]]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDomainRecordResult]:
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_domain_zonefile.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_domain_zonefile.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,17 +86,17 @@
     """
     __args__ = dict()
     __args__['domainId'] = domain_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getDomainZonefile:getDomainZonefile', __args__, opts=opts, typ=GetDomainZonefileResult).value
 
     return AwaitableGetDomainZonefileResult(
-        domain_id=__ret__.domain_id,
-        id=__ret__.id,
-        zone_files=__ret__.zone_files)
+        domain_id=pulumi.get(__ret__, 'domain_id'),
+        id=pulumi.get(__ret__, 'id'),
+        zone_files=pulumi.get(__ret__, 'zone_files'))
 
 
 @_utilities.lift_output_func(get_domain_zonefile)
 def get_domain_zonefile_output(domain_id: Optional[pulumi.Input[int]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDomainZonefileResult]:
     """
     Provides information about a Linode Domain Zonefile.
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_firewall.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_firewall.py`

 * *Files 8% similar despite different names*

```diff
@@ -175,25 +175,25 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getFirewall:getFirewall', __args__, opts=opts, typ=GetFirewallResult).value
 
     return AwaitableGetFirewallResult(
-        devices=__ret__.devices,
-        disabled=__ret__.disabled,
-        id=__ret__.id,
-        inbound_policy=__ret__.inbound_policy,
-        inbounds=__ret__.inbounds,
-        label=__ret__.label,
-        linodes=__ret__.linodes,
-        outbound_policy=__ret__.outbound_policy,
-        outbounds=__ret__.outbounds,
-        status=__ret__.status,
-        tags=__ret__.tags)
+        devices=pulumi.get(__ret__, 'devices'),
+        disabled=pulumi.get(__ret__, 'disabled'),
+        id=pulumi.get(__ret__, 'id'),
+        inbound_policy=pulumi.get(__ret__, 'inbound_policy'),
+        inbounds=pulumi.get(__ret__, 'inbounds'),
+        label=pulumi.get(__ret__, 'label'),
+        linodes=pulumi.get(__ret__, 'linodes'),
+        outbound_policy=pulumi.get(__ret__, 'outbound_policy'),
+        outbounds=pulumi.get(__ret__, 'outbounds'),
+        status=pulumi.get(__ret__, 'status'),
+        tags=pulumi.get(__ret__, 'tags'))
 
 
 @_utilities.lift_output_func(get_firewall)
 def get_firewall_output(id: Optional[pulumi.Input[int]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetFirewallResult]:
     """
     Provides details about a Linode Firewall.
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_image.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_image.py`

 * *Files 8% similar despite different names*

```diff
@@ -191,26 +191,26 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getImage:getImage', __args__, opts=opts, typ=GetImageResult).value
 
     return AwaitableGetImageResult(
-        created=__ret__.created,
-        created_by=__ret__.created_by,
-        deprecated=__ret__.deprecated,
-        description=__ret__.description,
-        expiry=__ret__.expiry,
-        id=__ret__.id,
-        is_public=__ret__.is_public,
-        label=__ret__.label,
-        size=__ret__.size,
-        status=__ret__.status,
-        type=__ret__.type,
-        vendor=__ret__.vendor)
+        created=pulumi.get(__ret__, 'created'),
+        created_by=pulumi.get(__ret__, 'created_by'),
+        deprecated=pulumi.get(__ret__, 'deprecated'),
+        description=pulumi.get(__ret__, 'description'),
+        expiry=pulumi.get(__ret__, 'expiry'),
+        id=pulumi.get(__ret__, 'id'),
+        is_public=pulumi.get(__ret__, 'is_public'),
+        label=pulumi.get(__ret__, 'label'),
+        size=pulumi.get(__ret__, 'size'),
+        status=pulumi.get(__ret__, 'status'),
+        type=pulumi.get(__ret__, 'type'),
+        vendor=pulumi.get(__ret__, 'vendor'))
 
 
 @_utilities.lift_output_func(get_image)
 def get_image_output(id: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetImageResult]:
     """
     Provides information about a Linode image
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_images.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_images.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,20 +163,20 @@
     __args__['latest'] = latest
     __args__['order'] = order
     __args__['orderBy'] = order_by
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getImages:getImages', __args__, opts=opts, typ=GetImagesResult).value
 
     return AwaitableGetImagesResult(
-        filters=__ret__.filters,
-        id=__ret__.id,
-        images=__ret__.images,
-        latest=__ret__.latest,
-        order=__ret__.order,
-        order_by=__ret__.order_by)
+        filters=pulumi.get(__ret__, 'filters'),
+        id=pulumi.get(__ret__, 'id'),
+        images=pulumi.get(__ret__, 'images'),
+        latest=pulumi.get(__ret__, 'latest'),
+        order=pulumi.get(__ret__, 'order'),
+        order_by=pulumi.get(__ret__, 'order_by'))
 
 
 @_utilities.lift_output_func(get_images)
 def get_images_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetImagesFilterArgs']]]]] = None,
                       images: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetImagesImageArgs']]]]] = None,
                       latest: Optional[pulumi.Input[Optional[bool]]] = None,
                       order: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_instance_backups.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_instance_backups.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,19 +91,19 @@
     """
     __args__ = dict()
     __args__['linodeId'] = linode_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getInstanceBackups:getInstanceBackups', __args__, opts=opts, typ=GetInstanceBackupsResult).value
 
     return AwaitableGetInstanceBackupsResult(
-        automatics=__ret__.automatics,
-        currents=__ret__.currents,
-        id=__ret__.id,
-        in_progresses=__ret__.in_progresses,
-        linode_id=__ret__.linode_id)
+        automatics=pulumi.get(__ret__, 'automatics'),
+        currents=pulumi.get(__ret__, 'currents'),
+        id=pulumi.get(__ret__, 'id'),
+        in_progresses=pulumi.get(__ret__, 'in_progresses'),
+        linode_id=pulumi.get(__ret__, 'linode_id'))
 
 
 @_utilities.lift_output_func(get_instance_backups)
 def get_instance_backups_output(linode_id: Optional[pulumi.Input[int]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstanceBackupsResult]:
     """
     Provides details about the backups of an Instance.
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_instance_networking.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_instance_networking.py`

 * *Files 6% similar despite different names*

```diff
@@ -82,18 +82,18 @@
     """
     __args__ = dict()
     __args__['linodeId'] = linode_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getInstanceNetworking:getInstanceNetworking', __args__, opts=opts, typ=GetInstanceNetworkingResult).value
 
     return AwaitableGetInstanceNetworkingResult(
-        id=__ret__.id,
-        ipv4s=__ret__.ipv4s,
-        ipv6s=__ret__.ipv6s,
-        linode_id=__ret__.linode_id)
+        id=pulumi.get(__ret__, 'id'),
+        ipv4s=pulumi.get(__ret__, 'ipv4s'),
+        ipv6s=pulumi.get(__ret__, 'ipv6s'),
+        linode_id=pulumi.get(__ret__, 'linode_id'))
 
 
 @_utilities.lift_output_func(get_instance_networking)
 def get_instance_networking_output(linode_id: Optional[pulumi.Input[int]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstanceNetworkingResult]:
     """
     Provides details about the networking configuration of an Instance.
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_instance_type.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_instance_type.py`

 * *Files 5% similar despite different names*

```diff
@@ -171,24 +171,24 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['label'] = label
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getInstanceType:getInstanceType', __args__, opts=opts, typ=GetInstanceTypeResult).value
 
     return AwaitableGetInstanceTypeResult(
-        addons=__ret__.addons,
-        class_=__ret__.class_,
-        disk=__ret__.disk,
-        id=__ret__.id,
-        label=__ret__.label,
-        memory=__ret__.memory,
-        network_out=__ret__.network_out,
-        price=__ret__.price,
-        transfer=__ret__.transfer,
-        vcpus=__ret__.vcpus)
+        addons=pulumi.get(__ret__, 'addons'),
+        class_=pulumi.get(__ret__, 'class_'),
+        disk=pulumi.get(__ret__, 'disk'),
+        id=pulumi.get(__ret__, 'id'),
+        label=pulumi.get(__ret__, 'label'),
+        memory=pulumi.get(__ret__, 'memory'),
+        network_out=pulumi.get(__ret__, 'network_out'),
+        price=pulumi.get(__ret__, 'price'),
+        transfer=pulumi.get(__ret__, 'transfer'),
+        vcpus=pulumi.get(__ret__, 'vcpus'))
 
 
 @_utilities.lift_output_func(get_instance_type)
 def get_instance_type_output(id: Optional[pulumi.Input[str]] = None,
                              label: Optional[pulumi.Input[Optional[str]]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstanceTypeResult]:
     """
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_instance_types.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_instance_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,19 +141,19 @@
     __args__['order'] = order
     __args__['orderBy'] = order_by
     __args__['types'] = types
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getInstanceTypes:getInstanceTypes', __args__, opts=opts, typ=GetInstanceTypesResult).value
 
     return AwaitableGetInstanceTypesResult(
-        filters=__ret__.filters,
-        id=__ret__.id,
-        order=__ret__.order,
-        order_by=__ret__.order_by,
-        types=__ret__.types)
+        filters=pulumi.get(__ret__, 'filters'),
+        id=pulumi.get(__ret__, 'id'),
+        order=pulumi.get(__ret__, 'order'),
+        order_by=pulumi.get(__ret__, 'order_by'),
+        types=pulumi.get(__ret__, 'types'))
 
 
 @_utilities.lift_output_func(get_instance_types)
 def get_instance_types_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetInstanceTypesFilterArgs']]]]] = None,
                               order: Optional[pulumi.Input[Optional[str]]] = None,
                               order_by: Optional[pulumi.Input[Optional[str]]] = None,
                               types: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetInstanceTypesTypeArgs']]]]] = None,
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_instances.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,19 +150,19 @@
     __args__['filters'] = filters
     __args__['order'] = order
     __args__['orderBy'] = order_by
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getInstances:getInstances', __args__, opts=opts, typ=GetInstancesResult).value
 
     return AwaitableGetInstancesResult(
-        filters=__ret__.filters,
-        id=__ret__.id,
-        instances=__ret__.instances,
-        order=__ret__.order,
-        order_by=__ret__.order_by)
+        filters=pulumi.get(__ret__, 'filters'),
+        id=pulumi.get(__ret__, 'id'),
+        instances=pulumi.get(__ret__, 'instances'),
+        order=pulumi.get(__ret__, 'order'),
+        order_by=pulumi.get(__ret__, 'order_by'))
 
 
 @_utilities.lift_output_func(get_instances)
 def get_instances_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetInstancesFilterArgs']]]]] = None,
                          order: Optional[pulumi.Input[Optional[str]]] = None,
                          order_by: Optional[pulumi.Input[Optional[str]]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstancesResult]:
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_ipv6_range.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_ipv6_range.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,20 +116,20 @@
     """
     __args__ = dict()
     __args__['range'] = range
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getIpv6Range:getIpv6Range', __args__, opts=opts, typ=GetIpv6RangeResult).value
 
     return AwaitableGetIpv6RangeResult(
-        id=__ret__.id,
-        is_bgp=__ret__.is_bgp,
-        linodes=__ret__.linodes,
-        prefix=__ret__.prefix,
-        range=__ret__.range,
-        region=__ret__.region)
+        id=pulumi.get(__ret__, 'id'),
+        is_bgp=pulumi.get(__ret__, 'is_bgp'),
+        linodes=pulumi.get(__ret__, 'linodes'),
+        prefix=pulumi.get(__ret__, 'prefix'),
+        range=pulumi.get(__ret__, 'range'),
+        region=pulumi.get(__ret__, 'region'))
 
 
 @_utilities.lift_output_func(get_ipv6_range)
 def get_ipv6_range_output(range: Optional[pulumi.Input[str]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetIpv6RangeResult]:
     """
     Provides information about a Linode IPv6 Range.
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_kernel.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_kernel.py`

 * *Files 4% similar despite different names*

```diff
@@ -146,22 +146,22 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getKernel:getKernel', __args__, opts=opts, typ=GetKernelResult).value
 
     return AwaitableGetKernelResult(
-        architecture=__ret__.architecture,
-        deprecated=__ret__.deprecated,
-        id=__ret__.id,
-        kvm=__ret__.kvm,
-        label=__ret__.label,
-        pvops=__ret__.pvops,
-        version=__ret__.version,
-        xen=__ret__.xen)
+        architecture=pulumi.get(__ret__, 'architecture'),
+        deprecated=pulumi.get(__ret__, 'deprecated'),
+        id=pulumi.get(__ret__, 'id'),
+        kvm=pulumi.get(__ret__, 'kvm'),
+        label=pulumi.get(__ret__, 'label'),
+        pvops=pulumi.get(__ret__, 'pvops'),
+        version=pulumi.get(__ret__, 'version'),
+        xen=pulumi.get(__ret__, 'xen'))
 
 
 @_utilities.lift_output_func(get_kernel)
 def get_kernel_output(id: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetKernelResult]:
     """
     Provides information about a Linode kernel
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_linode_object_storage_bucket.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_linode_object_storage_bucket.py`

 * *Files 10% similar despite different names*

```diff
@@ -104,21 +104,21 @@
     __args__ = dict()
     __args__['cluster'] = cluster
     __args__['label'] = label
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getLinodeObjectStorageBucket:getLinodeObjectStorageBucket', __args__, opts=opts, typ=GetLinodeObjectStorageBucketResult).value
 
     return AwaitableGetLinodeObjectStorageBucketResult(
-        cluster=__ret__.cluster,
-        created=__ret__.created,
-        hostname=__ret__.hostname,
-        id=__ret__.id,
-        label=__ret__.label,
-        objects=__ret__.objects,
-        size=__ret__.size)
+        cluster=pulumi.get(__ret__, 'cluster'),
+        created=pulumi.get(__ret__, 'created'),
+        hostname=pulumi.get(__ret__, 'hostname'),
+        id=pulumi.get(__ret__, 'id'),
+        label=pulumi.get(__ret__, 'label'),
+        objects=pulumi.get(__ret__, 'objects'),
+        size=pulumi.get(__ret__, 'size'))
 
 
 @_utilities.lift_output_func(get_linode_object_storage_bucket)
 def get_linode_object_storage_bucket_output(cluster: Optional[pulumi.Input[str]] = None,
                                             label: Optional[pulumi.Input[str]] = None,
                                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetLinodeObjectStorageBucketResult]:
     """
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_lke_cluster.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_lke_cluster.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,25 +178,25 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getLkeCluster:getLkeCluster', __args__, opts=opts, typ=GetLkeClusterResult).value
 
     return AwaitableGetLkeClusterResult(
-        api_endpoints=__ret__.api_endpoints,
-        control_planes=__ret__.control_planes,
-        dashboard_url=__ret__.dashboard_url,
-        id=__ret__.id,
-        k8s_version=__ret__.k8s_version,
-        kubeconfig=__ret__.kubeconfig,
-        label=__ret__.label,
-        pools=__ret__.pools,
-        region=__ret__.region,
-        status=__ret__.status,
-        tags=__ret__.tags)
+        api_endpoints=pulumi.get(__ret__, 'api_endpoints'),
+        control_planes=pulumi.get(__ret__, 'control_planes'),
+        dashboard_url=pulumi.get(__ret__, 'dashboard_url'),
+        id=pulumi.get(__ret__, 'id'),
+        k8s_version=pulumi.get(__ret__, 'k8s_version'),
+        kubeconfig=pulumi.get(__ret__, 'kubeconfig'),
+        label=pulumi.get(__ret__, 'label'),
+        pools=pulumi.get(__ret__, 'pools'),
+        region=pulumi.get(__ret__, 'region'),
+        status=pulumi.get(__ret__, 'status'),
+        tags=pulumi.get(__ret__, 'tags'))
 
 
 @_utilities.lift_output_func(get_lke_cluster)
 def get_lke_cluster_output(id: Optional[pulumi.Input[int]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetLkeClusterResult]:
     """
     Provides details about an LKE Cluster.
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_lke_versions.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_lke_versions.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,9 +69,9 @@
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getLkeVersions:getLkeVersions', __args__, opts=opts, typ=GetLkeVersionsResult).value
 
     return AwaitableGetLkeVersionsResult(
-        id=__ret__.id,
-        versions=__ret__.versions)
+        id=pulumi.get(__ret__, 'id'),
+        versions=pulumi.get(__ret__, 'versions'))
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_networking_ip.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_networking_ip.py`

 * *Files 6% similar despite different names*

```diff
@@ -170,24 +170,24 @@
     """
     __args__ = dict()
     __args__['address'] = address
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getNetworkingIp:getNetworkingIp', __args__, opts=opts, typ=GetNetworkingIpResult).value
 
     return AwaitableGetNetworkingIpResult(
-        address=__ret__.address,
-        gateway=__ret__.gateway,
-        id=__ret__.id,
-        linode_id=__ret__.linode_id,
-        prefix=__ret__.prefix,
-        public=__ret__.public,
-        rdns=__ret__.rdns,
-        region=__ret__.region,
-        subnet_mask=__ret__.subnet_mask,
-        type=__ret__.type)
+        address=pulumi.get(__ret__, 'address'),
+        gateway=pulumi.get(__ret__, 'gateway'),
+        id=pulumi.get(__ret__, 'id'),
+        linode_id=pulumi.get(__ret__, 'linode_id'),
+        prefix=pulumi.get(__ret__, 'prefix'),
+        public=pulumi.get(__ret__, 'public'),
+        rdns=pulumi.get(__ret__, 'rdns'),
+        region=pulumi.get(__ret__, 'region'),
+        subnet_mask=pulumi.get(__ret__, 'subnet_mask'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_networking_ip)
 def get_networking_ip_output(address: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNetworkingIpResult]:
     """
     Provides information about a Linode Networking IP Address
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_node_balancer.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_node_balancer.py`

 * *Files 8% similar despite different names*

```diff
@@ -169,25 +169,25 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getNodeBalancer:getNodeBalancer', __args__, opts=opts, typ=GetNodeBalancerResult).value
 
     return AwaitableGetNodeBalancerResult(
-        client_conn_throttle=__ret__.client_conn_throttle,
-        created=__ret__.created,
-        hostname=__ret__.hostname,
-        id=__ret__.id,
-        ipv4=__ret__.ipv4,
-        ipv6=__ret__.ipv6,
-        label=__ret__.label,
-        region=__ret__.region,
-        tags=__ret__.tags,
-        transfers=__ret__.transfers,
-        updated=__ret__.updated)
+        client_conn_throttle=pulumi.get(__ret__, 'client_conn_throttle'),
+        created=pulumi.get(__ret__, 'created'),
+        hostname=pulumi.get(__ret__, 'hostname'),
+        id=pulumi.get(__ret__, 'id'),
+        ipv4=pulumi.get(__ret__, 'ipv4'),
+        ipv6=pulumi.get(__ret__, 'ipv6'),
+        label=pulumi.get(__ret__, 'label'),
+        region=pulumi.get(__ret__, 'region'),
+        tags=pulumi.get(__ret__, 'tags'),
+        transfers=pulumi.get(__ret__, 'transfers'),
+        updated=pulumi.get(__ret__, 'updated'))
 
 
 @_utilities.lift_output_func(get_node_balancer)
 def get_node_balancer_output(id: Optional[pulumi.Input[int]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNodeBalancerResult]:
     """
     Provides details about a Linode NodeBalancer.
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_node_balancer_config.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_node_balancer_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -260,32 +260,32 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['nodebalancerId'] = nodebalancer_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getNodeBalancerConfig:getNodeBalancerConfig', __args__, opts=opts, typ=GetNodeBalancerConfigResult).value
 
     return AwaitableGetNodeBalancerConfigResult(
-        algorithm=__ret__.algorithm,
-        check=__ret__.check,
-        check_attempts=__ret__.check_attempts,
-        check_body=__ret__.check_body,
-        check_interval=__ret__.check_interval,
-        check_passive=__ret__.check_passive,
-        check_path=__ret__.check_path,
-        check_timeout=__ret__.check_timeout,
-        cipher_suite=__ret__.cipher_suite,
-        id=__ret__.id,
-        node_statuses=__ret__.node_statuses,
-        nodebalancer_id=__ret__.nodebalancer_id,
-        port=__ret__.port,
-        protocol=__ret__.protocol,
-        proxy_protocol=__ret__.proxy_protocol,
-        ssl_commonname=__ret__.ssl_commonname,
-        ssl_fingerprint=__ret__.ssl_fingerprint,
-        stickiness=__ret__.stickiness)
+        algorithm=pulumi.get(__ret__, 'algorithm'),
+        check=pulumi.get(__ret__, 'check'),
+        check_attempts=pulumi.get(__ret__, 'check_attempts'),
+        check_body=pulumi.get(__ret__, 'check_body'),
+        check_interval=pulumi.get(__ret__, 'check_interval'),
+        check_passive=pulumi.get(__ret__, 'check_passive'),
+        check_path=pulumi.get(__ret__, 'check_path'),
+        check_timeout=pulumi.get(__ret__, 'check_timeout'),
+        cipher_suite=pulumi.get(__ret__, 'cipher_suite'),
+        id=pulumi.get(__ret__, 'id'),
+        node_statuses=pulumi.get(__ret__, 'node_statuses'),
+        nodebalancer_id=pulumi.get(__ret__, 'nodebalancer_id'),
+        port=pulumi.get(__ret__, 'port'),
+        protocol=pulumi.get(__ret__, 'protocol'),
+        proxy_protocol=pulumi.get(__ret__, 'proxy_protocol'),
+        ssl_commonname=pulumi.get(__ret__, 'ssl_commonname'),
+        ssl_fingerprint=pulumi.get(__ret__, 'ssl_fingerprint'),
+        stickiness=pulumi.get(__ret__, 'stickiness'))
 
 
 @_utilities.lift_output_func(get_node_balancer_config)
 def get_node_balancer_config_output(id: Optional[pulumi.Input[int]] = None,
                                     nodebalancer_id: Optional[pulumi.Input[int]] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNodeBalancerConfigResult]:
     """
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_node_balancer_node.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_node_balancer_node.py`

 * *Files 5% similar despite different names*

```diff
@@ -146,22 +146,22 @@
     __args__['configId'] = config_id
     __args__['id'] = id
     __args__['nodebalancerId'] = nodebalancer_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getNodeBalancerNode:getNodeBalancerNode', __args__, opts=opts, typ=GetNodeBalancerNodeResult).value
 
     return AwaitableGetNodeBalancerNodeResult(
-        address=__ret__.address,
-        config_id=__ret__.config_id,
-        id=__ret__.id,
-        label=__ret__.label,
-        mode=__ret__.mode,
-        nodebalancer_id=__ret__.nodebalancer_id,
-        status=__ret__.status,
-        weight=__ret__.weight)
+        address=pulumi.get(__ret__, 'address'),
+        config_id=pulumi.get(__ret__, 'config_id'),
+        id=pulumi.get(__ret__, 'id'),
+        label=pulumi.get(__ret__, 'label'),
+        mode=pulumi.get(__ret__, 'mode'),
+        nodebalancer_id=pulumi.get(__ret__, 'nodebalancer_id'),
+        status=pulumi.get(__ret__, 'status'),
+        weight=pulumi.get(__ret__, 'weight'))
 
 
 @_utilities.lift_output_func(get_node_balancer_node)
 def get_node_balancer_node_output(config_id: Optional[pulumi.Input[int]] = None,
                                   id: Optional[pulumi.Input[int]] = None,
                                   nodebalancer_id: Optional[pulumi.Input[int]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNodeBalancerNodeResult]:
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_object_storage_cluster.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_object_storage_cluster.py`

 * *Files 9% similar despite different names*

```diff
@@ -110,19 +110,19 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getObjectStorageCluster:getObjectStorageCluster', __args__, opts=opts, typ=GetObjectStorageClusterResult).value
 
     return AwaitableGetObjectStorageClusterResult(
-        domain=__ret__.domain,
-        id=__ret__.id,
-        region=__ret__.region,
-        static_site_domain=__ret__.static_site_domain,
-        status=__ret__.status)
+        domain=pulumi.get(__ret__, 'domain'),
+        id=pulumi.get(__ret__, 'id'),
+        region=pulumi.get(__ret__, 'region'),
+        static_site_domain=pulumi.get(__ret__, 'static_site_domain'),
+        status=pulumi.get(__ret__, 'status'))
 
 
 @_utilities.lift_output_func(get_object_storage_cluster)
 def get_object_storage_cluster_output(id: Optional[pulumi.Input[str]] = None,
                                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetObjectStorageClusterResult]:
     """
     Provides information about a Linode Object Storage Cluster
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_profile.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -177,18 +177,18 @@
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getProfile:getProfile', __args__, opts=opts, typ=GetProfileResult).value
 
     return AwaitableGetProfileResult(
-        authorized_keys=__ret__.authorized_keys,
-        email=__ret__.email,
-        email_notifications=__ret__.email_notifications,
-        id=__ret__.id,
-        ip_whitelist_enabled=__ret__.ip_whitelist_enabled,
-        lish_auth_method=__ret__.lish_auth_method,
-        referrals=__ret__.referrals,
-        restricted=__ret__.restricted,
-        timezone=__ret__.timezone,
-        two_factor_auth=__ret__.two_factor_auth,
-        username=__ret__.username)
+        authorized_keys=pulumi.get(__ret__, 'authorized_keys'),
+        email=pulumi.get(__ret__, 'email'),
+        email_notifications=pulumi.get(__ret__, 'email_notifications'),
+        id=pulumi.get(__ret__, 'id'),
+        ip_whitelist_enabled=pulumi.get(__ret__, 'ip_whitelist_enabled'),
+        lish_auth_method=pulumi.get(__ret__, 'lish_auth_method'),
+        referrals=pulumi.get(__ret__, 'referrals'),
+        restricted=pulumi.get(__ret__, 'restricted'),
+        timezone=pulumi.get(__ret__, 'timezone'),
+        two_factor_auth=pulumi.get(__ret__, 'two_factor_auth'),
+        username=pulumi.get(__ret__, 'username'))
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_region.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_region.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,20 +123,20 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['resolvers'] = resolvers
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getRegion:getRegion', __args__, opts=opts, typ=GetRegionResult).value
 
     return AwaitableGetRegionResult(
-        capabilities=__ret__.capabilities,
-        country=__ret__.country,
-        id=__ret__.id,
-        label=__ret__.label,
-        resolvers=__ret__.resolvers,
-        status=__ret__.status)
+        capabilities=pulumi.get(__ret__, 'capabilities'),
+        country=pulumi.get(__ret__, 'country'),
+        id=pulumi.get(__ret__, 'id'),
+        label=pulumi.get(__ret__, 'label'),
+        resolvers=pulumi.get(__ret__, 'resolvers'),
+        status=pulumi.get(__ret__, 'status'))
 
 
 @_utilities.lift_output_func(get_region)
 def get_region_output(id: Optional[pulumi.Input[str]] = None,
                       resolvers: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetRegionResolverArgs']]]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRegionResult]:
     """
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_regions.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_regions.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,17 +95,17 @@
     __args__ = dict()
     __args__['filters'] = filters
     __args__['regions'] = regions
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getRegions:getRegions', __args__, opts=opts, typ=GetRegionsResult).value
 
     return AwaitableGetRegionsResult(
-        filters=__ret__.filters,
-        id=__ret__.id,
-        regions=__ret__.regions)
+        filters=pulumi.get(__ret__, 'filters'),
+        id=pulumi.get(__ret__, 'id'),
+        regions=pulumi.get(__ret__, 'regions'))
 
 
 @_utilities.lift_output_func(get_regions)
 def get_regions_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetRegionsFilterArgs']]]]] = None,
                        regions: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetRegionsRegionArgs']]]]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRegionsResult]:
     """
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_ssh_key.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_ssh_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,18 +101,18 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['label'] = label
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getSshKey:getSshKey', __args__, opts=opts, typ=GetSshKeyResult).value
 
     return AwaitableGetSshKeyResult(
-        created=__ret__.created,
-        id=__ret__.id,
-        label=__ret__.label,
-        ssh_key=__ret__.ssh_key)
+        created=pulumi.get(__ret__, 'created'),
+        id=pulumi.get(__ret__, 'id'),
+        label=pulumi.get(__ret__, 'label'),
+        ssh_key=pulumi.get(__ret__, 'ssh_key'))
 
 
 @_utilities.lift_output_func(get_ssh_key)
 def get_ssh_key_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                        label: Optional[pulumi.Input[str]] = None,
                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSshKeyResult]:
     """
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_stack_script.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_stack_script.py`

 * *Files 4% similar despite different names*

```diff
@@ -219,28 +219,28 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getStackScript:getStackScript', __args__, opts=opts, typ=GetStackScriptResult).value
 
     return AwaitableGetStackScriptResult(
-        created=__ret__.created,
-        deployments_active=__ret__.deployments_active,
-        deployments_total=__ret__.deployments_total,
-        description=__ret__.description,
-        id=__ret__.id,
-        images=__ret__.images,
-        is_public=__ret__.is_public,
-        label=__ret__.label,
-        rev_note=__ret__.rev_note,
-        script=__ret__.script,
-        updated=__ret__.updated,
-        user_defined_fields=__ret__.user_defined_fields,
-        user_gravatar_id=__ret__.user_gravatar_id,
-        username=__ret__.username)
+        created=pulumi.get(__ret__, 'created'),
+        deployments_active=pulumi.get(__ret__, 'deployments_active'),
+        deployments_total=pulumi.get(__ret__, 'deployments_total'),
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        images=pulumi.get(__ret__, 'images'),
+        is_public=pulumi.get(__ret__, 'is_public'),
+        label=pulumi.get(__ret__, 'label'),
+        rev_note=pulumi.get(__ret__, 'rev_note'),
+        script=pulumi.get(__ret__, 'script'),
+        updated=pulumi.get(__ret__, 'updated'),
+        user_defined_fields=pulumi.get(__ret__, 'user_defined_fields'),
+        user_gravatar_id=pulumi.get(__ret__, 'user_gravatar_id'),
+        username=pulumi.get(__ret__, 'username'))
 
 
 @_utilities.lift_output_func(get_stack_script)
 def get_stack_script_output(id: Optional[pulumi.Input[str]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetStackScriptResult]:
     """
     Provides details about a specific Linode StackScript.
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_stack_scripts.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_stack_scripts.py`

 * *Files 6% similar despite different names*

```diff
@@ -155,20 +155,20 @@
     __args__['order'] = order
     __args__['orderBy'] = order_by
     __args__['stackscripts'] = stackscripts
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getStackScripts:getStackScripts', __args__, opts=opts, typ=GetStackScriptsResult).value
 
     return AwaitableGetStackScriptsResult(
-        filters=__ret__.filters,
-        id=__ret__.id,
-        latest=__ret__.latest,
-        order=__ret__.order,
-        order_by=__ret__.order_by,
-        stackscripts=__ret__.stackscripts)
+        filters=pulumi.get(__ret__, 'filters'),
+        id=pulumi.get(__ret__, 'id'),
+        latest=pulumi.get(__ret__, 'latest'),
+        order=pulumi.get(__ret__, 'order'),
+        order_by=pulumi.get(__ret__, 'order_by'),
+        stackscripts=pulumi.get(__ret__, 'stackscripts'))
 
 
 @_utilities.lift_output_func(get_stack_scripts)
 def get_stack_scripts_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetStackScriptsFilterArgs']]]]] = None,
                              latest: Optional[pulumi.Input[Optional[bool]]] = None,
                              order: Optional[pulumi.Input[Optional[str]]] = None,
                              order_by: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_user.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_user.py`

 * *Files 3% similar despite different names*

```diff
@@ -245,29 +245,29 @@
     __args__['stackscriptGrants'] = stackscript_grants
     __args__['username'] = username
     __args__['volumeGrants'] = volume_grants
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getUser:getUser', __args__, opts=opts, typ=GetUserResult).value
 
     return AwaitableGetUserResult(
-        database_grants=__ret__.database_grants,
-        domain_grants=__ret__.domain_grants,
-        email=__ret__.email,
-        firewall_grants=__ret__.firewall_grants,
-        global_grants=__ret__.global_grants,
-        id=__ret__.id,
-        image_grants=__ret__.image_grants,
-        linode_grants=__ret__.linode_grants,
-        longview_grants=__ret__.longview_grants,
-        nodebalancer_grants=__ret__.nodebalancer_grants,
-        restricted=__ret__.restricted,
-        ssh_keys=__ret__.ssh_keys,
-        stackscript_grants=__ret__.stackscript_grants,
-        username=__ret__.username,
-        volume_grants=__ret__.volume_grants)
+        database_grants=pulumi.get(__ret__, 'database_grants'),
+        domain_grants=pulumi.get(__ret__, 'domain_grants'),
+        email=pulumi.get(__ret__, 'email'),
+        firewall_grants=pulumi.get(__ret__, 'firewall_grants'),
+        global_grants=pulumi.get(__ret__, 'global_grants'),
+        id=pulumi.get(__ret__, 'id'),
+        image_grants=pulumi.get(__ret__, 'image_grants'),
+        linode_grants=pulumi.get(__ret__, 'linode_grants'),
+        longview_grants=pulumi.get(__ret__, 'longview_grants'),
+        nodebalancer_grants=pulumi.get(__ret__, 'nodebalancer_grants'),
+        restricted=pulumi.get(__ret__, 'restricted'),
+        ssh_keys=pulumi.get(__ret__, 'ssh_keys'),
+        stackscript_grants=pulumi.get(__ret__, 'stackscript_grants'),
+        username=pulumi.get(__ret__, 'username'),
+        volume_grants=pulumi.get(__ret__, 'volume_grants'))
 
 
 @_utilities.lift_output_func(get_user)
 def get_user_output(database_grants: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetUserDatabaseGrantArgs']]]]] = None,
                     domain_grants: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetUserDomainGrantArgs']]]]] = None,
                     firewall_grants: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetUserFirewallGrantArgs']]]]] = None,
                     image_grants: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetUserImageGrantArgs']]]]] = None,
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_vlans.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_vlans.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,19 +124,19 @@
     __args__['order'] = order
     __args__['orderBy'] = order_by
     __args__['vlans'] = vlans
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getVlans:getVlans', __args__, opts=opts, typ=GetVlansResult).value
 
     return AwaitableGetVlansResult(
-        filters=__ret__.filters,
-        id=__ret__.id,
-        order=__ret__.order,
-        order_by=__ret__.order_by,
-        vlans=__ret__.vlans)
+        filters=pulumi.get(__ret__, 'filters'),
+        id=pulumi.get(__ret__, 'id'),
+        order=pulumi.get(__ret__, 'order'),
+        order_by=pulumi.get(__ret__, 'order_by'),
+        vlans=pulumi.get(__ret__, 'vlans'))
 
 
 @_utilities.lift_output_func(get_vlans)
 def get_vlans_output(filters: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetVlansFilterArgs']]]]] = None,
                      order: Optional[pulumi.Input[Optional[str]]] = None,
                      order_by: Optional[pulumi.Input[Optional[str]]] = None,
                      vlans: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetVlansVlanArgs']]]]] = None,
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/get_volume.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/get_volume.py`

 * *Files 4% similar despite different names*

```diff
@@ -173,24 +173,24 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('linode:index/getVolume:getVolume', __args__, opts=opts, typ=GetVolumeResult).value
 
     return AwaitableGetVolumeResult(
-        created=__ret__.created,
-        filesystem_path=__ret__.filesystem_path,
-        id=__ret__.id,
-        label=__ret__.label,
-        linode_id=__ret__.linode_id,
-        region=__ret__.region,
-        size=__ret__.size,
-        status=__ret__.status,
-        tags=__ret__.tags,
-        updated=__ret__.updated)
+        created=pulumi.get(__ret__, 'created'),
+        filesystem_path=pulumi.get(__ret__, 'filesystem_path'),
+        id=pulumi.get(__ret__, 'id'),
+        label=pulumi.get(__ret__, 'label'),
+        linode_id=pulumi.get(__ret__, 'linode_id'),
+        region=pulumi.get(__ret__, 'region'),
+        size=pulumi.get(__ret__, 'size'),
+        status=pulumi.get(__ret__, 'status'),
+        tags=pulumi.get(__ret__, 'tags'),
+        updated=pulumi.get(__ret__, 'updated'))
 
 
 @_utilities.lift_output_func(get_volume)
 def get_volume_output(id: Optional[pulumi.Input[int]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetVolumeResult]:
     """
     Provides information about a Linode Volume.
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/image.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/image.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/instance.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/instance_disk.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/instance_disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/instance_ip.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/instance_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/instance_shared_ips.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/instance_shared_ips.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/ipv6_range.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/ipv6_range.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/lke_cluster.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/lke_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/node_balancer.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/node_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/node_balancer_config.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/node_balancer_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/node_balancer_node.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/node_balancer_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/object_storage_bucket.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/object_storage_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/object_storage_key.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/object_storage_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/object_storage_object.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/object_storage_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/outputs.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/provider.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/rdns.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/rdns.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/ssh_key.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/stack_script.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/stack_script.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/token.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/user.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode/volume.py` & `pulumi_linode-4.5.0a1689096135/pulumi_linode/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode.egg-info/PKG-INFO` & `pulumi_linode-4.5.0a1689096135/pulumi_linode.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-linode
-Version: 4.5.0a1687671694
+Version: 4.5.0a1689096135
 Summary: A Pulumi package for creating and managing linode cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-linode
 Keywords: pulumi linode
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_linode-4.5.0a1687671694/pulumi_linode.egg-info/SOURCES.txt` & `pulumi_linode-4.5.0a1689096135/pulumi_linode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.5.0a1687671694/setup.py` & `pulumi_linode-4.5.0a1689096135/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.5.0a1687671694"
-PLUGIN_VERSION = "4.5.0-alpha.1687671694+b0c807b9"
+VERSION = "4.5.0a1689096135"
+PLUGIN_VERSION = "4.5.0-alpha.1689096135+5dbf35d7"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'linode', PLUGIN_VERSION])
         except OSError as error:
```

