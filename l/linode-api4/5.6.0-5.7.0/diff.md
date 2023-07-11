# Comparing `tmp/linode_api4-5.6.0.tar.gz` & `tmp/linode_api4-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linode_api4-5.6.0.tar", last modified: Mon Jun 26 18:46:48 2023, max compression
+gzip compressed data, was "linode_api4-5.7.0.tar", last modified: Tue Jul 11 19:36:11 2023, max compression
```

## Comparing `linode_api4-5.6.0.tar` & `linode_api4-5.7.0.tar`

### file list

```diff
@@ -1,222 +1,222 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:46:48.912485 linode_api4-5.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-06-26 18:46:18.000000 linode_api4-5.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-26 18:46:18.000000 linode_api4-5.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-06-26 18:46:48.912485 linode_api4-5.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6427 2023-06-26 18:46:18.000000 linode_api4-5.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-26 18:46:48.000000 linode_api4-5.6.0/baked_version
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:46:48.888485 linode_api4-5.6.0/linode_api4/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:46:48.892485 linode_api4-5.6.0/linode_api4/groups/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14565 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4296 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/linode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/lke.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/longview.py
--rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/nodebalancer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/obj.py
--rw-r--r--   0 runner    (1001) docker     (123)    13372 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/object_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)    10843 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/groups/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)    16203 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/linode_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    14902 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/login_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:46:48.896485 linode_api4-5.6.0/linode_api4/objects/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19006 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/account.py
--rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/dbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/filtering.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    52027 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/linode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10226 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/lke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/longview.py
--rw-r--r--   0 runner    (1001) docker     (123)     6426 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)    10549 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/nodebalancer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18397 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/object_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/region.py
--rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/support.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/objects/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/paginated_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/polling.py
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-06-26 18:46:18.000000 linode_api4-5.6.0/linode_api4/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:46:48.892485 linode_api4-5.6.0/linode_api4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-06-26 18:46:48.000000 linode_api4-5.6.0/linode_api4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7973 2023-06-26 18:46:48.000000 linode_api4-5.6.0/linode_api4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 18:46:48.000000 linode_api4-5.6.0/linode_api4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-26 18:46:48.000000 linode_api4-5.6.0/linode_api4.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 18:46:48.000000 linode_api4-5.6.0/linode_api4.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-26 18:46:18.000000 linode_api4-5.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 18:46:48.912485 linode_api4-5.6.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3884 2023-06-26 18:46:18.000000 linode_api4-5.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:46:48.896485 linode_api4-5.6.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:46:48.908485 linode_api4-5.6.0/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account.json
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account_events_123.json
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account_invoices.json
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account_invoices_123.json
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account_invoices_123456_items.json
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account_logins.json
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account_logins_123.json
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account_maintenance.json
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account_notifications.json
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account_oauth-clients_2737bf16b39ab5d7b4a1.json
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account_payment-method_123.json
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account_payment-methods.json
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account_payments.json
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account_promo-codes.json
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account_service-transfers.json
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account_service-transfers_12345.json
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account_settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/account_users_test-user.json
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/databases_engines.json
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/databases_instances.json
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/databases_mysql_instances.json
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/databases_mysql_instances_123_backups.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/databases_mysql_instances_123_backups_456_restore.json
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/databases_mysql_instances_123_credentials.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/databases_mysql_instances_123_credentials_reset.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/databases_mysql_instances_123_patch.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/databases_mysql_instances_123_ssl.json
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/databases_postgresql_instances.json
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/databases_postgresql_instances_123_backups.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/databases_postgresql_instances_123_backups_456_restore.json
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/databases_postgresql_instances_123_credentials.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/databases_postgresql_instances_123_credentials_reset.json
--rw-r--r--   0 runner    (1001) docker     (123)        2 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/databases_postgresql_instances_123_patch.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/databases_postgresql_instances_123_ssl.json
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/databases_types.json
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/domains.json
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/domains_12345_clone.json
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/domains_12345_records.json
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/domains_12345_zone-file.json
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/domains_import.json
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/images.json
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/images_private_1337.json
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/images_upload.json
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/linode_instances.json
--rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/linode_instances_123_backups.json
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/linode_instances_123_configs.json
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/linode_instances_123_configs_456789.json
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/linode_instances_123_disks.json
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/linode_instances_123_disks_12345_clone.json
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/linode_instances_123_firewalls.json
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/linode_instances_123_ips.json
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/linode_instances_123_nodebalancers.json
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/linode_instances_123_transfer.json
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/linode_instances_123_transfer_2023_4.json
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/linode_instances_123_volumes.json
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/linode_stackscripts_10079.json
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/linode_types.json
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/lke_clusters.json
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/lke_clusters_18881.json
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/lke_clusters_18881_dashboard.json
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/lke_clusters_18881_nodes_123456.json
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/lke_clusters_18881_pools_456.json
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/lke_versions.json
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/longview_clients.json
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/longview_plan.json
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/longview_subscriptions.json
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/mongodb.json
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/networking_firewalls.json
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/networking_firewalls_123.json
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/networking_firewalls_123_devices.json
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/networking_firewalls_123_devices_123.json
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/networking_firewalls_123_rules.json
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/networking_ips_127.0.0.1.json
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/networking_ipv6_pools.json
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/networking_ipv6_ranges.json
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/networking_ipv6_ranges_2600:3c01::.json
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/networking_vlans.json
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/nodebalancers.json
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/nodebalancers_123456_configs.json
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/nodebalancers_123456_configs_65432_nodes.json
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/nodebalancers_12345_configs_4567_rebuild.json
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/nodebalancers_12345_stats.json
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/object-storage_buckets.json
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/object-storage_buckets_us-east-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/object-storage_buckets_us-east-1_example-bucket.json
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/object-storage_buckets_us-east-1_example-bucket_object-acl.json
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/object-storage_buckets_us-east-1_example-bucket_object-list.json
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/object-storage_buckets_us-east-1_example-bucket_object-url.json
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/object-storage_buckets_us-east-1_example-bucket_ssl.json
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/object-storage_clusters.json
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/object-storage_keys.json
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/object-storage_transfer.json
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/profile.json
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/profile_device_123.json
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/profile_devices.json
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/profile_logins.json
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/profile_logins_123.json
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/profile_preferences.json
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/profile_security-questions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/profile_sshkeys.json
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/regions.json
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/support_tickets_123.json
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/tags.json
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/tags_nothing.json
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/tags_something.json
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/fixtures/volumes.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:46:48.908485 linode_api4-5.6.0/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:46:48.908485 linode_api4-5.6.0/test/integration/linode_client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/linode_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10215 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/linode_client/test_linode_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4027 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/linode_client/test_retry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:46:48.908485 linode_api4-5.6.0/test/integration/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/models/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/models/test_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/models/test_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2295 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/models/test_firewall.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/models/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    11151 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/models/test_linode.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/models/test_lke.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/models/test_longview.py
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/models/test_networking.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/models/test_nodebalancer.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/models/test_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/integration/models/test_volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:46:48.912485 linode_api4-5.6.0/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)    38608 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/linode_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/login_client_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 18:46:48.912485 linode_api4-5.6.0/test/unit/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/account_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/database_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/domain_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/firewall_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/image_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18219 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/linode_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/lke_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/longview_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/mapped_object_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/networking_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/nodebalancers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/object_storage_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/polling_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/profile_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/region_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/support_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/tag_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/objects/volume_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/paginated_list_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-26 18:46:18.000000 linode_api4-5.6.0/test/unit/util_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:36:11.885188 linode_api4-5.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-11 19:35:51.000000 linode_api4-5.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 19:35:51.000000 linode_api4-5.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-07-11 19:36:11.885188 linode_api4-5.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6423 2023-07-11 19:35:51.000000 linode_api4-5.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-11 19:36:11.000000 linode_api4-5.7.0/baked_version
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:36:11.849187 linode_api4-5.7.0/linode_api4/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:36:11.857188 linode_api4-5.7.0/linode_api4/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14997 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16737 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/linode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5450 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/lke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/longview.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/nodebalancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/obj.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13937 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11275 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4282 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/groups/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16304 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/linode_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14902 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/login_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:36:11.861188 linode_api4-5.7.0/linode_api4/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19006 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15686 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13272 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/dbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5704 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/filtering.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52231 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/linode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/lke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/longview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6436 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10592 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/nodebalancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18889 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5523 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/support.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/objects/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8251 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/paginated_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6337 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/polling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-07-11 19:35:51.000000 linode_api4-5.7.0/linode_api4/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:36:11.849187 linode_api4-5.7.0/linode_api4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7365 2023-07-11 19:36:11.000000 linode_api4-5.7.0/linode_api4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7979 2023-07-11 19:36:11.000000 linode_api4-5.7.0/linode_api4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 19:36:11.000000 linode_api4-5.7.0/linode_api4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-11 19:36:11.000000 linode_api4-5.7.0/linode_api4.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-11 19:36:11.000000 linode_api4-5.7.0/linode_api4.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-11 19:35:51.000000 linode_api4-5.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 19:36:11.885188 linode_api4-5.7.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3884 2023-07-11 19:35:51.000000 linode_api4-5.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:36:11.861188 linode_api4-5.7.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:36:11.877188 linode_api4-5.7.0/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account.json
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account_events_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account_invoices.json
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account_invoices_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account_invoices_123456_items.json
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account_logins.json
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account_logins_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account_maintenance.json
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account_notifications.json
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account_oauth-clients_2737bf16b39ab5d7b4a1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account_payment-method_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account_payment-methods.json
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account_payments.json
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account_promo-codes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account_service-transfers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account_service-transfers_12345.json
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account_settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/account_users_test-user.json
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/databases_engines.json
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/databases_instances.json
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/databases_mysql_instances.json
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/databases_mysql_instances_123_backups.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/databases_mysql_instances_123_backups_456_restore.json
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/databases_mysql_instances_123_credentials.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/databases_mysql_instances_123_credentials_reset.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/databases_mysql_instances_123_patch.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/databases_mysql_instances_123_ssl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/databases_postgresql_instances.json
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/databases_postgresql_instances_123_backups.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/databases_postgresql_instances_123_backups_456_restore.json
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/databases_postgresql_instances_123_credentials.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/databases_postgresql_instances_123_credentials_reset.json
+-rw-r--r--   0 runner    (1001) docker     (123)        2 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/databases_postgresql_instances_123_patch.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/databases_postgresql_instances_123_ssl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/databases_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/domains.json
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/domains_12345_clone.json
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/domains_12345_records.json
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/domains_12345_zone-file.json
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/domains_import.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/images.json
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/images_private_1337.json
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/images_upload.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/linode_instances.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1864 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/linode_instances_123_backups.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/linode_instances_123_configs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/linode_instances_123_configs_456789.json
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/linode_instances_123_disks.json
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/linode_instances_123_disks_12345_clone.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/linode_instances_123_firewalls.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/linode_instances_123_ips.json
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/linode_instances_123_nodebalancers.json
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/linode_instances_123_transfer.json
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/linode_instances_123_transfer_2023_4.json
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/linode_instances_123_volumes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/linode_stackscripts_10079.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/linode_types.json
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/lke_clusters.json
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/lke_clusters_18881.json
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/lke_clusters_18881_dashboard.json
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/lke_clusters_18881_nodes_123456.json
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/lke_clusters_18881_pools_456.json
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/lke_versions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/longview_clients.json
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/longview_plan.json
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/longview_subscriptions.json
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/mongodb.json
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/networking_firewalls.json
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/networking_firewalls_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/networking_firewalls_123_devices.json
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/networking_firewalls_123_devices_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/networking_firewalls_123_rules.json
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/networking_ips_127.0.0.1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/networking_ipv6_pools.json
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/networking_ipv6_ranges.json
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/networking_ipv6_ranges_2600%3A3c01%3A%3A.json
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/networking_vlans.json
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/nodebalancers.json
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/nodebalancers_123456_configs.json
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/nodebalancers_123456_configs_65432_nodes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/nodebalancers_12345_configs_4567_rebuild.json
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/nodebalancers_12345_stats.json
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/object-storage_buckets.json
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/object-storage_buckets_us-east-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/object-storage_buckets_us-east-1_example-bucket.json
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/object-storage_buckets_us-east-1_example-bucket_object-acl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/object-storage_buckets_us-east-1_example-bucket_object-list.json
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/object-storage_buckets_us-east-1_example-bucket_object-url.json
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/object-storage_buckets_us-east-1_example-bucket_ssl.json
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/object-storage_clusters.json
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/object-storage_keys.json
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/object-storage_transfer.json
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/profile.json
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/profile_device_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/profile_devices.json
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/profile_logins.json
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/profile_logins_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/profile_preferences.json
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/profile_security-questions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/profile_sshkeys.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/regions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/support_tickets_123.json
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/tags.json
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/tags_nothing.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/tags_something.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/fixtures/volumes.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:36:11.877188 linode_api4-5.7.0/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4637 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:36:11.877188 linode_api4-5.7.0/test/integration/linode_client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/linode_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10310 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/linode_client/test_linode_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/linode_client/test_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:36:11.881188 linode_api4-5.7.0/test/integration/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/models/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11229 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/models/test_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/models/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/models/test_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/models/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/models/test_linode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/models/test_lke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/models/test_longview.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/models/test_networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3053 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/models/test_nodebalancer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/models/test_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/integration/models/test_volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:36:11.881188 linode_api4-5.7.0/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5457 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38670 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/linode_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/login_client_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 19:36:11.885188 linode_api4-5.7.0/test/unit/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     8498 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/account_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/database_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/domain_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/firewall_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/linode_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/lke_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/longview_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/mapped_object_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/networking_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6570 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/nodebalancers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10079 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/object_storage_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/polling_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4096 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/profile_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/region_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/support_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/tag_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/objects/volume_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/paginated_list_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-11 19:35:51.000000 linode_api4-5.7.0/test/unit/util_test.py
```

### Comparing `linode_api4-5.6.0/LICENSE` & `linode_api4-5.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/PKG-INFO` & `linode_api4-5.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linode_api4
-Version: 5.6.0
+Version: 5.7.0
 Summary: The official python SDK for Linode API v4
 Home-page: https://github.com/linode/linode_api4-python
 Author: Linode
 Author-email: developers@linode.com
 License: BSD 3-Clause License
 Keywords: linode cloud hosting infrastructure
 Classifier: Development Status :: 5 - Production/Stable
@@ -161,15 +161,15 @@
 
 Integration Tests
 -----------------
 Integration tests live in the ``test/integration`` directory.
 
 Pre-requisite
 ^^^^^^^^^^^^^^^^^
-Export Linode API token as `LINODE_CLI_TOKEN` before running integration tests::
+Export Linode API token as `LINODE_TOKEN` before running integration tests::
 
     export LINODE_TOKEN = $(your_token)
 
 Running the tests
 ^^^^^^^^^^^^^^^^^
 Run the tests locally using the make command. Run the entire test suite using command below::
```

### Comparing `linode_api4-5.6.0/README.rst` & `linode_api4-5.7.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
 
 Integration Tests
 -----------------
 Integration tests live in the ``test/integration`` directory.
 
 Pre-requisite
 ^^^^^^^^^^^^^^^^^
-Export Linode API token as `LINODE_CLI_TOKEN` before running integration tests::
+Export Linode API token as `LINODE_TOKEN` before running integration tests::
 
     export LINODE_TOKEN = $(your_token)
 
 Running the tests
 ^^^^^^^^^^^^^^^^^
 Run the tests locally using the make command. Run the entire test suite using command below::
```

### Comparing `linode_api4-5.6.0/linode_api4/common.py` & `linode_api4-5.7.0/linode_api4/common.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/errors.py` & `linode_api4-5.7.0/linode_api4/errors.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/groups/account.py` & `linode_api4-5.7.0/linode_api4/groups/account.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
     def events(self, *filters):
         """
         Lists events on the current account matching the given filters.
 
         API Documentation: https://www.linode.com/docs/api/account/#events-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of events on the current account matching the given filters.
         :rtype: PaginatedList of Event
         """
 
         return self.client._get_and_filter(Event, *filters)
 
@@ -120,14 +122,16 @@
     def oauth_clients(self, *filters):
         """
         Returns the OAuth Clients associated with this account.
 
         API Documentation: https://www.linode.com/docs/api/account/#oauth-clients-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of OAuth Clients associated with this account.
         :rtype: PaginatedList of OAuthClient
         """
         return self.client._get_and_filter(OAuthClient, *filters)
 
     def oauth_client_create(self, name, redirect_uri, **kwargs):
@@ -163,14 +167,16 @@
     def users(self, *filters):
         """
         Returns a list of users on this account.
 
         API Documentation: https://www.linode.com/docs/api/account/#users-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of users on this account.
         :rtype: PaginatedList of User
         """
         return self.client._get_and_filter(User, *filters)
 
     def logins(self):
```

### Comparing `linode_api4-5.6.0/linode_api4/groups/database.py` & `linode_api4-5.7.0/linode_api4/groups/database.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,17 @@
         referenced to on their own. DatabaseTypes can be
         filtered to return specific types, for example::
 
            database_types = client.database.types(DatabaseType.deprecated == False)
 
         API Documentation: https://www.linode.com/docs/api/databases/#managed-database-types-list
 
-        :param filters: Any number of filters to apply to the query.
+        :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of types that match the query.
         :rtype: PaginatedList of DatabaseType
         """
         return self.client._get_and_filter(DatabaseType, *filters)
 
     def engines(self, *filters):
@@ -47,41 +49,47 @@
         referenced to on their own. Engines can be filtered to
         return specific engines, for example::
 
            mysql_engines = client.database.engines(DatabaseEngine.engine == 'mysql')
 
         API Documentation: https://www.linode.com/docs/api/databases/#managed-database-engines-list
 
-        :param filters: Any number of filters to apply to the query.
+        :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of types that match the query.
         :rtype: PaginatedList of DatabaseEngine
         """
         return self.client._get_and_filter(DatabaseEngine, *filters)
 
     def instances(self, *filters):
         """
         Returns a list of Managed Databases active on this account.
 
         API Documentation: https://www.linode.com/docs/api/databases/#managed-databases-list-all
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of databases that matched the query.
         :rtype: PaginatedList of Database
         """
         return self.client._get_and_filter(Database, *filters)
 
     def mysql_instances(self, *filters):
         """
         Returns a list of Managed MySQL Databases active on this account.
 
         API Documentation: https://www.linode.com/docs/api/databases/#managed-mysql-databases-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of MySQL databases that matched the query.
         :rtype: PaginatedList of MySQLDatabase
         """
         return self.client._get_and_filter(MySQLDatabase, *filters)
 
     def mysql_create(self, label, region, engine, ltype, **kwargs):
@@ -137,14 +145,16 @@
     def postgresql_instances(self, *filters):
         """
         Returns a list of Managed PostgreSQL Databases active on this account.
 
         API Documentation: https://www.linode.com/docs/api/databases/#managed-postgresql-databases-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of PostgreSQL databases that matched the query.
         :rtype: PaginatedList of PostgreSQLDatabase
         """
         return self.client._get_and_filter(PostgreSQLDatabase, *filters)
 
     def postgresql_create(self, label, region, engine, ltype, **kwargs):
```

### Comparing `linode_api4-5.6.0/linode_api4/groups/domain.py` & `linode_api4-5.7.0/linode_api4/groups/domain.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
         class, like this::
 
            domains = client.domains()
 
         API Documentation: https://www.linode.com/docs/api/domains/#domains-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of Domains the acting user can access.
         :rtype: PaginatedList of Domain
         """
         return self.client._get_and_filter(Domain, *filters)
 
     def create(self, domain, master=True, **kwargs):
```

### Comparing `linode_api4-5.6.0/linode_api4/groups/image.py` & `linode_api4-5.7.0/linode_api4/groups/image.py`

 * *Files 21% similar despite different names*

```diff
@@ -16,79 +16,95 @@
         retrieve only Images relevant to a specific query, for example::
 
            debian_images = client.images(
                Image.vendor == "debain")
 
         API Documentation: https://www.linode.com/docs/api/images/#images-list
 
-        :param filters: Any number of filters to apply to the query.
+        :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of available Images.
         :rtype: PaginatedList of Image
         """
         return self.client._get_and_filter(Image, *filters)
 
