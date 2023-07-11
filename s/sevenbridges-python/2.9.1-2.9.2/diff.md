# Comparing `tmp/sevenbridges-python-2.9.1.tar.gz` & `tmp/sevenbridges-python-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sevenbridges-python-2.9.1.tar", last modified: Wed Nov  2 15:32:32 2022, max compression
+gzip compressed data, was "sevenbridges-python-2.9.2.tar", last modified: Tue Jul 11 12:56:33 2023, max compression
```

## Comparing `sevenbridges-python-2.9.1.tar` & `sevenbridges-python-2.9.2.tar`

### file list

```diff
@@ -1,121 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:32.824811 sevenbridges-python-2.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8717 2022-11-02 15:32:32.824811 sevenbridges-python-2.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7884 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      174 2022-11-02 15:32:32.824811 sevenbridges-python-2.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:32.816811 sevenbridges-python-2.9.1/sevenbridges/
--rw-r--r--   0 runner    (1001) docker     (121)     3531 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4312 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4876 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     3113 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     4598 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:32.816811 sevenbridges-python-2.9.1/sevenbridges/http/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11881 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/http/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2343 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/http/error_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:32.816811 sevenbridges-python-2.9.1/sevenbridges/meta/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/meta/collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1715 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/meta/comp_mutable_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)     2039 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/meta/data.py
--rw-r--r--   0 runner    (1001) docker     (121)     6228 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/meta/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)     9317 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/meta/resource.py
--rw-r--r--   0 runner    (1001) docker     (121)    10566 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/meta/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:32.820811 sevenbridges-python-2.9.1/sevenbridges/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2001 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/actions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6973 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     5012 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/async_jobs.py
--rw-r--r--   0 runner    (1001) docker     (121)    31582 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/automation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2072 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/billing_analysis_breakdown.py
--rw-r--r--   0 runner    (1001) docker     (121)     1750 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/billing_egress_breakdown.py
--rw-r--r--   0 runner    (1001) docker     (121)     2882 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/billing_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/billing_storage_breakdown.py
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/bulk.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:32.820811 sevenbridges-python-2.9.1/sevenbridges/models/compound/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      681 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/analysis_cost.py
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/analysis_cost_breakdown.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:32.820811 sevenbridges-python-2.9.1/sevenbridges/models/compound/billing/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/billing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/billing/invoice_period.py
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/billing/project_breakdown.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/billing/task_breakdown.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/egress_cost.py
--rw-r--r--   0 runner    (1001) docker     (121)      564 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/error.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:32.820811 sevenbridges-python-2.9.1/sevenbridges/models/compound/files/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/files/download_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/files/file_origin.py
--rw-r--r--   0 runner    (1001) docker     (121)      515 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/files/file_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/files/metadata.py
--rw-r--r--   0 runner    (1001) docker     (121)      524 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/import_result.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:32.824811 sevenbridges-python-2.9.1/sevenbridges/models/compound/jobs/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/jobs/job.py
--rw-r--r--   0 runner    (1001) docker     (121)      373 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/jobs/job_docker.py
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/jobs/job_instance.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/jobs/job_instance_disk.py
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/jobs/job_log.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:32.824811 sevenbridges-python-2.9.1/sevenbridges/models/compound/limits/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/limits/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/limits/rate.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:32.824811 sevenbridges-python-2.9.1/sevenbridges/models/compound/markers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/markers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/markers/position.py
--rw-r--r--   0 runner    (1001) docker     (121)      432 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/measurement.py
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/price.py
--rw-r--r--   0 runner    (1001) docker     (121)      733 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/price_breakdown.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:32.824811 sevenbridges-python-2.9.1/sevenbridges/models/compound/projects/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/projects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      499 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/projects/permissions.py
--rw-r--r--   0 runner    (1001) docker     (121)      535 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/projects/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:32.824811 sevenbridges-python-2.9.1/sevenbridges/models/compound/tasks/
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1518 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/tasks/batch_by.py
--rw-r--r--   0 runner    (1001) docker     (121)      454 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/tasks/batch_group.py
--rw-r--r--   0 runner    (1001) docker     (121)     1314 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/tasks/execution_status.py
--rw-r--r--   0 runner    (1001) docker     (121)      675 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/tasks/input.py
--rw-r--r--   0 runner    (1001) docker     (121)      814 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/tasks/output.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:32.824811 sevenbridges-python-2.9.1/sevenbridges/models/compound/volumes/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/volumes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      503 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/volumes/import_destination.py
--rw-r--r--   0 runner    (1001) docker     (121)      502 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/volumes/properties.py
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/volumes/service.py
--rw-r--r--   0 runner    (1001) docker     (121)      578 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/volumes/volume_file.py
--rw-r--r--   0 runner    (1001) docker     (121)      549 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/volumes/volume_object.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/compound/volumes/volume_prefix.py
--rw-r--r--   0 runner    (1001) docker     (121)     5144 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1410 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/division.py
--rw-r--r--   0 runner    (1001) docker     (121)     4049 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/drs_import.py
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (121)     2352 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)      607 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/execution_details.py
--rw-r--r--   0 runner    (1001) docker     (121)    21153 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     1481 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/invoice.py
--rw-r--r--   0 runner    (1001) docker     (121)      605 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/link.py
--rw-r--r--   0 runner    (1001) docker     (121)     3587 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/marker.py
--rw-r--r--   0 runner    (1001) docker     (121)     1645 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/member.py
--rw-r--r--   0 runner    (1001) docker     (121)    14084 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/project.py
--rw-r--r--   0 runner    (1001) docker     (121)      633 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (121)     6333 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/storage_export.py
--rw-r--r--   0 runner    (1001) docker     (121)     8354 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/storage_import.py
--rw-r--r--   0 runner    (1001) docker     (121)    16820 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/task.py
--rw-r--r--   0 runner    (1001) docker     (121)     5439 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/team.py
--rw-r--r--   0 runner    (1001) docker     (121)      644 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/team_member.py
--rw-r--r--   0 runner    (1001) docker     (121)     2815 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/user.py
--rw-r--r--   0 runner    (1001) docker     (121)    18000 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/models/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:32.824811 sevenbridges-python-2.9.1/sevenbridges/transfer/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/transfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11512 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/transfer/download.py
--rw-r--r--   0 runner    (1001) docker     (121)    18680 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/transfer/upload.py
--rw-r--r--   0 runner    (1001) docker     (121)     1661 2022-11-02 15:32:21.000000 sevenbridges-python-2.9.1/sevenbridges/transfer/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-02 15:32:31.000000 sevenbridges-python-2.9.1/sevenbridges/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-02 15:32:32.824811 sevenbridges-python-2.9.1/sevenbridges_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8717 2022-11-02 15:32:32.000000 sevenbridges-python-2.9.1/sevenbridges_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4002 2022-11-02 15:32:32.000000 sevenbridges-python-2.9.1/sevenbridges_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-02 15:32:32.000000 sevenbridges-python-2.9.1/sevenbridges_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-02 15:32:32.000000 sevenbridges-python-2.9.1/sevenbridges_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-02 15:32:32.000000 sevenbridges-python-2.9.1/sevenbridges_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:33.608895 sevenbridges-python-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-07-11 12:56:33.608895 sevenbridges-python-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-11 12:56:33.608895 sevenbridges-python-2.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:33.584900 sevenbridges-python-2.9.2/sevenbridges/
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:33.588899 sevenbridges-python-2.9.2/sevenbridges/http/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11933 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/http/error_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:33.588899 sevenbridges-python-2.9.2/sevenbridges/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/meta/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/meta/comp_mutable_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/meta/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6228 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/meta/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9317 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/meta/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10566 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/meta/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:33.596897 sevenbridges-python-2.9.2/sevenbridges/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/async_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31582 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/automation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/billing_analysis_breakdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/billing_egress_breakdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2882 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/billing_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/billing_storage_breakdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/bulk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:33.596897 sevenbridges-python-2.9.2/sevenbridges/models/compound/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/analysis_cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/analysis_cost_breakdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:33.596897 sevenbridges-python-2.9.2/sevenbridges/models/compound/billing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/billing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/billing/invoice_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/billing/project_breakdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/billing/task_breakdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/egress_cost.py
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:33.596897 sevenbridges-python-2.9.2/sevenbridges/models/compound/files/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/files/download_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/files/file_origin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/files/file_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/files/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/import_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:33.600896 sevenbridges-python-2.9.2/sevenbridges/models/compound/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/jobs/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/jobs/job_docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/jobs/job_instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/jobs/job_instance_disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/jobs/job_log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:33.600896 sevenbridges-python-2.9.2/sevenbridges/models/compound/limits/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/limits/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/limits/rate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:33.600896 sevenbridges-python-2.9.2/sevenbridges/models/compound/markers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/markers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/markers/position.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/price_breakdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:33.600896 sevenbridges-python-2.9.2/sevenbridges/models/compound/projects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/projects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/projects/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/projects/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:33.604896 sevenbridges-python-2.9.2/sevenbridges/models/compound/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/tasks/batch_by.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/tasks/batch_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/tasks/execution_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/tasks/input.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/tasks/output.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:33.604896 sevenbridges-python-2.9.2/sevenbridges/models/compound/volumes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/volumes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/volumes/import_destination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/volumes/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/volumes/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/volumes/volume_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/volumes/volume_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/compound/volumes/volume_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5144 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/division.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/drs_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/execution_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21153 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/marker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/member.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14084 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6333 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/storage_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/storage_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16820 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/team_member.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2815 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/models/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:33.608895 sevenbridges-python-2.9.2/sevenbridges/transfer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/transfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11512 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/transfer/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18680 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/transfer/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-11 12:56:25.000000 sevenbridges-python-2.9.2/sevenbridges/transfer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-11 12:56:32.000000 sevenbridges-python-2.9.2/sevenbridges/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 12:56:33.608895 sevenbridges-python-2.9.2/sevenbridges_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8717 2023-07-11 12:56:33.000000 sevenbridges-python-2.9.2/sevenbridges_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4002 2023-07-11 12:56:33.000000 sevenbridges-python-2.9.2/sevenbridges_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 12:56:33.000000 sevenbridges-python-2.9.2/sevenbridges_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-11 12:56:33.000000 sevenbridges-python-2.9.2/sevenbridges_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 12:56:33.000000 sevenbridges-python-2.9.2/sevenbridges_python.egg-info/top_level.txt
```

### Comparing `sevenbridges-python-2.9.1/LICENCE` & `sevenbridges-python-2.9.2/LICENCE`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/PKG-INFO` & `sevenbridges-python-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sevenbridges-python
-Version: 2.9.1
+Version: 2.9.2
 Summary: SBG API python client bindings
 Home-page: https://github.com/sbg/sevenbridges-python
 Maintainer: Seven Bridges Genomics Inc.
 Maintainer-email: dejan.knezevic@sbgenomics.com
 License: Apache Software License 2.0
 Keywords: sevenbridges,sbg,api,cgc,cancer,genomics,cloud
 Platform: Windows
```

