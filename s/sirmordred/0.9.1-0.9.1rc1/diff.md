# Comparing `tmp/sirmordred-0.9.1.tar.gz` & `tmp/sirmordred-0.9.1rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirmordred-0.9.1.tar", max compression
+gzip compressed data, was "sirmordred-0.9.1rc1.tar", max compression
```

## Comparing `sirmordred-0.9.1.tar` & `sirmordred-0.9.1rc1.tar`

### file list

```diff
@@ -1,96 +1,96 @@
--rw-r--r--   0        0        0    35147 2023-07-11 16:27:03.049966 sirmordred-0.9.1/LICENSE
--rw-r--r--   0        0        0    40852 2023-07-11 16:27:03.049966 sirmordred-0.9.1/README.md
--rw-r--r--   0        0        0     8246 2023-07-11 16:27:03.049966 sirmordred-0.9.1/menu.yaml
--rw-r--r--   0        0        0     2166 2023-07-11 16:27:03.049966 sirmordred-0.9.1/pyproject.toml
--rw-r--r--   0        0        0      835 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/__init__.py
--rw-r--r--   0        0        0       86 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/_version.py
--rwxr-xr-x   0        0        0     4924 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/bin/sirmordred.py
--rw-r--r--   0        0        0    33508 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/config.py
--rw-r--r--   0        0        0     1836 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/error.py
--rw-r--r--   0        0        0     2306 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/github.py
--rwxr-xr-x   0        0        0    12672 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/sirmordred.py
--rw-r--r--   0        0        0     9833 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/task.py
--rw-r--r--   0        0        0     6487 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/task_collection.py
--rw-r--r--   0        0        0    20942 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/task_enrich.py
--rw-r--r--   0        0        0     3396 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/task_identities.py
--rw-r--r--   0        0        0     4424 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/task_manager.py
--rw-r--r--   0        0        0    29060 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/task_panels.py
--rw-r--r--   0        0        0     6484 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/task_projects.py
--rw-r--r--   0        0        0     1981 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/utils/find_affiliation_conflicts.py
--rw-r--r--   0        0        0      766 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/utils/grimoirelab_valid.yml
--rwxr-xr-x   0        0        0     4709 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/utils/healthcheck.py
--rw-r--r--   0        0        0        0 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/utils/logs/all.log
--rw-r--r--   0        0        0     7846 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/utils/micro.py
--rw-r--r--   0        0        0     2858 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/utils/panels_config.py
--rw-r--r--   0        0        0      864 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/utils/projects.json
--rw-r--r--   0        0        0     3141 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/utils/projects_json2yml.py
--rw-r--r--   0        0        0     3634 2023-07-11 16:27:03.053966 sirmordred-0.9.1/sirmordred/utils/setup.cfg
--rw-r--r--   0        0        0     4398 2023-07-11 16:27:03.053966 sirmordred-0.9.1/tests/aliases.json
--rw-r--r--   0        0        0   497664 2023-07-11 16:27:03.057966 sirmordred-0.9.1/tests/archives/askbot.archive
--rw-r--r--   0        0        0   150528 2023-07-11 16:27:03.057966 sirmordred-0.9.1/tests/archives/bugzilla.archive
--rw-r--r--   0        0        0    52224 2023-07-11 16:27:03.057966 sirmordred-0.9.1/tests/archives/bugzillarest.archive
--rw-r--r--   0        0        0    73728 2023-07-11 16:27:03.057966 sirmordred-0.9.1/tests/archives/confluence.archive
--rw-r--r--   0        0        0  7141376 2023-07-11 16:27:03.081967 sirmordred-0.9.1/tests/archives/crates.archive
--rw-r--r--   0        0        0   291840 2023-07-11 16:27:03.081967 sirmordred-0.9.1/tests/archives/discourse.archive
--rw-r--r--   0        0        0    16384 2023-07-11 16:27:03.081967 sirmordred-0.9.1/tests/archives/dockerhub.archive
--rw-r--r--   0        0        0  1713152 2023-07-11 16:27:03.089967 sirmordred-0.9.1/tests/archives/functest.archive
--rw-r--r--   0        0        0    49152 2023-07-11 16:27:03.089967 sirmordred-0.9.1/tests/archives/gerrit.archive
--rw-r--r--   0        0        0  9424896 2023-07-11 16:27:03.165969 sirmordred-0.9.1/tests/archives/github-issue.archive
--rw-r--r--   0        0        0 23023616 2023-07-11 16:27:03.197969 sirmordred-0.9.1/tests/archives/github-pull.archive
--rw-r--r--   0        0        0   208896 2023-07-11 16:27:03.197969 sirmordred-0.9.1/tests/archives/gitlab-issue.archive
--rw-r--r--   0        0        0   937984 2023-07-11 16:27:03.197969 sirmordred-0.9.1/tests/archives/gitlab-merge.archive
--rw-r--r--   0        0        0    65536 2023-07-11 16:27:03.201969 sirmordred-0.9.1/tests/archives/googlehits.archive
--rw-r--r--   0        0        0   228352 2023-07-11 16:27:03.201969 sirmordred-0.9.1/tests/archives/jenkins.archive
--rw-r--r--   0        0        0    86016 2023-07-11 16:27:03.201969 sirmordred-0.9.1/tests/archives/jira.archive
--rw-r--r--   0        0        0    69632 2023-07-11 16:27:03.201969 sirmordred-0.9.1/tests/archives/launchpad.archive
--rw-r--r--   0        0        0    31744 2023-07-11 16:27:03.201969 sirmordred-0.9.1/tests/archives/mediawiki-1.23.archive
--rw-r--r--   0        0        0   245760 2023-07-11 16:27:03.201969 sirmordred-0.9.1/tests/archives/mediawiki-1.28.archive
--rw-r--r--   0        0        0   136192 2023-07-11 16:27:03.201969 sirmordred-0.9.1/tests/archives/meetup.archive
--rw-r--r--   0        0        0  2310144 2023-07-11 16:27:03.209970 sirmordred-0.9.1/tests/archives/mozillaclub.archive
--rw-r--r--   0        0        0    35840 2023-07-11 16:27:03.209970 sirmordred-0.9.1/tests/archives/nntp.archive
--rw-r--r--   0        0        0    88064 2023-07-11 16:27:03.209970 sirmordred-0.9.1/tests/archives/phabricator.archive
--rw-r--r--   0        0        0    61440 2023-07-11 16:27:03.209970 sirmordred-0.9.1/tests/archives/redmine.archive
--rw-r--r--   0        0        0   182272 2023-07-11 16:27:03.209970 sirmordred-0.9.1/tests/archives/remo.archive
--rw-r--r--   0        0        0    25600 2023-07-11 16:27:03.209970 sirmordred-0.9.1/tests/archives/rss.archive
--rw-r--r--   0        0        0    86016 2023-07-11 16:27:03.209970 sirmordred-0.9.1/tests/archives/slack.archive
--rw-r--r--   0        0        0    17408 2023-07-11 16:27:03.209970 sirmordred-0.9.1/tests/archives/stackexchange.archive
--rw-r--r--   0        0        0    15360 2023-07-11 16:27:03.209970 sirmordred-0.9.1/tests/archives/telegram.archive
--rw-r--r--   0        0        0   385024 2023-07-11 16:27:03.213970 sirmordred-0.9.1/tests/archives/twitter.archive
--rw-r--r--   0        0        0     1769 2023-07-11 16:27:03.053966 sirmordred-0.9.1/tests/archives-test-projects.json
--rw-r--r--   0        0        0     5845 2023-07-11 16:27:03.053966 sirmordred-0.9.1/tests/archives-test.cfg
--rw-r--r--   0        0        0 15031534 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/data/eclipse-projects.json
--rw-r--r--   0        0        0       55 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/data/healthcheck_cache_invalid.json
--rw-r--r--   0        0        0       56 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/data/healthcheck_cache_valid.json
--rw-r--r--   0        0        0       56 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/data/healthcheck_cache_wrong_key.json
--rw-r--r--   0        0        0     2932 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/data/mordred.log
--rw-r--r--   0        0        0     3244 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/data/orgs_sortinghat.json
--rw-r--r--   0        0        0     3587 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/data/perceval_identities_sortinghat.json
--rw-r--r--   0        0        0     3607 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/data/remote_identities_sortinghat.json
--rw-r--r--   0        0        0     2032 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/data/task-identities-data.json
--rw-r--r--   0        0        0     4487 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/data/task-params-expected
--rw-r--r--   0        0        0     1716 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/data/task-params-test-projects.json
--rw-r--r--   0        0        0     4392 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/data/task-params-test.cfg
--rw-r--r--   0        0        0     2484 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/data/url-projects.json
--rwxr-xr-x   0        0        0     1166 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/run_tests.py
--rw-r--r--   0        0        0     6562 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/sortinghat_settings.py
--rw-r--r--   0        0        0     1451 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test-no-collection.cfg
--rw-r--r--   0        0        0     4655 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test-no-sh.cfg
--rw-r--r--   0        0        0      178 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test-projects-no-collection.json
--rw-r--r--   0        0        0     2484 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test-projects.json
--rw-r--r--   0        0        0      721 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test-repos-projects.json
--rw-r--r--   0        0        0     1798 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test-repos.cfg
--rw-r--r--   0        0        0     4936 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test.cfg
--rw-r--r--   0        0        0    14731 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test_config.py
--rw-r--r--   0        0        0     1849 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test_github.py
--rw-r--r--   0        0        0     3235 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test_healthcheck.py
--rw-r--r--   0        0        0     2706 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test_sirmordred.py
--rw-r--r--   0        0        0     7303 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test_studies.cfg
--rw-r--r--   0        0        0     5392 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test_task.py
--rw-r--r--   0        0        0     5956 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test_task_collection.py
--rw-r--r--   0        0        0    11770 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test_task_enrich.py
--rw-r--r--   0        0        0     5817 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test_task_identities.py
--rw-r--r--   0        0        0    10141 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test_task_manager.py
--rw-r--r--   0        0        0     6380 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test_task_panels.py
--rw-r--r--   0        0        0    13869 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test_task_projects.py
--rw-r--r--   0        0        0     1499 2023-07-11 16:27:03.265971 sirmordred-0.9.1/tests/test_wrong.cfg
--rw-r--r--   0        0        0    42442 1970-01-01 00:00:00.000000 sirmordred-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-07-11 14:54:31.751373 sirmordred-0.9.1rc1/LICENSE
+-rw-r--r--   0        0        0    40852 2023-07-11 14:54:31.751373 sirmordred-0.9.1rc1/README.md
+-rw-r--r--   0        0        0     8246 2023-07-11 14:54:31.751373 sirmordred-0.9.1rc1/menu.yaml
+-rw-r--r--   0        0        0     2171 2023-07-11 14:54:31.751373 sirmordred-0.9.1rc1/pyproject.toml
+-rw-r--r--   0        0        0      835 2023-07-11 14:54:31.751373 sirmordred-0.9.1rc1/sirmordred/__init__.py
+-rw-r--r--   0        0        0       91 2023-07-11 14:54:31.751373 sirmordred-0.9.1rc1/sirmordred/_version.py
+-rwxr-xr-x   0        0        0     4924 2023-07-11 14:54:31.751373 sirmordred-0.9.1rc1/sirmordred/bin/sirmordred.py
+-rw-r--r--   0        0        0    33508 2023-07-11 14:54:31.751373 sirmordred-0.9.1rc1/sirmordred/config.py
+-rw-r--r--   0        0        0     1836 2023-07-11 14:54:31.751373 sirmordred-0.9.1rc1/sirmordred/error.py
+-rw-r--r--   0        0        0     2306 2023-07-11 14:54:31.751373 sirmordred-0.9.1rc1/sirmordred/github.py
+-rwxr-xr-x   0        0        0    12672 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/sirmordred/sirmordred.py
+-rw-r--r--   0        0        0     9833 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/sirmordred/task.py
+-rw-r--r--   0        0        0     6487 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/sirmordred/task_collection.py
+-rw-r--r--   0        0        0    20942 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/sirmordred/task_enrich.py
+-rw-r--r--   0        0        0     3396 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/sirmordred/task_identities.py
+-rw-r--r--   0        0        0     4424 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/sirmordred/task_manager.py
+-rw-r--r--   0        0        0    29060 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/sirmordred/task_panels.py
+-rw-r--r--   0        0        0     6484 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/sirmordred/task_projects.py
+-rw-r--r--   0        0        0     1981 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/sirmordred/utils/find_affiliation_conflicts.py
+-rw-r--r--   0        0        0      766 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/sirmordred/utils/grimoirelab_valid.yml
+-rwxr-xr-x   0        0        0     4709 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/sirmordred/utils/healthcheck.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/sirmordred/utils/logs/all.log
+-rw-r--r--   0        0        0     7846 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/sirmordred/utils/micro.py
+-rw-r--r--   0        0        0     2858 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/sirmordred/utils/panels_config.py
+-rw-r--r--   0        0        0      864 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/sirmordred/utils/projects.json
+-rw-r--r--   0        0        0     3141 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/sirmordred/utils/projects_json2yml.py
+-rw-r--r--   0        0        0     3634 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/sirmordred/utils/setup.cfg
+-rw-r--r--   0        0        0     4398 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/tests/aliases.json
+-rw-r--r--   0        0        0   497664 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/tests/archives/askbot.archive
+-rw-r--r--   0        0        0   150528 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/tests/archives/bugzilla.archive
+-rw-r--r--   0        0        0    52224 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/tests/archives/bugzillarest.archive
+-rw-r--r--   0        0        0    73728 2023-07-11 14:54:31.759373 sirmordred-0.9.1rc1/tests/archives/confluence.archive
+-rw-r--r--   0        0        0  7141376 2023-07-11 14:54:31.779374 sirmordred-0.9.1rc1/tests/archives/crates.archive
+-rw-r--r--   0        0        0   291840 2023-07-11 14:54:31.779374 sirmordred-0.9.1rc1/tests/archives/discourse.archive
+-rw-r--r--   0        0        0    16384 2023-07-11 14:54:31.779374 sirmordred-0.9.1rc1/tests/archives/dockerhub.archive
+-rw-r--r--   0        0        0  1713152 2023-07-11 14:54:31.783374 sirmordred-0.9.1rc1/tests/archives/functest.archive
+-rw-r--r--   0        0        0    49152 2023-07-11 14:54:31.783374 sirmordred-0.9.1rc1/tests/archives/gerrit.archive
+-rw-r--r--   0        0        0  9424896 2023-07-11 14:54:31.847375 sirmordred-0.9.1rc1/tests/archives/github-issue.archive
+-rw-r--r--   0        0        0 23023616 2023-07-11 14:54:31.875376 sirmordred-0.9.1rc1/tests/archives/github-pull.archive
+-rw-r--r--   0        0        0   208896 2023-07-11 14:54:31.879376 sirmordred-0.9.1rc1/tests/archives/gitlab-issue.archive
+-rw-r--r--   0        0        0   937984 2023-07-11 14:54:31.879376 sirmordred-0.9.1rc1/tests/archives/gitlab-merge.archive
+-rw-r--r--   0        0        0    65536 2023-07-11 14:54:31.879376 sirmordred-0.9.1rc1/tests/archives/googlehits.archive
+-rw-r--r--   0        0        0   228352 2023-07-11 14:54:31.879376 sirmordred-0.9.1rc1/tests/archives/jenkins.archive
+-rw-r--r--   0        0        0    86016 2023-07-11 14:54:31.879376 sirmordred-0.9.1rc1/tests/archives/jira.archive
+-rw-r--r--   0        0        0    69632 2023-07-11 14:54:31.879376 sirmordred-0.9.1rc1/tests/archives/launchpad.archive
+-rw-r--r--   0        0        0    31744 2023-07-11 14:54:31.883376 sirmordred-0.9.1rc1/tests/archives/mediawiki-1.23.archive
+-rw-r--r--   0        0        0   245760 2023-07-11 14:54:31.883376 sirmordred-0.9.1rc1/tests/archives/mediawiki-1.28.archive
+-rw-r--r--   0        0        0   136192 2023-07-11 14:54:31.883376 sirmordred-0.9.1rc1/tests/archives/meetup.archive
+-rw-r--r--   0        0        0  2310144 2023-07-11 14:54:31.887376 sirmordred-0.9.1rc1/tests/archives/mozillaclub.archive
+-rw-r--r--   0        0        0    35840 2023-07-11 14:54:31.887376 sirmordred-0.9.1rc1/tests/archives/nntp.archive
+-rw-r--r--   0        0        0    88064 2023-07-11 14:54:31.887376 sirmordred-0.9.1rc1/tests/archives/phabricator.archive
+-rw-r--r--   0        0        0    61440 2023-07-11 14:54:31.887376 sirmordred-0.9.1rc1/tests/archives/redmine.archive
+-rw-r--r--   0        0        0   182272 2023-07-11 14:54:31.887376 sirmordred-0.9.1rc1/tests/archives/remo.archive
+-rw-r--r--   0        0        0    25600 2023-07-11 14:54:31.887376 sirmordred-0.9.1rc1/tests/archives/rss.archive
+-rw-r--r--   0        0        0    86016 2023-07-11 14:54:31.887376 sirmordred-0.9.1rc1/tests/archives/slack.archive
+-rw-r--r--   0        0        0    17408 2023-07-11 14:54:31.891376 sirmordred-0.9.1rc1/tests/archives/stackexchange.archive
+-rw-r--r--   0        0        0    15360 2023-07-11 14:54:31.891376 sirmordred-0.9.1rc1/tests/archives/telegram.archive
+-rw-r--r--   0        0        0   385024 2023-07-11 14:54:31.891376 sirmordred-0.9.1rc1/tests/archives/twitter.archive
+-rw-r--r--   0        0        0     1769 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/tests/archives-test-projects.json
+-rw-r--r--   0        0        0     5845 2023-07-11 14:54:31.755373 sirmordred-0.9.1rc1/tests/archives-test.cfg
+-rw-r--r--   0        0        0 15031534 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/data/eclipse-projects.json
+-rw-r--r--   0        0        0       55 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/data/healthcheck_cache_invalid.json
+-rw-r--r--   0        0        0       56 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/data/healthcheck_cache_valid.json
+-rw-r--r--   0        0        0       56 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/data/healthcheck_cache_wrong_key.json
+-rw-r--r--   0        0        0     2932 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/data/mordred.log
+-rw-r--r--   0        0        0     3244 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/data/orgs_sortinghat.json
+-rw-r--r--   0        0        0     3587 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/data/perceval_identities_sortinghat.json
+-rw-r--r--   0        0        0     3607 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/data/remote_identities_sortinghat.json
+-rw-r--r--   0        0        0     2032 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/data/task-identities-data.json
+-rw-r--r--   0        0        0     4487 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/data/task-params-expected
+-rw-r--r--   0        0        0     1716 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/data/task-params-test-projects.json
+-rw-r--r--   0        0        0     4392 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/data/task-params-test.cfg
+-rw-r--r--   0        0        0     2484 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/data/url-projects.json
+-rwxr-xr-x   0        0        0     1166 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/run_tests.py
+-rw-r--r--   0        0        0     6562 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/sortinghat_settings.py
+-rw-r--r--   0        0        0     1451 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test-no-collection.cfg
+-rw-r--r--   0        0        0     4655 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test-no-sh.cfg
+-rw-r--r--   0        0        0      178 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test-projects-no-collection.json
+-rw-r--r--   0        0        0     2484 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test-projects.json
+-rw-r--r--   0        0        0      721 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test-repos-projects.json
+-rw-r--r--   0        0        0     1798 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test-repos.cfg
+-rw-r--r--   0        0        0     4936 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test.cfg
+-rw-r--r--   0        0        0    14731 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test_config.py
+-rw-r--r--   0        0        0     1849 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test_github.py
+-rw-r--r--   0        0        0     3235 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test_healthcheck.py
+-rw-r--r--   0        0        0     2706 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test_sirmordred.py
+-rw-r--r--   0        0        0     7303 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test_studies.cfg
+-rw-r--r--   0        0        0     5392 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test_task.py
+-rw-r--r--   0        0        0     5956 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test_task_collection.py
+-rw-r--r--   0        0        0    11770 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test_task_enrich.py
+-rw-r--r--   0        0        0     5817 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test_task_identities.py
+-rw-r--r--   0        0        0    10141 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test_task_manager.py
+-rw-r--r--   0        0        0     6380 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test_task_panels.py
+-rw-r--r--   0        0        0    13869 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test_task_projects.py
+-rw-r--r--   0        0        0     1499 2023-07-11 14:54:31.935377 sirmordred-0.9.1rc1/tests/test_wrong.cfg
+-rw-r--r--   0        0        0    42445 1970-01-01 00:00:00.000000 sirmordred-0.9.1rc1/PKG-INFO
```

### Comparing `sirmordred-0.9.1/LICENSE` & `sirmordred-0.9.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/README.md` & `sirmordred-0.9.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/menu.yaml` & `sirmordred-0.9.1rc1/menu.yaml`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/pyproject.toml` & `sirmordred-0.9.1rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sirmordred"
-version = "0.9.1"
+version = "0.9.1-rc.1"
 description = "Drive GrimoireLab tools to produce a dashboard"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `sirmordred-0.9.1/sirmordred/__init__.py` & `sirmordred-0.9.1rc1/sirmordred/__init__.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/bin/sirmordred.py` & `sirmordred-0.9.1rc1/sirmordred/bin/sirmordred.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/config.py` & `sirmordred-0.9.1rc1/sirmordred/config.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/error.py` & `sirmordred-0.9.1rc1/sirmordred/error.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/github.py` & `sirmordred-0.9.1rc1/sirmordred/github.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/sirmordred.py` & `sirmordred-0.9.1rc1/sirmordred/sirmordred.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/task.py` & `sirmordred-0.9.1rc1/sirmordred/task.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/task_collection.py` & `sirmordred-0.9.1rc1/sirmordred/task_collection.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/task_enrich.py` & `sirmordred-0.9.1rc1/sirmordred/task_enrich.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/task_identities.py` & `sirmordred-0.9.1rc1/sirmordred/task_identities.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/task_manager.py` & `sirmordred-0.9.1rc1/sirmordred/task_manager.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/task_panels.py` & `sirmordred-0.9.1rc1/sirmordred/task_panels.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/task_projects.py` & `sirmordred-0.9.1rc1/sirmordred/task_projects.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/utils/find_affiliation_conflicts.py` & `sirmordred-0.9.1rc1/sirmordred/utils/find_affiliation_conflicts.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/utils/grimoirelab_valid.yml` & `sirmordred-0.9.1rc1/sirmordred/utils/grimoirelab_valid.yml`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/utils/healthcheck.py` & `sirmordred-0.9.1rc1/sirmordred/utils/healthcheck.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/utils/micro.py` & `sirmordred-0.9.1rc1/sirmordred/utils/micro.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/utils/panels_config.py` & `sirmordred-0.9.1rc1/sirmordred/utils/panels_config.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/utils/projects.json` & `sirmordred-0.9.1rc1/sirmordred/utils/projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/utils/projects_json2yml.py` & `sirmordred-0.9.1rc1/sirmordred/utils/projects_json2yml.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/sirmordred/utils/setup.cfg` & `sirmordred-0.9.1rc1/sirmordred/utils/setup.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/aliases.json` & `sirmordred-0.9.1rc1/tests/aliases.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/askbot.archive` & `sirmordred-0.9.1rc1/tests/archives/askbot.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/bugzilla.archive` & `sirmordred-0.9.1rc1/tests/archives/bugzilla.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/bugzillarest.archive` & `sirmordred-0.9.1rc1/tests/archives/bugzillarest.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/confluence.archive` & `sirmordred-0.9.1rc1/tests/archives/confluence.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/crates.archive` & `sirmordred-0.9.1rc1/tests/archives/crates.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/discourse.archive` & `sirmordred-0.9.1rc1/tests/archives/discourse.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/dockerhub.archive` & `sirmordred-0.9.1rc1/tests/archives/dockerhub.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/functest.archive` & `sirmordred-0.9.1rc1/tests/archives/functest.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/gerrit.archive` & `sirmordred-0.9.1rc1/tests/archives/gerrit.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/github-issue.archive` & `sirmordred-0.9.1rc1/tests/archives/github-issue.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/github-pull.archive` & `sirmordred-0.9.1rc1/tests/archives/github-pull.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/gitlab-issue.archive` & `sirmordred-0.9.1rc1/tests/archives/gitlab-issue.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/gitlab-merge.archive` & `sirmordred-0.9.1rc1/tests/archives/gitlab-merge.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/googlehits.archive` & `sirmordred-0.9.1rc1/tests/archives/googlehits.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/jenkins.archive` & `sirmordred-0.9.1rc1/tests/archives/jenkins.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/jira.archive` & `sirmordred-0.9.1rc1/tests/archives/jira.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/launchpad.archive` & `sirmordred-0.9.1rc1/tests/archives/launchpad.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/mediawiki-1.23.archive` & `sirmordred-0.9.1rc1/tests/archives/mediawiki-1.23.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/mediawiki-1.28.archive` & `sirmordred-0.9.1rc1/tests/archives/mediawiki-1.28.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/meetup.archive` & `sirmordred-0.9.1rc1/tests/archives/meetup.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/mozillaclub.archive` & `sirmordred-0.9.1rc1/tests/archives/mozillaclub.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/nntp.archive` & `sirmordred-0.9.1rc1/tests/archives/nntp.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/phabricator.archive` & `sirmordred-0.9.1rc1/tests/archives/phabricator.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/redmine.archive` & `sirmordred-0.9.1rc1/tests/archives/redmine.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/remo.archive` & `sirmordred-0.9.1rc1/tests/archives/remo.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/rss.archive` & `sirmordred-0.9.1rc1/tests/archives/rss.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/slack.archive` & `sirmordred-0.9.1rc1/tests/archives/slack.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/stackexchange.archive` & `sirmordred-0.9.1rc1/tests/archives/stackexchange.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/telegram.archive` & `sirmordred-0.9.1rc1/tests/archives/telegram.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives/twitter.archive` & `sirmordred-0.9.1rc1/tests/archives/twitter.archive`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives-test-projects.json` & `sirmordred-0.9.1rc1/tests/archives-test-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/archives-test.cfg` & `sirmordred-0.9.1rc1/tests/archives-test.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/data/eclipse-projects.json` & `sirmordred-0.9.1rc1/tests/data/eclipse-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/data/mordred.log` & `sirmordred-0.9.1rc1/tests/data/mordred.log`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/data/orgs_sortinghat.json` & `sirmordred-0.9.1rc1/tests/data/orgs_sortinghat.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/data/perceval_identities_sortinghat.json` & `sirmordred-0.9.1rc1/tests/data/perceval_identities_sortinghat.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/data/remote_identities_sortinghat.json` & `sirmordred-0.9.1rc1/tests/data/remote_identities_sortinghat.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/data/task-identities-data.json` & `sirmordred-0.9.1rc1/tests/data/task-identities-data.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/data/task-params-expected` & `sirmordred-0.9.1rc1/tests/data/task-params-expected`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/data/task-params-test-projects.json` & `sirmordred-0.9.1rc1/tests/data/task-params-test-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/data/task-params-test.cfg` & `sirmordred-0.9.1rc1/tests/data/task-params-test.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/data/url-projects.json` & `sirmordred-0.9.1rc1/tests/data/url-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/run_tests.py` & `sirmordred-0.9.1rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/sortinghat_settings.py` & `sirmordred-0.9.1rc1/tests/sortinghat_settings.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test-no-collection.cfg` & `sirmordred-0.9.1rc1/tests/test-no-collection.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test-no-sh.cfg` & `sirmordred-0.9.1rc1/tests/test-no-sh.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test-projects.json` & `sirmordred-0.9.1rc1/tests/test-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test-repos-projects.json` & `sirmordred-0.9.1rc1/tests/test-repos-projects.json`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test-repos.cfg` & `sirmordred-0.9.1rc1/tests/test-repos.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test.cfg` & `sirmordred-0.9.1rc1/tests/test.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test_config.py` & `sirmordred-0.9.1rc1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test_github.py` & `sirmordred-0.9.1rc1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test_healthcheck.py` & `sirmordred-0.9.1rc1/tests/test_healthcheck.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test_sirmordred.py` & `sirmordred-0.9.1rc1/tests/test_sirmordred.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test_studies.cfg` & `sirmordred-0.9.1rc1/tests/test_studies.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test_task.py` & `sirmordred-0.9.1rc1/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test_task_collection.py` & `sirmordred-0.9.1rc1/tests/test_task_collection.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test_task_enrich.py` & `sirmordred-0.9.1rc1/tests/test_task_enrich.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test_task_identities.py` & `sirmordred-0.9.1rc1/tests/test_task_identities.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test_task_manager.py` & `sirmordred-0.9.1rc1/tests/test_task_manager.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test_task_panels.py` & `sirmordred-0.9.1rc1/tests/test_task_panels.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test_task_projects.py` & `sirmordred-0.9.1rc1/tests/test_task_projects.py`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/tests/test_wrong.cfg` & `sirmordred-0.9.1rc1/tests/test_wrong.cfg`

 * *Files identical despite different names*

### Comparing `sirmordred-0.9.1/PKG-INFO` & `sirmordred-0.9.1rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirmordred
-Version: 0.9.1
+Version: 0.9.1rc1
 Summary: Drive GrimoireLab tools to produce a dashboard
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
```