-    def create(self, disk, label=None, description=None):
+    def create(self, disk, label=None, description=None, cloud_init=False):
         """
         Creates a new Image from a disk you own.
 
         API Documentation: https://www.linode.com/docs/api/images/#image-create
 
         :param disk: The Disk to imagize.
         :type disk: Disk or int
         :param label: The label for the resulting Image (defaults to the disk's
                       label.
         :type label: str
         :param description: The description for the new Image.
         :type description: str
+        :param cloud_init: Whether this Image supports cloud-init.
+        :type cloud_init: bool
 
         :returns: The new Image.
         :rtype: Image
         """
         params = {
             "disk_id": disk.id if issubclass(type(disk), Base) else disk,
         }
 
         if label is not None:
             params["label"] = label
 
         if description is not None:
             params["description"] = description
 
+        if cloud_init:
+            params["cloud_init"] = cloud_init
+
         result = self.client.post("/images", data=params)
 
         if not "id" in result:
             raise UnexpectedResponseError(
                 "Unexpected response when creating an Image from disk {}".format(
                     disk
                 )
             )
 
         return Image(self.client, result["id"], result)
 
     def create_upload(
-        self, label: str, region: str, description: str = None
+        self,
+        label: str,
+        region: str,
+        description: str = None,
+        cloud_init: bool = False,
     ) -> Tuple[Image, str]:
         """
         Creates a new Image and returns the corresponding upload URL.
 
         API Documentation: https://www.linode.com/docs/api/images/#image-upload
 
         :param label: The label of the Image to create.
         :type label: str
         :param region: The region to upload to. Once the image has been created, it can be used in any region.
         :type region: str
         :param description: The description for the new Image.
         :type description: str
+        :param cloud_init: Whether this Image supports cloud-init.
+        :type cloud_init: bool
 
         :returns: A tuple containing the new image and the image upload URL.
         :rtype: (Image, str)
         """
         params = {"label": label, "region": region, "description": description}
 
+        if cloud_init:
+            params["cloud_init"] = cloud_init
+
         result = self.client.post("/images/upload", data=drop_null_keys(params))
 
         if "image" not in result:
             raise UnexpectedResponseError(
                 "Unexpected response when creating an Image upload URL"
             )