### Comparing `sevenbridges-python-2.9.1/README.md` & `sevenbridges-python-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/setup.py` & `sevenbridges-python-2.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/__init__.py` & `sevenbridges-python-2.9.2/sevenbridges/__init__.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/api.py` & `sevenbridges-python-2.9.2/sevenbridges/api.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/config.py` & `sevenbridges-python-2.9.2/sevenbridges/config.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/decorators.py` & `sevenbridges-python-2.9.2/sevenbridges/decorators.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/errors.py` & `sevenbridges-python-2.9.2/sevenbridges/errors.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/http/client.py` & `sevenbridges-python-2.9.2/sevenbridges/http/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,14 +108,15 @@
             pass
     return None, None, None, None
 
 
 def mask_secrets(request_data):
     masked = copy.deepcopy(request_data)
     masked['headers']['X-SBG-Auth-Token'] = '*****'
+    masked['headers']['X-SBG-Session-Id'] = '*****'
     return masked
 
 
 class HttpClient:
     """
     Implementation of all low-level API stuff, creating and sending requests,
     returning raw responses, authorization, etc.
```

### Comparing `sevenbridges-python-2.9.1/sevenbridges/http/error_handlers.py` & `sevenbridges-python-2.9.2/sevenbridges/http/error_handlers.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/meta/collection.py` & `sevenbridges-python-2.9.2/sevenbridges/meta/collection.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/meta/comp_mutable_dict.py` & `sevenbridges-python-2.9.2/sevenbridges/meta/comp_mutable_dict.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/meta/data.py` & `sevenbridges-python-2.9.2/sevenbridges/meta/data.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/meta/fields.py` & `sevenbridges-python-2.9.2/sevenbridges/meta/fields.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/meta/resource.py` & `sevenbridges-python-2.9.2/sevenbridges/meta/resource.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/meta/transformer.py` & `sevenbridges-python-2.9.2/sevenbridges/meta/transformer.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/actions.py` & `sevenbridges-python-2.9.2/sevenbridges/models/actions.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/app.py` & `sevenbridges-python-2.9.2/sevenbridges/models/app.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/async_jobs.py` & `sevenbridges-python-2.9.2/sevenbridges/models/async_jobs.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/automation.py` & `sevenbridges-python-2.9.2/sevenbridges/models/automation.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/billing_analysis_breakdown.py` & `sevenbridges-python-2.9.2/sevenbridges/models/billing_analysis_breakdown.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/billing_egress_breakdown.py` & `sevenbridges-python-2.9.2/sevenbridges/models/billing_egress_breakdown.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/billing_group.py` & `sevenbridges-python-2.9.2/sevenbridges/models/billing_group.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/billing_storage_breakdown.py` & `sevenbridges-python-2.9.2/sevenbridges/models/billing_storage_breakdown.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/bulk.py` & `sevenbridges-python-2.9.2/sevenbridges/models/bulk.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/analysis_cost.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/analysis_cost.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/analysis_cost_breakdown.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/analysis_cost_breakdown.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/billing/project_breakdown.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/billing/project_breakdown.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/billing/task_breakdown.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/billing/task_breakdown.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/error.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/error.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/files/file_storage.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/files/file_storage.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/files/metadata.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/files/metadata.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/import_result.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/import_result.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/jobs/job.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/jobs/job.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/jobs/job_instance.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/jobs/job_instance.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/jobs/job_log.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/jobs/job_log.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/price.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/price.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/price_breakdown.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/price_breakdown.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/projects/settings.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/projects/settings.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/tasks/__init__.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/tasks/batch_by.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/tasks/batch_by.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/tasks/execution_status.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/tasks/execution_status.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/tasks/input.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/tasks/input.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/tasks/output.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/tasks/output.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/volumes/service.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/volumes/service.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/volumes/volume_file.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/volumes/volume_file.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/compound/volumes/volume_object.py` & `sevenbridges-python-2.9.2/sevenbridges/models/compound/volumes/volume_object.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/dataset.py` & `sevenbridges-python-2.9.2/sevenbridges/models/dataset.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/division.py` & `sevenbridges-python-2.9.2/sevenbridges/models/division.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/drs_import.py` & `sevenbridges-python-2.9.2/sevenbridges/models/drs_import.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/endpoints.py` & `sevenbridges-python-2.9.2/sevenbridges/models/endpoints.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/enums.py` & `sevenbridges-python-2.9.2/sevenbridges/models/enums.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/execution_details.py` & `sevenbridges-python-2.9.2/sevenbridges/models/execution_details.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/file.py` & `sevenbridges-python-2.9.2/sevenbridges/models/file.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/invoice.py` & `sevenbridges-python-2.9.2/sevenbridges/models/invoice.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/link.py` & `sevenbridges-python-2.9.2/sevenbridges/models/link.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/marker.py` & `sevenbridges-python-2.9.2/sevenbridges/models/marker.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/member.py` & `sevenbridges-python-2.9.2/sevenbridges/models/member.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/project.py` & `sevenbridges-python-2.9.2/sevenbridges/models/project.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/rate_limit.py` & `sevenbridges-python-2.9.2/sevenbridges/models/rate_limit.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/storage_export.py` & `sevenbridges-python-2.9.2/sevenbridges/models/storage_export.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/storage_import.py` & `sevenbridges-python-2.9.2/sevenbridges/models/storage_import.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/task.py` & `sevenbridges-python-2.9.2/sevenbridges/models/task.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/team.py` & `sevenbridges-python-2.9.2/sevenbridges/models/team.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/team_member.py` & `sevenbridges-python-2.9.2/sevenbridges/models/team_member.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/user.py` & `sevenbridges-python-2.9.2/sevenbridges/models/user.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/models/volume.py` & `sevenbridges-python-2.9.2/sevenbridges/models/volume.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/transfer/download.py` & `sevenbridges-python-2.9.2/sevenbridges/transfer/download.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/transfer/upload.py` & `sevenbridges-python-2.9.2/sevenbridges/transfer/upload.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges/transfer/utils.py` & `sevenbridges-python-2.9.2/sevenbridges/transfer/utils.py`

 * *Files identical despite different names*

### Comparing `sevenbridges-python-2.9.1/sevenbridges_python.egg-info/PKG-INFO` & `sevenbridges-python-2.9.2/sevenbridges_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sevenbridges-python
-Version: 2.9.1
+Version: 2.9.2
 Summary: SBG API python client bindings
 Home-page: https://github.com/sbg/sevenbridges-python
 Maintainer: Seven Bridges Genomics Inc.
 Maintainer-email: dejan.knezevic@sbgenomics.com
 License: Apache Software License 2.0
 Keywords: sevenbridges,sbg,api,cgc,cancer,genomics,cloud
 Platform: Windows
```

### Comparing `sevenbridges-python-2.9.1/sevenbridges_python.egg-info/SOURCES.txt` & `sevenbridges-python-2.9.2/sevenbridges_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