```

### Comparing `linode_api4-5.6.0/linode_api4/groups/linode.py` & `linode_api4-5.7.0/linode_api4/groups/linode.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import base64
 import os
 
 from linode_api4 import Profile
 from linode_api4.common import SSH_KEY_TYPES, load_and_validate_keys
 from linode_api4.errors import UnexpectedResponseError
 from linode_api4.groups import Group
 from linode_api4.objects import (
@@ -37,15 +38,17 @@
         or resize Linodes, or simply referenced on their own.  Types can be
         filtered to return specific types, for example::
 
            standard_types = client.linode.types(Type.class == "standard")
 
         API documentation: https://www.linode.com/docs/api/linode-types/#types-list
 
-        :param filters: Any number of filters to apply to the query.
+        :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of types that match the query.
         :rtype: PaginatedList of Type
         """
         return self.client._get_and_filter(Type, *filters)
 
     def instances(self, *filters):
@@ -54,14 +57,16 @@
         this query to return only Linodes that match specific criteria::
 
            prod_linodes = client.linode.instances(Instance.group == "prod")
 
         API Documentation: https://www.linode.com/docs/api/linode-instances/#linodes-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of Instances that matched the query.
         :rtype: PaginatedList of Instance
         """
         return self.client._get_and_filter(Instance, *filters)
 
     def stackscripts(self, *filters, **kwargs):
@@ -72,14 +77,16 @@
         also request only your own private :any:`StackScripts<StackScript>`::
 
            my_stackscripts = client.linode.stackscripts(mine_only=True)
 
         API Documentation: https://www.linode.com/docs/api/stackscripts/#stackscripts-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
         :param mine_only: If True, returns only private StackScripts
         :type mine_only: bool
 
         :returns: A list of StackScripts matching the query.
         :rtype: PaginatedList of StackScript
         """
         # python2 can't handle *args and a single keyword argument, so this is a workaround
@@ -107,14 +114,16 @@
         """
         Returns a list of available :any:`Kernels<Kernel>`.  Kernels are used
         when creating or updating :any:`LinodeConfigs,LinodeConfig>`.
 
         API Documentation: https://www.linode.com/docs/api/linode-instances/#kernels-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of available kernels that match the query.
         :rtype: PaginatedList of Kernel
         """
         return self.client._get_and_filter(Kernel, *filters)
 
     # create things
@@ -233,14 +242,18 @@
         :param tags: A list of tags to apply to the new instance.  If any of the
                      tags included do not exist, they will be created as part of
                      this operation.
         :type tags: list[str]
         :param private_ip: Whether the new Instance should have private networking
                            enabled and assigned a private IPv4 address.
         :type private_ip: bool
+        :param metadata: Metadata-related fields to use when creating the new Instance.
+                         The contents of this field can be built using the
+                         :any:`build_instance_metadata` method.
+        :type metadata: dict
 
         :returns: A new Instance object, or a tuple containing the new Instance and
                   the generated password.
         :rtype: Instance or tuple(Instance, str)
         :raises ApiError: If contacting the API fails
         :raises UnexpectedResponseError: If the API response is somehow malformed.
                                          This usually indicates that you are using
@@ -289,14 +302,48 @@
             )
 
         l = Instance(self.client, result["id"], result)
         if not ret_pass:
             return l
         return l, ret_pass
 
+    @staticmethod
+    def build_instance_metadata(user_data=None, encode_user_data=True):
+        """
+        Builds the contents of the ``metadata`` field to be passed into
+        the :any:`instance_create` method. This helper can also be used
+        when cloning and rebuilding Instances.
+        **Creating an Instance with User Data**::
+            new_linode, password = client.linode.instance_create(
+                "g6-standard-2",
+                "us-east",
+                image="linode/ubuntu22.04",
+                metadata=client.linode.build_instance_metadata(user_data="myuserdata")
+            )
+        :param user_data: User-defined data to provide to the Linode Instance through
+                          the Metadata service.
+        :type user_data: str
+        :param encode_user_data: If true, the provided user_data field will be automatically
+                                 encoded to a valid base64 string. This field should only
+                                 be set to false if the user_data param is already base64-encoded.
+        :type encode_user_data: bool
+        :returns: The built ``metadata`` structure.
+        :rtype: dict
+        """
+        result = {}
+
+        if user_data is not None:
+            result["user_data"] = (
+                base64.b64encode(user_data.encode()).decode()
+                if encode_user_data
+                else user_data
+            )
+
+        return result
+
     def stackscript_create(
         self, label, script, images, desc=None, public=False, **kwargs
     ):
         """
         Creates a new :any:`StackScript` on your account.
 
         API Documentation: https://www.linode.com/docs/api/stackscripts/#stackscript-create
```

### Comparing `linode_api4-5.6.0/linode_api4/groups/lke.py` & `linode_api4-5.7.0/linode_api4/groups/lke.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,29 +18,33 @@
     def versions(self, *filters):
         """
         Returns a :any:`PaginatedList` of :any:`KubeVersion` objects that can be
         used when creating an LKE Cluster.
 
         API Documentation: https://www.linode.com/docs/api/linode-kubernetes-engine-lke/#kubernetes-versions-list
 
-        :param filters: Any number of filters to apply to the query.
+        :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A Paginated List of kube versions that match the query.
         :rtype: PaginatedList of KubeVersion
         """
         return self.client._get_and_filter(KubeVersion, *filters)
 
     def clusters(self, *filters):
         """
         Returns a :any:`PaginagtedList` of :any:`LKECluster` objects that belong
         to this account.
 
         https://www.linode.com/docs/api/linode-kubernetes-engine-lke/#kubernetes-clusters-list
 
-        :param filters: Any number of filters to apply to the query.
+        :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A Paginated List of LKE clusters that match the query.
         :rtype: PaginatedList of LKECluster
         """
         return self.client._get_and_filter(LKECluster, *filters)
 
     def cluster_create(self, region, label, node_pools, kube_version, **kwargs):
```

### Comparing `linode_api4-5.6.0/linode_api4/groups/longview.py` & `linode_api4-5.7.0/linode_api4/groups/longview.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
         """
         Requests and returns a paginated list of LongviewClients on your
         account.
 
         API Documentation: https://www.linode.com/docs/api/longview/#longview-clients-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of Longview Clients matching the given filters.
         :rtype: PaginatedList of LongviewClient
         """
         return self.client._get_and_filter(LongviewClient, *filters)
 
     def client_create(self, label=None):
@@ -55,14 +57,16 @@
     def subscriptions(self, *filters):
         """
         Requests and returns a paginated list of LongviewSubscriptions available
 
         API Documentation: https://www.linode.com/docs/api/longview/#longview-subscriptions-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of Longview Subscriptions matching the given filters.
         :rtype: PaginatedList of LongviewSubscription
         """
         return self.client._get_and_filter(LongviewSubscription, *filters)
 
     def longview_plan_update(self, longview_subscription):
```

### Comparing `linode_api4-5.6.0/linode_api4/groups/networking.py` & `linode_api4-5.7.0/linode_api4/groups/networking.py`

 * *Files 17% similar despite different names*

```diff
@@ -20,14 +20,16 @@
     def firewalls(self, *filters):
         """
         Retrieves the Firewalls your user has access to.
 
         API Documentation: https://www.linode.com/docs/api/networking/#firewalls-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of Firewalls the acting user can access.
         :rtype: PaginatedList of Firewall
         """
         return self.client._get_and_filter(Firewall, *filters)
 
     def firewall_create(self, label, rules, **kwargs):
@@ -94,40 +96,46 @@
     def ips(self, *filters):
         """
         Returns a list of IP addresses on this account, excluding private addresses.
 
         API Documentation: https://www.linode.com/docs/api/networking/#ip-addresses-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of IP addresses on this account.
         :rtype: PaginatedList of IPAddress
         """
         return self.client._get_and_filter(IPAddress, *filters)
 
     def ipv6_ranges(self, *filters):
         """
         Returns a list of IPv6 ranges on this account.
 
         API Documentation: https://www.linode.com/docs/api/networking/#ipv6-ranges-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of IPv6 ranges on this account.
         :rtype: PaginatedList of IPv6Range
         """
         return self.client._get_and_filter(IPv6Range, *filters)
 
     def ipv6_pools(self, *filters):
         """
         Returns a list of IPv6 pools on this account.
 
         API Documentation: https://www.linode.com/docs/api/networking/#ipv6-pools-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of IPv6 pools on this account.
         :rtype: PaginatedList of IPv6Pool
         """
 
         return self.client._get_and_filter(IPv6Pool, *filters)
 
@@ -136,14 +144,16 @@
         .. note:: This endpoint is in beta. This will only function if base_url is set to `https://api.linode.com/v4beta`.
 
         Returns a list of VLANs on your account.
 
         API Documentation: https://www.linode.com/docs/api/networking/#vlans-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A List of VLANs on your account.
         :rtype: PaginatedList of VLAN
         """
         return self.client._get_and_filter(VLAN, *filters)
 
     def ips_assign(self, region, *assignments):
```

### Comparing `linode_api4-5.6.0/linode_api4/groups/nodebalancer.py` & `linode_api4-5.7.0/linode_api4/groups/nodebalancer.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,16 @@
         class, like this::
 
            nodebalancers = client.nodebalancers()
 
         API Documentation: https://www.linode.com/docs/api/nodebalancers/#nodebalancers-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of NodeBalancers the acting user can access.
         :rtype: PaginatedList of NodeBalancers
         """
         return self.client._get_and_filter(NodeBalancer, *filters)
 
     def create(self, region, **kwargs):
```

### Comparing `linode_api4-5.6.0/linode_api4/groups/obj.py` & `linode_api4-5.7.0/linode_api4/groups/obj.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,28 +15,32 @@
         this query to return only Clusters that are available in a specific region::
 
            us_east_clusters = client.object_storage.clusters(ObjectStorageCluster.region == "us-east")
 
         API Documentation: https://www.linode.com/docs/api/object-storage/#clusters-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of Object Storage Clusters that matched the query.
         :rtype: PaginatedList of ObjectStorageCluster
         """
         return self.client._get_and_filter(ObjectStorageCluster, *filters)
 
     def keys(self, *filters):
         """
         Returns a list of Object Storage Keys active on this account.  These keys
         allow third-party applications to interact directly with Linode Object Storage.
 
         API Documentation: https://www.linode.com/docs/api/object-storage/#object-storage-keys-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of Object Storage Keys that matched the query.
         :rtype: PaginatedList of ObjectStorageKeys
         """
         return self.client._get_and_filter(ObjectStorageKeys, *filters)
 
     def keys_create(self, label, bucket_access=None):
```

### Comparing `linode_api4-5.6.0/linode_api4/groups/object_storage.py` & `linode_api4-5.7.0/linode_api4/groups/object_storage.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from urllib import parse
+
 from linode_api4.errors import UnexpectedResponseError
 from linode_api4.groups import Group
 from linode_api4.objects import (
     Base,
     MappedObject,
     ObjectStorageACL,
     ObjectStorageBucket,
@@ -23,28 +25,32 @@
         this query to return only Clusters that are available in a specific region::
 
            us_east_clusters = client.object_storage.clusters(ObjectStorageCluster.region == "us-east")
 
         API Documentation: https://www.linode.com/docs/api/object-storage/#clusters-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of Object Storage Clusters that matched the query.
         :rtype: PaginatedList of ObjectStorageCluster
         """
         return self.client._get_and_filter(ObjectStorageCluster, *filters)
 
     def keys(self, *filters):
         """
         Returns a list of Object Storage Keys active on this account.  These keys
         allow third-party applications to interact directly with Linode Object Storage.
 
         API Documentation: https://www.linode.com/docs/api/object-storage/#object-storage-keys-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of Object Storage Keys that matched the query.
         :rtype: PaginatedList of ObjectStorageKeys
         """
         return self.client._get_and_filter(ObjectStorageKeys, *filters)
 
     def keys_create(self, label, bucket_access=None):
@@ -170,14 +176,18 @@
         """
         Returns a paginated list of all Object Storage Buckets that you own.
         This endpoint is available for convenience.
         It is recommended that instead you use the more fully-featured S3 API directly.
 
         API Documentation: https://www.linode.com/docs/api/object-storage/#object-storage-buckets-list
 
+        :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
+
         :returns: A list of Object Storage Buckets that matched the query.
         :rtype: PaginatedList of ObjectStorageBucket
         """
         return self.client._get_and_filter(ObjectStorageBucket, *filters)
 
     def bucket_create(
         self,
@@ -315,15 +325,15 @@
             "name": name,
             "expires_in": expires_in,
             "content_type": content_type,
         }
 
         result = self.client.post(
             "/object-storage/buckets/{}/{}/object-url".format(
-                cluster_id, bucket
+                parse.quote(str(cluster_id)), parse.quote(str(bucket))
             ),
             data=drop_null_keys(params),
         )
 
         if not "url" in result:
             raise UnexpectedResponseError(
                 "Unexpected response when creating the access url of an object!",
```

### Comparing `linode_api4-5.6.0/linode_api4/groups/polling.py` & `linode_api4-5.7.0/linode_api4/groups/polling.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/groups/profile.py` & `linode_api4-5.7.0/linode_api4/groups/profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -223,14 +223,16 @@
     def tokens(self, *filters):
         """
         Returns the Person Access Tokens active for this user.
 
         API Documentation: https://www.linode.com/docs/api/profile/#personal-access-tokens-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of tokens that matches the query.
         :rtype: PaginatedList of PersonalAccessToken
         """
         return self.client._get_and_filter(PersonalAccessToken, *filters)
 
     def token_create(self, label=None, expiry=None, scopes=None, **kwargs):
@@ -272,27 +274,31 @@
     def apps(self, *filters):
         """
         Returns the Authorized Applications for this user
 
         API Documentation: https://www.linode.com/docs/api/profile/#authorized-apps-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of Authorized Applications for this user
         :rtype: PaginatedList of AuthorizedApp
         """
         return self.client._get_and_filter(AuthorizedApp, *filters)
 
     def ssh_keys(self, *filters):
         """
         Returns the SSH Public Keys uploaded to your profile.
 
         API Documentation: https://www.linode.com/docs/api/profile/#ssh-keys-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of SSH Keys for this profile.
         :rtype: PaginatedList of SSHKey
         """
         return self.client._get_and_filter(SSHKey, *filters)
 
     def ssh_key_upload(self, key, label):
```

### Comparing `linode_api4-5.6.0/linode_api4/groups/region.py` & `linode_api4-5.7.0/linode_api4/groups/region.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,14 +10,16 @@
         This is intended to be called off of the :any:`LinodeClient`
         class, like this::
 
            region = client.regions()
 
         API Documentation: https://www.linode.com/docs/api/regions/#regions-list
 
-        :param filters: Any number of filters to apply to the query.
+        :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of available Regions.
         :rtype: PaginatedList of Region
         """
 
         return self.client._get_and_filter(Region, *filters)
```

### Comparing `linode_api4-5.6.0/linode_api4/groups/support.py` & `linode_api4-5.7.0/linode_api4/groups/support.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,16 @@
     def tickets(self, *filters):
         """
         Returns a list of support tickets on this account.
 
         API Documentation: https://www.linode.com/docs/api/support/#support-tickets-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of support tickets on this account.
         :rtype: PaginatedList of SupportTicket
         """
 
         return self.client._get_and_filter(SupportTicket, *filters)
```

### Comparing `linode_api4-5.6.0/linode_api4/groups/tag.py` & `linode_api4-5.7.0/linode_api4/groups/tag.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,16 @@
         class, like this::
 
            tags = client.tags()
 
         API Documentation: https://www.linode.com/docs/api/domains/#domain-create
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of Tags on the account.
         :rtype: PaginatedList of Tag
         """
         return self.client._get_and_filter(Tag, *filters)
 
     def create(
```

### Comparing `linode_api4-5.6.0/linode_api4/groups/volume.py` & `linode_api4-5.7.0/linode_api4/groups/volume.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,14 +12,16 @@
         class, like this::
 
            volumes = client.volumes()
 
         API Documentation: https://www.linode.com/docs/api/volumes/#volumes-list
 
         :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of Volumes the acting user can access.
         :rtype: PaginatedList of Volume
         """
         return self.client._get_and_filter(Volume, *filters)
 
     def create(self, label, region=None, linode=None, size=20, **kwargs):
```

### Comparing `linode_api4-5.6.0/linode_api4/linode_client.py` & `linode_api4-5.7.0/linode_api4/linode_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import json
 import logging
 from typing import BinaryIO, Tuple
+from urllib import parse
 
 import pkg_resources
 import requests
 from requests.adapters import HTTPAdapter, Retry
 
 from linode_api4.errors import ApiError, UnexpectedResponseError
 from linode_api4.groups import *
@@ -223,15 +224,18 @@
         if not self.token:
             raise RuntimeError("You do not have an API token!")
 
         if not method:
             raise ValueError("Method is required for API calls!")
 
         if model:
-            endpoint = endpoint.format(**vars(model))
+            endpoint = endpoint.format(
+                **{k: parse.quote(str(v)) for k, v in vars(model).items()}
+            )
+
         url = "{}{}".format(self.base_url, endpoint)
         headers = {
             "Authorization": "Bearer {}".format(self.token),
             "Content-Type": "application/json",
             "User-Agent": self._user_agent,
         }
```

### Comparing `linode_api4-5.6.0/linode_api4/login_client.py` & `linode_api4-5.7.0/linode_api4/login_client.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/objects/__init__.py` & `linode_api4-5.7.0/linode_api4/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/objects/account.py` & `linode_api4-5.7.0/linode_api4/objects/account.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/objects/base.py` & `linode_api4-5.7.0/linode_api4/objects/base.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/objects/database.py` & `linode_api4-5.7.0/linode_api4/objects/database.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/objects/dbase.py` & `linode_api4-5.7.0/linode_api4/objects/dbase.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/objects/domain.py` & `linode_api4-5.7.0/linode_api4/objects/domain.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/objects/filtering.py` & `linode_api4-5.7.0/linode_api4/objects/filtering.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,460 +14,474 @@
 000000d0: 7920 6e75 6d62 6572 206f 6620 6669 6c74  y number of filt
 000000e0: 6572 7320 6d61 7920 6265 2070 6173 7365  ers may be passe
 000000f0: 6420 696e 2061 7320 626f 6f6c 6561 6e0a  d in as boolean.
 00000100: 636f 6d70 6172 6973 6f6e 7320 6265 7477  comparisons betw
 00000110: 6565 6e20 6174 7472 6962 7574 6573 206f  een attributes o
 00000120: 6620 7468 6520 6d6f 6465 6c20 7265 7475  f the model retu
 00000130: 726e 6564 2062 7920 7468 6520 636f 6c6c  rned by the coll
-00000140: 6563 7469 6f6e 2e0a 0a46 6f72 2065 7861  ection...For exa
-00000150: 6d70 6c65 2c20 6361 6c6c 696e 6720 3a61  mple, calling :a
-00000160: 6e79 3a60 696e 7374 616e 6365 7360 2072  ny:`instances` r
-00000170: 6574 7572 6e73 2061 206c 6973 7420 6f66  eturns a list of
-00000180: 203a 616e 793a 6049 6e73 7461 6e63 6560   :any:`Instance`
-00000190: 0a6f 626a 6563 7473 2c20 736f 2077 6520  .objects, so we 
-000001a0: 6361 6e20 7573 6520 7072 6f70 6572 7469  can use properti
-000001b0: 6573 206f 6620 3a61 6e79 3a60 496e 7374  es of :any:`Inst
-000001c0: 616e 6365 6020 746f 2066 696c 7465 7220  ance` to filter 
-000001d0: 7468 6520 7265 7375 6c74 733a 3a0a 0a20  the results::.. 
-000001e0: 2020 2320 7265 7475 726e 7320 616c 6c20    # returns all 
-000001f0: 496e 7374 616e 6365 7320 696e 2074 6865  Instances in the
-00000200: 2022 7072 6f64 2220 6772 6f75 700a 2020   "prod" group.  
-00000210: 2063 6c69 656e 742e 6c69 6e6f 6465 2e69   client.linode.i
-00000220: 6e73 7461 6e63 6573 2849 6e73 7461 6e63  nstances(Instanc
-00000230: 652e 6772 6f75 7020 3d3d 2022 7072 6f64  e.group == "prod
-00000240: 2229 0a0a 596f 7520 6361 6e20 7573 6520  ")..You can use 
-00000250: 616e 7920 626f 6f6c 6561 6e20 636f 6d70  any boolean comp
-00000260: 6172 6973 6f6e 7320 7768 656e 2066 696c  arisons when fil
-00000270: 7465 7269 6e67 2063 6f6c 6c65 6374 696f  tering collectio
-00000280: 6e73 3a3a 0a0a 2020 2023 2072 6574 7572  ns::..   # retur
-00000290: 6e73 2061 6c6c 2049 6e73 7461 6e63 6573  ns all Instances
-000002a0: 205f 6e6f 745f 2069 6e20 7573 2d65 6173   _not_ in us-eas
-000002b0: 742d 3161 0a20 2020 636c 6965 6e74 2e6c  t-1a.   client.l
-000002c0: 696e 6f64 652e 696e 7374 616e 6365 7328  inode.instances(
-000002d0: 496e 7374 616e 6365 2e72 6567 696f 6e20  Instance.region 
-000002e0: 213d 2022 7573 2d65 6173 742d 3161 2229  != "us-east-1a")
-000002f0: 0a0a 596f 7520 6361 6e20 636f 6d62 696e  ..You can combin
-00000300: 6520 6669 6c74 6572 7320 746f 2062 6520  e filters to be 
-00000310: 6576 656e 206d 6f72 6520 7370 6563 6966  even more specif
-00000320: 6963 202d 2062 7920 6465 6661 756c 7420  ic - by default 
-00000330: 616c 6c20 6669 6c74 6572 7320 6172 650a  all filters are.
-00000340: 636f 6e73 6964 6572 6564 3a3a 0a0a 2020  considered::..  
-00000350: 2023 2072 6574 7572 6e73 2061 6c6c 2049   # returns all I
-00000360: 6e73 7461 6e63 6573 2069 6e20 7468 6520  nstances in the 
-00000370: 2270 726f 6422 2067 726f 7570 2074 6861  "prod" group tha
-00000380: 7420 6172 6520 696e 2075 732d 6561 7374  t are in us-east
-00000390: 2d31 610a 2020 2063 6c69 656e 742e 6c69  -1a.   client.li
-000003a0: 6e6f 6465 2e69 6e73 7461 6e63 6573 2849  node.instances(I
-000003b0: 6e73 7461 6e63 652e 6772 6f75 7020 3d3d  nstance.group ==
-000003c0: 2022 7072 6f64 222c 0a20 2020 2020 2020   "prod",.       
-000003d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000003e0: 2020 2020 2020 2020 496e 7374 616e 6365          Instance
-000003f0: 2e72 6567 696f 6e20 3d3d 2022 7573 2d65  .region == "us-e
-00000400: 6173 742d 3161 2229 0a0a 4966 2079 6f75  ast-1a")..If you
-00000410: 206e 6565 6420 746f 2063 6f6d 6269 6e65   need to combine
-00000420: 2074 6865 2072 6573 756c 7473 206f 6620   the results of 
-00000430: 7477 6f20 6669 6c74 6572 732c 2079 6f75  two filters, you
-00000440: 2063 616e 2075 7365 203a 616e 793a 606f   can use :any:`o
-00000450: 725f 6020 746f 2064 6566 696e 650a 7468  r_` to define.th
-00000460: 6973 2072 656c 6174 696f 6e73 6869 703a  is relationship:
-00000470: 3a0a 0a20 2020 2320 7265 7475 726e 7320  :..   # returns 
-00000480: 616c 6c20 496e 7374 616e 6365 2069 6e20  all Instance in 
-00000490: 6569 7468 6572 2074 6865 2022 7072 6f64  either the "prod
-000004a0: 2220 6f72 2022 7374 6167 696e 6722 2067  " or "staging" g
-000004b0: 726f 7570 730a 2020 2063 6c69 656e 742e  roups.   client.
-000004c0: 6c69 6e6f 6465 2e69 6e73 7461 6e63 6573  linode.instances
-000004d0: 286f 725f 2849 6e73 7461 6e63 652e 6772  (or_(Instance.gr
-000004e0: 6f75 7020 3d3d 2022 7072 6f64 222c 0a20  oup == "prod",. 
-000004f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000510: 2020 496e 7374 616e 6365 2e67 726f 7570    Instance.group
-00000520: 203d 3d20 2273 7461 6769 6e67 2229 290a   == "staging")).
-00000530: 0a3a 616e 793a 6061 6e64 5f60 2069 7320  .:any:`and_` is 
-00000540: 616c 736f 2061 7661 696c 6162 6c65 2069  also available i
-00000550: 6e20 6361 7365 2079 6f75 206e 6565 6420  n case you need 
-00000560: 746f 2064 6f20 6465 6570 6c79 2d6e 6573  to do deeply-nes
-00000570: 7465 6420 636f 6d70 6172 6973 6f6e 733a  ted comparisons:
-00000580: 3a0a 0a20 2020 2320 7265 7475 726e 7320  :..   # returns 
-00000590: 616c 6c20 496e 7374 616e 6365 7320 696e  all Instances in
-000005a0: 2074 6865 2067 726f 7570 2022 7374 6167   the group "stag
-000005b0: 696e 6722 2061 6e64 2061 6e79 2049 6e73  ing" and any Ins
-000005c0: 7461 6e63 6573 2069 6e20 7468 6520 2270  tances in the "p
-000005d0: 726f 6422 0a20 2020 2320 6772 6f75 7020  rod".   # group 
-000005e0: 7468 6174 2061 7265 206c 6f63 6174 6564  that are located
-000005f0: 2069 6e20 2275 732d 6561 7374 2d31 6122   in "us-east-1a"
-00000600: 0a20 2020 636c 6965 6e74 2e6c 696e 6f64  .   client.linod
-00000610: 652e 696e 7374 616e 6365 7328 6f72 5f28  e.instances(or_(
-00000620: 496e 7374 616e 6365 2e67 726f 7570 203d  Instance.group =
-00000630: 3d20 2273 7461 6769 6e67 222c 0a20 2020  = "staging",.   
-00000640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000660: 616e 645f 2849 6e73 7461 6e63 652e 6772  and_(Instance.gr
-00000670: 6f75 7020 3d3d 2022 7072 6f64 222c 0a20  oup == "prod",. 
-00000680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000006a0: 2020 2020 2020 2049 6e73 7461 6e63 652e         Instance.
-000006b0: 7265 6769 6f6e 203d 3d20 2275 732d 6561  region == "us-ea
-000006c0: 7374 2d31 6122 2929 0a0a 2222 220a 0a0a  st-1a")).."""...
-000006d0: 6465 6620 6f72 5f28 612c 2062 293a 0a20  def or_(a, b):. 
-000006e0: 2020 2022 2222 0a20 2020 2043 6f6d 6269     """.    Combi
-000006f0: 6e65 7320 7477 6f20 3a61 6e79 3a60 4669  nes two :any:`Fi
-00000700: 6c74 6572 733c 4669 6c74 6572 3e60 2077  lters<Filter>` w
-00000710: 6974 6820 616e 2022 6f72 2220 6f70 6572  ith an "or" oper
-00000720: 6174 696f 6e2c 206d 6174 6368 696e 670a  ation, matching.
-00000730: 2020 2020 616e 7920 7265 7375 6c74 7320      any results 
-00000740: 7468 6174 206d 6174 6368 2061 6e79 206f  that match any o
-00000750: 6620 7468 6520 6769 7665 6e20 6669 6c74  f the given filt
-00000760: 6572 732e 0a0a 2020 2020 3a70 6172 616d  ers...    :param
-00000770: 2061 3a20 5468 6520 6669 7273 7420 6669   a: The first fi
-00000780: 6c74 6572 2074 6f20 636f 6e73 6964 6572  lter to consider
-00000790: 2e0a 2020 2020 3a74 7970 6520 613a 2046  ..    :type a: F
-000007a0: 696c 7465 720a 2020 2020 3a70 6172 616d  ilter.    :param
-000007b0: 2062 3a20 5468 6520 7365 636f 6e64 2066   b: The second f
-000007c0: 696c 7465 7220 746f 2063 6f6e 7369 6465  ilter to conside
-000007d0: 722e 0a20 2020 203a 7479 7065 2062 3a20  r..    :type b: 
-000007e0: 4669 6c74 6572 0a0a 2020 2020 3a72 6574  Filter..    :ret
-000007f0: 7572 6e73 3a20 4120 6669 6c74 6572 2074  urns: A filter t
-00000800: 6861 7420 6d61 7463 6865 7320 6569 7468  hat matches eith
-00000810: 6572 2061 206f 7212 2062 0a20 2020 203a  er a or. b.    :
-00000820: 7274 7970 653a 2046 696c 7465 720a 2020  rtype: Filter.  
-00000830: 2020 2222 220a 2020 2020 6966 206e 6f74    """.    if not
-00000840: 2069 7369 6e73 7461 6e63 6528 612c 2046   isinstance(a, F
-00000850: 696c 7465 7229 206f 7220 6e6f 7420 6973  ilter) or not is
-00000860: 696e 7374 616e 6365 2862 2c20 4669 6c74  instance(b, Filt
-00000870: 6572 293a 0a20 2020 2020 2020 2072 6169  er):.        rai
-00000880: 7365 2054 7970 6545 7272 6f72 0a20 2020  se TypeError.   
-00000890: 2072 6574 7572 6e20 612e 5f5f 6f72 5f5f   return a.__or__
-000008a0: 2862 290a 0a0a 6465 6620 616e 645f 2861  (b)...def and_(a
-000008b0: 2c20 6229 3a0a 2020 2020 2222 220a 2020  , b):.    """.  
-000008c0: 2020 436f 6d62 696e 6573 2074 776f 203a    Combines two :
-000008d0: 616e 793a 6046 696c 7465 7273 3c46 696c  any:`Filters<Fil
-000008e0: 7465 723e 6020 7769 7468 2061 6e20 2261  ter>` with an "a
-000008f0: 6e64 2220 6f70 6572 6174 696f 6e2c 206d  nd" operation, m
-00000900: 6174 6368 696e 670a 2020 2020 616e 7920  atching.    any 
-00000910: 7265 7375 6c74 7320 7468 6174 206d 6174  results that mat
-00000920: 6368 2062 6f74 6820 6f66 2074 6865 2067  ch both of the g
-00000930: 6976 656e 2066 696c 7465 7273 2e0a 0a20  iven filters... 
-00000940: 2020 203a 7061 7261 6d20 613a 2054 6865     :param a: The
-00000950: 2066 6972 7374 2066 696c 7465 7220 746f   first filter to
-00000960: 2063 6f6e 7369 6465 722e 0a20 2020 203a   consider..    :
-00000970: 7479 7065 2061 3a20 4669 6c74 6572 0a20  type a: Filter. 
-00000980: 2020 203a 7061 7261 6d20 623a 2054 6865     :param b: The
-00000990: 2073 6563 6f6e 6420 6669 6c74 6572 2074   second filter t
-000009a0: 6f20 636f 6e73 6964 6572 2e0a 2020 2020  o consider..    
-000009b0: 3a74 7970 6520 623a 2046 696c 7465 720a  :type b: Filter.
-000009c0: 0a20 2020 203a 7265 7475 726e 733a 2041  .    :returns: A
-000009d0: 2066 696c 7465 7220 7468 6174 206d 6174   filter that mat
-000009e0: 6368 6573 2062 6f74 6820 6120 616e 6420  ches both a and 
-000009f0: 620a 2020 2020 3a72 7479 7065 3a20 4669  b.    :rtype: Fi
-00000a00: 6c74 6572 0a20 2020 2022 2222 0a20 2020  lter.    """.   
-00000a10: 2072 6574 7572 6e20 612e 5f5f 616e 645f   return a.__and_
-00000a20: 5f28 6229 0a0a 0a64 6566 206f 7264 6572  _(b)...def order
-00000a30: 5f62 7928 6669 656c 642c 2064 6573 633d  _by(field, desc=
-00000a40: 4661 6c73 6529 3a0a 2020 2020 2222 220a  False):.    """.
-00000a50: 2020 2020 416c 6c6f 7773 206f 7264 6572      Allows order
-00000a60: 696e 6720 6f66 2072 6573 756c 7473 2e20  ing of results. 
-00000a70: 2059 6f75 206d 6179 206f 6e6c 7920 6576   You may only ev
-00000a80: 6572 206f 7264 6572 2061 2063 6f6c 6c65  er order a colle
-00000a90: 6374 696f 6e27 7320 7265 7375 6c74 730a  ction's results.
-00000aa0: 2020 2020 6f6e 6365 2069 6e20 6120 6769      once in a gi
-00000ab0: 7665 6e20 7265 7175 6573 742e 2020 466f  ven request.  Fo
-00000ac0: 7220 6578 616d 706c 653a 3a0a 0a20 2020  r example::..   
-00000ad0: 2020 2020 2320 736f 7274 2072 6573 756c      # sort resul
-00000ae0: 7473 2062 7920 496e 7374 616e 6365 7320  ts by Instances 
-00000af0: 6772 6f75 700a 2020 2020 2020 2063 6c69  group.       cli
-00000b00: 656e 742e 6c69 6e6f 6465 2e69 6e73 7461  ent.linode.insta
-00000b10: 6e63 6573 286f 7264 6572 5f62 7928 496e  nces(order_by(In
-00000b20: 7374 616e 6365 2e67 726f 7570 2929 0a0a  stance.group))..
-00000b30: 2020 2020 3a70 6172 616d 2066 6965 6c64      :param field
-00000b40: 3a20 5468 6520 6669 656c 6420 746f 206f  : The field to o
-00000b50: 7264 6572 2072 6573 756c 7473 2062 792e  rder results by.
-00000b60: 2020 4d75 7374 2062 6520 6120 6669 6c74    Must be a filt
-00000b70: 6572 6162 6c65 2061 7474 7269 6275 7465  erable attribute
-00000b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000b90: 2020 206f 6620 7468 6520 6d6f 6465 6c2e     of the model.
-00000ba0: 0a20 2020 203a 7479 7065 2066 6965 6c64  .    :type field
-00000bb0: 3a20 4669 6c74 6572 6162 6c65 4174 7472  : FilterableAttr
-00000bc0: 6962 7574 650a 2020 2020 3a70 6172 616d  ibute.    :param
-00000bd0: 2064 6573 633a 2049 6620 5472 7565 2c20   desc: If True, 
-00000be0: 7265 7475 726e 2072 6573 756c 7473 2069  return results i
-00000bf0: 6e20 6465 7363 656e 6469 6e67 206f 7264  n descending ord
-00000c00: 6572 2e20 2044 6566 6175 6c74 7320 746f  er.  Defaults to
-00000c10: 2046 616c 7365 0a20 2020 203a 7479 7065   False.    :type
-00000c20: 2064 6573 633a 2062 6f6f 6c0a 0a20 2020   desc: bool..   
-00000c30: 203a 7265 7475 726e 733a 2041 2066 696c   :returns: A fil
-00000c40: 7465 7220 7468 6174 2077 696c 6c20 6f72  ter that will or
-00000c50: 6465 7220 7265 7375 6c74 7320 6173 2072  der results as r
-00000c60: 6571 7565 7374 6564 2e0a 2020 2020 3a72  equested..    :r
-00000c70: 7479 7065 3a20 4669 6c74 6572 0a20 2020  type: Filter.   
-00000c80: 2022 2222 0a20 2020 2072 6574 7572 6e20   """.    return 
-00000c90: 4669 6c74 6572 287b 7d29 2e6f 7264 6572  Filter({}).order
-00000ca0: 5f62 7928 6669 656c 642c 2064 6573 6329  _by(field, desc)
-00000cb0: 0a0a 0a64 6566 206c 696d 6974 2861 6d6f  ...def limit(amo
-00000cc0: 756e 7429 3a0a 2020 2020 2222 220a 2020  unt):.    """.  
-00000cd0: 2020 416c 6c6f 7773 206c 696d 6974 696e    Allows limitin
-00000ce0: 6720 6f66 2072 6573 756c 7473 2069 6e20  g of results in 
-00000cf0: 6120 636f 6c6c 6563 7469 6f6e 2e20 2059  a collection.  Y
-00000d00: 6f75 206d 6179 206f 6e6c 7920 6576 6572  ou may only ever
-00000d10: 2061 7070 6c79 2061 206c 696d 6974 0a20   apply a limit. 
-00000d20: 2020 206f 6e63 6520 7065 7220 7265 7175     once per requ
-00000d30: 6573 742e 2020 466f 7220 6578 616d 706c  est.  For exampl
-00000d40: 653a 3a0a 0a20 2020 2020 2020 2023 2072  e::..        # r
-00000d50: 6574 7572 6e73 206d 7920 6669 7273 7420  eturns my first 
-00000d60: 3520 496e 7374 616e 6365 730a 2020 2020  5 Instances.    
-00000d70: 2020 2020 636c 6965 6e74 2e6c 696e 6f64      client.linod
-00000d80: 652e 696e 7374 616e 6365 7328 6c69 6d69  e.instances(limi
-00000d90: 7428 3529 290a 0a20 2020 203a 7061 7261  t(5))..    :para
-00000da0: 6d20 616d 6f75 6e74 3a20 5468 6520 6e75  m amount: The nu
-00000db0: 6d62 6572 206f 6620 7265 7375 6c74 7320  mber of results 
-00000dc0: 746f 2072 6574 7572 6e2e 0a20 2020 203a  to return..    :
-00000dd0: 7479 7065 2061 6d6f 756e 743a 2069 6e74  type amount: int
-00000de0: 0a0a 2020 2020 3a72 6574 7572 6e73 3a20  ..    :returns: 
-00000df0: 4120 6669 6c74 6572 2074 6861 7420 7769  A filter that wi
-00000e00: 6c6c 206c 696d 6974 2074 6865 206e 756d  ll limit the num
-00000e10: 6265 7220 6f66 2072 6573 756c 7473 2072  ber of results r
-00000e20: 6574 7572 6e65 642e 0a20 2020 203a 7274  eturned..    :rt
-00000e30: 7970 653a 2046 696c 7465 720a 2020 2020  ype: Filter.    
-00000e40: 2222 220a 2020 2020 7265 7475 726e 2046  """.    return F
-00000e50: 696c 7465 7228 7b7d 292e 6c69 6d69 7428  ilter({}).limit(
-00000e60: 616d 6f75 6e74 290a 0a0a 636c 6173 7320  amount)...class 
-00000e70: 4669 6c74 6572 3a0a 2020 2020 2222 220a  Filter:.    """.
-00000e80: 2020 2020 4120 4669 6c74 6572 2072 6570      A Filter rep
-00000e90: 7265 7365 6e74 7320 6120 636f 6d70 6172  resents a compar
-00000ea0: 6973 6f6e 2074 6f20 7365 6e64 2074 6f20  ison to send to 
-00000eb0: 7468 6520 4150 492e 2020 5468 6573 6520  the API.  These 
-00000ec0: 7368 6f75 6c64 206e 6f74 2062 650a 2020  should not be.  
-00000ed0: 2020 636f 6e73 7472 7563 7465 6420 6e6f    constructed no
-00000ee0: 726d 616c 6c79 2c20 6275 7420 696e 7374  rmally, but inst
-00000ef0: 6561 6420 7368 6f75 6c64 2062 6520 7265  ead should be re
-00000f00: 7475 726e 6564 2066 726f 6d20 636f 6d70  turned from comp
-00000f10: 6172 6973 6f6e 730a 2020 2020 6265 7477  arisons.    betw
-00000f20: 6565 6e20 636c 6173 7320 6174 7472 6962  een class attrib
-00000f30: 7574 6573 206f 6620 6669 6c74 6572 6162  utes of filterab
-00000f40: 6c65 2063 6c61 7373 6573 2028 7365 6520  le classes (see 
-00000f50: 6162 6f76 6529 2e20 2046 696c 7465 7273  above).  Filters
-00000f60: 2063 616e 0a20 2020 2062 6520 636f 6d62   can.    be comb
-00000f70: 696e 6564 2077 6974 6820 3a61 6e79 3a60  ined with :any:`
-00000f80: 616e 645f 6020 616e 6420 3a61 6e79 3a60  and_` and :any:`
-00000f90: 6f72 5f60 2e0a 2020 2020 2222 220a 0a20  or_`..    """.. 
-00000fa0: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00000fb0: 7365 6c66 2c20 6463 7429 3a0a 2020 2020  self, dct):.    
-00000fc0: 2020 2020 7365 6c66 2e64 6374 203d 2064      self.dct = d
-00000fd0: 6374 0a0a 2020 2020 6465 6620 5f5f 6f72  ct..    def __or
-00000fe0: 5f5f 2873 656c 662c 206f 7468 6572 293a  __(self, other):
-00000ff0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00001000: 6973 696e 7374 616e 6365 286f 7468 6572  isinstance(other
-00001010: 2c20 4669 6c74 6572 293a 0a20 2020 2020  , Filter):.     
-00001020: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
-00001030: 6545 7272 6f72 2822 596f 7520 6361 6e20  eError("You can 
-00001040: 6f6e 6c79 206f 7220 4669 6c74 6572 2074  only or Filter t
-00001050: 7970 6573 2122 290a 2020 2020 2020 2020  ypes!").        
-00001060: 6966 2022 2b6f 7222 2069 6e20 7365 6c66  if "+or" in self
-00001070: 2e64 6374 3a0a 2020 2020 2020 2020 2020  .dct:.          
-00001080: 2020 7265 7475 726e 2046 696c 7465 7228    return Filter(
-00001090: 7b22 2b6f 7222 3a20 7365 6c66 2e64 6374  {"+or": self.dct
-000010a0: 5b22 2b6f 7222 5d20 2b20 5b6f 7468 6572  ["+or"] + [other
-000010b0: 2e64 6374 5d7d 290a 2020 2020 2020 2020  .dct]}).        
-000010c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000010d0: 2020 7265 7475 726e 2046 696c 7465 7228    return Filter(
-000010e0: 7b22 2b6f 7222 3a20 5b73 656c 662e 6463  {"+or": [self.dc
-000010f0: 742c 206f 7468 6572 2e64 6374 5d7d 290a  t, other.dct]}).
-00001100: 0a20 2020 2064 6566 205f 5f61 6e64 5f5f  .    def __and__
-00001110: 2873 656c 662c 206f 7468 6572 293a 0a20  (self, other):. 
-00001120: 2020 2020 2020 2069 6620 6e6f 7420 6973         if not is
-00001130: 696e 7374 616e 6365 286f 7468 6572 2c20  instance(other, 
-00001140: 4669 6c74 6572 293a 0a20 2020 2020 2020  Filter):.       
-00001150: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
-00001160: 7272 6f72 2822 596f 7520 6361 6e20 6f6e  rror("You can on
-00001170: 6c79 2061 6e64 2046 696c 7465 7220 7479  ly and Filter ty
-00001180: 7065 7321 2229 0a20 2020 2020 2020 2069  pes!").        i
-00001190: 6620 222b 616e 6422 2069 6e20 7365 6c66  f "+and" in self
-000011a0: 2e64 6374 3a0a 2020 2020 2020 2020 2020  .dct:.          
-000011b0: 2020 7265 7475 726e 2046 696c 7465 7228    return Filter(
-000011c0: 7b22 2b61 6e64 223a 2073 656c 662e 6463  {"+and": self.dc
-000011d0: 745b 222b 616e 6422 5d20 2b20 5b6f 7468  t["+and"] + [oth
-000011e0: 6572 2e64 6374 5d7d 290a 2020 2020 2020  er.dct]}).      
-000011f0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00001200: 2020 2020 7265 7475 726e 2046 696c 7465      return Filte
-00001210: 7228 7b22 2b61 6e64 223a 205b 7365 6c66  r({"+and": [self
-00001220: 2e64 6374 2c20 6f74 6865 722e 6463 745d  .dct, other.dct]
-00001230: 7d29 0a0a 2020 2020 6465 6620 6f72 6465  })..    def orde
-00001240: 725f 6279 2873 656c 662c 2066 6965 6c64  r_by(self, field
-00001250: 2c20 6465 7363 3d46 616c 7365 293a 0a20  , desc=False):. 
-00001260: 2020 2020 2020 2023 2077 6520 6361 6e27         # we can'
-00001270: 7420 696e 636c 7564 6520 7477 6f20 6f72  t include two or
-00001280: 6465 725f 6279 730a 2020 2020 2020 2020  der_bys.        
-00001290: 6966 2022 2b6f 7264 6572 5f62 7922 2069  if "+order_by" i
-000012a0: 6e20 7365 6c66 2e64 6374 3a0a 2020 2020  n self.dct:.    
-000012b0: 2020 2020 2020 2020 7261 6973 6520 4173          raise As
-000012c0: 7365 7274 696f 6e45 7272 6f72 2822 596f  sertionError("Yo
-000012d0: 7520 6d61 7920 6f6e 6c79 206f 7264 6572  u may only order
-000012e0: 2062 7920 6f6e 6365 2122 290a 0a20 2020   by once!")..   
-000012f0: 2020 2020 2069 6620 6e6f 7420 6973 696e       if not isin
-00001300: 7374 616e 6365 2866 6965 6c64 2c20 4669  stance(field, Fi
-00001310: 6c74 6572 6162 6c65 4174 7472 6962 7574  lterableAttribut
-00001320: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-00001330: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
-00001340: 2243 616e 206f 6e6c 7920 6f72 6465 7220  "Can only order 
-00001350: 6279 2066 696c 7465 7261 626c 6520 6174  by filterable at
-00001360: 7472 6962 7574 6573 2122 290a 0a20 2020  tributes!")..   
-00001370: 2020 2020 2073 656c 662e 6463 745b 222b       self.dct["+
-00001380: 6f72 6465 725f 6279 225d 203d 2066 6965  order_by"] = fie
-00001390: 6c64 2e6e 616d 650a 2020 2020 2020 2020  ld.name.        
-000013a0: 6966 2064 6573 633a 0a20 2020 2020 2020  if desc:.       
-000013b0: 2020 2020 2073 656c 662e 6463 745b 222b       self.dct["+
-000013c0: 6f72 6465 7222 5d20 3d20 2264 6573 6322  order"] = "desc"
-000013d0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-000013e0: 2073 656c 660a 0a20 2020 2064 6566 206c   self..    def l
-000013f0: 696d 6974 2873 656c 662c 206c 696d 6974  imit(self, limit
-00001400: 293a 0a20 2020 2020 2020 2023 2077 6520  ):.        # we 
-00001410: 6361 6e27 7420 6c69 6d69 7420 7477 6963  can't limit twic
-00001420: 650a 2020 2020 2020 2020 6966 2022 2b6c  e.        if "+l
-00001430: 696d 6974 2220 696e 2073 656c 662e 6463  imit" in self.dc
-00001440: 743a 0a20 2020 2020 2020 2020 2020 2072  t:.            r
-00001450: 6169 7365 2041 7373 6572 7469 6f6e 4572  aise AssertionEr
-00001460: 726f 7228 2259 6f75 206d 6179 206f 6e6c  ror("You may onl
-00001470: 7920 6c69 6d69 7420 6f6e 6365 2122 290a  y limit once!").
-00001480: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00001490: 7479 7065 286c 696d 6974 2920 3d3d 2069  type(limit) == i
-000014a0: 6e74 3a0a 2020 2020 2020 2020 2020 2020  nt:.            
-000014b0: 7261 6973 6520 5479 7065 4572 726f 7228  raise TypeError(
-000014c0: 224c 696d 6974 206d 7573 7420 6265 2061  "Limit must be a
-000014d0: 6e20 696e 7421 2229 0a0a 2020 2020 2020  n int!")..      
-000014e0: 2020 7365 6c66 2e64 6374 5b22 2b6c 696d    self.dct["+lim
-000014f0: 6974 225d 203d 206c 696d 6974 0a0a 2020  it"] = limit..  
-00001500: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00001510: 660a 0a0a 636c 6173 7320 4669 6c74 6572  f...class Filter
-00001520: 6162 6c65 4174 7472 6962 7574 653a 0a20  ableAttribute:. 
-00001530: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00001540: 7365 6c66 2c20 6e61 6d65 293a 0a20 2020  self, name):.   
-00001550: 2020 2020 2073 656c 662e 6e61 6d65 203d       self.name =
-00001560: 206e 616d 650a 0a20 2020 2064 6566 205f   name..    def _
-00001570: 5f65 715f 5f28 7365 6c66 2c20 6f74 6865  _eq__(self, othe
-00001580: 7229 3a0a 2020 2020 2020 2020 7265 7475  r):.        retu
-00001590: 726e 2046 696c 7465 7228 7b73 656c 662e  rn Filter({self.
-000015a0: 6e61 6d65 3a20 6f74 6865 727d 290a 0a20  name: other}).. 
-000015b0: 2020 2064 6566 205f 5f6e 655f 5f28 7365     def __ne__(se
-000015c0: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
-000015d0: 2020 2020 7265 7475 726e 2046 696c 7465      return Filte
-000015e0: 7228 7b73 656c 662e 6e61 6d65 3a20 7b22  r({self.name: {"
-000015f0: 2b6e 6571 223a 206f 7468 6572 7d7d 290a  +neq": other}}).
-00001600: 0a20 2020 2023 2022 696e 2220 6576 616c  .    # "in" eval
-00001610: 7561 7465 7320 7468 6520 7265 7475 726e  uates the return
-00001620: 2076 616c 7565 202d 2068 6176 6520 746f   value - have to
-00001630: 2075 7365 0a20 2020 2023 2074 7970 652e   use.    # type.
-00001640: 636f 6e74 6169 6e73 2069 6e73 7465 6164  contains instead
-00001650: 0a20 2020 2064 6566 2063 6f6e 7461 696e  .    def contain
-00001660: 7328 7365 6c66 2c20 6f74 6865 7229 3a0a  s(self, other):.
-00001670: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-00001680: 696c 7465 7228 7b73 656c 662e 6e61 6d65  ilter({self.name
-00001690: 3a20 7b22 2b63 6f6e 7461 696e 7322 3a20  : {"+contains": 
-000016a0: 6f74 6865 727d 7d29 0a0a 2020 2020 6465  other}})..    de
-000016b0: 6620 5f5f 6774 5f5f 2873 656c 662c 206f  f __gt__(self, o
-000016c0: 7468 6572 293a 0a20 2020 2020 2020 2072  ther):.        r
-000016d0: 6574 7572 6e20 4669 6c74 6572 287b 7365  eturn Filter({se
-000016e0: 6c66 2e6e 616d 653a 207b 222b 6774 223a  lf.name: {"+gt":
-000016f0: 206f 7468 6572 7d7d 290a 0a20 2020 2064   other}})..    d
-00001700: 6566 205f 5f6c 745f 5f28 7365 6c66 2c20  ef __lt__(self, 
-00001710: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
-00001720: 7265 7475 726e 2046 696c 7465 7228 7b73  return Filter({s
-00001730: 656c 662e 6e61 6d65 3a20 7b22 2b6c 7422  elf.name: {"+lt"
-00001740: 3a20 6f74 6865 727d 7d29 0a0a 2020 2020  : other}})..    
-00001750: 6465 6620 5f5f 6765 5f5f 2873 656c 662c  def __ge__(self,
-00001760: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-00001770: 2072 6574 7572 6e20 4669 6c74 6572 287b   return Filter({
-00001780: 7365 6c66 2e6e 616d 653a 207b 222b 6774  self.name: {"+gt
-00001790: 6522 3a20 6f74 6865 727d 7d29 0a0a 2020  e": other}})..  
-000017a0: 2020 6465 6620 5f5f 6c65 5f5f 2873 656c    def __le__(sel
-000017b0: 662c 206f 7468 6572 293a 0a20 2020 2020  f, other):.     
-000017c0: 2020 2072 6574 7572 6e20 4669 6c74 6572     return Filter
-000017d0: 287b 7365 6c66 2e6e 616d 653a 207b 222b  ({self.name: {"+
-000017e0: 6c74 6522 3a20 6f74 6865 727d 7d29 0a0a  lte": other}})..
-000017f0: 0a63 6c61 7373 204e 6f6e 4669 6c74 6572  .class NonFilter
-00001800: 6162 6c65 4174 7472 6962 7574 653a 0a20  ableAttribute:. 
-00001810: 2020 2064 6566 205f 5f69 6e69 745f 5f28     def __init__(
-00001820: 7365 6c66 2c20 636c 736e 616d 652c 2061  self, clsname, a
-00001830: 7472 6e61 6d65 293a 0a20 2020 2020 2020  trname):.       
-00001840: 2073 656c 662e 636c 736e 616d 6520 3d20   self.clsname = 
-00001850: 636c 736e 616d 650a 2020 2020 2020 2020  clsname.        
-00001860: 7365 6c66 2e61 7472 6e61 6d65 203d 2061  self.atrname = a
-00001870: 7472 6e61 6d65 0a0a 2020 2020 6465 6620  trname..    def 
-00001880: 5f5f 6571 5f5f 2873 656c 662c 206f 7468  __eq__(self, oth
-00001890: 6572 293a 0a20 2020 2020 2020 2072 6169  er):.        rai
-000018a0: 7365 2041 7474 7269 6275 7465 4572 726f  se AttributeErro
-000018b0: 7228 0a20 2020 2020 2020 2020 2020 2022  r(.            "
-000018c0: 7b7d 2063 616e 6e6f 7420 6265 2066 696c  {} cannot be fil
-000018d0: 7465 7265 6420 6279 207b 7d22 2e66 6f72  tered by {}".for
-000018e0: 6d61 7428 7365 6c66 2e63 6c73 6e61 6d65  mat(self.clsname
-000018f0: 2c20 7365 6c66 2e61 7472 6e61 6d65 290a  , self.atrname).
-00001900: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-00001910: 6566 205f 5f6e 655f 5f28 7365 6c66 2c20  ef __ne__(self, 
-00001920: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
-00001930: 7261 6973 6520 4174 7472 6962 7574 6545  raise AttributeE
-00001940: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
-00001950: 2020 227b 7d20 6361 6e6e 6f74 2062 6520    "{} cannot be 
-00001960: 6669 6c74 6572 6564 2062 7920 7b7d 222e  filtered by {}".
-00001970: 666f 726d 6174 2873 656c 662e 636c 736e  format(self.clsn
-00001980: 616d 652c 2073 656c 662e 6174 726e 616d  ame, self.atrnam
-00001990: 6529 0a20 2020 2020 2020 2029 0a0a 2020  e).        )..  
-000019a0: 2020 6465 6620 636f 6e74 6169 6e73 2873    def contains(s
-000019b0: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
-000019c0: 2020 2020 2072 6169 7365 2041 7474 7269       raise Attri
-000019d0: 6275 7465 4572 726f 7228 0a20 2020 2020  buteError(.     
-000019e0: 2020 2020 2020 2022 7b7d 2063 616e 6e6f         "{} canno
-000019f0: 7420 6265 2066 696c 7465 7265 6420 6279  t be filtered by
-00001a00: 207b 7d22 2e66 6f72 6d61 7428 7365 6c66   {}".format(self
-00001a10: 2e63 6c73 6e61 6d65 2c20 7365 6c66 2e61  .clsname, self.a
-00001a20: 7472 6e61 6d65 290a 2020 2020 2020 2020  trname).        
-00001a30: 290a 0a20 2020 2064 6566 205f 5f67 745f  )..    def __gt_
-00001a40: 5f28 7365 6c66 2c20 6f74 6865 7229 3a0a  _(self, other):.
-00001a50: 2020 2020 2020 2020 7261 6973 6520 4174          raise At
-00001a60: 7472 6962 7574 6545 7272 6f72 280a 2020  tributeError(.  
-00001a70: 2020 2020 2020 2020 2020 227b 7d20 6361            "{} ca
-00001a80: 6e6e 6f74 2062 6520 6669 6c74 6572 6564  nnot be filtered
-00001a90: 2062 7920 7b7d 222e 666f 726d 6174 2873   by {}".format(s
-00001aa0: 656c 662e 636c 736e 616d 652c 2073 656c  elf.clsname, sel
-00001ab0: 662e 6174 726e 616d 6529 0a20 2020 2020  f.atrname).     
-00001ac0: 2020 2029 0a0a 2020 2020 6465 6620 5f5f     )..    def __
-00001ad0: 6c74 5f5f 2873 656c 662c 206f 7468 6572  lt__(self, other
-00001ae0: 293a 0a20 2020 2020 2020 2072 6169 7365  ):.        raise
-00001af0: 2041 7474 7269 6275 7465 4572 726f 7228   AttributeError(
-00001b00: 0a20 2020 2020 2020 2020 2020 2022 7b7d  .            "{}
-00001b10: 2063 616e 6e6f 7420 6265 2066 696c 7465   cannot be filte
-00001b20: 7265 6420 6279 207b 7d22 2e66 6f72 6d61  red by {}".forma
-00001b30: 7428 7365 6c66 2e63 6c73 6e61 6d65 2c20  t(self.clsname, 
-00001b40: 7365 6c66 2e61 7472 6e61 6d65 290a 2020  self.atrname).  
-00001b50: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
-00001b60: 205f 5f67 655f 5f28 7365 6c66 2c20 6f74   __ge__(self, ot
-00001b70: 6865 7229 3a0a 2020 2020 2020 2020 7261  her):.        ra
-00001b80: 6973 6520 4174 7472 6962 7574 6545 7272  ise AttributeErr
-00001b90: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
-00001ba0: 227b 7d20 6361 6e6e 6f74 2062 6520 6669  "{} cannot be fi
-00001bb0: 6c74 6572 6564 2062 7920 7b7d 222e 666f  ltered by {}".fo
-00001bc0: 726d 6174 2873 656c 662e 636c 736e 616d  rmat(self.clsnam
-00001bd0: 652c 2073 656c 662e 6174 726e 616d 6529  e, self.atrname)
-00001be0: 0a20 2020 2020 2020 2029 0a0a 2020 2020  .        )..    
-00001bf0: 6465 6620 5f5f 6c65 5f5f 2873 656c 662c  def __le__(self,
-00001c00: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-00001c10: 2072 6169 7365 2041 7474 7269 6275 7465   raise Attribute
-00001c20: 4572 726f 7228 0a20 2020 2020 2020 2020  Error(.         
-00001c30: 2020 2022 7b7d 2063 616e 6e6f 7420 6265     "{} cannot be
-00001c40: 2066 696c 7465 7265 6420 6279 207b 7d22   filtered by {}"
-00001c50: 2e66 6f72 6d61 7428 7365 6c66 2e63 6c73  .format(self.cls
-00001c60: 6e61 6d65 2c20 7365 6c66 2e61 7472 6e61  name, self.atrna
-00001c70: 6d65 290a 2020 2020 2020 2020 290a 0a0a  me).        )...
-00001c80: 636c 6173 7320 4669 6c74 6572 6162 6c65  class Filterable
-00001c90: 4d65 7461 636c 6173 7328 7479 7065 293a  Metaclass(type):
-00001ca0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
-00001cb0: 5f28 636c 732c 206e 616d 652c 2062 6173  _(cls, name, bas
-00001cc0: 6573 2c20 6463 7429 3a0a 2020 2020 2020  es, dct):.      
-00001cd0: 2020 6966 2068 6173 6174 7472 2863 6c73    if hasattr(cls
-00001ce0: 2c20 2270 726f 7065 7274 6965 7322 293a  , "properties"):
-00001cf0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-00001d00: 206b 6579 2069 6e20 636c 732e 7072 6f70   key in cls.prop
-00001d10: 6572 7469 6573 2e6b 6579 7328 293a 0a20  erties.keys():. 
-00001d20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001d30: 6574 6174 7472 2863 6c73 2c20 6b65 792c  etattr(cls, key,
-00001d40: 2046 696c 7465 7261 626c 6541 7474 7269   FilterableAttri
-00001d50: 6275 7465 286b 6579 2929 0a0a 2020 2020  bute(key))..    
-00001d60: 2020 2020 7375 7065 7228 292e 5f5f 696e      super().__in
-00001d70: 6974 5f5f 286e 616d 652c 2062 6173 6573  it__(name, bases
-00001d80: 2c20 6463 7429 0a                        , dct).
+00000140: 6563 7469 6f6e 2e0a 0a57 6865 6e20 6669  ection...When fi
+00000150: 6c74 6572 696e 6720 6f6e 2041 5049 2072  ltering on API r
+00000160: 6573 706f 6e73 6573 2066 6f72 206c 6973  esponses for lis
+00000170: 7420 656e 6470 6f69 6e74 732c 2079 6f75  t endpoints, you
+00000180: 2077 696c 6c20 6669 7273 7420 6e65 6564   will first need
+00000190: 0a74 6f20 696d 706f 7274 2074 6865 2063  .to import the c
+000001a0: 6f72 7265 7370 6f6e 6469 6e67 206f 626a  orresponding obj
+000001b0: 6563 7420 636c 6173 732e 0a46 6f72 2065  ect class..For e
+000001c0: 7861 6d70 6c65 2c20 746f 2066 696c 7465  xample, to filte
+000001d0: 7220 6f6e 2069 6e73 7461 6e63 6573 2079  r on instances y
+000001e0: 6f75 206d 7573 7420 6669 7273 7420 496d  ou must first Im
+000001f0: 706f 7274 203a 616e 793a 6049 6e73 7461  port :any:`Insta
+00000200: 6e63 6560 3a3a 0a0a 2020 2020 6672 6f6d  nce`::..    from
+00000210: 206c 696e 6f64 655f 6170 6934 2069 6d70   linode_api4 imp
+00000220: 6f72 7420 496e 7374 616e 6365 0a0a 466f  ort Instance..Fo
+00000230: 7220 6578 616d 706c 652c 2063 616c 6c69  r example, calli
+00000240: 6e67 203a 616e 793a 6069 6e73 7461 6e63  ng :any:`instanc
+00000250: 6573 6020 7265 7475 726e 7320 6120 6c69  es` returns a li
+00000260: 7374 206f 6620 3a61 6e79 3a60 496e 7374  st of :any:`Inst
+00000270: 616e 6365 600a 6f62 6a65 6374 732c 2073  ance`.objects, s
+00000280: 6f20 7765 2063 616e 2075 7365 2070 726f  o we can use pro
+00000290: 7065 7274 6965 7320 6f66 203a 616e 793a  perties of :any:
+000002a0: 6049 6e73 7461 6e63 6560 2074 6f20 6669  `Instance` to fi
+000002b0: 6c74 6572 2074 6865 2072 6573 756c 7473  lter the results
+000002c0: 3a3a 0a0a 2020 2023 2072 6574 7572 6e73  ::..   # returns
+000002d0: 2061 6c6c 2049 6e73 7461 6e63 6573 2069   all Instances i
+000002e0: 6e20 7468 6520 2270 726f 6422 2067 726f  n the "prod" gro
+000002f0: 7570 0a20 2020 636c 6965 6e74 2e6c 696e  up.   client.lin
+00000300: 6f64 652e 696e 7374 616e 6365 7328 496e  ode.instances(In
+00000310: 7374 616e 6365 2e67 726f 7570 203d 3d20  stance.group == 
+00000320: 2270 726f 6422 290a 0a59 6f75 2063 616e  "prod")..You can
+00000330: 2075 7365 2061 6e79 2062 6f6f 6c65 616e   use any boolean
+00000340: 2063 6f6d 7061 7269 736f 6e73 2077 6865   comparisons whe
+00000350: 6e20 6669 6c74 6572 696e 6720 636f 6c6c  n filtering coll
+00000360: 6563 7469 6f6e 733a 3a0a 0a20 2020 2320  ections::..   # 
+00000370: 7265 7475 726e 7320 616c 6c20 496e 7374  returns all Inst
+00000380: 616e 6365 7320 5f6e 6f74 5f20 696e 2075  ances _not_ in u
+00000390: 732d 6561 7374 2d31 610a 2020 2063 6c69  s-east-1a.   cli
+000003a0: 656e 742e 6c69 6e6f 6465 2e69 6e73 7461  ent.linode.insta
+000003b0: 6e63 6573 2849 6e73 7461 6e63 652e 7265  nces(Instance.re
+000003c0: 6769 6f6e 2021 3d20 2275 732d 6561 7374  gion != "us-east
+000003d0: 2d31 6122 290a 0a59 6f75 2063 616e 2063  -1a")..You can c
+000003e0: 6f6d 6269 6e65 2066 696c 7465 7273 2074  ombine filters t
+000003f0: 6f20 6265 2065 7665 6e20 6d6f 7265 2073  o be even more s
+00000400: 7065 6369 6669 6320 2d20 6279 2064 6566  pecific - by def
+00000410: 6175 6c74 2061 6c6c 2066 696c 7465 7273  ault all filters
+00000420: 2061 7265 0a63 6f6e 7369 6465 7265 643a   are.considered:
+00000430: 3a0a 0a20 2020 2320 7265 7475 726e 7320  :..   # returns 
+00000440: 616c 6c20 496e 7374 616e 6365 7320 696e  all Instances in
+00000450: 2074 6865 2022 7072 6f64 2220 6772 6f75   the "prod" grou
+00000460: 7020 7468 6174 2061 7265 2069 6e20 7573  p that are in us
+00000470: 2d65 6173 742d 3161 0a20 2020 636c 6965  -east-1a.   clie
+00000480: 6e74 2e6c 696e 6f64 652e 696e 7374 616e  nt.linode.instan
+00000490: 6365 7328 496e 7374 616e 6365 2e67 726f  ces(Instance.gro
+000004a0: 7570 203d 3d20 2270 726f 6422 2c0a 2020  up == "prod",.  
+000004b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000004c0: 2020 2020 2020 2020 2020 2020 2049 6e73               Ins
+000004d0: 7461 6e63 652e 7265 6769 6f6e 203d 3d20  tance.region == 
+000004e0: 2275 732d 6561 7374 2d31 6122 290a 0a49  "us-east-1a")..I
+000004f0: 6620 796f 7520 6e65 6564 2074 6f20 636f  f you need to co
+00000500: 6d62 696e 6520 7468 6520 7265 7375 6c74  mbine the result
+00000510: 7320 6f66 2074 776f 2066 696c 7465 7273  s of two filters
+00000520: 2c20 796f 7520 6361 6e20 7573 6520 3a61  , you can use :a
+00000530: 6e79 3a60 6f72 5f60 2074 6f20 6465 6669  ny:`or_` to defi
+00000540: 6e65 0a74 6869 7320 7265 6c61 7469 6f6e  ne.this relation
+00000550: 7368 6970 3a3a 0a0a 2020 2023 2072 6574  ship::..   # ret
+00000560: 7572 6e73 2061 6c6c 2049 6e73 7461 6e63  urns all Instanc
+00000570: 6520 696e 2065 6974 6865 7220 7468 6520  e in either the 
+00000580: 2270 726f 6422 206f 7220 2273 7461 6769  "prod" or "stagi
+00000590: 6e67 2220 6772 6f75 7073 0a20 2020 636c  ng" groups.   cl
+000005a0: 6965 6e74 2e6c 696e 6f64 652e 696e 7374  ient.linode.inst
+000005b0: 616e 6365 7328 6f72 5f28 496e 7374 616e  ances(or_(Instan
+000005c0: 6365 2e67 726f 7570 203d 3d20 2270 726f  ce.group == "pro
+000005d0: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+000005e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005f0: 2020 2020 2020 2049 6e73 7461 6e63 652e         Instance.
+00000600: 6772 6f75 7020 3d3d 2022 7374 6167 696e  group == "stagin
+00000610: 6722 2929 0a0a 3a61 6e79 3a60 616e 645f  g"))..:any:`and_
+00000620: 6020 6973 2061 6c73 6f20 6176 6169 6c61  ` is also availa
+00000630: 626c 6520 696e 2063 6173 6520 796f 7520  ble in case you 
+00000640: 6e65 6564 2074 6f20 646f 2064 6565 706c  need to do deepl
+00000650: 792d 6e65 7374 6564 2063 6f6d 7061 7269  y-nested compari
+00000660: 736f 6e73 3a3a 0a0a 2020 2023 2072 6574  sons::..   # ret
+00000670: 7572 6e73 2061 6c6c 2049 6e73 7461 6e63  urns all Instanc
+00000680: 6573 2069 6e20 7468 6520 6772 6f75 7020  es in the group 
+00000690: 2273 7461 6769 6e67 2220 616e 6420 616e  "staging" and an
+000006a0: 7920 496e 7374 616e 6365 7320 696e 2074  y Instances in t
+000006b0: 6865 2022 7072 6f64 220a 2020 2023 2067  he "prod".   # g
+000006c0: 726f 7570 2074 6861 7420 6172 6520 6c6f  roup that are lo
+000006d0: 6361 7465 6420 696e 2022 7573 2d65 6173  cated in "us-eas
+000006e0: 742d 3161 220a 2020 2063 6c69 656e 742e  t-1a".   client.
+000006f0: 6c69 6e6f 6465 2e69 6e73 7461 6e63 6573  linode.instances
+00000700: 286f 725f 2849 6e73 7461 6e63 652e 6772  (or_(Instance.gr
+00000710: 6f75 7020 3d3d 2022 7374 6167 696e 6722  oup == "staging"
+00000720: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00000730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000740: 2020 2020 2061 6e64 5f28 496e 7374 616e       and_(Instan
+00000750: 6365 2e67 726f 7570 203d 3d20 2270 726f  ce.group == "pro
+00000760: 6422 2c0a 2020 2020 2020 2020 2020 2020  d",.            
+00000770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000780: 2020 2020 2020 2020 2020 2020 496e 7374              Inst
+00000790: 616e 6365 2e72 6567 696f 6e20 3d3d 2022  ance.region == "
+000007a0: 7573 2d65 6173 742d 3161 2229 290a 0a22  us-east-1a")).."
+000007b0: 2222 0a0a 0a64 6566 206f 725f 2861 2c20  ""...def or_(a, 
+000007c0: 6229 3a0a 2020 2020 2222 220a 2020 2020  b):.    """.    
+000007d0: 436f 6d62 696e 6573 2074 776f 203a 616e  Combines two :an
+000007e0: 793a 6046 696c 7465 7273 3c46 696c 7465  y:`Filters<Filte
+000007f0: 723e 6020 7769 7468 2061 6e20 226f 7222  r>` with an "or"
+00000800: 206f 7065 7261 7469 6f6e 2c20 6d61 7463   operation, matc
+00000810: 6869 6e67 0a20 2020 2061 6e79 2072 6573  hing.    any res
+00000820: 756c 7473 2074 6861 7420 6d61 7463 6820  ults that match 
+00000830: 616e 7920 6f66 2074 6865 2067 6976 656e  any of the given
+00000840: 2066 696c 7465 7273 2e0a 0a20 2020 203a   filters...    :
+00000850: 7061 7261 6d20 613a 2054 6865 2066 6972  param a: The fir
+00000860: 7374 2066 696c 7465 7220 746f 2063 6f6e  st filter to con
+00000870: 7369 6465 722e 0a20 2020 203a 7479 7065  sider..    :type
+00000880: 2061 3a20 4669 6c74 6572 0a20 2020 203a   a: Filter.    :
+00000890: 7061 7261 6d20 623a 2054 6865 2073 6563  param b: The sec
+000008a0: 6f6e 6420 6669 6c74 6572 2074 6f20 636f  ond filter to co
+000008b0: 6e73 6964 6572 2e0a 2020 2020 3a74 7970  nsider..    :typ
+000008c0: 6520 623a 2046 696c 7465 720a 0a20 2020  e b: Filter..   
+000008d0: 203a 7265 7475 726e 733a 2041 2066 696c   :returns: A fil
+000008e0: 7465 7220 7468 6174 206d 6174 6368 6573  ter that matches
+000008f0: 2065 6974 6865 7220 6120 6f72 1220 620a   either a or. b.
+00000900: 2020 2020 3a72 7479 7065 3a20 4669 6c74      :rtype: Filt
+00000910: 6572 0a20 2020 2022 2222 0a20 2020 2069  er.    """.    i
+00000920: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+00000930: 2861 2c20 4669 6c74 6572 2920 6f72 206e  (a, Filter) or n
+00000940: 6f74 2069 7369 6e73 7461 6e63 6528 622c  ot isinstance(b,
+00000950: 2046 696c 7465 7229 3a0a 2020 2020 2020   Filter):.      
+00000960: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
+00000970: 720a 2020 2020 7265 7475 726e 2061 2e5f  r.    return a._
+00000980: 5f6f 725f 5f28 6229 0a0a 0a64 6566 2061  _or__(b)...def a
+00000990: 6e64 5f28 612c 2062 293a 0a20 2020 2022  nd_(a, b):.    "
+000009a0: 2222 0a20 2020 2043 6f6d 6269 6e65 7320  "".    Combines 
+000009b0: 7477 6f20 3a61 6e79 3a60 4669 6c74 6572  two :any:`Filter
+000009c0: 733c 4669 6c74 6572 3e60 2077 6974 6820  s<Filter>` with 
+000009d0: 616e 2022 616e 6422 206f 7065 7261 7469  an "and" operati
+000009e0: 6f6e 2c20 6d61 7463 6869 6e67 0a20 2020  on, matching.   
+000009f0: 2061 6e79 2072 6573 756c 7473 2074 6861   any results tha
+00000a00: 7420 6d61 7463 6820 626f 7468 206f 6620  t match both of 
+00000a10: 7468 6520 6769 7665 6e20 6669 6c74 6572  the given filter
+00000a20: 732e 0a0a 2020 2020 3a70 6172 616d 2061  s...    :param a
+00000a30: 3a20 5468 6520 6669 7273 7420 6669 6c74  : The first filt
+00000a40: 6572 2074 6f20 636f 6e73 6964 6572 2e0a  er to consider..
+00000a50: 2020 2020 3a74 7970 6520 613a 2046 696c      :type a: Fil
+00000a60: 7465 720a 2020 2020 3a70 6172 616d 2062  ter.    :param b
+00000a70: 3a20 5468 6520 7365 636f 6e64 2066 696c  : The second fil
+00000a80: 7465 7220 746f 2063 6f6e 7369 6465 722e  ter to consider.
+00000a90: 0a20 2020 203a 7479 7065 2062 3a20 4669  .    :type b: Fi
+00000aa0: 6c74 6572 0a0a 2020 2020 3a72 6574 7572  lter..    :retur
+00000ab0: 6e73 3a20 4120 6669 6c74 6572 2074 6861  ns: A filter tha
+00000ac0: 7420 6d61 7463 6865 7320 626f 7468 2061  t matches both a
+00000ad0: 2061 6e64 2062 0a20 2020 203a 7274 7970   and b.    :rtyp
+00000ae0: 653a 2046 696c 7465 720a 2020 2020 2222  e: Filter.    ""
+00000af0: 220a 2020 2020 7265 7475 726e 2061 2e5f  ".    return a._
+00000b00: 5f61 6e64 5f5f 2862 290a 0a0a 6465 6620  _and__(b)...def 
+00000b10: 6f72 6465 725f 6279 2866 6965 6c64 2c20  order_by(field, 
+00000b20: 6465 7363 3d46 616c 7365 293a 0a20 2020  desc=False):.   
+00000b30: 2022 2222 0a20 2020 2041 6c6c 6f77 7320   """.    Allows 
+00000b40: 6f72 6465 7269 6e67 206f 6620 7265 7375  ordering of resu
+00000b50: 6c74 732e 2020 596f 7520 6d61 7920 6f6e  lts.  You may on
+00000b60: 6c79 2065 7665 7220 6f72 6465 7220 6120  ly ever order a 
+00000b70: 636f 6c6c 6563 7469 6f6e 2773 2072 6573  collection's res
+00000b80: 756c 7473 0a20 2020 206f 6e63 6520 696e  ults.    once in
+00000b90: 2061 2067 6976 656e 2072 6571 7565 7374   a given request
+00000ba0: 2e20 2046 6f72 2065 7861 6d70 6c65 3a3a  .  For example::
+00000bb0: 0a0a 2020 2020 2020 2023 2073 6f72 7420  ..       # sort 
+00000bc0: 7265 7375 6c74 7320 6279 2049 6e73 7461  results by Insta
+00000bd0: 6e63 6573 2067 726f 7570 0a20 2020 2020  nces group.     
+00000be0: 2020 636c 6965 6e74 2e6c 696e 6f64 652e    client.linode.
+00000bf0: 696e 7374 616e 6365 7328 6f72 6465 725f  instances(order_
+00000c00: 6279 2849 6e73 7461 6e63 652e 6772 6f75  by(Instance.grou
+00000c10: 7029 290a 0a20 2020 203a 7061 7261 6d20  p))..    :param 
+00000c20: 6669 656c 643a 2054 6865 2066 6965 6c64  field: The field
+00000c30: 2074 6f20 6f72 6465 7220 7265 7375 6c74   to order result
+00000c40: 7320 6279 2e20 204d 7573 7420 6265 2061  s by.  Must be a
+00000c50: 2066 696c 7465 7261 626c 6520 6174 7472   filterable attr
+00000c60: 6962 7574 650a 2020 2020 2020 2020 2020  ibute.          
+00000c70: 2020 2020 2020 2020 6f66 2074 6865 206d          of the m
+00000c80: 6f64 656c 2e0a 2020 2020 3a74 7970 6520  odel..    :type 
+00000c90: 6669 656c 643a 2046 696c 7465 7261 626c  field: Filterabl
+00000ca0: 6541 7474 7269 6275 7465 0a20 2020 203a  eAttribute.    :
+00000cb0: 7061 7261 6d20 6465 7363 3a20 4966 2054  param desc: If T
+00000cc0: 7275 652c 2072 6574 7572 6e20 7265 7375  rue, return resu
+00000cd0: 6c74 7320 696e 2064 6573 6365 6e64 696e  lts in descendin
+00000ce0: 6720 6f72 6465 722e 2020 4465 6661 756c  g order.  Defaul
+00000cf0: 7473 2074 6f20 4661 6c73 650a 2020 2020  ts to False.    
+00000d00: 3a74 7970 6520 6465 7363 3a20 626f 6f6c  :type desc: bool
+00000d10: 0a0a 2020 2020 3a72 6574 7572 6e73 3a20  ..    :returns: 
+00000d20: 4120 6669 6c74 6572 2074 6861 7420 7769  A filter that wi
+00000d30: 6c6c 206f 7264 6572 2072 6573 756c 7473  ll order results
+00000d40: 2061 7320 7265 7175 6573 7465 642e 0a20   as requested.. 
+00000d50: 2020 203a 7274 7970 653a 2046 696c 7465     :rtype: Filte
+00000d60: 720a 2020 2020 2222 220a 2020 2020 7265  r.    """.    re
+00000d70: 7475 726e 2046 696c 7465 7228 7b7d 292e  turn Filter({}).
+00000d80: 6f72 6465 725f 6279 2866 6965 6c64 2c20  order_by(field, 
+00000d90: 6465 7363 290a 0a0a 6465 6620 6c69 6d69  desc)...def limi
+00000da0: 7428 616d 6f75 6e74 293a 0a20 2020 2022  t(amount):.    "
+00000db0: 2222 0a20 2020 2041 6c6c 6f77 7320 6c69  "".    Allows li
+00000dc0: 6d69 7469 6e67 206f 6620 7265 7375 6c74  miting of result
+00000dd0: 7320 696e 2061 2063 6f6c 6c65 6374 696f  s in a collectio
+00000de0: 6e2e 2020 596f 7520 6d61 7920 6f6e 6c79  n.  You may only
+00000df0: 2065 7665 7220 6170 706c 7920 6120 6c69   ever apply a li
+00000e00: 6d69 740a 2020 2020 6f6e 6365 2070 6572  mit.    once per
+00000e10: 2072 6571 7565 7374 2e20 2046 6f72 2065   request.  For e
+00000e20: 7861 6d70 6c65 3a3a 0a0a 2020 2020 2020  xample::..      
+00000e30: 2020 2320 7265 7475 726e 7320 6d79 2066    # returns my f
+00000e40: 6972 7374 2035 2049 6e73 7461 6e63 6573  irst 5 Instances
+00000e50: 0a20 2020 2020 2020 2063 6c69 656e 742e  .        client.
+00000e60: 6c69 6e6f 6465 2e69 6e73 7461 6e63 6573  linode.instances
+00000e70: 286c 696d 6974 2835 2929 0a0a 2020 2020  (limit(5))..    
+00000e80: 3a70 6172 616d 2061 6d6f 756e 743a 2054  :param amount: T
+00000e90: 6865 206e 756d 6265 7220 6f66 2072 6573  he number of res
+00000ea0: 756c 7473 2074 6f20 7265 7475 726e 2e0a  ults to return..
+00000eb0: 2020 2020 3a74 7970 6520 616d 6f75 6e74      :type amount
+00000ec0: 3a20 696e 740a 0a20 2020 203a 7265 7475  : int..    :retu
+00000ed0: 726e 733a 2041 2066 696c 7465 7220 7468  rns: A filter th
+00000ee0: 6174 2077 696c 6c20 6c69 6d69 7420 7468  at will limit th
+00000ef0: 6520 6e75 6d62 6572 206f 6620 7265 7375  e number of resu
+00000f00: 6c74 7320 7265 7475 726e 6564 2e0a 2020  lts returned..  
+00000f10: 2020 3a72 7479 7065 3a20 4669 6c74 6572    :rtype: Filter
+00000f20: 0a20 2020 2022 2222 0a20 2020 2072 6574  .    """.    ret
+00000f30: 7572 6e20 4669 6c74 6572 287b 7d29 2e6c  urn Filter({}).l
+00000f40: 696d 6974 2861 6d6f 756e 7429 0a0a 0a63  imit(amount)...c
+00000f50: 6c61 7373 2046 696c 7465 723a 0a20 2020  lass Filter:.   
+00000f60: 2022 2222 0a20 2020 2041 2046 696c 7465   """.    A Filte
+00000f70: 7220 7265 7072 6573 656e 7473 2061 2063  r represents a c
+00000f80: 6f6d 7061 7269 736f 6e20 746f 2073 656e  omparison to sen
+00000f90: 6420 746f 2074 6865 2041 5049 2e20 2054  d to the API.  T
+00000fa0: 6865 7365 2073 686f 756c 6420 6e6f 7420  hese should not 
+00000fb0: 6265 0a20 2020 2063 6f6e 7374 7275 6374  be.    construct
+00000fc0: 6564 206e 6f72 6d61 6c6c 792c 2062 7574  ed normally, but
+00000fd0: 2069 6e73 7465 6164 2073 686f 756c 6420   instead should 
+00000fe0: 6265 2072 6574 7572 6e65 6420 6672 6f6d  be returned from
+00000ff0: 2063 6f6d 7061 7269 736f 6e73 0a20 2020   comparisons.   
+00001000: 2062 6574 7765 656e 2063 6c61 7373 2061   between class a
+00001010: 7474 7269 6275 7465 7320 6f66 2066 696c  ttributes of fil
+00001020: 7465 7261 626c 6520 636c 6173 7365 7320  terable classes 
+00001030: 2873 6565 2061 626f 7665 292e 2020 4669  (see above).  Fi
+00001040: 6c74 6572 7320 6361 6e0a 2020 2020 6265  lters can.    be
+00001050: 2063 6f6d 6269 6e65 6420 7769 7468 203a   combined with :
+00001060: 616e 793a 6061 6e64 5f60 2061 6e64 203a  any:`and_` and :
+00001070: 616e 793a 606f 725f 602e 0a20 2020 2022  any:`or_`..    "
+00001080: 2222 0a0a 2020 2020 6465 6620 5f5f 696e  ""..    def __in
+00001090: 6974 5f5f 2873 656c 662c 2064 6374 293a  it__(self, dct):
+000010a0: 0a20 2020 2020 2020 2073 656c 662e 6463  .        self.dc
+000010b0: 7420 3d20 6463 740a 0a20 2020 2064 6566  t = dct..    def
+000010c0: 205f 5f6f 725f 5f28 7365 6c66 2c20 6f74   __or__(self, ot
+000010d0: 6865 7229 3a0a 2020 2020 2020 2020 6966  her):.        if
+000010e0: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+000010f0: 6f74 6865 722c 2046 696c 7465 7229 3a0a  other, Filter):.
+00001100: 2020 2020 2020 2020 2020 2020 7261 6973              rais
+00001110: 6520 5479 7065 4572 726f 7228 2259 6f75  e TypeError("You
+00001120: 2063 616e 206f 6e6c 7920 6f72 2046 696c   can only or Fil
+00001130: 7465 7220 7479 7065 7321 2229 0a20 2020  ter types!").   
+00001140: 2020 2020 2069 6620 222b 6f72 2220 696e       if "+or" in
+00001150: 2073 656c 662e 6463 743a 0a20 2020 2020   self.dct:.     
+00001160: 2020 2020 2020 2072 6574 7572 6e20 4669         return Fi
+00001170: 6c74 6572 287b 222b 6f72 223a 2073 656c  lter({"+or": sel
+00001180: 662e 6463 745b 222b 6f72 225d 202b 205b  f.dct["+or"] + [
+00001190: 6f74 6865 722e 6463 745d 7d29 0a20 2020  other.dct]}).   
+000011a0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+000011b0: 2020 2020 2020 2072 6574 7572 6e20 4669         return Fi
+000011c0: 6c74 6572 287b 222b 6f72 223a 205b 7365  lter({"+or": [se
+000011d0: 6c66 2e64 6374 2c20 6f74 6865 722e 6463  lf.dct, other.dc
+000011e0: 745d 7d29 0a0a 2020 2020 6465 6620 5f5f  t]})..    def __
+000011f0: 616e 645f 5f28 7365 6c66 2c20 6f74 6865  and__(self, othe
+00001200: 7229 3a0a 2020 2020 2020 2020 6966 206e  r):.        if n
+00001210: 6f74 2069 7369 6e73 7461 6e63 6528 6f74  ot isinstance(ot
+00001220: 6865 722c 2046 696c 7465 7229 3a0a 2020  her, Filter):.  
+00001230: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00001240: 5479 7065 4572 726f 7228 2259 6f75 2063  TypeError("You c
+00001250: 616e 206f 6e6c 7920 616e 6420 4669 6c74  an only and Filt
+00001260: 6572 2074 7970 6573 2122 290a 2020 2020  er types!").    
+00001270: 2020 2020 6966 2022 2b61 6e64 2220 696e      if "+and" in
+00001280: 2073 656c 662e 6463 743a 0a20 2020 2020   self.dct:.     
+00001290: 2020 2020 2020 2072 6574 7572 6e20 4669         return Fi
+000012a0: 6c74 6572 287b 222b 616e 6422 3a20 7365  lter({"+and": se
+000012b0: 6c66 2e64 6374 5b22 2b61 6e64 225d 202b  lf.dct["+and"] +
+000012c0: 205b 6f74 6865 722e 6463 745d 7d29 0a20   [other.dct]}). 
+000012d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000012e0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000012f0: 4669 6c74 6572 287b 222b 616e 6422 3a20  Filter({"+and": 
+00001300: 5b73 656c 662e 6463 742c 206f 7468 6572  [self.dct, other
+00001310: 2e64 6374 5d7d 290a 0a20 2020 2064 6566  .dct]})..    def
+00001320: 206f 7264 6572 5f62 7928 7365 6c66 2c20   order_by(self, 
+00001330: 6669 656c 642c 2064 6573 633d 4661 6c73  field, desc=Fals
+00001340: 6529 3a0a 2020 2020 2020 2020 2320 7765  e):.        # we
+00001350: 2063 616e 2774 2069 6e63 6c75 6465 2074   can't include t
+00001360: 776f 206f 7264 6572 5f62 7973 0a20 2020  wo order_bys.   
+00001370: 2020 2020 2069 6620 222b 6f72 6465 725f       if "+order_
+00001380: 6279 2220 696e 2073 656c 662e 6463 743a  by" in self.dct:
+00001390: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+000013a0: 7365 2041 7373 6572 7469 6f6e 4572 726f  se AssertionErro
+000013b0: 7228 2259 6f75 206d 6179 206f 6e6c 7920  r("You may only 
+000013c0: 6f72 6465 7220 6279 206f 6e63 6521 2229  order by once!")
+000013d0: 0a0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
+000013e0: 2069 7369 6e73 7461 6e63 6528 6669 656c   isinstance(fiel
+000013f0: 642c 2046 696c 7465 7261 626c 6541 7474  d, FilterableAtt
+00001400: 7269 6275 7465 293a 0a20 2020 2020 2020  ribute):.       
+00001410: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
+00001420: 7272 6f72 2822 4361 6e20 6f6e 6c79 206f  rror("Can only o
+00001430: 7264 6572 2062 7920 6669 6c74 6572 6162  rder by filterab
+00001440: 6c65 2061 7474 7269 6275 7465 7321 2229  le attributes!")
+00001450: 0a0a 2020 2020 2020 2020 7365 6c66 2e64  ..        self.d
+00001460: 6374 5b22 2b6f 7264 6572 5f62 7922 5d20  ct["+order_by"] 
+00001470: 3d20 6669 656c 642e 6e61 6d65 0a20 2020  = field.name.   
+00001480: 2020 2020 2069 6620 6465 7363 3a0a 2020       if desc:.  
+00001490: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+000014a0: 6374 5b22 2b6f 7264 6572 225d 203d 2022  ct["+order"] = "
+000014b0: 6465 7363 220a 0a20 2020 2020 2020 2072  desc"..        r
+000014c0: 6574 7572 6e20 7365 6c66 0a0a 2020 2020  eturn self..    
+000014d0: 6465 6620 6c69 6d69 7428 7365 6c66 2c20  def limit(self, 
+000014e0: 6c69 6d69 7429 3a0a 2020 2020 2020 2020  limit):.        
+000014f0: 2320 7765 2063 616e 2774 206c 696d 6974  # we can't limit
+00001500: 2074 7769 6365 0a20 2020 2020 2020 2069   twice.        i
+00001510: 6620 222b 6c69 6d69 7422 2069 6e20 7365  f "+limit" in se
+00001520: 6c66 2e64 6374 3a0a 2020 2020 2020 2020  lf.dct:.        
+00001530: 2020 2020 7261 6973 6520 4173 7365 7274      raise Assert
+00001540: 696f 6e45 7272 6f72 2822 596f 7520 6d61  ionError("You ma
+00001550: 7920 6f6e 6c79 206c 696d 6974 206f 6e63  y only limit onc
+00001560: 6521 2229 0a0a 2020 2020 2020 2020 6966  e!")..        if
+00001570: 206e 6f74 2074 7970 6528 6c69 6d69 7429   not type(limit)
+00001580: 203d 3d20 696e 743a 0a20 2020 2020 2020   == int:.       
+00001590: 2020 2020 2072 6169 7365 2054 7970 6545       raise TypeE
+000015a0: 7272 6f72 2822 4c69 6d69 7420 6d75 7374  rror("Limit must
+000015b0: 2062 6520 616e 2069 6e74 2122 290a 0a20   be an int!").. 
+000015c0: 2020 2020 2020 2073 656c 662e 6463 745b         self.dct[
+000015d0: 222b 6c69 6d69 7422 5d20 3d20 6c69 6d69  "+limit"] = limi
+000015e0: 740a 0a20 2020 2020 2020 2072 6574 7572  t..        retur
+000015f0: 6e20 7365 6c66 0a0a 0a63 6c61 7373 2046  n self...class F
+00001600: 696c 7465 7261 626c 6541 7474 7269 6275  ilterableAttribu
+00001610: 7465 3a0a 2020 2020 6465 6620 5f5f 696e  te:.    def __in
+00001620: 6974 5f5f 2873 656c 662c 206e 616d 6529  it__(self, name)
+00001630: 3a0a 2020 2020 2020 2020 7365 6c66 2e6e  :.        self.n
+00001640: 616d 6520 3d20 6e61 6d65 0a0a 2020 2020  ame = name..    
+00001650: 6465 6620 5f5f 6571 5f5f 2873 656c 662c  def __eq__(self,
+00001660: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
+00001670: 2072 6574 7572 6e20 4669 6c74 6572 287b   return Filter({
+00001680: 7365 6c66 2e6e 616d 653a 206f 7468 6572  self.name: other
+00001690: 7d29 0a0a 2020 2020 6465 6620 5f5f 6e65  })..    def __ne
+000016a0: 5f5f 2873 656c 662c 206f 7468 6572 293a  __(self, other):
+000016b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000016c0: 4669 6c74 6572 287b 7365 6c66 2e6e 616d  Filter({self.nam
+000016d0: 653a 207b 222b 6e65 7122 3a20 6f74 6865  e: {"+neq": othe
+000016e0: 727d 7d29 0a0a 2020 2020 2320 2269 6e22  r}})..    # "in"
+000016f0: 2065 7661 6c75 6174 6573 2074 6865 2072   evaluates the r
+00001700: 6574 7572 6e20 7661 6c75 6520 2d20 6861  eturn value - ha
+00001710: 7665 2074 6f20 7573 650a 2020 2020 2320  ve to use.    # 
+00001720: 7479 7065 2e63 6f6e 7461 696e 7320 696e  type.contains in
+00001730: 7374 6561 640a 2020 2020 6465 6620 636f  stead.    def co
+00001740: 6e74 6169 6e73 2873 656c 662c 206f 7468  ntains(self, oth
+00001750: 6572 293a 0a20 2020 2020 2020 2072 6574  er):.        ret
+00001760: 7572 6e20 4669 6c74 6572 287b 7365 6c66  urn Filter({self
+00001770: 2e6e 616d 653a 207b 222b 636f 6e74 6169  .name: {"+contai
+00001780: 6e73 223a 206f 7468 6572 7d7d 290a 0a20  ns": other}}).. 
+00001790: 2020 2064 6566 205f 5f67 745f 5f28 7365     def __gt__(se
+000017a0: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
+000017b0: 2020 2020 7265 7475 726e 2046 696c 7465      return Filte
+000017c0: 7228 7b73 656c 662e 6e61 6d65 3a20 7b22  r({self.name: {"
+000017d0: 2b67 7422 3a20 6f74 6865 727d 7d29 0a0a  +gt": other}})..
+000017e0: 2020 2020 6465 6620 5f5f 6c74 5f5f 2873      def __lt__(s
+000017f0: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
+00001800: 2020 2020 2072 6574 7572 6e20 4669 6c74       return Filt
+00001810: 6572 287b 7365 6c66 2e6e 616d 653a 207b  er({self.name: {
+00001820: 222b 6c74 223a 206f 7468 6572 7d7d 290a  "+lt": other}}).
+00001830: 0a20 2020 2064 6566 205f 5f67 655f 5f28  .    def __ge__(
+00001840: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
+00001850: 2020 2020 2020 7265 7475 726e 2046 696c        return Fil
+00001860: 7465 7228 7b73 656c 662e 6e61 6d65 3a20  ter({self.name: 
+00001870: 7b22 2b67 7465 223a 206f 7468 6572 7d7d  {"+gte": other}}
+00001880: 290a 0a20 2020 2064 6566 205f 5f6c 655f  )..    def __le_
+00001890: 5f28 7365 6c66 2c20 6f74 6865 7229 3a0a  _(self, other):.
+000018a0: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+000018b0: 696c 7465 7228 7b73 656c 662e 6e61 6d65  ilter({self.name
+000018c0: 3a20 7b22 2b6c 7465 223a 206f 7468 6572  : {"+lte": other
+000018d0: 7d7d 290a 0a0a 636c 6173 7320 4e6f 6e46  }})...class NonF
+000018e0: 696c 7465 7261 626c 6541 7474 7269 6275  ilterableAttribu
+000018f0: 7465 3a0a 2020 2020 6465 6620 5f5f 696e  te:.    def __in
+00001900: 6974 5f5f 2873 656c 662c 2063 6c73 6e61  it__(self, clsna
+00001910: 6d65 2c20 6174 726e 616d 6529 3a0a 2020  me, atrname):.  
+00001920: 2020 2020 2020 7365 6c66 2e63 6c73 6e61        self.clsna
+00001930: 6d65 203d 2063 6c73 6e61 6d65 0a20 2020  me = clsname.   
+00001940: 2020 2020 2073 656c 662e 6174 726e 616d       self.atrnam
+00001950: 6520 3d20 6174 726e 616d 650a 0a20 2020  e = atrname..   
+00001960: 2064 6566 205f 5f65 715f 5f28 7365 6c66   def __eq__(self
+00001970: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
+00001980: 2020 7261 6973 6520 4174 7472 6962 7574    raise Attribut
+00001990: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
+000019a0: 2020 2020 227b 7d20 6361 6e6e 6f74 2062      "{} cannot b
+000019b0: 6520 6669 6c74 6572 6564 2062 7920 7b7d  e filtered by {}
+000019c0: 222e 666f 726d 6174 2873 656c 662e 636c  ".format(self.cl
+000019d0: 736e 616d 652c 2073 656c 662e 6174 726e  sname, self.atrn
+000019e0: 616d 6529 0a20 2020 2020 2020 2029 0a0a  ame).        )..
+000019f0: 2020 2020 6465 6620 5f5f 6e65 5f5f 2873      def __ne__(s
+00001a00: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
+00001a10: 2020 2020 2072 6169 7365 2041 7474 7269       raise Attri
+00001a20: 6275 7465 4572 726f 7228 0a20 2020 2020  buteError(.     
+00001a30: 2020 2020 2020 2022 7b7d 2063 616e 6e6f         "{} canno
+00001a40: 7420 6265 2066 696c 7465 7265 6420 6279  t be filtered by
+00001a50: 207b 7d22 2e66 6f72 6d61 7428 7365 6c66   {}".format(self
+00001a60: 2e63 6c73 6e61 6d65 2c20 7365 6c66 2e61  .clsname, self.a
+00001a70: 7472 6e61 6d65 290a 2020 2020 2020 2020  trname).        
+00001a80: 290a 0a20 2020 2064 6566 2063 6f6e 7461  )..    def conta
+00001a90: 696e 7328 7365 6c66 2c20 6f74 6865 7229  ins(self, other)
+00001aa0: 3a0a 2020 2020 2020 2020 7261 6973 6520  :.        raise 
+00001ab0: 4174 7472 6962 7574 6545 7272 6f72 280a  AttributeError(.
+00001ac0: 2020 2020 2020 2020 2020 2020 227b 7d20              "{} 
+00001ad0: 6361 6e6e 6f74 2062 6520 6669 6c74 6572  cannot be filter
+00001ae0: 6564 2062 7920 7b7d 222e 666f 726d 6174  ed by {}".format
+00001af0: 2873 656c 662e 636c 736e 616d 652c 2073  (self.clsname, s
+00001b00: 656c 662e 6174 726e 616d 6529 0a20 2020  elf.atrname).   
+00001b10: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+00001b20: 5f5f 6774 5f5f 2873 656c 662c 206f 7468  __gt__(self, oth
+00001b30: 6572 293a 0a20 2020 2020 2020 2072 6169  er):.        rai
+00001b40: 7365 2041 7474 7269 6275 7465 4572 726f  se AttributeErro
+00001b50: 7228 0a20 2020 2020 2020 2020 2020 2022  r(.            "
+00001b60: 7b7d 2063 616e 6e6f 7420 6265 2066 696c  {} cannot be fil
+00001b70: 7465 7265 6420 6279 207b 7d22 2e66 6f72  tered by {}".for
+00001b80: 6d61 7428 7365 6c66 2e63 6c73 6e61 6d65  mat(self.clsname
+00001b90: 2c20 7365 6c66 2e61 7472 6e61 6d65 290a  , self.atrname).
+00001ba0: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
+00001bb0: 6566 205f 5f6c 745f 5f28 7365 6c66 2c20  ef __lt__(self, 
+00001bc0: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
+00001bd0: 7261 6973 6520 4174 7472 6962 7574 6545  raise AttributeE
+00001be0: 7272 6f72 280a 2020 2020 2020 2020 2020  rror(.          
+00001bf0: 2020 227b 7d20 6361 6e6e 6f74 2062 6520    "{} cannot be 
+00001c00: 6669 6c74 6572 6564 2062 7920 7b7d 222e  filtered by {}".
+00001c10: 666f 726d 6174 2873 656c 662e 636c 736e  format(self.clsn
+00001c20: 616d 652c 2073 656c 662e 6174 726e 616d  ame, self.atrnam
+00001c30: 6529 0a20 2020 2020 2020 2029 0a0a 2020  e).        )..  
+00001c40: 2020 6465 6620 5f5f 6765 5f5f 2873 656c    def __ge__(sel
+00001c50: 662c 206f 7468 6572 293a 0a20 2020 2020  f, other):.     
+00001c60: 2020 2072 6169 7365 2041 7474 7269 6275     raise Attribu
+00001c70: 7465 4572 726f 7228 0a20 2020 2020 2020  teError(.       
+00001c80: 2020 2020 2022 7b7d 2063 616e 6e6f 7420       "{} cannot 
+00001c90: 6265 2066 696c 7465 7265 6420 6279 207b  be filtered by {
+00001ca0: 7d22 2e66 6f72 6d61 7428 7365 6c66 2e63  }".format(self.c
+00001cb0: 6c73 6e61 6d65 2c20 7365 6c66 2e61 7472  lsname, self.atr
+00001cc0: 6e61 6d65 290a 2020 2020 2020 2020 290a  name).        ).
+00001cd0: 0a20 2020 2064 6566 205f 5f6c 655f 5f28  .    def __le__(
+00001ce0: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
+00001cf0: 2020 2020 2020 7261 6973 6520 4174 7472        raise Attr
+00001d00: 6962 7574 6545 7272 6f72 280a 2020 2020  ibuteError(.    
+00001d10: 2020 2020 2020 2020 227b 7d20 6361 6e6e          "{} cann
+00001d20: 6f74 2062 6520 6669 6c74 6572 6564 2062  ot be filtered b
+00001d30: 7920 7b7d 222e 666f 726d 6174 2873 656c  y {}".format(sel
+00001d40: 662e 636c 736e 616d 652c 2073 656c 662e  f.clsname, self.
+00001d50: 6174 726e 616d 6529 0a20 2020 2020 2020  atrname).       
+00001d60: 2029 0a0a 0a63 6c61 7373 2046 696c 7465   )...class Filte
+00001d70: 7261 626c 654d 6574 6163 6c61 7373 2874  rableMetaclass(t
+00001d80: 7970 6529 3a0a 2020 2020 6465 6620 5f5f  ype):.    def __
+00001d90: 696e 6974 5f5f 2863 6c73 2c20 6e61 6d65  init__(cls, name
+00001da0: 2c20 6261 7365 732c 2064 6374 293a 0a20  , bases, dct):. 
+00001db0: 2020 2020 2020 2069 6620 6861 7361 7474         if hasatt
+00001dc0: 7228 636c 732c 2022 7072 6f70 6572 7469  r(cls, "properti
+00001dd0: 6573 2229 3a0a 2020 2020 2020 2020 2020  es"):.          
+00001de0: 2020 666f 7220 6b65 7920 696e 2063 6c73    for key in cls
+00001df0: 2e70 726f 7065 7274 6965 732e 6b65 7973  .properties.keys
+00001e00: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00001e10: 2020 2020 7365 7461 7474 7228 636c 732c      setattr(cls,
+00001e20: 206b 6579 2c20 4669 6c74 6572 6162 6c65   key, Filterable
+00001e30: 4174 7472 6962 7574 6528 6b65 7929 290a  Attribute(key)).
+00001e40: 0a20 2020 2020 2020 2073 7570 6572 2829  .        super()
+00001e50: 2e5f 5f69 6e69 745f 5f28 6e61 6d65 2c20  .__init__(name, 
+00001e60: 6261 7365 732c 2064 6374 290a            bases, dct).
```

### Comparing `linode_api4-5.6.0/linode_api4/objects/image.py` & `linode_api4-5.7.0/linode_api4/objects/image.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,8 +21,9 @@
         "created_by": Property(),
         "updated": Property(is_datetime=True),
         "type": Property(),
         "is_public": Property(),
         "vendor": Property(),
         "size": Property(),
         "deprecated": Property(),
+        "capabilities": Property(),
     }
```

### Comparing `linode_api4-5.6.0/linode_api4/objects/linode.py` & `linode_api4-5.7.0/linode_api4/objects/linode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import string
 import sys
 from datetime import datetime
 from enum import Enum
 from os import urandom
 from random import randint
+from urllib import parse
 
 from linode_api4 import util
 from linode_api4.common import load_and_validate_keys
 from linode_api4.errors import UnexpectedResponseError
 from linode_api4.objects import Base, DerivedBase, Image, Property, Region
 from linode_api4.objects.base import MappedObject
 from linode_api4.objects.filtering import FilterableAttribute
@@ -407,14 +408,15 @@
         "ipv4": Property(),
         "ipv6": Property(),
         "hypervisor": Property(),
         "specs": Property(),
         "tags": Property(mutable=True),
         "host_uuid": Property(),
         "watchdog_enabled": Property(mutable=True),
+        "has_user_data": Property(),
     }
 
     @property
     def ips(self):
         """
         The ips related collection is not normalized like the others, so we have to
         make an ad-hoc object to return for its response
@@ -586,15 +588,19 @@
         :type: month: int
 
         :returns: The network transfer statistics for the specified month.
         :rtype: MappedObject
         """
 
         result = self._client.get(
-            "{}/transfer/{}/{}".format(Instance.api_endpoint, year, month),
+            "{}/transfer/{}/{}".format(
+                Instance.api_endpoint,
+                parse.quote(str(year)),
+                parse.quote(str(month)),
+            ),
             model=self,
         )
 
         return MappedObject(**result)
 
     @property
     def transfer(self):
@@ -1411,15 +1417,17 @@
         :returns: The JSON stats for this Instance at the specified Datetime
         :rtype: dict
         """
         # TODO - this would be nicer if we formatted the stats
         if not isinstance(dt, datetime):
             raise TypeError("stats_for requires a datetime object!")
         return self._client.get(
-            "{}/stats/{}".format(Instance.api_endpoint, dt.strftime("%Y/%m")),
+            "{}/stats/{}".format(
+                Instance.api_endpoint, parse.quote(dt.strftime("%Y/%m"))
+            ),
             model=self,
         )
 
 
 class UserDefinedFieldType(Enum):
     text = 1
     select_one = 2
```

### Comparing `linode_api4-5.6.0/linode_api4/objects/lke.py` & `linode_api4-5.7.0/linode_api4/objects/lke.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from urllib import parse
+
 from linode_api4.errors import UnexpectedResponseError
 from linode_api4.objects import (
     Base,
     DerivedBase,
     Instance,
     MappedObject,
     Property,
@@ -67,15 +69,15 @@
         "cluster_id": Property(identifier=True),
         "type": Property(slug_relationship=Type),
         "disks": Property(),
         "count": Property(mutable=True),
         "nodes": Property(
             volatile=True
         ),  # this is formatted in _populate below
-        "autoscaler": Property(),
+        "autoscaler": Property(mutable=True),
         "tags": Property(mutable=True),
     }
 
     def _populate(self, json):
         """
         Parse Nodes into more useful LKENodePoolNode objects
         """
@@ -113,17 +115,17 @@
     properties = {
         "id": Property(identifier=True),
         "created": Property(is_datetime=True),
         "label": Property(mutable=True),
         "tags": Property(mutable=True),
         "updated": Property(is_datetime=True),
         "region": Property(slug_relationship=Region),
-        "k8s_version": Property(slug_relationship=KubeVersion),
+        "k8s_version": Property(slug_relationship=KubeVersion, mutable=True),
         "pools": Property(derived_class=LKENodePool),
-        "control_plane": Property(),
+        "control_plane": Property(mutable=True),
     }
 
     @property
     def api_endpoints(self):
         """
         A list of API Endpoints for this Cluster.
 
@@ -250,15 +252,18 @@
         :type nodeId: str
 
         :returns: The specified Node
         :rtype: LKENodePoolNode
         """
 
         node = self._client.get(
-            "{}/nodes/{}".format(LKECluster.api_endpoint, nodeId), model=self
+            "{}/nodes/{}".format(
+                LKECluster.api_endpoint, parse.quote(str(nodeId))
+            ),
+            model=self,
         )
 
         return LKENodePoolNode(self._client, node)
 
     def node_delete(self, nodeId):
         """
         Delete a specific Node from a Node Pool.
@@ -266,29 +271,34 @@
         API Documentation: https://www.linode.com/docs/api/linode-kubernetes-engine-lke/#node-delete
 
         :param nodeId: ID of the Node to delete.
         :type nodeId: str
         """
 
         self._client.delete(
-            "{}/nodes/{}".format(LKECluster.api_endpoint, nodeId), model=self
+            "{}/nodes/{}".format(
+                LKECluster.api_endpoint, parse.quote(str(nodeId))
+            ),
+            model=self,
         )
 
     def node_recycle(self, nodeId):
         """
         Recycle a specific Node from an LKE cluster.
 
         API Documentation: https://www.linode.com/docs/api/linode-kubernetes-engine-lke/#node-recycle
 
         :param nodeId: ID of the Node to recycle.
         :type nodeId: str
         """
 
         self._client.post(
-            "{}/nodes/{}/recycle".format(LKECluster.api_endpoint, nodeId),
+            "{}/nodes/{}/recycle".format(
+                LKECluster.api_endpoint, parse.quote(str(nodeId))
+            ),
             model=self,
         )
 
     def cluster_nodes_recycle(self):
         """
         Recycles all nodes in all pools of a designated Kubernetes Cluster.
```

### Comparing `linode_api4-5.6.0/linode_api4/objects/longview.py` & `linode_api4-5.7.0/linode_api4/objects/longview.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/objects/networking.py` & `linode_api4-5.7.0/linode_api4/objects/networking.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 class IPv6Pool(Base):
     """
     DEPRECATED
     """
 
-    api_endpoint = "/networking/ipv6/pools/{}"
+    api_endpoint = "/networking/ipv6/pools/{range}"
     id_attribute = "range"
 
     properties = {
         "range": Property(identifier=True),
         "region": Property(slug_relationship=Region),
     }
 
@@ -97,15 +97,15 @@
     An instance of a Linode VLAN.
     VLANs provide a mechanism for secure communication between two or more Linodes that are assigned to the same VLAN.
     VLANs are implicitly created during Instance or Instance Config creation.
 
     API Documentation: https://www.linode.com/docs/api/networking/#vlans-list
     """
 
-    api_endpoint = "/networking/vlans/{}"
+    api_endpoint = "/networking/vlans/{label}"
     id_attribute = "label"
 
     properties = {
         "label": Property(identifier=True),
         "created": Property(is_datetime=True),
         "linodes": Property(),
         "region": Property(slug_relationship=Region),
```

### Comparing `linode_api4-5.6.0/linode_api4/objects/nodebalancer.py` & `linode_api4-5.7.0/linode_api4/objects/nodebalancer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+from urllib import parse
 
 from linode_api4.errors import UnexpectedResponseError
 from linode_api4.objects import (
     Base,
     DerivedBase,
     MappedObject,
     Property,
@@ -267,15 +268,15 @@
         params = {
             "nodes": nodes,
         }
         params.update(kwargs)
 
         result = self._client.post(
             "{}/configs/{}/rebuild".format(
-                NodeBalancer.api_endpoint, config_id
+                NodeBalancer.api_endpoint, parse.quote(str(config_id))
             ),
             model=self,
             data=params,
         )
 
         if not "id" in result:
             raise UnexpectedResponseError(
```

### Comparing `linode_api4-5.6.0/linode_api4/objects/object_storage.py` & `linode_api4-5.7.0/linode_api4/objects/object_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from urllib import parse
+
 from linode_api4.errors import UnexpectedResponseError
 from linode_api4.objects import (
     Base,
     DerivedBase,
     MappedObject,
     Property,
     Region,
@@ -95,15 +97,15 @@
         params = {
             "acl": acl,
             "cors_enabled": cors_enabled,
         }
 
         resp = self._client.post(
             "/object-storage/buckets/{}/{}/access".format(
-                self.cluster, self.id
+                parse.quote(str(self.cluster)), parse.quote(str(self.id))
             ),
             data=drop_null_keys(params),
         )
 
         if "errors" in resp:
             raise UnexpectedResponseError(
                 "Unexpected response when modifying the access to a bucket!",
@@ -143,15 +145,15 @@
         params = {
             "acl": acl,
             "cors_enabled": cors_enabled,
         }
 
         resp = self._client.put(
             "/object-storage/buckets/{}/{}/access".format(
-                self.cluster, self.id
+                parse.quote(str(self.cluster)), parse.quote(str(self.id))
             ),
             data=drop_null_keys(params),
         )
 
         if "errors" in resp:
             raise UnexpectedResponseError(
                 "Unexpected response when updating the access to a bucket!",
@@ -173,15 +175,17 @@
         :type bucket: str
 
         :returns: True if the TLS/SSL certificate and private key in the bucket were successfully deleted.
         :rtype: bool
         """
 
         resp = self._client.delete(
-            "/object-storage/buckets/{}/{}/ssl".format(self.cluster, self.id)
+            "/object-storage/buckets/{}/{}/ssl".format(
+                parse.quote(str(self.cluster)), parse.quote(str(self.id))
+            )
         )
 
         if "error" in resp:
             raise UnexpectedResponseError(
                 "Unexpected response when deleting a bucket!",
                 json=resp,
             )
@@ -202,15 +206,17 @@
         :type bucket: str
 
         :returns: A result object which has a bool field indicating if this Bucket has a corresponding
                   TLS/SSL certificate that was uploaded by an Account user.
         :rtype: MappedObject
         """
         result = self._client.get(
-            "/object-storage/buckets/{}/{}/ssl".format(self.cluster, self.id)
+            "/object-storage/buckets/{}/{}/ssl".format(
+                parse.quote(str(self.cluster)), parse.quote(str(self.id))
+            )
         )
 
         if not "ssl" in result:
             raise UnexpectedResponseError(
                 "Unexpected response when getting the TLS/SSL certs indicator of a bucket!",
                 json=result,
             )
@@ -249,15 +255,17 @@
         :rtype: MappedObject
         """
         params = {
             "certificate": certificate,
             "private_key": private_key,
         }
         result = self._client.post(
-            "/object-storage/buckets/{}/{}/ssl".format(self.cluster, self.id),
+            "/object-storage/buckets/{}/{}/ssl".format(
+                parse.quote(str(self.cluster)), parse.quote(str(self.id))
+            ),
             data=params,
         )
 
         if not "ssl" in result:
             raise UnexpectedResponseError(
                 "Unexpected response when uploading TLS/SSL certs!",
                 json=result,
@@ -321,15 +329,15 @@
             "marker": marker,
             "delimiter": delimiter,
             "prefix": prefix,
             "page_size": page_size,
         }
         result = self._client.get(
             "/object-storage/buckets/{}/{}/object-list".format(
-                self.cluster, self.id
+                parse.quote(str(self.cluster)), parse.quote(str(self.id))
             ),
             data=drop_null_keys(params),
         )
 
         if not "data" in result:
             raise UnexpectedResponseError(
                 "Unexpected response when getting the contents of a bucket!",
@@ -477,25 +485,28 @@
         Returns a list of Buckets in this cluster belonging to this Account.
 
         This endpoint is available for convenience.
         It is recommended that instead you use the more fully-featured S3 API directly.
 
         API Documentation: https://www.linode.com/docs/api/object-storage/#object-storage-buckets-in-cluster-list
 
-        :param cluster_id: The ID of the cluster this bucket exists in.
-        :type cluster_id: str
+        :param filters: Any number of filters to apply to this query.
+                        See :doc:`Filtering Collections</linode_api4/objects/filtering>`
+                        for more details on filtering.
 
         :returns: A list of Object Storage Buckets that in the requested cluster.
         :rtype: PaginatedList of ObjectStorageBucket
         """
 
         return self._client._get_and_filter(
             ObjectStorageBucket,
             *filters,
-            endpoint="/object-storage/buckets/{}".format(self.id),
+            endpoint="/object-storage/buckets/{}".format(
+                parse.quote(str(self.id))
+            ),
         )
 
 
 class ObjectStorageKeys(Base):
     """
     A keypair that allows third-party applications to access Linode Object Storage.
```

### Comparing `linode_api4-5.6.0/linode_api4/objects/profile.py` & `linode_api4-5.7.0/linode_api4/objects/profile.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/objects/region.py` & `linode_api4-5.7.0/linode_api4/objects/region.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/objects/support.py` & `linode_api4-5.7.0/linode_api4/objects/support.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/objects/tag.py` & `linode_api4-5.7.0/linode_api4/objects/tag.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/objects/volume.py` & `linode_api4-5.7.0/linode_api4/objects/volume.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/paginated_list.py` & `linode_api4-5.7.0/linode_api4/paginated_list.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/polling.py` & `linode_api4-5.7.0/linode_api4/polling.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4/util.py` & `linode_api4-5.7.0/linode_api4/util.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/linode_api4.egg-info/PKG-INFO` & `linode_api4-5.7.0/linode_api4.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linode-api4
-Version: 5.6.0
+Version: 5.7.0
 Summary: The official python SDK for Linode API v4
 Home-page: https://github.com/linode/linode_api4-python
 Author: Linode
 Author-email: developers@linode.com
 License: BSD 3-Clause License
 Keywords: linode cloud hosting infrastructure
 Classifier: Development Status :: 5 - Production/Stable
@@ -161,15 +161,15 @@
 
 Integration Tests
 -----------------
 Integration tests live in the ``test/integration`` directory.
 
 Pre-requisite
 ^^^^^^^^^^^^^^^^^
-Export Linode API token as `LINODE_CLI_TOKEN` before running integration tests::
+Export Linode API token as `LINODE_TOKEN` before running integration tests::
 
     export LINODE_TOKEN = $(your_token)
 
 Running the tests
 ^^^^^^^^^^^^^^^^^
 Run the tests locally using the make command. Run the entire test suite using command below::
```

### Comparing `linode_api4-5.6.0/linode_api4.egg-info/SOURCES.txt` & `linode_api4-5.7.0/linode_api4.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 test/fixtures/networking_firewalls_123.json
 test/fixtures/networking_firewalls_123_devices.json
 test/fixtures/networking_firewalls_123_devices_123.json
 test/fixtures/networking_firewalls_123_rules.json
 test/fixtures/networking_ips_127.0.0.1.json
 test/fixtures/networking_ipv6_pools.json
 test/fixtures/networking_ipv6_ranges.json
-test/fixtures/networking_ipv6_ranges_2600:3c01::.json
+test/fixtures/networking_ipv6_ranges_2600%3A3c01%3A%3A.json
 test/fixtures/networking_vlans.json
 test/fixtures/nodebalancers.json
 test/fixtures/nodebalancers_123456_configs.json
 test/fixtures/nodebalancers_123456_configs_65432_nodes.json
 test/fixtures/nodebalancers_12345_configs_4567_rebuild.json
 test/fixtures/nodebalancers_12345_stats.json
 test/fixtures/object-storage_buckets.json
```

### Comparing `linode_api4-5.6.0/setup.py` & `linode_api4-5.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/account.json` & `linode_api4-5.7.0/test/fixtures/account.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/account_events_123.json` & `linode_api4-5.7.0/test/fixtures/account_events_123.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/databases_instances.json` & `linode_api4-5.7.0/test/fixtures/databases_instances.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/databases_mysql_instances.json` & `linode_api4-5.7.0/test/fixtures/databases_mysql_instances.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/databases_postgresql_instances.json` & `linode_api4-5.7.0/test/fixtures/databases_postgresql_instances.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/databases_types.json` & `linode_api4-5.7.0/test/fixtures/databases_types.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/images.json` & `linode_api4-5.7.0/test/fixtures/images.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9916666666666667%*

 * *Differences: {"'data'": "{0: {'capabilities': []}, 1: {'capabilities': []}, 2: {'capabilities': []}, 3: "*

 * *           "{'capabilities': ['cloud-init']}}"}*

```diff
@@ -1,10 +1,11 @@
 {
     "data": [
         {
+            "capabilities": [],
             "created": "2017-01-01T00:01:01",
             "created_by": "linode",
             "deprecated": false,
             "description": null,
             "eol": "2026-07-01T04:00:00",
             "expiry": "2026-08-01T04:00:00",
             "id": "linode/debian9",
@@ -13,14 +14,15 @@
             "size": 1100,
             "status": "available",
             "type": "manual",
             "updated": "2020-07-01T04:00:00",
             "vendor": "Debian"
         },
         {
+            "capabilities": [],
             "created": "2017-01-01T00:01:01",
             "created_by": "linode",
             "deprecated": false,
             "description": null,
             "eol": "2026-07-01T04:00:00",
             "expiry": "2026-08-01T04:00:00",
             "id": "linode/ubuntu17.04",
@@ -29,14 +31,15 @@
             "size": 1500,
             "status": "available",
             "type": "manual",
             "updated": "2020-07-01T04:00:00",
             "vendor": "Ubuntu"
         },
         {
+            "capabilities": [],
             "created": "2017-01-01T00:01:01",
             "created_by": "linode",
             "deprecated": false,
             "description": null,
             "eol": "2026-07-01T04:00:00",
             "expiry": "2026-08-01T04:00:00",
             "id": "linode/fedora26",
@@ -45,14 +48,17 @@
             "size": 1500,
             "status": "available",
             "type": "manual",
             "updated": "2020-07-01T04:00:00",
             "vendor": "Fedora"
         },
         {
+            "capabilities": [
+                "cloud-init"
+            ],
             "created": "2017-08-20T14:01:01",
             "created_by": "testguy",
             "deprecated": false,
             "description": null,
             "eol": "2026-07-01T04:00:00",
             "expiry": "2026-08-01T04:00:00",
             "id": "private/123",
```

### Comparing `linode_api4-5.6.0/test/fixtures/linode_instances.json` & `linode_api4-5.7.0/test/fixtures/linode_instances.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/linode_instances_123_backups.json` & `linode_api4-5.7.0/test/fixtures/linode_instances_123_backups.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/linode_instances_123_configs.json` & `linode_api4-5.7.0/test/fixtures/linode_instances_123_configs.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/linode_instances_123_configs_456789.json` & `linode_api4-5.7.0/test/fixtures/linode_instances_123_configs_456789.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/linode_instances_123_firewalls.json` & `linode_api4-5.7.0/test/fixtures/linode_instances_123_firewalls.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/linode_instances_123_ips.json` & `linode_api4-5.7.0/test/fixtures/linode_instances_123_ips.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/linode_instances_123_nodebalancers.json` & `linode_api4-5.7.0/test/fixtures/linode_instances_123_nodebalancers.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/linode_instances_123_volumes.json` & `linode_api4-5.7.0/test/fixtures/linode_instances_123_volumes.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/linode_stackscripts_10079.json` & `linode_api4-5.7.0/test/fixtures/linode_stackscripts_10079.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/linode_types.json` & `linode_api4-5.7.0/test/fixtures/linode_types.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/longview_clients.json` & `linode_api4-5.7.0/test/fixtures/longview_clients.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/longview_subscriptions.json` & `linode_api4-5.7.0/test/fixtures/longview_subscriptions.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/nodebalancers.json` & `linode_api4-5.7.0/test/fixtures/nodebalancers.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/nodebalancers_123456_configs.json` & `linode_api4-5.7.0/test/fixtures/nodebalancers_123456_configs.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/nodebalancers_12345_configs_4567_rebuild.json` & `linode_api4-5.7.0/test/fixtures/nodebalancers_12345_configs_4567_rebuild.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/profile.json` & `linode_api4-5.7.0/test/fixtures/profile.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/profile_sshkeys.json` & `linode_api4-5.7.0/test/fixtures/profile_sshkeys.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/regions.json` & `linode_api4-5.7.0/test/fixtures/regions.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/support_tickets_123.json` & `linode_api4-5.7.0/test/fixtures/support_tickets_123.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/tags_something.json` & `linode_api4-5.7.0/test/fixtures/tags_something.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/fixtures/volumes.json` & `linode_api4-5.7.0/test/fixtures/volumes.json`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/integration/conftest.py` & `linode_api4-5.7.0/test/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/integration/helpers.py` & `linode_api4-5.7.0/test/integration/helpers.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/integration/linode_client/test_linode_client.py` & `linode_api4-5.7.0/test/integration/linode_client/test_linode_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,35 +42,38 @@
     assert re.search("^$|[a-zA-Z]+", account.state)
     assert re.search("^$|[a-zA-Z]+", account.country)
     assert re.search("^$|[a-zA-Z0-9]+", account.zip)
     if account.tax_id:
         assert re.search("^$|[0-9]+", account.tax_id)
 
 
+@pytest.mark.smoke
 def test_fails_to_create_domain_without_soa_email(setup_client_and_linode):
     client = setup_client_and_linode[0]
 
     timestamp = str(int(time.time()))
     domain_addr = timestamp + "example.com"
     try:
         domain = client.domain_create(domain=domain_addr)
     except ApiError as e:
         assert e.status == 400
 
 
+@pytest.mark.smoke
 def test_get_domains(get_client, create_domain):
     client = get_client
     domain = create_domain
     domain_dict = client.domains()
 
     dom_list = [i.domain for i in domain_dict]
 
     assert domain.domain in dom_list
 
 
+@pytest.mark.smoke
 def test_image_create(setup_client_and_linode):
     client = setup_client_and_linode[0]
     linode = setup_client_and_linode[1]
 
     label = get_test_label()
     description = "Test description"
     disk_id = linode.disks.first().id
@@ -161,14 +164,15 @@
     tag_label_list = [i.label for i in tags]
 
     tag.delete()
 
     assert label in tag_label_list
 
 
+@pytest.mark.smoke
 def test_create_tag_with_entities(
     setup_client_and_linode, create_nodebalancer, create_domain, create_volume
 ):
     client = setup_client_and_linode[0]
     linode = setup_client_and_linode[1]
     nodebalancer = create_nodebalancer
     domain = create_domain
@@ -219,14 +223,15 @@
     assert linode_instance.image is None
 
     res = linode_instance.delete()
 
     assert res
 
 
+@pytest.mark.smoke
 def test_create_linode_instance_with_image(setup_client_and_linode):
     linode = setup_client_and_linode[1]
 
     assert re.search("linode/debian9", str(linode.image))
 
 
 # LongviewGroupTests
```

### Comparing `linode_api4-5.6.0/test/integration/linode_client/test_retry.py` & `linode_api4-5.7.0/test/integration/linode_client/test_retry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from test.integration.conftest import get_token
 
 import httpretty
+import pytest
 
 from linode_api4 import ApiError, LinodeClient
 
 """
 Tests for retrying on intermittent errors.
 
 .. warning::
@@ -32,14 +33,15 @@
 def get_retry_client():
     client = LinodeClient(token=get_token(), base_url="https://localhost")
     # sidestep the validation to do immediate retries so tests aren't slow
     client.retry_rate_limit_interval = 0.1
     return client
 
 
+@pytest.mark.smoke
 @httpretty.activate
 def test_get_retry_statuses():
     """
     Tests that retries work as expected on 408 and 429 responses.
     """
 
     httpretty.register_uri(
@@ -68,15 +70,15 @@
 
 @httpretty.activate
 def test_post_retry_statuses():
     httpretty.register_uri(
         httpretty.POST, "https://localhost/test", responses=ERROR_RESPONSES
     )
 
-    get_retry_client.post("/test")
+    get_retry_client().post("/test")
 
     assert len(httpretty.latest_requests()) == 3
 
 
 @httpretty.activate
 def test_delete_retry_statuses():
     httpretty.register_uri(
```

### Comparing `linode_api4-5.6.0/test/integration/models/test_account.py` & `linode_api4-5.7.0/test/integration/models/test_account.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import time
 from test.integration.helpers import get_test_label
 
+import pytest
+
 from linode_api4.objects import (
     Account,
     AccountSettings,
     Event,
     Login,
     OAuthClient,
     User,
 )
 
 
+@pytest.mark.smoke
 def test_get_account(get_client):
     client = get_client
     account = client.account()
     account_id = account.id
     account_get = client.load(Account, account_id)
 
     assert account_get.first_name == account.first_name
@@ -52,14 +55,15 @@
     assert "managed" in str(account_settings._raw_json)
     assert "network_helper" in str(account_settings._raw_json)
     assert "longview_subscription" in str(account_settings._raw_json)
     assert "backups_enabled" in str(account_settings._raw_json)
     assert "object_storage" in str(account_settings._raw_json)
 
 
+@pytest.mark.smoke
 def test_latest_get_event(get_client):
     client = get_client
 
     available_regions = client.regions()
     chosen_region = available_regions[0]
     label = get_test_label()
```

### Comparing `linode_api4-5.6.0/test/integration/models/test_database.py` & `linode_api4-5.7.0/test/integration/models/test_database.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/integration/models/test_domain.py` & `linode_api4-5.7.0/test/integration/models/test_domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from test.integration.helpers import wait_for_condition
 
 import pytest
 
 from linode_api4.objects import Domain, DomainRecord
 
 
+@pytest.mark.smoke
 def test_get_domain_record(get_client, create_domain):
     dr = DomainRecord(
         get_client, create_domain.records.first().id, create_domain.id
     )
 
     assert dr.id == create_domain.records.first().id
```

### Comparing `linode_api4-5.6.0/test/integration/models/test_firewall.py` & `linode_api4-5.7.0/test/integration/models/test_firewall.py`

 * *Files 15% similar despite different names*

```diff
@@ -17,22 +17,24 @@
     )
 
     yield linode_instance
 
     linode_instance.delete()
 
 
+@pytest.mark.smoke
 def test_get_firewall_rules(get_client, create_firewall):
     firewall = get_client.load(Firewall, create_firewall.id)
     rules = firewall.rules
 
     assert rules.inbound_policy in ["ACCEPT", "DROP"]
     assert rules.outbound_policy in ["ACCEPT", "DROP"]
 
 
+@pytest.mark.smoke
 def test_update_firewall_rules(get_client, create_firewall):
     firewall = get_client.load(Firewall, create_firewall.id)
     new_rules = {
         "inbound": [
             {
                 "action": "ACCEPT",
                 "addresses": {
```

### Comparing `linode_api4-5.6.0/test/integration/models/test_image.py` & `linode_api4-5.7.0/test/integration/models/test_image.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     yield image
 
     image.delete()
     images = get_client.images()
     delete_instance_with_test_kw(images)
 
 
+@pytest.mark.smoke
 def test_get_image(get_client, image_upload):
     image = get_client.load(Image, image_upload.id)
 
     assert image.label == image_upload.label
 
 
 def test_image_create_upload(get_client):
```

### Comparing `linode_api4-5.6.0/test/integration/models/test_linode.py` & `linode_api4-5.7.0/test/integration/models/test_linode.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
     volume.detach()
     # wait for volume detach, can't currently get the attach/unattached status via SDK
     time.sleep(30)
 
     volume.delete()
 
 
+@pytest.mark.smoke
 @pytest.fixture
 def create_linode_for_long_running_tests(get_client):
     client = get_client
     available_regions = client.regions()
     chosen_region = available_regions[0]
     label = get_test_label()
```

### Comparing `linode_api4-5.6.0/test/integration/models/test_lke.py` & `linode_api4-5.7.0/test/integration/models/test_lke.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 
 def get_node_status(cluster: LKECluster, status: str):
     node = cluster.pools[0].nodes[0]
     return node.status == status
 
 
+@pytest.mark.smoke
 def test_get_lke_clusters(get_client, create_lke_cluster):
     cluster = get_client.load(LKECluster, create_lke_cluster.id)
 
     assert cluster._raw_json == create_lke_cluster._raw_json
 
 
 def test_get_lke_pool(get_client, create_lke_cluster):
```

### Comparing `linode_api4-5.6.0/test/integration/models/test_longview.py` & `linode_api4-5.7.0/test/integration/models/test_longview.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import re
 import time
 
+import pytest
+
 from linode_api4.objects import LongviewClient, LongviewSubscription
 
 
+@pytest.mark.smoke
 def test_get_longview_client(get_client, create_longview_client):
     longview = get_client.load(LongviewClient, create_longview_client.id)
 
     assert longview.id == create_longview_client.id
 
 
 def test_update_longview_label(get_client, create_longview_client):
```

### Comparing `linode_api4-5.6.0/test/integration/models/test_nodebalancer.py` & `linode_api4-5.7.0/test/integration/models/test_nodebalancer.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,24 +47,25 @@
     config = get_client.load(
         NodeBalancerConfig,
         create_nb_config.id,
         create_nb_config.nodebalancer_id,
     )
 
 
+@pytest.mark.smoke
 def test_create_nb_node(
     get_client, create_nb_config, create_linode_with_private_ip
 ):
     config = get_client.load(
         NodeBalancerConfig,
         create_nb_config.id,
         create_nb_config.nodebalancer_id,
     )
     linode = create_linode_with_private_ip
-    address = [a for a in linode.ipv4 if re.search("192.+", a)][0]
+    address = [a for a in linode.ipv4 if re.search("192.168.+", a)][0]
     node = config.node_create(
         "node_test", address + ":80", weight=50, mode="accept"
     )
 
     assert re.search("192.168.+:[0-9]+", node.address)
     assert "node_test" == node.label
```

### Comparing `linode_api4-5.6.0/test/integration/models/test_volume.py` & `linode_api4-5.7.0/test/integration/models/test_volume.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 def get_status(volume: Volume, status: str):
     client = LinodeClient(token=get_token())
     volume = client.load(Volume, volume.id)
     return volume.status == status
 
 
+@pytest.mark.smoke
 def test_get_volume(get_client, create_volume):
     volume = get_client.load(Volume, create_volume.id)
 
     assert volume.id == create_volume.id
 
 
 def test_update_volume_tag(get_client, create_volume):
```

### Comparing `linode_api4-5.6.0/test/unit/base.py` & `linode_api4-5.7.0/test/unit/base.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/fixtures.py` & `linode_api4-5.7.0/test/unit/fixtures.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/linode_client_test.py` & `linode_api4-5.7.0/test/unit/linode_client_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -125,14 +125,15 @@
         Tests that an Image can be created successfully
         """
         with self.mock_post("images/private/123") as m:
             i = self.client.image_create(654, "Test-Image", "This is a test")
 
             self.assertIsNotNone(i)
             self.assertEqual(i.id, "private/123")
+            self.assertEqual(i.capabilities[0], "cloud-init")
 
             self.assertEqual(m.call_url, "/images")
 
             self.assertEqual(
                 m.call_data,
                 {
                     "disk_id": 654,
```

### Comparing `linode_api4-5.6.0/test/unit/login_client_test.py` & `linode_api4-5.7.0/test/unit/login_client_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/objects/account_test.py` & `linode_api4-5.7.0/test/unit/objects/account_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/objects/database_test.py` & `linode_api4-5.7.0/test/unit/objects/database_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/objects/domain_test.py` & `linode_api4-5.7.0/test/unit/objects/domain_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/objects/firewall_test.py` & `linode_api4-5.7.0/test/unit/objects/firewall_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/objects/linode_test.py` & `linode_api4-5.7.0/test/unit/objects/linode_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -383,14 +383,53 @@
                     "authorized_users": ["test"],
                     "read_only": False,
                 },
             )
 
         assert disk.id == 12345
 
+    def test_instance_create_with_user_data(self):
+        """
+        Tests that the metadata field is populated on Linode create.
+        """
+
+        with self.mock_post("linode/instances/123") as m:
+            self.client.linode.instance_create(
+                "g6-nanode-1",
+                "us-southeast",
+                metadata=self.client.linode.build_instance_metadata(
+                    user_data="cool"
+                ),
+            )
+
+            self.assertEqual(
+                m.call_data,
+                {
+                    "region": "us-southeast",
+                    "type": "g6-nanode-1",
+                    "metadata": {"user_data": "Y29vbA=="},
+                },
+            )
+
+    def test_build_instance_metadata(self):
+        """
+        Tests that the metadata field is built correctly.
+        """
+        self.assertEqual(
+            self.client.linode.build_instance_metadata(user_data="cool"),
+            {"user_data": "Y29vbA=="},
+        )
+
+        self.assertEqual(
+            self.client.linode.build_instance_metadata(
+                user_data="cool", encode_user_data=False
+            ),
+            {"user_data": "cool"},
+        )
+
 
 class DiskTest(ClientBaseCase):
     """
     Tests for the Disk object
     """
 
     def test_resize(self):
```

### Comparing `linode_api4-5.6.0/test/unit/objects/lke_test.py` & `linode_api4-5.7.0/test/unit/objects/lke_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/objects/longview_test.py` & `linode_api4-5.7.0/test/unit/objects/longview_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/objects/mapped_object_test.py` & `linode_api4-5.7.0/test/unit/objects/mapped_object_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/objects/networking_test.py` & `linode_api4-5.7.0/test/unit/objects/networking_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/objects/nodebalancers_test.py` & `linode_api4-5.7.0/test/unit/objects/nodebalancers_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/objects/object_storage_test.py` & `linode_api4-5.7.0/test/unit/objects/object_storage_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/objects/polling_test.py` & `linode_api4-5.7.0/test/unit/objects/polling_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/objects/profile_test.py` & `linode_api4-5.7.0/test/unit/objects/profile_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/objects/region_test.py` & `linode_api4-5.7.0/test/unit/objects/region_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/objects/support_test.py` & `linode_api4-5.7.0/test/unit/objects/support_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/objects/tag_test.py` & `linode_api4-5.7.0/test/unit/objects/tag_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/objects/volume_test.py` & `linode_api4-5.7.0/test/unit/objects/volume_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/paginated_list_test.py` & `linode_api4-5.7.0/test/unit/paginated_list_test.py`

 * *Files identical despite different names*

### Comparing `linode_api4-5.6.0/test/unit/util_test.py` & `linode_api4-5.7.0/test/unit/util_test.py`

 * *Files identical despite different names*

