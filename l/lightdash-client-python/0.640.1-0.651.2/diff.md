# Comparing `tmp/lightdash_client_python-0.640.1.tar.gz` & `tmp/lightdash_client_python-0.651.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightdash_client_python-0.640.1.tar", last modified: Thu Jul  6 00:20:34 2023, max compression
+gzip compressed data, was "lightdash_client_python-0.651.2.tar", last modified: Tue Jul 11 01:36:57 2023, max compression
```

## Comparing `lightdash_client_python-0.640.1.tar` & `lightdash_client_python-0.651.2.tar`

### file list

```diff
@@ -1,1199 +1,1199 @@
--rw-r--r--   0        0        0     1040 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/.openapi-generator-ignore
--rw-r--r--   0        0        0        8 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/.python-version
--rw-r--r--   0        0        0    11357 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/LICENSE
--rw-r--r--   0        0        0     3258 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/README.md
--rw-r--r--   0        0        0      182 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/__init__.py
--rw-r--r--   0        0        0       47 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/__init__.py
--rw-r--r--   0        0        0        0 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/charts/__init__.py
--rw-r--r--   0        0        0     4749 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/charts/post_chart_results.py
--rw-r--r--   0        0        0        0 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/content/__init__.py
--rw-r--r--   0        0        0     4592 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/content/get_pinned_items.py
--rw-r--r--   0        0        0     5871 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/content/update_pinned_items_order.py
--rw-r--r--   0        0        0        0 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/exploring/__init__.py
--rw-r--r--   0        0        0     5223 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/exploring/post_run_query.py
--rw-r--r--   0        0        0     5659 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/exploring/post_run_underlying_data_query.py
--rw-r--r--   0        0        0        0 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/exports/__init__.py
--rw-r--r--   0        0        0     3852 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/exports/get_csv_url.py
--rw-r--r--   0        0        0        0 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/integrations/__init__.py
--rw-r--r--   0        0        0     4545 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0     4511 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0     4956 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/integrations/get_dbt_cloud_metrics.py
--rw-r--r--   0        0        0     3655 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/integrations/get_slack_channels.py
--rw-r--r--   0        0        0     4543 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0        0 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/my_account/__init__.py
--rw-r--r--   0        0        0     4215 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/my_account/create_email_one_time_passcode.py
--rw-r--r--   0        0        0     3518 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/my_account/delete_me.py
--rw-r--r--   0        0        0     4750 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/my_account/get_email_verification_status.py
--rw-r--r--   0        0        0     4914 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/my_account/join_organization.py
--rw-r--r--   0        0        0     4375 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/my_account/list_my_available_organizations.py
--rw-r--r--   0        0        0        0 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/organizations/__init__.py
--rw-r--r--   0        0        0     4823 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/organizations/create_group_in_organization.py
--rw-r--r--   0        0        0     5097 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/organizations/create_organization.py
--rw-r--r--   0        0        0     4439 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/organizations/delete_my_organization.py
--rw-r--r--   0        0        0     4292 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/organizations/delete_organization_member.py
--rw-r--r--   0        0        0     3725 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/organizations/get_my_organization.py
--rw-r--r--   0        0        0     3909 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/organizations/list_groups_in_organization.py
--rw-r--r--   0        0        0     4022 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/organizations/list_organization_email_domains.py
--rw-r--r--   0        0        0     3898 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/organizations/list_organization_members.py
--rw-r--r--   0        0        0     3902 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/organizations/list_organization_projects.py
--rw-r--r--   0        0        0     4654 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/organizations/update_my_organization.py
--rw-r--r--   0        0        0     5049 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/organizations/update_organization_email_domains.py
--rw-r--r--   0        0        0        0 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/projects/__init__.py
--rw-r--r--   0        0        0     4743 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/projects/delete_validation_dismiss.py
--rw-r--r--   0        0        0     5908 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/projects/get_latest_validation_results.py
--rw-r--r--   0        0        0     4077 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/projects/get_project.py
--rw-r--r--   0        0        0     4191 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/projects/list_charts_in_project.py
--rw-r--r--   0        0        0     4191 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/projects/list_spaces_in_project.py
--rw-r--r--   0        0        0     6431 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/projects/validate_project.py
--rw-r--r--   0        0        0        0 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/__init__.py
--rw-r--r--   0        0        0     5295 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/add_space_share_to_user.py
--rw-r--r--   0        0        0     4946 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/create_space_in_project.py
--rw-r--r--   0        0        0     4941 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/get_project_access_list.py
--rw-r--r--   0        0        0     5041 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/grant_project_access_to_user.py
--rw-r--r--   0        0        0     4688 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py
--rw-r--r--   0        0        0     5031 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py
--rw-r--r--   0        0        0     5256 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/update_organization_member.py
--rw-r--r--   0        0        0     5467 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/update_project_access_for_user.py
--rw-r--r--   0        0        0     5071 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/update_space.py
--rw-r--r--   0        0        0        0 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/schedulers/__init__.py
--rw-r--r--   0        0        0     4140 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/schedulers/delete_scheduler.py
--rw-r--r--   0        0        0     4151 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/schedulers/get_scheduled_jobs.py
--rw-r--r--   0        0        0     4081 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/schedulers/get_scheduler.py
--rw-r--r--   0        0        0     4332 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/schedulers/get_scheduler_job_status.py
--rw-r--r--   0        0        0     4111 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/schedulers/get_scheduler_logs.py
--rw-r--r--   0        0        0     4615 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/schedulers/update_scheduler.py
--rw-r--r--   0        0        0        0 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/share_links/__init__.py
--rw-r--r--   0        0        0     4687 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/share_links/create_share_url.py
--rw-r--r--   0        0        0     4004 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/share_links/get_share_url.py
--rw-r--r--   0        0        0        0 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/spaces/__init__.py
--rw-r--r--   0        0        0     4485 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/spaces/delete_space.py
--rw-r--r--   0        0        0     4463 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/spaces/get_space.py
--rw-r--r--   0        0        0        0 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/ssh_keypairs/__init__.py
--rw-r--r--   0        0        0     3585 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py
--rw-r--r--   0        0        0        0 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/user_groups/__init__.py
--rw-r--r--   0        0        0     4462 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/user_groups/add_user_to_group.py
--rw-r--r--   0        0        0     3983 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/user_groups/delete_group.py
--rw-r--r--   0        0        0     3953 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/user_groups/get_group.py
--rw-r--r--   0        0        0     4077 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/user_groups/get_group_members.py
--rw-r--r--   0        0        0     4510 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/user_groups/remove_user_from_group.py
--rw-r--r--   0        0        0     4885 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/api/user_groups/update_group.py
--rw-r--r--   0        0        0     2888 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/client.py
--rw-r--r--   0        0        0      470 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/errors.py
--rw-r--r--   0        0        0   177549 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/__init__.py
--rw-r--r--   0        0        0     1415 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/add_space_share.py
--rw-r--r--   0        0        0     1497 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/add_space_share_to_user_json_body.py
--rw-r--r--   0        0        0     2003 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/add_space_share_to_user_response_200.py
--rw-r--r--   0        0        0      155 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/add_space_share_to_user_response_200_status.py
--rw-r--r--   0        0        0     1949 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/add_user_to_group_response_200.py
--rw-r--r--   0        0        0      150 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/add_user_to_group_response_200_status.py
--rw-r--r--   0        0        0     6478 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/additional_metric.py
--rw-r--r--   0        0        0      241 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/additional_metric_compact_type_0.py
--rw-r--r--   0        0        0      281 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/additional_metric_compact_type_1.py
--rw-r--r--   0        0        0     2365 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/additional_metric_filters_item.py
--rw-r--r--   0        0        0      616 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/additional_metric_filters_item_operator.py
--rw-r--r--   0        0        0     1521 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/additional_metric_filters_item_target.py
--rw-r--r--   0        0        0      393 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/additional_metric_type.py
--rw-r--r--   0        0        0      162 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/allowed_email_domain_projects_role_type_0.py
--rw-r--r--   0        0        0      186 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/allowed_email_domain_projects_role_type_1.py
--rw-r--r--   0        0        0      162 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/allowed_email_domain_projects_role_type_2.py
--rw-r--r--   0        0        0     4988 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/allowed_email_domains.py
--rw-r--r--   0        0        0     3595 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/allowed_email_domains_projects_item.py
--rw-r--r--   0        0        0      167 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/allowed_email_domains_projects_item_role_type_0.py
--rw-r--r--   0        0        0      191 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/allowed_email_domains_projects_item_role_type_1.py
--rw-r--r--   0        0        0      167 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/allowed_email_domains_projects_item_role_type_2.py
--rw-r--r--   0        0        0      155 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/allowed_email_domains_role_type_0.py
--rw-r--r--   0        0        0      179 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/allowed_email_domains_role_type_1.py
--rw-r--r--   0        0        0      155 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/allowed_email_domains_role_type_2.py
--rw-r--r--   0        0        0      155 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/allowed_email_domains_role_type_3.py
--rw-r--r--   0        0        0     2563 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_chart_summary_list_response.py
--rw-r--r--   0        0        0     4038 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_chart_summary_list_response_results_item.py
--rw-r--r--   0        0        0      246 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_chart_summary_list_response_results_item_chart_type.py
--rw-r--r--   0        0        0      152 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_chart_summary_list_response_status.py
--rw-r--r--   0        0        0     2016 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_csv_url_response.py
--rw-r--r--   0        0        0     1580 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_csv_url_response_results.py
--rw-r--r--   0        0        0      142 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_csv_url_response_status.py
--rw-r--r--   0        0        0     2776 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_dbt_cloud_integration_settings.py
--rw-r--r--   0        0        0     1737 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_dbt_cloud_integration_settings_results.py
--rw-r--r--   0        0        0      155 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_dbt_cloud_integration_settings_status.py
--rw-r--r--   0        0        0     2122 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_dbt_cloud_metrics.py
--rw-r--r--   0        0        0     2325 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_dbt_cloud_metrics_results.py
--rw-r--r--   0        0        0     2526 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_dbt_cloud_metrics_results_metrics_item.py
--rw-r--r--   0        0        0      143 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_dbt_cloud_metrics_status.py
--rw-r--r--   0        0        0     2019 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_dbt_cloud_settings_delete_success.py
--rw-r--r--   0        0        0      157 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_dbt_cloud_settings_delete_success_status.py
--rw-r--r--   0        0        0     2224 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_email_status_response.py
--rw-r--r--   0        0        0     2709 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_email_status_response_results.py
--rw-r--r--   0        0        0     2813 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_email_status_response_results_otp.py
--rw-r--r--   0        0        0      147 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_email_status_response_status.py
--rw-r--r--   0        0        0     2049 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_error_payload.py
--rw-r--r--   0        0        0     2277 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_error_payload_error.py
--rw-r--r--   0        0        0      146 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_error_payload_status.py
--rw-r--r--   0        0        0     2429 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_group_list_response.py
--rw-r--r--   0        0        0     2320 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_group_list_response_results_item.py
--rw-r--r--   0        0        0      145 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_group_list_response_status.py
--rw-r--r--   0        0        0     2480 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_group_members_response.py
--rw-r--r--   0        0        0     2218 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_group_members_response_results_item.py
--rw-r--r--   0        0        0      148 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_group_members_response_status.py
--rw-r--r--   0        0        0     1993 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_group_response.py
--rw-r--r--   0        0        0     2274 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_group_response_results.py
--rw-r--r--   0        0        0      141 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_group_response_status.py
--rw-r--r--   0        0        0     2160 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_job_scheduled_response.py
--rw-r--r--   0        0        0     1476 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_job_scheduled_response_results.py
--rw-r--r--   0        0        0      148 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_job_scheduled_response_status.py
--rw-r--r--   0        0        0     2067 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_job_status_response.py
--rw-r--r--   0        0        0     1463 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_job_status_response_results.py
--rw-r--r--   0        0        0      145 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_job_status_response_status.py
--rw-r--r--   0        0        0     2003 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization.py
--rw-r--r--   0        0        0     2362 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_allowed_email_domains.py
--rw-r--r--   0        0        0     5921 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_allowed_email_domains_results.py
--rw-r--r--   0        0        0     4175 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item.py
--rw-r--r--   0        0        0      189 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item_role_type_0.py
--rw-r--r--   0        0        0      213 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item_role_type_1.py
--rw-r--r--   0        0        0      189 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item_role_type_2.py
--rw-r--r--   0        0        0      177 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_allowed_email_domains_results_role_type_0.py
--rw-r--r--   0        0        0      201 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_allowed_email_domains_results_role_type_1.py
--rw-r--r--   0        0        0      177 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_allowed_email_domains_results_role_type_2.py
--rw-r--r--   0        0        0      177 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_allowed_email_domains_results_role_type_3.py
--rw-r--r--   0        0        0      159 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_allowed_email_domains_status.py
--rw-r--r--   0        0        0     2305 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_member_profile.py
--rw-r--r--   0        0        0     3624 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_member_profile_results.py
--rw-r--r--   0        0        0      304 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_member_profile_results_role.py
--rw-r--r--   0        0        0      153 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_member_profile_status.py
--rw-r--r--   0        0        0     2591 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_member_profiles.py
--rw-r--r--   0        0        0     3678 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_member_profiles_results_item.py
--rw-r--r--   0        0        0      309 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_member_profiles_results_item_role.py
--rw-r--r--   0        0        0      154 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_member_profiles_status.py
--rw-r--r--   0        0        0     2519 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_projects.py
--rw-r--r--   0        0        0     2151 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_projects_results_item.py
--rw-r--r--   0        0        0      191 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_projects_results_item_type.py
--rw-r--r--   0        0        0      148 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_projects_status.py
--rw-r--r--   0        0        0     3203 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_results.py
--rw-r--r--   0        0        0      140 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_organization_status.py
--rw-r--r--   0        0        0     4640 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items.py
--rw-r--r--   0        0        0     2288 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_0.py
--rw-r--r--   0        0        0     7025 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_0_data.py
--rw-r--r--   0        0        0     1271 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_0_data_updated_by_user.py
--rw-r--r--   0        0        0     2207 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_0_data_validation_errors_item.py
--rw-r--r--   0        0        0      167 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_0_type.py
--rw-r--r--   0        0        0     2288 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_1.py
--rw-r--r--   0        0        0     7876 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_1_data.py
--rw-r--r--   0        0        0      366 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_1_data_chart_type.py
--rw-r--r--   0        0        0     1271 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_1_data_updated_by_user.py
--rw-r--r--   0        0        0     2207 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_1_data_validation_errors_item.py
--rw-r--r--   0        0        0      159 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_1_type.py
--rw-r--r--   0        0        0     2225 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_2.py
--rw-r--r--   0        0        0     3849 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_2_data.py
--rw-r--r--   0        0        0      159 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_2_type.py
--rw-r--r--   0        0        0      139 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_status.py
--rw-r--r--   0        0        0     2580 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_access_list_response.py
--rw-r--r--   0        0        0     2719 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_access_list_response_results_item.py
--rw-r--r--   0        0        0      286 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_access_list_response_results_item_role.py
--rw-r--r--   0        0        0      153 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_access_list_response_status.py
--rw-r--r--   0        0        0     2027 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response.py
--rw-r--r--   0        0        0    20745 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results.py
--rw-r--r--   0        0        0     3377 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_0.py
--rw-r--r--   0        0        0     1755 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_0_environment_item.py
--rw-r--r--   0        0        0      168 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_0_type.py
--rw-r--r--   0        0        0     2541 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_1.py
--rw-r--r--   0        0        0      188 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_1_type.py
--rw-r--r--   0        0        0     4004 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_2.py
--rw-r--r--   0        0        0     1755 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_2_environment_item.py
--rw-r--r--   0        0        0      174 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_2_type.py
--rw-r--r--   0        0        0     4186 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_3.py
--rw-r--r--   0        0        0     1755 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_3_environment_item.py
--rw-r--r--   0        0        0      180 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_3_type.py
--rw-r--r--   0        0        0     4004 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_4.py
--rw-r--r--   0        0        0     1755 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_4_environment_item.py
--rw-r--r--   0        0        0      174 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_4_type.py
--rw-r--r--   0        0        0     4097 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_5.py
--rw-r--r--   0        0        0     1755 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_5_environment_item.py
--rw-r--r--   0        0        0      186 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_5_type.py
--rw-r--r--   0        0        0     3152 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_6.py
--rw-r--r--   0        0        0     1755 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_6_environment_item.py
--rw-r--r--   0        0        0      170 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_6_type.py
--rw-r--r--   0        0        0      182 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_type.py
--rw-r--r--   0        0        0     5577 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_0.py
--rw-r--r--   0        0        0     1419 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_0_start_of_week.py
--rw-r--r--   0        0        0      186 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_0_type.py
--rw-r--r--   0        0        0     6883 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_1.py
--rw-r--r--   0        0        0     1419 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_1_start_of_week.py
--rw-r--r--   0        0        0      184 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_1_type.py
--rw-r--r--   0        0        0     7128 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_2.py
--rw-r--r--   0        0        0     1419 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_2_start_of_week.py
--rw-r--r--   0        0        0      184 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_2_type.py
--rw-r--r--   0        0        0     6150 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_3.py
--rw-r--r--   0        0        0      214 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_priority.py
--rw-r--r--   0        0        0     1419 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_start_of_week.py
--rw-r--r--   0        0        0      184 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_type.py
--rw-r--r--   0        0        0     4260 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_4.py
--rw-r--r--   0        0        0     1419 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_4_start_of_week.py
--rw-r--r--   0        0        0      188 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_4_type.py
--rw-r--r--   0        0        0     4197 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_5.py
--rw-r--r--   0        0        0     1419 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_5_start_of_week.py
--rw-r--r--   0        0        0      178 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_5_type.py
--rw-r--r--   0        0        0      143 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_status.py
--rw-r--r--   0        0        0     2050 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response.py
--rw-r--r--   0        0        0     2119 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results.py
--rw-r--r--   0        0        0     6314 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query.py
--rw-r--r--   0        0        0     8094 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item.py
--rw-r--r--   0        0        0      283 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_compact_type_0.py
--rw-r--r--   0        0        0      323 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_compact_type_1.py
--rw-r--r--   0        0        0     3077 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item.py
--rw-r--r--   0        0        0      658 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item_operator.py
--rw-r--r--   0        0        0     1779 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item_target.py
--rw-r--r--   0        0        0      435 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_type.py
--rw-r--r--   0        0        0     8170 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_filters.py
--rw-r--r--   0        0        0     1767 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_0.py
--rw-r--r--   0        0        0     1777 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_1.py
--rw-r--r--   0        0        0     1752 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_0.py
--rw-r--r--   0        0        0     1762 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_1.py
--rw-r--r--   0        0        0     1792 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_sorts_item.py
--rw-r--r--   0        0        0     3437 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item.py
--rw-r--r--   0        0        0     5063 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format.py
--rw-r--r--   0        0        0      284 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format_compact.py
--rw-r--r--   0        0        0      342 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format_separator.py
--rw-r--r--   0        0        0      269 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format_type.py
--rw-r--r--   0        0        0      144 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_status.py
--rw-r--r--   0        0        0     2497 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduled_jobs_response.py
--rw-r--r--   0        0        0     1711 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduled_jobs_response_results_item.py
--rw-r--r--   0        0        0      149 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduled_jobs_response_status.py
--rw-r--r--   0        0        0     2294 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_and_targets_response.py
--rw-r--r--   0        0        0     4066 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_and_targets_response_results.py
--rw-r--r--   0        0        0     2779 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_0.py
--rw-r--r--   0        0        0     2799 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_1.py
--rw-r--r--   0        0        0      155 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_and_targets_response_status.py
--rw-r--r--   0        0        0     2177 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response.py
--rw-r--r--   0        0        0     5791 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results.py
--rw-r--r--   0        0        0     1777 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_charts_item.py
--rw-r--r--   0        0        0     1779 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_dashboards_item.py
--rw-r--r--   0        0        0     5858 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_logs_item.py
--rw-r--r--   0        0        0     1392 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_logs_item_details.py
--rw-r--r--   0        0        0      250 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_logs_item_status.py
--rw-r--r--   0        0        0      194 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_logs_item_target_type.py
--rw-r--r--   0        0        0      470 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_logs_item_task.py
--rw-r--r--   0        0        0     4266 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item.py
--rw-r--r--   0        0        0     2822 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_0.py
--rw-r--r--   0        0        0     2842 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_1.py
--rw-r--r--   0        0        0     1952 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_users_item.py
--rw-r--r--   0        0        0      149 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_status.py
--rw-r--r--   0        0        0     2148 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_share_response.py
--rw-r--r--   0        0        0     3477 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_share_response_results.py
--rw-r--r--   0        0        0      141 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_share_response_status.py
--rw-r--r--   0        0        0     2497 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_slack_channels_response.py
--rw-r--r--   0        0        0     1608 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_slack_channels_response_results_item.py
--rw-r--r--   0        0        0      149 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_slack_channels_response_status.py
--rw-r--r--   0        0        0     1993 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_space_response.py
--rw-r--r--   0        0        0     5415 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results.py
--rw-r--r--   0        0        0     2283 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results_access_item.py
--rw-r--r--   0        0        0      280 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results_access_item_role.py
--rw-r--r--   0        0        0     7498 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results_dashboards_item.py
--rw-r--r--   0        0        0     1279 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results_dashboards_item_updated_by_user.py
--rw-r--r--   0        0        0     2216 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results_dashboards_item_validation_errors_item.py
--rw-r--r--   0        0        0     7797 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results_queries_item.py
--rw-r--r--   0        0        0      366 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results_queries_item_chart_type.py
--rw-r--r--   0        0        0     1267 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results_queries_item_updated_by_user.py
--rw-r--r--   0        0        0     2201 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results_queries_item_validation_errors_item.py
--rw-r--r--   0        0        0      141 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_status.py
--rw-r--r--   0        0        0     2563 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_space_summary_list_response.py
--rw-r--r--   0        0        0     2535 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_space_summary_list_response_results_item.py
--rw-r--r--   0        0        0      152 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_space_summary_list_response_status.py
--rw-r--r--   0        0        0     2178 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_ssh_key_pair_response.py
--rw-r--r--   0        0        0     1572 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_ssh_key_pair_response_results.py
--rw-r--r--   0        0        0      146 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_ssh_key_pair_response_status.py
--rw-r--r--   0        0        0     1828 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_success_empty.py
--rw-r--r--   0        0        0      140 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_success_empty_status.py
--rw-r--r--   0        0        0     2699 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_user_allowed_organizations_response.py
--rw-r--r--   0        0        0     2048 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_user_allowed_organizations_response_results_item.py
--rw-r--r--   0        0        0      160 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_user_allowed_organizations_response_status.py
--rw-r--r--   0        0        0     4920 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_validate_response.py
--rw-r--r--   0        0        0     6933 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_validate_response_results_item_type_0.py
--rw-r--r--   0        0        0      367 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_validate_response_results_item_type_0_chart_type.py
--rw-r--r--   0        0        0      285 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_validate_response_results_item_type_0_error_type.py
--rw-r--r--   0        0        0      214 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_validate_response_results_item_type_0_source.py
--rw-r--r--   0        0        0     6161 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_validate_response_results_item_type_1.py
--rw-r--r--   0        0        0      285 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_validate_response_results_item_type_1_error_type.py
--rw-r--r--   0        0        0      214 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_validate_response_results_item_type_1_source.py
--rw-r--r--   0        0        0     4038 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_validate_response_results_item_type_2.py
--rw-r--r--   0        0        0      285 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_validate_response_results_item_type_2_error_type.py
--rw-r--r--   0        0        0      214 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_validate_response_results_item_type_2_source.py
--rw-r--r--   0        0        0      144 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_validate_response_status.py
--rw-r--r--   0        0        0     1674 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_validation_dismiss_response.py
--rw-r--r--   0        0        0      153 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/api_validation_dismiss_response_status.py
--rw-r--r--   0        0        0     5370 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/bigquery_credentials.py
--rw-r--r--   0        0        0      184 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/bigquery_credentials_priority.py
--rw-r--r--   0        0        0     1251 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/bigquery_credentials_start_of_week.py
--rw-r--r--   0        0        0      154 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/bigquery_credentials_type.py
--rw-r--r--   0        0        0      332 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/chart_kind.py
--rw-r--r--   0        0        0     4853 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/chart_scheduler.py
--rw-r--r--   0        0        0      161 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/chart_scheduler_format.py
--rw-r--r--   0        0        0     2484 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/chart_scheduler_options_type_0.py
--rw-r--r--   0        0        0      177 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/chart_scheduler_options_type_0_limit_type_1.py
--rw-r--r--   0        0        0     1231 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/chart_scheduler_options_type_1.py
--rw-r--r--   0        0        0     3723 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/chart_summary.py
--rw-r--r--   0        0        0      220 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/chart_summary_chart_type.py
--rw-r--r--   0        0        0      208 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/chart_type.py
--rw-r--r--   0        0        0      220 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/compact.py
--rw-r--r--   0        0        0      232 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/compact_or_alias_type_0.py
--rw-r--r--   0        0        0      272 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/compact_or_alias_type_1.py
--rw-r--r--   0        0        0      600 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/conditional_operator.py
--rw-r--r--   0        0        0     2523 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_email_one_time_passcode_response_200.py
--rw-r--r--   0        0        0     2919 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_email_one_time_passcode_response_200_results.py
--rw-r--r--   0        0        0     2897 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_email_one_time_passcode_response_200_results_otp.py
--rw-r--r--   0        0        0      162 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_email_one_time_passcode_response_200_status.py
--rw-r--r--   0        0        0     1528 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_group_in_organization_json_body.py
--rw-r--r--   0        0        0     2402 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_group_in_organization_response_200.py
--rw-r--r--   0        0        0     2383 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_group_in_organization_response_200_results.py
--rw-r--r--   0        0        0      161 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_group_in_organization_response_200_status.py
--rw-r--r--   0        0        0     1481 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_organization.py
--rw-r--r--   0        0        0     1494 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_organization_json_body.py
--rw-r--r--   0        0        0     1981 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_organization_response_200.py
--rw-r--r--   0        0        0      154 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_organization_response_200_status.py
--rw-r--r--   0        0        0     1896 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_project_member.py
--rw-r--r--   0        0        0      266 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_project_member_role.py
--rw-r--r--   0        0        0     1624 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_share_url.py
--rw-r--r--   0        0        0     1652 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_share_url_json_body.py
--rw-r--r--   0        0        0     2364 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_share_url_response_201.py
--rw-r--r--   0        0        0     3528 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_share_url_response_201_results.py
--rw-r--r--   0        0        0      150 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_share_url_response_201_status.py
--rw-r--r--   0        0        0     2601 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space.py
--rw-r--r--   0        0        0     2146 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space_access_item.py
--rw-r--r--   0        0        0      268 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space_access_item_role.py
--rw-r--r--   0        0        0     2867 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_json_body.py
--rw-r--r--   0        0        0     2341 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_json_body_access_item.py
--rw-r--r--   0        0        0      285 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_json_body_access_item_role.py
--rw-r--r--   0        0        0     2317 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200.py
--rw-r--r--   0        0        0     5832 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results.py
--rw-r--r--   0        0        0     2445 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results_access_item.py
--rw-r--r--   0        0        0      295 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results_access_item_role.py
--rw-r--r--   0        0        0     7875 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item.py
--rw-r--r--   0        0        0     1345 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_updated_by_user.py
--rw-r--r--   0        0        0     2300 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_validation_errors_item.py
--rw-r--r--   0        0        0     8225 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results_queries_item.py
--rw-r--r--   0        0        0      381 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results_queries_item_chart_type.py
--rw-r--r--   0        0        0     1333 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results_queries_item_updated_by_user.py
--rw-r--r--   0        0        0     2285 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results_queries_item_validation_errors_item.py
--rw-r--r--   0        0        0      156 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_status.py
--rw-r--r--   0        0        0     2312 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_ssh_key_pair_response_201.py
--rw-r--r--   0        0        0     1605 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_ssh_key_pair_response_201_results.py
--rw-r--r--   0        0        0      152 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/create_ssh_key_pair_response_201_status.py
--rw-r--r--   0        0        0     7127 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dashboard_basic_details.py
--rw-r--r--   0        0        0     1209 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dashboard_basic_details_updated_by_user.py
--rw-r--r--   0        0        0     2127 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dashboard_basic_details_validation_errors_item.py
--rw-r--r--   0        0        0     5078 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dashboard_scheduler.py
--rw-r--r--   0        0        0      165 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dashboard_scheduler_format.py
--rw-r--r--   0        0        0     2536 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dashboard_scheduler_options_type_0.py
--rw-r--r--   0        0        0      181 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dashboard_scheduler_options_type_0_limit_type_1.py
--rw-r--r--   0        0        0     1251 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dashboard_scheduler_options_type_1.py
--rw-r--r--   0        0        0     3711 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/databricks_credentials.py
--rw-r--r--   0        0        0     1261 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/databricks_credentials_start_of_week.py
--rw-r--r--   0        0        0      160 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/databricks_credentials_type.py
--rw-r--r--   0        0        0     3801 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_azure_dev_ops_project_config.py
--rw-r--r--   0        0        0     1669 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_azure_dev_ops_project_config_environment_item.py
--rw-r--r--   0        0        0      170 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_azure_dev_ops_project_config_type.py
--rw-r--r--   0        0        0     3844 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_bit_bucket_project_config.py
--rw-r--r--   0        0        0     1656 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_bit_bucket_project_config_environment_item.py
--rw-r--r--   0        0        0      162 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_bit_bucket_project_config_type.py
--rw-r--r--   0        0        0     2352 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_cloud_ide_project_config.py
--rw-r--r--   0        0        0      169 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_cloud_ide_project_config_type.py
--rw-r--r--   0        0        0     1638 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_cloud_integration.py
--rw-r--r--   0        0        0     2397 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_cloud_metadata_response_metrics.py
--rw-r--r--   0        0        0     2556 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_cloud_metadata_response_metrics_metrics_item.py
--rw-r--r--   0        0        0     2404 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_cloud_metric.py
--rw-r--r--   0        0        0     3609 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_github_project_config.py
--rw-r--r--   0        0        0     1638 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_github_project_config_environment_item.py
--rw-r--r--   0        0        0      153 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_github_project_config_type.py
--rw-r--r--   0        0        0     3609 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_gitlab_project_config.py
--rw-r--r--   0        0        0     1638 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_gitlab_project_config_environment_item.py
--rw-r--r--   0        0        0      153 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_gitlab_project_config_type.py
--rw-r--r--   0        0        0     2966 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_local_project_config.py
--rw-r--r--   0        0        0     1633 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_local_project_config_environment_item.py
--rw-r--r--   0        0        0      146 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_local_project_config_type.py
--rw-r--r--   0        0        0     2725 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_none_project_config.py
--rw-r--r--   0        0        0     1628 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_none_project_config_environment_item.py
--rw-r--r--   0        0        0      147 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_none_project_config_type.py
--rw-r--r--   0        0        0     1636 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_0_environment_item.py
--rw-r--r--   0        0        0      146 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_0_type.py
--rw-r--r--   0        0        0     2325 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_1.py
--rw-r--r--   0        0        0      166 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_1_type.py
--rw-r--r--   0        0        0     1636 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_2_environment_item.py
--rw-r--r--   0        0        0      152 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_2_type.py
--rw-r--r--   0        0        0     1636 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_3_environment_item.py
--rw-r--r--   0        0        0      158 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_3_type.py
--rw-r--r--   0        0        0     1636 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_4_environment_item.py
--rw-r--r--   0        0        0      152 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_4_type.py
--rw-r--r--   0        0        0     1636 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_5_environment_item.py
--rw-r--r--   0        0        0      164 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_5_type.py
--rw-r--r--   0        0        0     1636 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_6_environment_item.py
--rw-r--r--   0        0        0      148 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_6_type.py
--rw-r--r--   0        0        0     1592 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_environment_variable.py
--rw-r--r--   0        0        0      295 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_type.py
--rw-r--r--   0        0        0      164 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_type_azuredevops.py
--rw-r--r--   0        0        0      156 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_type_bitbucket.py
--rw-r--r--   0        0        0      138 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_type_dbt.py
--rw-r--r--   0        0        0      166 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_type_dbtcloudide.py
--rw-r--r--   0        0        0      147 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_type_github.py
--rw-r--r--   0        0        0      147 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_type_gitlab.py
--rw-r--r--   0        0        0      141 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_type_none.py
--rw-r--r--   0        0        0     2143 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/delete_dbt_cloud_integration_settings_response_200.py
--rw-r--r--   0        0        0      169 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/delete_dbt_cloud_integration_settings_response_200_status.py
--rw-r--r--   0        0        0     1902 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/delete_group_response_200.py
--rw-r--r--   0        0        0      147 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/delete_group_response_200_status.py
--rw-r--r--   0        0        0     1872 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/delete_me_response_200.py
--rw-r--r--   0        0        0      144 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/delete_me_response_200_status.py
--rw-r--r--   0        0        0     2005 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/delete_my_organization_response_200.py
--rw-r--r--   0        0        0      156 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/delete_my_organization_response_200_status.py
--rw-r--r--   0        0        0     2045 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/delete_organization_member_response_200.py
--rw-r--r--   0        0        0      160 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/delete_organization_member_response_200_status.py
--rw-r--r--   0        0        0     1951 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/delete_scheduler_response_201.py
--rw-r--r--   0        0        0      151 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/delete_scheduler_response_201_status.py
--rw-r--r--   0        0        0     1902 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/delete_space_response_204.py
--rw-r--r--   0        0        0      147 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/delete_space_response_204_status.py
--rw-r--r--   0        0        0     1738 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/delete_validation_dismiss_response_200.py
--rw-r--r--   0        0        0      159 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/delete_validation_dismiss_response_200_status.py
--rw-r--r--   0        0        0     1931 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/email_one_time_password.py
--rw-r--r--   0        0        0     2677 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/email_one_time_password_expiring.py
--rw-r--r--   0        0        0     2281 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/email_status.py
--rw-r--r--   0        0        0     2527 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/email_status_expiring.py
--rw-r--r--   0        0        0     2757 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/email_status_expiring_otp.py
--rw-r--r--   0        0        0     1898 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/email_status_otp.py
--rw-r--r--   0        0        0     1574 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/filter_group_response_type_0.py
--rw-r--r--   0        0        0     1584 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/filter_group_response_type_1.py
--rw-r--r--   0        0        0     5812 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/filters.py
--rw-r--r--   0        0        0     1561 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/filters_dimensions_type_0.py
--rw-r--r--   0        0        0     1571 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/filters_dimensions_type_1.py
--rw-r--r--   0        0        0     1546 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/filters_metrics_type_0.py
--rw-r--r--   0        0        0     1556 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/filters_metrics_type_1.py
--rw-r--r--   0        0        0     2098 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_csv_url_response_200.py
--rw-r--r--   0        0        0     1598 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_csv_url_response_200_results.py
--rw-r--r--   0        0        0      145 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_csv_url_response_200_status.py
--rw-r--r--   0        0        0     2986 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_dbt_cloud_integration_settings_response_200.py
--rw-r--r--   0        0        0     1798 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_dbt_cloud_integration_settings_response_200_results.py
--rw-r--r--   0        0        0      166 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_dbt_cloud_integration_settings_response_200_status.py
--rw-r--r--   0        0        0     2372 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_dbt_cloud_metrics_response_200.py
--rw-r--r--   0        0        0     2467 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_dbt_cloud_metrics_response_200_results.py
--rw-r--r--   0        0        0     2587 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_dbt_cloud_metrics_response_200_results_metrics_item.py
--rw-r--r--   0        0        0      154 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_dbt_cloud_metrics_response_200_status.py
--rw-r--r--   0        0        0     2517 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_email_verification_status_response_200.py
--rw-r--r--   0        0        0     2914 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_email_verification_status_response_200_results.py
--rw-r--r--   0        0        0     2894 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_email_verification_status_response_200_results_otp.py
--rw-r--r--   0        0        0      162 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_email_verification_status_response_200_status.py
--rw-r--r--   0        0        0     2546 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_group_members_response_200.py
--rw-r--r--   0        0        0     2236 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_group_members_response_200_results_item.py
--rw-r--r--   0        0        0      151 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_group_members_response_200_status.py
--rw-r--r--   0        0        0     2050 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_group_response_200.py
--rw-r--r--   0        0        0     2292 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_group_response_200_results.py
--rw-r--r--   0        0        0      144 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_group_response_200_status.py
--rw-r--r--   0        0        0     5697 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_latest_validation_results_response_200.py
--rw-r--r--   0        0        0     7347 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0.py
--rw-r--r--   0        0        0      385 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0_chart_type.py
--rw-r--r--   0        0        0      303 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0_error_type.py
--rw-r--r--   0        0        0      232 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0_source.py
--rw-r--r--   0        0        0     6464 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1.py
--rw-r--r--   0        0        0      303 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1_error_type.py
--rw-r--r--   0        0        0      232 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1_source.py
--rw-r--r--   0        0        0     4341 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2.py
--rw-r--r--   0        0        0      303 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2_error_type.py
--rw-r--r--   0        0        0      232 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2_source.py
--rw-r--r--   0        0        0      162 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_latest_validation_results_response_200_status.py
--rw-r--r--   0        0        0     2293 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_my_organization_response_200.py
--rw-r--r--   0        0        0     3277 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_my_organization_response_200_results.py
--rw-r--r--   0        0        0      153 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_my_organization_response_200_status.py
--rw-r--r--   0        0        0     5193 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200.py
--rw-r--r--   0        0        0     2499 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0.py
--rw-r--r--   0        0        0     7259 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data.py
--rw-r--r--   0        0        0     1319 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_updated_by_user.py
--rw-r--r--   0        0        0     2268 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_validation_errors_item.py
--rw-r--r--   0        0        0      178 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_type.py
--rw-r--r--   0        0        0     2499 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1.py
--rw-r--r--   0        0        0     8178 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data.py
--rw-r--r--   0        0        0      377 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_chart_type.py
--rw-r--r--   0        0        0     1319 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_updated_by_user.py
--rw-r--r--   0        0        0     2268 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_validation_errors_item.py
--rw-r--r--   0        0        0      170 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_type.py
--rw-r--r--   0        0        0     2424 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_2.py
--rw-r--r--   0        0        0     3910 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_2_data.py
--rw-r--r--   0        0        0      170 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_2_type.py
--rw-r--r--   0        0        0      150 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_status.py
--rw-r--r--   0        0        0     2637 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_access_list_response_200.py
--rw-r--r--   0        0        0     2753 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_access_list_response_200_results_item.py
--rw-r--r--   0        0        0      289 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_access_list_response_200_results_item_role.py
--rw-r--r--   0        0        0      156 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_access_list_response_200_status.py
--rw-r--r--   0        0        0     2109 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200.py
--rw-r--r--   0        0        0    21254 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results.py
--rw-r--r--   0        0        0     3430 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0.py
--rw-r--r--   0        0        0     1773 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0_environment_item.py
--rw-r--r--   0        0        0      171 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0_type.py
--rw-r--r--   0        0        0     2571 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_1.py
--rw-r--r--   0        0        0      191 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_1_type.py
--rw-r--r--   0        0        0     4057 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2.py
--rw-r--r--   0        0        0     1773 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2_environment_item.py
--rw-r--r--   0        0        0      177 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2_type.py
--rw-r--r--   0        0        0     4239 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3.py
--rw-r--r--   0        0        0     1773 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3_environment_item.py
--rw-r--r--   0        0        0      183 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3_type.py
--rw-r--r--   0        0        0     4057 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4.py
--rw-r--r--   0        0        0     1773 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4_environment_item.py
--rw-r--r--   0        0        0      177 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4_type.py
--rw-r--r--   0        0        0     4150 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5.py
--rw-r--r--   0        0        0     1773 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5_environment_item.py
--rw-r--r--   0        0        0      189 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5_type.py
--rw-r--r--   0        0        0     3205 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6.py
--rw-r--r--   0        0        0     1773 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6_environment_item.py
--rw-r--r--   0        0        0      173 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6_type.py
--rw-r--r--   0        0        0      185 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_type.py
--rw-r--r--   0        0        0     5637 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0.py
--rw-r--r--   0        0        0     1437 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0_start_of_week.py
--rw-r--r--   0        0        0      189 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0_type.py
--rw-r--r--   0        0        0     6943 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1.py
--rw-r--r--   0        0        0     1437 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1_start_of_week.py
--rw-r--r--   0        0        0      187 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1_type.py
--rw-r--r--   0        0        0     7188 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2.py
--rw-r--r--   0        0        0     1437 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2_start_of_week.py
--rw-r--r--   0        0        0      187 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2_type.py
--rw-r--r--   0        0        0     6229 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3.py
--rw-r--r--   0        0        0      217 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_priority.py
--rw-r--r--   0        0        0     1437 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_start_of_week.py
--rw-r--r--   0        0        0      187 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_type.py
--rw-r--r--   0        0        0     4320 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4.py
--rw-r--r--   0        0        0     1437 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4_start_of_week.py
--rw-r--r--   0        0        0      191 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4_type.py
--rw-r--r--   0        0        0     4257 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5.py
--rw-r--r--   0        0        0     1437 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5_start_of_week.py
--rw-r--r--   0        0        0      181 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5_type.py
--rw-r--r--   0        0        0      146 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_status.py
--rw-r--r--   0        0        0     2563 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduled_jobs_response_200.py
--rw-r--r--   0        0        0     1729 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduled_jobs_response_200_results_item.py
--rw-r--r--   0        0        0      152 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduled_jobs_response_200_status.py
--rw-r--r--   0        0        0     2334 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_job_status_response_200.py
--rw-r--r--   0        0        0     1529 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_job_status_response_200_results.py
--rw-r--r--   0        0        0      157 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_job_status_response_200_status.py
--rw-r--r--   0        0        0     2243 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200.py
--rw-r--r--   0        0        0     5924 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results.py
--rw-r--r--   0        0        0     1795 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_charts_item.py
--rw-r--r--   0        0        0     1797 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_dashboards_item.py
--rw-r--r--   0        0        0     5953 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item.py
--rw-r--r--   0        0        0     1410 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_details.py
--rw-r--r--   0        0        0      253 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_status.py
--rw-r--r--   0        0        0      197 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_target_type.py
--rw-r--r--   0        0        0      473 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_task.py
--rw-r--r--   0        0        0     4392 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item.py
--rw-r--r--   0        0        0     2840 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_0.py
--rw-r--r--   0        0        0     2860 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_1.py
--rw-r--r--   0        0        0     1970 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_users_item.py
--rw-r--r--   0        0        0      152 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_status.py
--rw-r--r--   0        0        0     2160 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_response_200.py
--rw-r--r--   0        0        0     3838 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_response_200_results.py
--rw-r--r--   0        0        0     2741 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_0.py
--rw-r--r--   0        0        0     2761 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_1.py
--rw-r--r--   0        0        0      148 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_response_200_status.py
--rw-r--r--   0        0        0     2304 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_share_url_response_200.py
--rw-r--r--   0        0        0     3513 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_share_url_response_200_results.py
--rw-r--r--   0        0        0      147 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_share_url_response_200_status.py
--rw-r--r--   0        0        0     2563 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_slack_channels_response_200.py
--rw-r--r--   0        0        0     1626 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_slack_channels_response_200_results_item.py
--rw-r--r--   0        0        0      152 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_slack_channels_response_200_status.py
--rw-r--r--   0        0        0     2050 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200.py
--rw-r--r--   0        0        0     5502 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results.py
--rw-r--r--   0        0        0     2317 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results_access_item.py
--rw-r--r--   0        0        0      283 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results_access_item_role.py
--rw-r--r--   0        0        0     7565 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results_dashboards_item.py
--rw-r--r--   0        0        0     1293 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results_dashboards_item_updated_by_user.py
--rw-r--r--   0        0        0     2234 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results_dashboards_item_validation_errors_item.py
--rw-r--r--   0        0        0     7883 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results_queries_item.py
--rw-r--r--   0        0        0      369 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results_queries_item_chart_type.py
--rw-r--r--   0        0        0     1281 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results_queries_item_updated_by_user.py
--rw-r--r--   0        0        0     2219 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results_queries_item_validation_errors_item.py
--rw-r--r--   0        0        0      144 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_status.py
--rw-r--r--   0        0        0     2051 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/grant_project_access_to_user_json_body.py
--rw-r--r--   0        0        0      279 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/grant_project_access_to_user_json_body_role.py
--rw-r--r--   0        0        0     2053 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/grant_project_access_to_user_response_200.py
--rw-r--r--   0        0        0      160 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/grant_project_access_to_user_response_200_status.py
--rw-r--r--   0        0        0     2175 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/group.py
--rw-r--r--   0        0        0     2091 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/group_member.py
--rw-r--r--   0        0        0     1961 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/join_organization_response_200.py
--rw-r--r--   0        0        0      152 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/join_organization_response_200_status.py
--rw-r--r--   0        0        0     2620 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_charts_in_project_response_200.py
--rw-r--r--   0        0        0     4075 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_charts_in_project_response_200_results_item.py
--rw-r--r--   0        0        0      249 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_charts_in_project_response_200_results_item_chart_type.py
--rw-r--r--   0        0        0      155 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_charts_in_project_response_200_status.py
--rw-r--r--   0        0        0     2705 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_groups_in_organization_response_200.py
--rw-r--r--   0        0        0     2401 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_groups_in_organization_response_200_results_item.py
--rw-r--r--   0        0        0      160 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_groups_in_organization_response_200_status.py
--rw-r--r--   0        0        0     2773 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_my_available_organizations_response_200.py
--rw-r--r--   0        0        0     2071 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_my_available_organizations_response_200_results_item.py
--rw-r--r--   0        0        0      164 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_my_available_organizations_response_200_status.py
--rw-r--r--   0        0        0     2453 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_email_domains_response_200.py
--rw-r--r--   0        0        0     6137 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_email_domains_response_200_results.py
--rw-r--r--   0        0        0     4306 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item.py
--rw-r--r--   0        0        0      194 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item_role_type_0.py
--rw-r--r--   0        0        0      218 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item_role_type_1.py
--rw-r--r--   0        0        0      194 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item_role_type_2.py
--rw-r--r--   0        0        0      182 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_email_domains_response_200_results_role_type_0.py
--rw-r--r--   0        0        0      206 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_email_domains_response_200_results_role_type_1.py
--rw-r--r--   0        0        0      182 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_email_domains_response_200_results_role_type_2.py
--rw-r--r--   0        0        0      182 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_email_domains_response_200_results_role_type_3.py
--rw-r--r--   0        0        0      164 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_email_domains_response_200_status.py
--rw-r--r--   0        0        0     2682 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_members_response_200.py
--rw-r--r--   0        0        0     3732 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_members_response_200_results_item.py
--rw-r--r--   0        0        0      314 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_members_response_200_results_item_role.py
--rw-r--r--   0        0        0      159 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_members_response_200_status.py
--rw-r--r--   0        0        0     2744 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_projects_response_200.py
--rw-r--r--   0        0        0     2279 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_projects_response_200_results_item.py
--rw-r--r--   0        0        0      203 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_projects_response_200_results_item_type.py
--rw-r--r--   0        0        0      160 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_organization_projects_response_200_status.py
--rw-r--r--   0        0        0     2620 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_spaces_in_project_response_200.py
--rw-r--r--   0        0        0     2553 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_spaces_in_project_response_200_results_item.py
--rw-r--r--   0        0        0      155 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/list_spaces_in_project_response_200_status.py
--rw-r--r--   0        0        0     2133 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_filter_rule.py
--rw-r--r--   0        0        0      605 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_filter_rule_operator.py
--rw-r--r--   0        0        0     1463 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_filter_rule_target.py
--rw-r--r--   0        0        0     5557 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response.py
--rw-r--r--   0        0        0     7432 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_additional_metrics_item.py
--rw-r--r--   0        0        0      265 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_additional_metrics_item_compact_type_0.py
--rw-r--r--   0        0        0      305 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_additional_metrics_item_compact_type_1.py
--rw-r--r--   0        0        0     2769 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item.py
--rw-r--r--   0        0        0      640 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item_operator.py
--rw-r--r--   0        0        0     1653 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item_target.py
--rw-r--r--   0        0        0      417 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_additional_metrics_item_type.py
--rw-r--r--   0        0        0     7034 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_filters.py
--rw-r--r--   0        0        0     1665 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_filters_dimensions_type_0.py
--rw-r--r--   0        0        0     1675 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_filters_dimensions_type_1.py
--rw-r--r--   0        0        0     1650 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_filters_metrics_type_0.py
--rw-r--r--   0        0        0     1660 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_filters_metrics_type_1.py
--rw-r--r--   0        0        0     1690 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_sorts_item.py
--rw-r--r--   0        0        0     3183 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_table_calculations_item.py
--rw-r--r--   0        0        0     4643 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_table_calculations_item_format.py
--rw-r--r--   0        0        0      266 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_table_calculations_item_format_compact.py
--rw-r--r--   0        0        0      324 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_table_calculations_item_format_separator.py
--rw-r--r--   0        0        0      251 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_table_calculations_item_format_type.py
--rw-r--r--   0        0        0      383 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/metric_type.py
--rw-r--r--   0        0        0      284 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/number_separator.py
--rw-r--r--   0        0        0     5630 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid.py
--rw-r--r--   0        0        0     4125 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item.py
--rw-r--r--   0        0        0      187 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item_role_type_0.py
--rw-r--r--   0        0        0      211 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item_role_type_1.py
--rw-r--r--   0        0        0      187 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item_role_type_2.py
--rw-r--r--   0        0        0      175 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_role_type_0.py
--rw-r--r--   0        0        0      199 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_role_type_1.py
--rw-r--r--   0        0        0      175 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_role_type_2.py
--rw-r--r--   0        0        0      175 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_role_type_3.py
--rw-r--r--   0        0        0     6420 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0      224 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_priority.py
--rw-r--r--   0        0        0     1469 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      194 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     4520 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1479 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      200 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     7338 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1469 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      194 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     7093 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1469 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      194 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     5805 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1474 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      197 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     4353 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1454 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      185 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     3794 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_validation_response_base_name.py
--rw-r--r--   0        0        0      280 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_validation_response_base_name_error_type.py
--rw-r--r--   0        0        0      209 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/omit_validation_response_base_name_source.py
--rw-r--r--   0        0        0     3147 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/organization.py
--rw-r--r--   0        0        0     3507 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/organization_member_profile.py
--rw-r--r--   0        0        0      294 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/organization_member_profile_role.py
--rw-r--r--   0        0        0     1674 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/organization_member_profile_update.py
--rw-r--r--   0        0        0      300 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/organization_member_profile_update_role.py
--rw-r--r--   0        0        0      287 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/organization_member_role.py
--rw-r--r--   0        0        0      155 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/organization_member_role_editor.py
--rw-r--r--   0        0        0      190 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/organization_member_role_interactiveviewer.py
--rw-r--r--   0        0        0      155 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/organization_member_role_member.py
--rw-r--r--   0        0        0      155 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/organization_member_role_viewer.py
--rw-r--r--   0        0        0     1980 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/organization_project.py
--rw-r--r--   0        0        0      176 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/organization_project_type.py
--rw-r--r--   0        0        0     2713 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py
--rw-r--r--   0        0        0     6971 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py
--rw-r--r--   0        0        0     5108 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item.py
--rw-r--r--   0        0        0      218 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item_role_type_0.py
--rw-r--r--   0        0        0      242 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item_role_type_1.py
--rw-r--r--   0        0        0      218 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item_role_type_2.py
--rw-r--r--   0        0        0      206 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_role_type_0.py
--rw-r--r--   0        0        0      230 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_role_type_1.py
--rw-r--r--   0        0        0      206 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_role_type_2.py
--rw-r--r--   0        0        0      206 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_role_type_3.py
--rw-r--r--   0        0        0     7661 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0      267 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_priority.py
--rw-r--r--   0        0        0     1728 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      231 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     5374 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1748 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      245 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     1769 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py
--rw-r--r--   0        0        0     1493 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_group_name.py
--rw-r--r--   0        0        0     8285 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1728 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      231 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     8036 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1728 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      231 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     6654 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1738 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      235 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     5124 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names.py
--rw-r--r--   0        0        0     1693 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py
--rw-r--r--   0        0        0      219 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names_type.py
--rw-r--r--   0        0        0     9895 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors.py
--rw-r--r--   0        0        0     1834 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py
--rw-r--r--   0        0        0     2946 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py
--rw-r--r--   0        0        0     7951 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     1840 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py
--rw-r--r--   0        0        0     1460 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_group_name.py
--rw-r--r--   0        0        0     1494 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_organization_name.py
--rw-r--r--   0        0        0     1926 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     3654 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py
--rw-r--r--   0        0        0     5491 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py
--rw-r--r--   0        0        0     1610 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py
--rw-r--r--   0        0        0     1685 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_share_url_path_or_params.py
--rw-r--r--   0        0        0     2537 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py
--rw-r--r--   0        0        0     3330 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py
--rw-r--r--   0        0        0    11635 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors.py
--rw-r--r--   0        0        0      496 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_chart_type.py
--rw-r--r--   0        0        0     1838 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py
--rw-r--r--   0        0        0     2952 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py
--rw-r--r--   0        0        0     1547 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_ssh_key_pair_public_key.py
--rw-r--r--   0        0        0     4356 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py
--rw-r--r--   0        0        0      314 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name_error_type.py
--rw-r--r--   0        0        0      243 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name_source.py
--rw-r--r--   0        0        0     2194 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py
--rw-r--r--   0        0        0     1227 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pinned_items_item_type_0_data_updated_by_user.py
--rw-r--r--   0        0        0     2151 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pinned_items_item_type_0_data_validation_errors_item.py
--rw-r--r--   0        0        0      157 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pinned_items_item_type_0_type.py
--rw-r--r--   0        0        0      356 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pinned_items_item_type_1_data_chart_type.py
--rw-r--r--   0        0        0     1227 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pinned_items_item_type_1_data_updated_by_user.py
--rw-r--r--   0        0        0     2151 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pinned_items_item_type_1_data_validation_errors_item.py
--rw-r--r--   0        0        0      149 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pinned_items_item_type_1_type.py
--rw-r--r--   0        0        0     3793 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pinned_items_item_type_2_data.py
--rw-r--r--   0        0        0      149 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/pinned_items_item_type_2_type.py
--rw-r--r--   0        0        0     2212 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_json_body.py
--rw-r--r--   0        0        0     7343 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_json_body_filters.py
--rw-r--r--   0        0        0     1696 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_0.py
--rw-r--r--   0        0        0     1706 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_1.py
--rw-r--r--   0        0        0     1681 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_0.py
--rw-r--r--   0        0        0     1691 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_1.py
--rw-r--r--   0        0        0     2243 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200.py
--rw-r--r--   0        0        0     2220 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results.py
--rw-r--r--   0        0        0     6589 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query.py
--rw-r--r--   0        0        0     8425 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item.py
--rw-r--r--   0        0        0      291 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_compact_type_0.py
--rw-r--r--   0        0        0      331 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_compact_type_1.py
--rw-r--r--   0        0        0     3254 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item.py
--rw-r--r--   0        0        0      666 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py
--rw-r--r--   0        0        0     1822 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_target.py
--rw-r--r--   0        0        0      443 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_type.py
--rw-r--r--   0        0        0     8643 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters.py
--rw-r--r--   0        0        0     1810 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_0.py
--rw-r--r--   0        0        0     1820 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_1.py
--rw-r--r--   0        0        0     1795 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_0.py
--rw-r--r--   0        0        0     1805 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_1.py
--rw-r--r--   0        0        0     1835 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_sorts_item.py
--rw-r--r--   0        0        0     3546 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item.py
--rw-r--r--   0        0        0     5245 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format.py
--rw-r--r--   0        0        0      292 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format_compact.py
--rw-r--r--   0        0        0      350 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format_separator.py
--rw-r--r--   0        0        0      277 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format_type.py
--rw-r--r--   0        0        0      152 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_status.py
--rw-r--r--   0        0        0     5967 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body.py
--rw-r--r--   0        0        0     7477 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_additional_metrics_item.py
--rw-r--r--   0        0        0      266 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_additional_metrics_item_compact_type_0.py
--rw-r--r--   0        0        0      306 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_additional_metrics_item_compact_type_1.py
--rw-r--r--   0        0        0     2795 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item.py
--rw-r--r--   0        0        0      641 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item_operator.py
--rw-r--r--   0        0        0     1664 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item_target.py
--rw-r--r--   0        0        0      418 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_additional_metrics_item_type.py
--rw-r--r--   0        0        0     1855 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_filters.py
--rw-r--r--   0        0        0     1701 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_sorts_item.py
--rw-r--r--   0        0        0     3206 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_table_calculations_item.py
--rw-r--r--   0        0        0     4677 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_table_calculations_item_format.py
--rw-r--r--   0        0        0      267 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_table_calculations_item_format_compact.py
--rw-r--r--   0        0        0      325 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_table_calculations_item_format_separator.py
--rw-r--r--   0        0        0      252 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_table_calculations_item_format_type.py
--rw-r--r--   0        0        0     2166 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200.py
--rw-r--r--   0        0        0     2172 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results.py
--rw-r--r--   0        0        0     6457 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query.py
--rw-r--r--   0        0        0     8263 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item.py
--rw-r--r--   0        0        0      287 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_compact_type_0.py
--rw-r--r--   0        0        0      327 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_compact_type_1.py
--rw-r--r--   0        0        0     3168 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item.py
--rw-r--r--   0        0        0      662 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py
--rw-r--r--   0        0        0     1802 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.py
--rw-r--r--   0        0        0      439 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_type.py
--rw-r--r--   0        0        0     8417 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_filters.py
--rw-r--r--   0        0        0     1790 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_dimensions_type_0.py
--rw-r--r--   0        0        0     1800 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_dimensions_type_1.py
--rw-r--r--   0        0        0     1775 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_metrics_type_0.py
--rw-r--r--   0        0        0     1785 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_metrics_type_1.py
--rw-r--r--   0        0        0     1815 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_sorts_item.py
--rw-r--r--   0        0        0     3494 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item.py
--rw-r--r--   0        0        0     5157 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format.py
--rw-r--r--   0        0        0      288 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format_compact.py
--rw-r--r--   0        0        0      346 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format_separator.py
--rw-r--r--   0        0        0      273 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format_type.py
--rw-r--r--   0        0        0      148 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_status.py
--rw-r--r--   0        0        0     6528 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body.py
--rw-r--r--   0        0        0     8001 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item.py
--rw-r--r--   0        0        0      280 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_compact_type_0.py
--rw-r--r--   0        0        0      320 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_compact_type_1.py
--rw-r--r--   0        0        0     3029 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item.py
--rw-r--r--   0        0        0      655 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_operator.py
--rw-r--r--   0        0        0     1740 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_target.py
--rw-r--r--   0        0        0      432 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_type.py
--rw-r--r--   0        0        0     1931 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_filters.py
--rw-r--r--   0        0        0     1777 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_sorts_item.py
--rw-r--r--   0        0        0     3398 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item.py
--rw-r--r--   0        0        0     4997 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format.py
--rw-r--r--   0        0        0      281 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format_compact.py
--rw-r--r--   0        0        0      339 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format_separator.py
--rw-r--r--   0        0        0      266 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format_type.py
--rw-r--r--   0        0        0     2425 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200.py
--rw-r--r--   0        0        0     2350 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results.py
--rw-r--r--   0        0        0     7047 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query.py
--rw-r--r--   0        0        0     8971 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item.py
--rw-r--r--   0        0        0      301 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_compact_type_0.py
--rw-r--r--   0        0        0      341 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_compact_type_1.py
--rw-r--r--   0        0        0     3456 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item.py
--rw-r--r--   0        0        0      676 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py
--rw-r--r--   0        0        0     1934 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.py
--rw-r--r--   0        0        0      453 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_type.py
--rw-r--r--   0        0        0     9367 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters.py
--rw-r--r--   0        0        0     1890 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_0.py
--rw-r--r--   0        0        0     1900 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_1.py
--rw-r--r--   0        0        0     1875 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_0.py
--rw-r--r--   0        0        0     1885 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_1.py
--rw-r--r--   0        0        0     1891 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_sorts_item.py
--rw-r--r--   0        0        0     3740 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item.py
--rw-r--r--   0        0        0     5635 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format.py
--rw-r--r--   0        0        0      302 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format_compact.py
--rw-r--r--   0        0        0      360 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format_separator.py
--rw-r--r--   0        0        0      287 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format_type.py
--rw-r--r--   0        0        0      162 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_status.py
--rw-r--r--   0        0        0     6543 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/postgres_credentials.py
--rw-r--r--   0        0        0     1251 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/postgres_credentials_start_of_week.py
--rw-r--r--   0        0        0      154 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/postgres_credentials_type.py
--rw-r--r--   0        0        0    17362 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project.py
--rw-r--r--   0        0        0     3035 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_0.py
--rw-r--r--   0        0        0     1656 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_0_environment_item.py
--rw-r--r--   0        0        0      150 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_0_type.py
--rw-r--r--   0        0        0     2361 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_1.py
--rw-r--r--   0        0        0      170 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_1_type.py
--rw-r--r--   0        0        0     3662 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_2.py
--rw-r--r--   0        0        0     1656 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_2_environment_item.py
--rw-r--r--   0        0        0      156 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_2_type.py
--rw-r--r--   0        0        0     3844 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_3.py
--rw-r--r--   0        0        0     1656 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_3_environment_item.py
--rw-r--r--   0        0        0      162 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_3_type.py
--rw-r--r--   0        0        0     3662 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_4.py
--rw-r--r--   0        0        0     1656 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_4_environment_item.py
--rw-r--r--   0        0        0      156 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_4_type.py
--rw-r--r--   0        0        0     3755 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_5.py
--rw-r--r--   0        0        0     1656 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_5_environment_item.py
--rw-r--r--   0        0        0      168 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_5_type.py
--rw-r--r--   0        0        0     2810 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_6.py
--rw-r--r--   0        0        0     1656 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_6_environment_item.py
--rw-r--r--   0        0        0      152 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_6_type.py
--rw-r--r--   0        0        0     2504 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_member_profile.py
--rw-r--r--   0        0        0      267 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_member_profile_role.py
--rw-r--r--   0        0        0      260 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_member_role.py
--rw-r--r--   0        0        0      150 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_member_role_editor.py
--rw-r--r--   0        0        0      185 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_member_role_interactiveviewer.py
--rw-r--r--   0        0        0      150 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_member_role_viewer.py
--rw-r--r--   0        0        0      164 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_type.py
--rw-r--r--   0        0        0     5235 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_0.py
--rw-r--r--   0        0        0     1320 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_0_start_of_week.py
--rw-r--r--   0        0        0      168 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_0_type.py
--rw-r--r--   0        0        0     6541 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_1.py
--rw-r--r--   0        0        0     1320 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_1_start_of_week.py
--rw-r--r--   0        0        0      166 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_1_type.py
--rw-r--r--   0        0        0     6786 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_2.py
--rw-r--r--   0        0        0     1320 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_2_start_of_week.py
--rw-r--r--   0        0        0      166 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_2_type.py
--rw-r--r--   0        0        0     5697 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_3.py
--rw-r--r--   0        0        0      196 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_3_priority.py
--rw-r--r--   0        0        0     1320 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_3_start_of_week.py
--rw-r--r--   0        0        0      166 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_3_type.py
--rw-r--r--   0        0        0     3918 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_4.py
--rw-r--r--   0        0        0     1320 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_4_start_of_week.py
--rw-r--r--   0        0        0      170 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_4_type.py
--rw-r--r--   0        0        0     3855 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_5.py
--rw-r--r--   0        0        0     1320 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_5_start_of_week.py
--rw-r--r--   0        0        0      160 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_5_type.py
--rw-r--r--   0        0        0     1222 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/record_string_any.py
--rw-r--r--   0        0        0     6298 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/redshift_credentials.py
--rw-r--r--   0        0        0     1251 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/redshift_credentials_start_of_week.py
--rw-r--r--   0        0        0      154 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/redshift_credentials_type.py
--rw-r--r--   0        0        0     1999 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/remove_user_from_group_response_200.py
--rw-r--r--   0        0        0      155 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/remove_user_from_group_response_200_status.py
--rw-r--r--   0        0        0     2066 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_chart_item.py
--rw-r--r--   0        0        0     7618 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_chart_item_data.py
--rw-r--r--   0        0        0      357 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_chart_item_data_chart_type.py
--rw-r--r--   0        0        0     1229 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_chart_item_data_updated_by_user.py
--rw-r--r--   0        0        0     2153 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_chart_item_data_validation_errors_item.py
--rw-r--r--   0        0        0      150 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_chart_item_type.py
--rw-r--r--   0        0        0     2159 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_dashboard_item.py
--rw-r--r--   0        0        0     6904 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_dashboard_item_data.py
--rw-r--r--   0        0        0     1245 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_dashboard_item_data_updated_by_user.py
--rw-r--r--   0        0        0     2173 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_dashboard_item_data_validation_errors_item.py
--rw-r--r--   0        0        0      162 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_dashboard_item_type.py
--rw-r--r--   0        0        0      193 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_item_type.py
--rw-r--r--   0        0        0      150 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_item_type_chart.py
--rw-r--r--   0        0        0      162 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_item_type_dashboard.py
--rw-r--r--   0        0        0      150 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_item_type_space.py
--rw-r--r--   0        0        0     2003 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_space_item.py
--rw-r--r--   0        0        0     3795 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_space_item_data.py
--rw-r--r--   0        0        0      150 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/resource_view_space_item_type.py
--rw-r--r--   0        0        0     2073 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/revoke_project_access_for_user_response_200.py
--rw-r--r--   0        0        0      162 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/revoke_project_access_for_user_response_200_status.py
--rw-r--r--   0        0        0     2053 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/revoke_space_access_for_user_response_200.py
--rw-r--r--   0        0        0      160 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/revoke_space_access_for_user_response_200_status.py
--rw-r--r--   0        0        0     5680 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/run_query_request.py
--rw-r--r--   0        0        0     7266 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_additional_metrics_item.py
--rw-r--r--   0        0        0      261 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_additional_metrics_item_compact_type_0.py
--rw-r--r--   0        0        0      301 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_additional_metrics_item_compact_type_1.py
--rw-r--r--   0        0        0     2705 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_additional_metrics_item_filters_item.py
--rw-r--r--   0        0        0      636 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_additional_metrics_item_filters_item_operator.py
--rw-r--r--   0        0        0     1633 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_additional_metrics_item_filters_item_target.py
--rw-r--r--   0        0        0      413 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_additional_metrics_item_type.py
--rw-r--r--   0        0        0     1824 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_filters.py
--rw-r--r--   0        0        0     1670 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_sorts_item.py
--rw-r--r--   0        0        0     3131 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_table_calculations_item.py
--rw-r--r--   0        0        0     4555 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_table_calculations_item_format.py
--rw-r--r--   0        0        0      262 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_table_calculations_item_format_compact.py
--rw-r--r--   0        0        0      320 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_table_calculations_item_format_separator.py
--rw-r--r--   0        0        0      247 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_table_calculations_item_format_type.py
--rw-r--r--   0        0        0     1589 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduled_jobs.py
--rw-r--r--   0        0        0     3502 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_and_targets.py
--rw-r--r--   0        0        0     2680 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_and_targets_targets_item_type_0.py
--rw-r--r--   0        0        0     2700 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_and_targets_targets_item_type_1.py
--rw-r--r--   0        0        0     4849 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_base.py
--rw-r--r--   0        0        0      160 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_base_format.py
--rw-r--r--   0        0        0     2471 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_base_options_type_0.py
--rw-r--r--   0        0        0      176 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_base_options_type_0_limit_type_1.py
--rw-r--r--   0        0        0     1226 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_base_options_type_1.py
--rw-r--r--   0        0        0     2376 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_csv_options.py
--rw-r--r--   0        0        0      170 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_csv_options_limit_type_1.py
--rw-r--r--   0        0        0     2613 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_email_target.py
--rw-r--r--   0        0        0      156 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_format.py
--rw-r--r--   0        0        0     1200 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_image_options.py
--rw-r--r--   0        0        0      223 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_job_status.py
--rw-r--r--   0        0        0     4954 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_log.py
--rw-r--r--   0        0        0     1242 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_log_details.py
--rw-r--r--   0        0        0      223 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_log_status.py
--rw-r--r--   0        0        0      167 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_log_target_type.py
--rw-r--r--   0        0        0      443 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_log_task.py
--rw-r--r--   0        0        0     2415 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_options_type_0.py
--rw-r--r--   0        0        0      172 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_options_type_0_limit_type_1.py
--rw-r--r--   0        0        0     1203 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_options_type_1.py
--rw-r--r--   0        0        0     2593 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_slack_target.py
--rw-r--r--   0        0        0      161 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_type_0_format.py
--rw-r--r--   0        0        0     2488 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_type_0_options_type_0.py
--rw-r--r--   0        0        0      177 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_type_0_options_type_0_limit_type_1.py
--rw-r--r--   0        0        0     1234 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_type_0_options_type_1.py
--rw-r--r--   0        0        0      161 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_type_1_format.py
--rw-r--r--   0        0        0     2488 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_type_1_options_type_0.py
--rw-r--r--   0        0        0      177 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_type_1_options_type_0_limit_type_1.py
--rw-r--r--   0        0        0     1234 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_type_1_options_type_1.py
--rw-r--r--   0        0        0     5079 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs.py
--rw-r--r--   0        0        0     1701 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_charts_item.py
--rw-r--r--   0        0        0     1703 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_dashboards_item.py
--rw-r--r--   0        0        0     5415 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_logs_item.py
--rw-r--r--   0        0        0     1316 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_logs_item_details.py
--rw-r--r--   0        0        0      236 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_logs_item_status.py
--rw-r--r--   0        0        0      180 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_logs_item_target_type.py
--rw-r--r--   0        0        0      456 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_logs_item_task.py
--rw-r--r--   0        0        0     3862 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_schedulers_item.py
--rw-r--r--   0        0        0     2746 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_0.py
--rw-r--r--   0        0        0     2766 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_1.py
--rw-r--r--   0        0        0     1876 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_users_item.py
--rw-r--r--   0        0        0     3396 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/share_url.py
--rw-r--r--   0        0        0     1481 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/slack_channel.py
--rw-r--r--   0        0        0     5010 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/snowflake_credentials.py
--rw-r--r--   0        0        0     1256 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/snowflake_credentials_start_of_week.py
--rw-r--r--   0        0        0      157 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/snowflake_credentials_type.py
--rw-r--r--   0        0        0     1586 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/sort_field.py
--rw-r--r--   0        0        0     4794 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space.py
--rw-r--r--   0        0        0     2082 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_access_item.py
--rw-r--r--   0        0        0      262 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_access_item_role.py
--rw-r--r--   0        0        0     6938 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_dashboard.py
--rw-r--r--   0        0        0     1179 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_dashboard_updated_by_user.py
--rw-r--r--   0        0        0     2089 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_dashboard_validation_errors_item.py
--rw-r--r--   0        0        0     7087 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_dashboards_item.py
--rw-r--r--   0        0        0     1201 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_dashboards_item_updated_by_user.py
--rw-r--r--   0        0        0     2117 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_dashboards_item_validation_errors_item.py
--rw-r--r--   0        0        0     7266 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_queries_item.py
--rw-r--r--   0        0        0      348 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_queries_item_chart_type.py
--rw-r--r--   0        0        0     1189 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_queries_item_updated_by_user.py
--rw-r--r--   0        0        0     2102 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_queries_item_validation_errors_item.py
--rw-r--r--   0        0        0     7060 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_query.py
--rw-r--r--   0        0        0      342 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_query_chart_type.py
--rw-r--r--   0        0        0     1163 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_query_updated_by_user.py
--rw-r--r--   0        0        0     2069 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_query_validation_errors_item.py
--rw-r--r--   0        0        0     2028 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_share.py
--rw-r--r--   0        0        0      257 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_share_role.py
--rw-r--r--   0        0        0     2390 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/space_summary.py
--rw-r--r--   0        0        0      242 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/table_calculation_format_compact.py
--rw-r--r--   0        0        0      300 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/table_calculation_format_separator.py
--rw-r--r--   0        0        0      227 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/table_calculation_format_type.py
--rw-r--r--   0        0        0     3516 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/trino_credentials.py
--rw-r--r--   0        0        0     1236 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/trino_credentials_start_of_week.py
--rw-r--r--   0        0        0      145 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/trino_credentials_type.py
--rw-r--r--   0        0        0     5066 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_allowed_email_domains.py
--rw-r--r--   0        0        0     3751 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_allowed_email_domains_projects_item.py
--rw-r--r--   0        0        0      173 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_allowed_email_domains_projects_item_role_type_0.py
--rw-r--r--   0        0        0      197 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_allowed_email_domains_projects_item_role_type_1.py
--rw-r--r--   0        0        0      173 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_allowed_email_domains_projects_item_role_type_2.py
--rw-r--r--   0        0        0      161 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_allowed_email_domains_role_type_0.py
--rw-r--r--   0        0        0      185 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_allowed_email_domains_role_type_1.py
--rw-r--r--   0        0        0      161 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_allowed_email_domains_role_type_2.py
--rw-r--r--   0        0        0      161 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_allowed_email_domains_role_type_3.py
--rw-r--r--   0        0        0     3040 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_dbt_cloud_integration_settings_response_200.py
--rw-r--r--   0        0        0     1813 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_dbt_cloud_integration_settings_response_200_results.py
--rw-r--r--   0        0        0      169 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_dbt_cloud_integration_settings_response_200_status.py
--rw-r--r--   0        0        0     1447 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_group.py
--rw-r--r--   0        0        0     1493 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_group_json_body.py
--rw-r--r--   0        0        0     2126 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_group_response_200.py
--rw-r--r--   0        0        0     2307 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_group_response_200_results.py
--rw-r--r--   0        0        0      147 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_group_response_200_status.py
--rw-r--r--   0        0        0     2575 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_my_organization_json_body.py
--rw-r--r--   0        0        0     2005 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_my_organization_response_200.py
--rw-r--r--   0        0        0      156 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_my_organization_response_200_status.py
--rw-r--r--   0        0        0     2520 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization.py
--rw-r--r--   0        0        0     5551 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_json_body.py
--rw-r--r--   0        0        0     4100 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_json_body_projects_item.py
--rw-r--r--   0        0        0      186 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_json_body_projects_item_role_type_0.py
--rw-r--r--   0        0        0      210 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_json_body_projects_item_role_type_1.py
--rw-r--r--   0        0        0      186 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_json_body_projects_item_role_type_2.py
--rw-r--r--   0        0        0      174 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_json_body_role_type_0.py
--rw-r--r--   0        0        0      198 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_json_body_role_type_1.py
--rw-r--r--   0        0        0      174 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_json_body_role_type_2.py
--rw-r--r--   0        0        0      174 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_json_body_role_type_3.py
--rw-r--r--   0        0        0     2487 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_response_200.py
--rw-r--r--   0        0        0     6215 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_response_200_results.py
--rw-r--r--   0        0        0     4356 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item.py
--rw-r--r--   0        0        0      196 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item_role_type_0.py
--rw-r--r--   0        0        0      220 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item_role_type_1.py
--rw-r--r--   0        0        0      196 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item_role_type_2.py
--rw-r--r--   0        0        0      184 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_response_200_results_role_type_0.py
--rw-r--r--   0        0        0      208 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_response_200_results_role_type_1.py
--rw-r--r--   0        0        0      184 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_response_200_results_role_type_2.py
--rw-r--r--   0        0        0      184 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_response_200_results_role_type_3.py
--rw-r--r--   0        0        0      166 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_response_200_status.py
--rw-r--r--   0        0        0     1715 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_member_json_body.py
--rw-r--r--   0        0        0      301 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_member_json_body_role.py
--rw-r--r--   0        0        0     2430 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_member_response_200.py
--rw-r--r--   0        0        0     3698 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_member_response_200_results.py
--rw-r--r--   0        0        0      311 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_member_response_200_results_role.py
--rw-r--r--   0        0        0      160 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_organization_member_response_200_status.py
--rw-r--r--   0        0        0     2066 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_item_order.py
--rw-r--r--   0        0        0     1798 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_item_order_data.py
--rw-r--r--   0        0        0      198 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_item_order_type.py
--rw-r--r--   0        0        0     2356 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_json_body_item.py
--rw-r--r--   0        0        0     1872 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_json_body_item_data.py
--rw-r--r--   0        0        0      211 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_json_body_item_type.py
--rw-r--r--   0        0        0     5525 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200.py
--rw-r--r--   0        0        0     2641 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0.py
--rw-r--r--   0        0        0     7522 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data.py
--rw-r--r--   0        0        0     1353 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_updated_by_user.py
--rw-r--r--   0        0        0     2311 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_validation_errors_item.py
--rw-r--r--   0        0        0      186 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_type.py
--rw-r--r--   0        0        0     2641 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1.py
--rw-r--r--   0        0        0     8490 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data.py
--rw-r--r--   0        0        0      385 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_chart_type.py
--rw-r--r--   0        0        0     1353 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_updated_by_user.py
--rw-r--r--   0        0        0     2311 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_validation_errors_item.py
--rw-r--r--   0        0        0      178 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_type.py
--rw-r--r--   0        0        0     2566 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2.py
--rw-r--r--   0        0        0     3953 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2_data.py
--rw-r--r--   0        0        0      178 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2_type.py
--rw-r--r--   0        0        0      158 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_status.py
--rw-r--r--   0        0        0     1716 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_project_access_for_user_json_body.py
--rw-r--r--   0        0        0      281 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_project_access_for_user_json_body_role.py
--rw-r--r--   0        0        0     2073 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_project_access_for_user_response_200.py
--rw-r--r--   0        0        0      162 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_project_access_for_user_response_200_status.py
--rw-r--r--   0        0        0     1541 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_project_member.py
--rw-r--r--   0        0        0      266 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_project_member_role.py
--rw-r--r--   0        0        0     2220 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_scheduler_response_201.py
--rw-r--r--   0        0        0     3910 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_scheduler_response_201_results.py
--rw-r--r--   0        0        0     2756 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_0.py
--rw-r--r--   0        0        0     2776 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_1.py
--rw-r--r--   0        0        0      151 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_scheduler_response_201_status.py
--rw-r--r--   0        0        0     1556 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_space.py
--rw-r--r--   0        0        0     1602 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_space_json_body.py
--rw-r--r--   0        0        0     2126 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200.py
--rw-r--r--   0        0        0     5580 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results.py
--rw-r--r--   0        0        0     2347 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results_access_item.py
--rw-r--r--   0        0        0      286 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results_access_item_role.py
--rw-r--r--   0        0        0     7625 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results_dashboards_item.py
--rw-r--r--   0        0        0     1305 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results_dashboards_item_updated_by_user.py
--rw-r--r--   0        0        0     2249 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results_dashboards_item_validation_errors_item.py
--rw-r--r--   0        0        0     7961 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results_queries_item.py
--rw-r--r--   0        0        0      372 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results_queries_item_chart_type.py
--rw-r--r--   0        0        0     1293 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results_queries_item_updated_by_user.py
--rw-r--r--   0        0        0     2234 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results_queries_item_validation_errors_item.py
--rw-r--r--   0        0        0      147 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_status.py
--rw-r--r--   0        0        0     1119 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/updated_by_user.py
--rw-r--r--   0        0        0     1921 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/user_allowed_organization.py
--rw-r--r--   0        0        0     1837 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validate_project_json_body.py
--rw-r--r--   0        0        0     2220 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validate_project_response_200.py
--rw-r--r--   0        0        0     1491 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validate_project_response_200_results.py
--rw-r--r--   0        0        0      151 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validate_project_response_200_status.py
--rw-r--r--   0        0        0     6761 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_error_chart_response.py
--rw-r--r--   0        0        0      360 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_error_chart_response_chart_type.py
--rw-r--r--   0        0        0      278 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_error_chart_response_error_type.py
--rw-r--r--   0        0        0      207 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_error_chart_response_source.py
--rw-r--r--   0        0        0     6098 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_error_dashboard_response.py
--rw-r--r--   0        0        0      282 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_error_dashboard_response_error_type.py
--rw-r--r--   0        0        0      211 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_error_dashboard_response_source.py
--rw-r--r--   0        0        0     3911 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_error_table_response.py
--rw-r--r--   0        0        0      278 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_error_table_response_error_type.py
--rw-r--r--   0        0        0      207 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_error_table_response_source.py
--rw-r--r--   0        0        0      260 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_error_type.py
--rw-r--r--   0        0        0     3711 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_response_base.py
--rw-r--r--   0        0        0      272 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_response_base_error_type.py
--rw-r--r--   0        0        0      201 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_response_base_source.py
--rw-r--r--   0        0        0     6642 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_response_type_0.py
--rw-r--r--   0        0        0      355 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_response_type_0_chart_type.py
--rw-r--r--   0        0        0      273 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_response_type_0_error_type.py
--rw-r--r--   0        0        0      202 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_response_type_0_source.py
--rw-r--r--   0        0        0     5945 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_response_type_1.py
--rw-r--r--   0        0        0      273 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_response_type_1_error_type.py
--rw-r--r--   0        0        0      202 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_response_type_1_source.py
--rw-r--r--   0        0        0     3822 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_response_type_2.py
--rw-r--r--   0        0        0      273 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_response_type_2_error_type.py
--rw-r--r--   0        0        0      202 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_response_type_2_source.py
--rw-r--r--   0        0        0      193 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_source_type.py
--rw-r--r--   0        0        0     1995 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/validation_summary.py
--rw-r--r--   0        0        0     2525 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/view_statistics.py
--rw-r--r--   0        0        0     1287 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_0_start_of_week.py
--rw-r--r--   0        0        0      162 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_0_type.py
--rw-r--r--   0        0        0     1287 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_1_start_of_week.py
--rw-r--r--   0        0        0      160 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_1_type.py
--rw-r--r--   0        0        0     1287 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_2_start_of_week.py
--rw-r--r--   0        0        0      160 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_2_type.py
--rw-r--r--   0        0        0      190 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_3_priority.py
--rw-r--r--   0        0        0     1287 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_3_start_of_week.py
--rw-r--r--   0        0        0      160 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_3_type.py
--rw-r--r--   0        0        0     1287 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_4_start_of_week.py
--rw-r--r--   0        0        0      164 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_4_type.py
--rw-r--r--   0        0        0     1287 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_5_start_of_week.py
--rw-r--r--   0        0        0      154 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_5_type.py
--rw-r--r--   0        0        0      153 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_types_bigquery.py
--rw-r--r--   0        0        0      159 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_types_databricks.py
--rw-r--r--   0        0        0      153 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_types_postgres.py
--rw-r--r--   0        0        0      153 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_types_redshift.py
--rw-r--r--   0        0        0      156 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_types_snowflake.py
--rw-r--r--   0        0        0      144 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/warehouse_types_trino.py
--rw-r--r--   0        0        0      225 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/models/week_day.py
--rw-r--r--   0        0        0       26 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/py.typed
--rw-r--r--   0        0        0      993 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/lightdash_client/types.py
--rw-r--r--   0        0        0     1862 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/pyproject.toml
--rw-r--r--   0        0        0      830 2023-07-06 00:20:34.000000 lightdash_client_python-0.640.1/setup.py
--rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 lightdash_client_python-0.640.1/PKG-INFO
+-rw-r--r--   0        0        0     1040 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/.openapi-generator-ignore
+-rw-r--r--   0        0        0        8 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/.python-version
+-rw-r--r--   0        0        0    11357 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/LICENSE
+-rw-r--r--   0        0        0     3258 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/README.md
+-rw-r--r--   0        0        0      182 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/__init__.py
+-rw-r--r--   0        0        0       47 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/charts/__init__.py
+-rw-r--r--   0        0        0     4749 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/charts/post_chart_results.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/content/__init__.py
+-rw-r--r--   0        0        0     4592 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/content/get_pinned_items.py
+-rw-r--r--   0        0        0     5871 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/content/update_pinned_items_order.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/exploring/__init__.py
+-rw-r--r--   0        0        0     5223 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/exploring/post_run_query.py
+-rw-r--r--   0        0        0     5659 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/exploring/post_run_underlying_data_query.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/exports/__init__.py
+-rw-r--r--   0        0        0     3852 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/exports/get_csv_url.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/integrations/__init__.py
+-rw-r--r--   0        0        0     4545 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0     4511 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0     4956 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/integrations/get_dbt_cloud_metrics.py
+-rw-r--r--   0        0        0     3655 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/integrations/get_slack_channels.py
+-rw-r--r--   0        0        0     4543 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/my_account/__init__.py
+-rw-r--r--   0        0        0     4215 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/my_account/create_email_one_time_passcode.py
+-rw-r--r--   0        0        0     3518 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/my_account/delete_me.py
+-rw-r--r--   0        0        0     4750 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/my_account/get_email_verification_status.py
+-rw-r--r--   0        0        0     4914 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/my_account/join_organization.py
+-rw-r--r--   0        0        0     4375 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/my_account/list_my_available_organizations.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/__init__.py
+-rw-r--r--   0        0        0     4823 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/create_group_in_organization.py
+-rw-r--r--   0        0        0     5097 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/create_organization.py
+-rw-r--r--   0        0        0     4439 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/delete_my_organization.py
+-rw-r--r--   0        0        0     4292 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/delete_organization_member.py
+-rw-r--r--   0        0        0     3725 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/get_my_organization.py
+-rw-r--r--   0        0        0     3909 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/list_groups_in_organization.py
+-rw-r--r--   0        0        0     4022 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/list_organization_email_domains.py
+-rw-r--r--   0        0        0     3898 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/list_organization_members.py
+-rw-r--r--   0        0        0     3902 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/list_organization_projects.py
+-rw-r--r--   0        0        0     4654 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/update_my_organization.py
+-rw-r--r--   0        0        0     5049 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/organizations/update_organization_email_domains.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/projects/__init__.py
+-rw-r--r--   0        0        0     4743 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/projects/delete_validation_dismiss.py
+-rw-r--r--   0        0        0     5908 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/projects/get_latest_validation_results.py
+-rw-r--r--   0        0        0     4077 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/projects/get_project.py
+-rw-r--r--   0        0        0     4191 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/projects/list_charts_in_project.py
+-rw-r--r--   0        0        0     4191 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/projects/list_spaces_in_project.py
+-rw-r--r--   0        0        0     6431 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/projects/validate_project.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/__init__.py
+-rw-r--r--   0        0        0     5295 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/add_space_share_to_user.py
+-rw-r--r--   0        0        0     4946 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/create_space_in_project.py
+-rw-r--r--   0        0        0     4941 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/get_project_access_list.py
+-rw-r--r--   0        0        0     5041 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/grant_project_access_to_user.py
+-rw-r--r--   0        0        0     4688 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py
+-rw-r--r--   0        0        0     5031 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py
+-rw-r--r--   0        0        0     5256 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/update_organization_member.py
+-rw-r--r--   0        0        0     5467 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/update_project_access_for_user.py
+-rw-r--r--   0        0        0     5071 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/update_space.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/schedulers/__init__.py
+-rw-r--r--   0        0        0     4140 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/schedulers/delete_scheduler.py
+-rw-r--r--   0        0        0     4151 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/schedulers/get_scheduled_jobs.py
+-rw-r--r--   0        0        0     4081 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/schedulers/get_scheduler.py
+-rw-r--r--   0        0        0     4332 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/schedulers/get_scheduler_job_status.py
+-rw-r--r--   0        0        0     4111 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/schedulers/get_scheduler_logs.py
+-rw-r--r--   0        0        0     4615 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/schedulers/update_scheduler.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/share_links/__init__.py
+-rw-r--r--   0        0        0     4687 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/share_links/create_share_url.py
+-rw-r--r--   0        0        0     4004 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/share_links/get_share_url.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/spaces/__init__.py
+-rw-r--r--   0        0        0     4485 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/spaces/delete_space.py
+-rw-r--r--   0        0        0     4463 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/spaces/get_space.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/ssh_keypairs/__init__.py
+-rw-r--r--   0        0        0     3585 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py
+-rw-r--r--   0        0        0        0 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/user_groups/__init__.py
+-rw-r--r--   0        0        0     4462 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/user_groups/add_user_to_group.py
+-rw-r--r--   0        0        0     3983 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/user_groups/delete_group.py
+-rw-r--r--   0        0        0     3953 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/user_groups/get_group.py
+-rw-r--r--   0        0        0     4077 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/user_groups/get_group_members.py
+-rw-r--r--   0        0        0     4510 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/user_groups/remove_user_from_group.py
+-rw-r--r--   0        0        0     4885 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/api/user_groups/update_group.py
+-rw-r--r--   0        0        0     2888 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/client.py
+-rw-r--r--   0        0        0      470 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/errors.py
+-rw-r--r--   0        0        0   177550 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/__init__.py
+-rw-r--r--   0        0        0     1415 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/add_space_share.py
+-rw-r--r--   0        0        0     1497 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/add_space_share_to_user_json_body.py
+-rw-r--r--   0        0        0     2003 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/add_space_share_to_user_response_200.py
+-rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/add_space_share_to_user_response_200_status.py
+-rw-r--r--   0        0        0     1949 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/add_user_to_group_response_200.py
+-rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/add_user_to_group_response_200_status.py
+-rw-r--r--   0        0        0     6478 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/additional_metric.py
+-rw-r--r--   0        0        0      241 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_compact_type_0.py
+-rw-r--r--   0        0        0      281 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_compact_type_1.py
+-rw-r--r--   0        0        0     2365 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_filters_item.py
+-rw-r--r--   0        0        0      650 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_filters_item_operator.py
+-rw-r--r--   0        0        0     1521 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_filters_item_target.py
+-rw-r--r--   0        0        0      393 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_type.py
+-rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domain_projects_role_type_0.py
+-rw-r--r--   0        0        0      186 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domain_projects_role_type_1.py
+-rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domain_projects_role_type_2.py
+-rw-r--r--   0        0        0     4988 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains.py
+-rw-r--r--   0        0        0     3595 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_projects_item.py
+-rw-r--r--   0        0        0      167 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_projects_item_role_type_0.py
+-rw-r--r--   0        0        0      191 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_projects_item_role_type_1.py
+-rw-r--r--   0        0        0      167 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_projects_item_role_type_2.py
+-rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_role_type_0.py
+-rw-r--r--   0        0        0      179 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_role_type_1.py
+-rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_role_type_2.py
+-rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_role_type_3.py
+-rw-r--r--   0        0        0     2563 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_chart_summary_list_response.py
+-rw-r--r--   0        0        0     4038 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_chart_summary_list_response_results_item.py
+-rw-r--r--   0        0        0      246 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_chart_summary_list_response_results_item_chart_type.py
+-rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_chart_summary_list_response_status.py
+-rw-r--r--   0        0        0     2016 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_csv_url_response.py
+-rw-r--r--   0        0        0     1580 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_csv_url_response_results.py
+-rw-r--r--   0        0        0      142 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_csv_url_response_status.py
+-rw-r--r--   0        0        0     2776 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_integration_settings.py
+-rw-r--r--   0        0        0     1737 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_integration_settings_results.py
+-rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_integration_settings_status.py
+-rw-r--r--   0        0        0     2122 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_metrics.py
+-rw-r--r--   0        0        0     2325 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_metrics_results.py
+-rw-r--r--   0        0        0     2526 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_metrics_results_metrics_item.py
+-rw-r--r--   0        0        0      143 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_metrics_status.py
+-rw-r--r--   0        0        0     2019 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_settings_delete_success.py
+-rw-r--r--   0        0        0      157 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_settings_delete_success_status.py
+-rw-r--r--   0        0        0     2224 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_email_status_response.py
+-rw-r--r--   0        0        0     2709 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_email_status_response_results.py
+-rw-r--r--   0        0        0     2813 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_email_status_response_results_otp.py
+-rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_email_status_response_status.py
+-rw-r--r--   0        0        0     2049 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_error_payload.py
+-rw-r--r--   0        0        0     2277 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_error_payload_error.py
+-rw-r--r--   0        0        0      146 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_error_payload_status.py
+-rw-r--r--   0        0        0     2429 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_list_response.py
+-rw-r--r--   0        0        0     2320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_list_response_results_item.py
+-rw-r--r--   0        0        0      145 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_list_response_status.py
+-rw-r--r--   0        0        0     2480 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_members_response.py
+-rw-r--r--   0        0        0     2218 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_members_response_results_item.py
+-rw-r--r--   0        0        0      148 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_members_response_status.py
+-rw-r--r--   0        0        0     1993 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_response.py
+-rw-r--r--   0        0        0     2274 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_response_results.py
+-rw-r--r--   0        0        0      141 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_group_response_status.py
+-rw-r--r--   0        0        0     2160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_job_scheduled_response.py
+-rw-r--r--   0        0        0     1476 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_job_scheduled_response_results.py
+-rw-r--r--   0        0        0      148 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_job_scheduled_response_status.py
+-rw-r--r--   0        0        0     2067 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_job_status_response.py
+-rw-r--r--   0        0        0     1463 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_job_status_response_results.py
+-rw-r--r--   0        0        0      145 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_job_status_response_status.py
+-rw-r--r--   0        0        0     2003 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization.py
+-rw-r--r--   0        0        0     2362 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains.py
+-rw-r--r--   0        0        0     5921 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results.py
+-rw-r--r--   0        0        0     4175 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item.py
+-rw-r--r--   0        0        0      189 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item_role_type_0.py
+-rw-r--r--   0        0        0      213 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item_role_type_1.py
+-rw-r--r--   0        0        0      189 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item_role_type_2.py
+-rw-r--r--   0        0        0      177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_role_type_0.py
+-rw-r--r--   0        0        0      201 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_role_type_1.py
+-rw-r--r--   0        0        0      177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_role_type_2.py
+-rw-r--r--   0        0        0      177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_role_type_3.py
+-rw-r--r--   0        0        0      159 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_status.py
+-rw-r--r--   0        0        0     2305 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profile.py
+-rw-r--r--   0        0        0     3624 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profile_results.py
+-rw-r--r--   0        0        0      304 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profile_results_role.py
+-rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profile_status.py
+-rw-r--r--   0        0        0     2591 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profiles.py
+-rw-r--r--   0        0        0     3678 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profiles_results_item.py
+-rw-r--r--   0        0        0      309 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profiles_results_item_role.py
+-rw-r--r--   0        0        0      154 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profiles_status.py
+-rw-r--r--   0        0        0     2519 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_projects.py
+-rw-r--r--   0        0        0     2151 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_projects_results_item.py
+-rw-r--r--   0        0        0      191 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_projects_results_item_type.py
+-rw-r--r--   0        0        0      148 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_projects_status.py
+-rw-r--r--   0        0        0     3203 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_results.py
+-rw-r--r--   0        0        0      140 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_organization_status.py
+-rw-r--r--   0        0        0     4640 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items.py
+-rw-r--r--   0        0        0     2288 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0.py
+-rw-r--r--   0        0        0     7025 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0_data.py
+-rw-r--r--   0        0        0     1271 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0_data_updated_by_user.py
+-rw-r--r--   0        0        0     2207 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0_data_validation_errors_item.py
+-rw-r--r--   0        0        0      167 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0_type.py
+-rw-r--r--   0        0        0     2288 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1.py
+-rw-r--r--   0        0        0     7876 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1_data.py
+-rw-r--r--   0        0        0      366 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1_data_chart_type.py
+-rw-r--r--   0        0        0     1271 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1_data_updated_by_user.py
+-rw-r--r--   0        0        0     2207 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1_data_validation_errors_item.py
+-rw-r--r--   0        0        0      159 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1_type.py
+-rw-r--r--   0        0        0     2225 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_2.py
+-rw-r--r--   0        0        0     3849 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_2_data.py
+-rw-r--r--   0        0        0      159 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_2_type.py
+-rw-r--r--   0        0        0      139 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_status.py
+-rw-r--r--   0        0        0     2580 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_access_list_response.py
+-rw-r--r--   0        0        0     2719 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_access_list_response_results_item.py
+-rw-r--r--   0        0        0      286 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_access_list_response_results_item_role.py
+-rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_access_list_response_status.py
+-rw-r--r--   0        0        0     2027 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response.py
+-rw-r--r--   0        0        0    20745 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results.py
+-rw-r--r--   0        0        0     3377 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_0.py
+-rw-r--r--   0        0        0     1755 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_0_environment_item.py
+-rw-r--r--   0        0        0      168 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_0_type.py
+-rw-r--r--   0        0        0     2541 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_1.py
+-rw-r--r--   0        0        0      188 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_1_type.py
+-rw-r--r--   0        0        0     4004 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_2.py
+-rw-r--r--   0        0        0     1755 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_2_environment_item.py
+-rw-r--r--   0        0        0      174 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_2_type.py
+-rw-r--r--   0        0        0     4186 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_3.py
+-rw-r--r--   0        0        0     1755 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_3_environment_item.py
+-rw-r--r--   0        0        0      180 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_3_type.py
+-rw-r--r--   0        0        0     4004 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_4.py
+-rw-r--r--   0        0        0     1755 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_4_environment_item.py
+-rw-r--r--   0        0        0      174 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_4_type.py
+-rw-r--r--   0        0        0     4097 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_5.py
+-rw-r--r--   0        0        0     1755 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_5_environment_item.py
+-rw-r--r--   0        0        0      186 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_5_type.py
+-rw-r--r--   0        0        0     3152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_6.py
+-rw-r--r--   0        0        0     1755 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_6_environment_item.py
+-rw-r--r--   0        0        0      170 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_6_type.py
+-rw-r--r--   0        0        0      182 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_type.py
+-rw-r--r--   0        0        0     5577 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_0.py
+-rw-r--r--   0        0        0     1419 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_0_start_of_week.py
+-rw-r--r--   0        0        0      186 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_0_type.py
+-rw-r--r--   0        0        0     6883 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_1.py
+-rw-r--r--   0        0        0     1419 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_1_start_of_week.py
+-rw-r--r--   0        0        0      184 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_1_type.py
+-rw-r--r--   0        0        0     7128 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_2.py
+-rw-r--r--   0        0        0     1419 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_2_start_of_week.py
+-rw-r--r--   0        0        0      184 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_2_type.py
+-rw-r--r--   0        0        0     6150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_3.py
+-rw-r--r--   0        0        0      214 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_priority.py
+-rw-r--r--   0        0        0     1419 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_start_of_week.py
+-rw-r--r--   0        0        0      184 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_type.py
+-rw-r--r--   0        0        0     4260 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_4.py
+-rw-r--r--   0        0        0     1419 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_4_start_of_week.py
+-rw-r--r--   0        0        0      188 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_4_type.py
+-rw-r--r--   0        0        0     4197 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_5.py
+-rw-r--r--   0        0        0     1419 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_5_start_of_week.py
+-rw-r--r--   0        0        0      178 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_5_type.py
+-rw-r--r--   0        0        0      143 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_status.py
+-rw-r--r--   0        0        0     2050 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response.py
+-rw-r--r--   0        0        0     2119 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results.py
+-rw-r--r--   0        0        0     6314 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query.py
+-rw-r--r--   0        0        0     8094 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item.py
+-rw-r--r--   0        0        0      283 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      323 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0     3077 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item.py
+-rw-r--r--   0        0        0      692 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item_operator.py
+-rw-r--r--   0        0        0     1779 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item_target.py
+-rw-r--r--   0        0        0      435 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     8170 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters.py
+-rw-r--r--   0        0        0     1767 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1777 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1752 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1762 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     1792 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_sorts_item.py
+-rw-r--r--   0        0        0     3437 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item.py
+-rw-r--r--   0        0        0     5063 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format.py
+-rw-r--r--   0        0        0      284 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format_compact.py
+-rw-r--r--   0        0        0      342 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      269 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0      144 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_status.py
+-rw-r--r--   0        0        0     2497 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduled_jobs_response.py
+-rw-r--r--   0        0        0     1711 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduled_jobs_response_results_item.py
+-rw-r--r--   0        0        0      149 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduled_jobs_response_status.py
+-rw-r--r--   0        0        0     2294 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response.py
+-rw-r--r--   0        0        0     4066 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response_results.py
+-rw-r--r--   0        0        0     2779 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_0.py
+-rw-r--r--   0        0        0     2799 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_1.py
+-rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response_status.py
+-rw-r--r--   0        0        0     2177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response.py
+-rw-r--r--   0        0        0     5791 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results.py
+-rw-r--r--   0        0        0     1777 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_charts_item.py
+-rw-r--r--   0        0        0     1779 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_dashboards_item.py
+-rw-r--r--   0        0        0     5858 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_logs_item.py
+-rw-r--r--   0        0        0     1392 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_logs_item_details.py
+-rw-r--r--   0        0        0      250 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_logs_item_status.py
+-rw-r--r--   0        0        0      194 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_logs_item_target_type.py
+-rw-r--r--   0        0        0      470 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_logs_item_task.py
+-rw-r--r--   0        0        0     4266 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item.py
+-rw-r--r--   0        0        0     2822 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_0.py
+-rw-r--r--   0        0        0     2842 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_1.py
+-rw-r--r--   0        0        0     1952 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_users_item.py
+-rw-r--r--   0        0        0      149 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_status.py
+-rw-r--r--   0        0        0     2148 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_share_response.py
+-rw-r--r--   0        0        0     3477 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_share_response_results.py
+-rw-r--r--   0        0        0      141 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_share_response_status.py
+-rw-r--r--   0        0        0     2497 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_slack_channels_response.py
+-rw-r--r--   0        0        0     1608 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_slack_channels_response_results_item.py
+-rw-r--r--   0        0        0      149 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_slack_channels_response_status.py
+-rw-r--r--   0        0        0     1993 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response.py
+-rw-r--r--   0        0        0     5415 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results.py
+-rw-r--r--   0        0        0     2283 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_access_item.py
+-rw-r--r--   0        0        0      280 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_access_item_role.py
+-rw-r--r--   0        0        0     7498 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_dashboards_item.py
+-rw-r--r--   0        0        0     1279 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_dashboards_item_updated_by_user.py
+-rw-r--r--   0        0        0     2216 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_dashboards_item_validation_errors_item.py
+-rw-r--r--   0        0        0     7797 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_queries_item.py
+-rw-r--r--   0        0        0      366 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_queries_item_chart_type.py
+-rw-r--r--   0        0        0     1267 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_queries_item_updated_by_user.py
+-rw-r--r--   0        0        0     2201 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_queries_item_validation_errors_item.py
+-rw-r--r--   0        0        0      141 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_status.py
+-rw-r--r--   0        0        0     2563 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_summary_list_response.py
+-rw-r--r--   0        0        0     2535 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_summary_list_response_results_item.py
+-rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_space_summary_list_response_status.py
+-rw-r--r--   0        0        0     2178 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_ssh_key_pair_response.py
+-rw-r--r--   0        0        0     1572 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_ssh_key_pair_response_results.py
+-rw-r--r--   0        0        0      146 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_ssh_key_pair_response_status.py
+-rw-r--r--   0        0        0     1828 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_success_empty.py
+-rw-r--r--   0        0        0      140 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_success_empty_status.py
+-rw-r--r--   0        0        0     2699 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_user_allowed_organizations_response.py
+-rw-r--r--   0        0        0     2048 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_user_allowed_organizations_response_results_item.py
+-rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_user_allowed_organizations_response_status.py
+-rw-r--r--   0        0        0     4920 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response.py
+-rw-r--r--   0        0        0     6933 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_0.py
+-rw-r--r--   0        0        0      367 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_0_chart_type.py
+-rw-r--r--   0        0        0      285 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_0_error_type.py
+-rw-r--r--   0        0        0      214 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_0_source.py
+-rw-r--r--   0        0        0     6161 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_1.py
+-rw-r--r--   0        0        0      285 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_1_error_type.py
+-rw-r--r--   0        0        0      214 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_1_source.py
+-rw-r--r--   0        0        0     4038 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_2.py
+-rw-r--r--   0        0        0      285 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_2_error_type.py
+-rw-r--r--   0        0        0      214 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_2_source.py
+-rw-r--r--   0        0        0      144 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_status.py
+-rw-r--r--   0        0        0     1674 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validation_dismiss_response.py
+-rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/api_validation_dismiss_response_status.py
+-rw-r--r--   0        0        0     5370 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/bigquery_credentials.py
+-rw-r--r--   0        0        0      184 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/bigquery_credentials_priority.py
+-rw-r--r--   0        0        0     1251 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/bigquery_credentials_start_of_week.py
+-rw-r--r--   0        0        0      154 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/bigquery_credentials_type.py
+-rw-r--r--   0        0        0      332 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_kind.py
+-rw-r--r--   0        0        0     4853 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_scheduler.py
+-rw-r--r--   0        0        0      161 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_scheduler_format.py
+-rw-r--r--   0        0        0     2484 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_scheduler_options_type_0.py
+-rw-r--r--   0        0        0      177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_scheduler_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1231 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_scheduler_options_type_1.py
+-rw-r--r--   0        0        0     3723 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_summary.py
+-rw-r--r--   0        0        0      220 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_summary_chart_type.py
+-rw-r--r--   0        0        0      208 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/chart_type.py
+-rw-r--r--   0        0        0      220 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/compact.py
+-rw-r--r--   0        0        0      232 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/compact_or_alias_type_0.py
+-rw-r--r--   0        0        0      272 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/compact_or_alias_type_1.py
+-rw-r--r--   0        0        0      634 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/conditional_operator.py
+-rw-r--r--   0        0        0     2523 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_email_one_time_passcode_response_200.py
+-rw-r--r--   0        0        0     2919 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_email_one_time_passcode_response_200_results.py
+-rw-r--r--   0        0        0     2897 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_email_one_time_passcode_response_200_results_otp.py
+-rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_email_one_time_passcode_response_200_status.py
+-rw-r--r--   0        0        0     1528 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_group_in_organization_json_body.py
+-rw-r--r--   0        0        0     2402 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_group_in_organization_response_200.py
+-rw-r--r--   0        0        0     2383 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_group_in_organization_response_200_results.py
+-rw-r--r--   0        0        0      161 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_group_in_organization_response_200_status.py
+-rw-r--r--   0        0        0     1481 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_organization.py
+-rw-r--r--   0        0        0     1494 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_organization_json_body.py
+-rw-r--r--   0        0        0     1981 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_organization_response_200.py
+-rw-r--r--   0        0        0      154 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_organization_response_200_status.py
+-rw-r--r--   0        0        0     1896 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_project_member.py
+-rw-r--r--   0        0        0      266 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_project_member_role.py
+-rw-r--r--   0        0        0     1624 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_share_url.py
+-rw-r--r--   0        0        0     1652 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_share_url_json_body.py
+-rw-r--r--   0        0        0     2364 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_share_url_response_201.py
+-rw-r--r--   0        0        0     3528 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_share_url_response_201_results.py
+-rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_share_url_response_201_status.py
+-rw-r--r--   0        0        0     2601 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space.py
+-rw-r--r--   0        0        0     2146 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_access_item.py
+-rw-r--r--   0        0        0      268 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_access_item_role.py
+-rw-r--r--   0        0        0     2867 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_json_body.py
+-rw-r--r--   0        0        0     2341 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_json_body_access_item.py
+-rw-r--r--   0        0        0      285 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_json_body_access_item_role.py
+-rw-r--r--   0        0        0     2317 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200.py
+-rw-r--r--   0        0        0     5832 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results.py
+-rw-r--r--   0        0        0     2445 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_access_item.py
+-rw-r--r--   0        0        0      295 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_access_item_role.py
+-rw-r--r--   0        0        0     7875 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item.py
+-rw-r--r--   0        0        0     1345 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_updated_by_user.py
+-rw-r--r--   0        0        0     2300 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_validation_errors_item.py
+-rw-r--r--   0        0        0     8225 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_queries_item.py
+-rw-r--r--   0        0        0      381 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_queries_item_chart_type.py
+-rw-r--r--   0        0        0     1333 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_queries_item_updated_by_user.py
+-rw-r--r--   0        0        0     2285 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_queries_item_validation_errors_item.py
+-rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_status.py
+-rw-r--r--   0        0        0     2312 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_ssh_key_pair_response_201.py
+-rw-r--r--   0        0        0     1605 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_ssh_key_pair_response_201_results.py
+-rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/create_ssh_key_pair_response_201_status.py
+-rw-r--r--   0        0        0     7127 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dashboard_basic_details.py
+-rw-r--r--   0        0        0     1209 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dashboard_basic_details_updated_by_user.py
+-rw-r--r--   0        0        0     2127 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dashboard_basic_details_validation_errors_item.py
+-rw-r--r--   0        0        0     5078 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dashboard_scheduler.py
+-rw-r--r--   0        0        0      165 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dashboard_scheduler_format.py
+-rw-r--r--   0        0        0     2536 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dashboard_scheduler_options_type_0.py
+-rw-r--r--   0        0        0      181 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dashboard_scheduler_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1251 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dashboard_scheduler_options_type_1.py
+-rw-r--r--   0        0        0     3711 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/databricks_credentials.py
+-rw-r--r--   0        0        0     1261 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/databricks_credentials_start_of_week.py
+-rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/databricks_credentials_type.py
+-rw-r--r--   0        0        0     3801 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_azure_dev_ops_project_config.py
+-rw-r--r--   0        0        0     1669 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_azure_dev_ops_project_config_environment_item.py
+-rw-r--r--   0        0        0      170 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_azure_dev_ops_project_config_type.py
+-rw-r--r--   0        0        0     3844 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_bit_bucket_project_config.py
+-rw-r--r--   0        0        0     1656 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_bit_bucket_project_config_environment_item.py
+-rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_bit_bucket_project_config_type.py
+-rw-r--r--   0        0        0     2352 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_ide_project_config.py
+-rw-r--r--   0        0        0      169 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_ide_project_config_type.py
+-rw-r--r--   0        0        0     1638 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_integration.py
+-rw-r--r--   0        0        0     2397 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_metadata_response_metrics.py
+-rw-r--r--   0        0        0     2556 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_metadata_response_metrics_metrics_item.py
+-rw-r--r--   0        0        0     2404 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_metric.py
+-rw-r--r--   0        0        0     3609 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_github_project_config.py
+-rw-r--r--   0        0        0     1638 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_github_project_config_environment_item.py
+-rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_github_project_config_type.py
+-rw-r--r--   0        0        0     3609 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_gitlab_project_config.py
+-rw-r--r--   0        0        0     1638 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_gitlab_project_config_environment_item.py
+-rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_gitlab_project_config_type.py
+-rw-r--r--   0        0        0     2966 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_local_project_config.py
+-rw-r--r--   0        0        0     1633 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_local_project_config_environment_item.py
+-rw-r--r--   0        0        0      146 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_local_project_config_type.py
+-rw-r--r--   0        0        0     2725 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_none_project_config.py
+-rw-r--r--   0        0        0     1628 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_none_project_config_environment_item.py
+-rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_none_project_config_type.py
+-rw-r--r--   0        0        0     1636 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_0_environment_item.py
+-rw-r--r--   0        0        0      146 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_0_type.py
+-rw-r--r--   0        0        0     2325 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_1.py
+-rw-r--r--   0        0        0      166 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_1_type.py
+-rw-r--r--   0        0        0     1636 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_2_environment_item.py
+-rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_2_type.py
+-rw-r--r--   0        0        0     1636 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_3_environment_item.py
+-rw-r--r--   0        0        0      158 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_3_type.py
+-rw-r--r--   0        0        0     1636 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_4_environment_item.py
+-rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_4_type.py
+-rw-r--r--   0        0        0     1636 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_5_environment_item.py
+-rw-r--r--   0        0        0      164 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_5_type.py
+-rw-r--r--   0        0        0     1636 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_6_environment_item.py
+-rw-r--r--   0        0        0      148 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_6_type.py
+-rw-r--r--   0        0        0     1592 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_environment_variable.py
+-rw-r--r--   0        0        0      295 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_type.py
+-rw-r--r--   0        0        0      164 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_type_azuredevops.py
+-rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_type_bitbucket.py
+-rw-r--r--   0        0        0      138 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_type_dbt.py
+-rw-r--r--   0        0        0      166 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_type_dbtcloudide.py
+-rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_type_github.py
+-rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_type_gitlab.py
+-rw-r--r--   0        0        0      141 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_type_none.py
+-rw-r--r--   0        0        0     2143 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_dbt_cloud_integration_settings_response_200.py
+-rw-r--r--   0        0        0      169 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_dbt_cloud_integration_settings_response_200_status.py
+-rw-r--r--   0        0        0     1902 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_group_response_200.py
+-rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_group_response_200_status.py
+-rw-r--r--   0        0        0     1872 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_me_response_200.py
+-rw-r--r--   0        0        0      144 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_me_response_200_status.py
+-rw-r--r--   0        0        0     2005 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_my_organization_response_200.py
+-rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_my_organization_response_200_status.py
+-rw-r--r--   0        0        0     2045 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_organization_member_response_200.py
+-rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_organization_member_response_200_status.py
+-rw-r--r--   0        0        0     1951 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_scheduler_response_201.py
+-rw-r--r--   0        0        0      151 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_scheduler_response_201_status.py
+-rw-r--r--   0        0        0     1902 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_space_response_204.py
+-rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_space_response_204_status.py
+-rw-r--r--   0        0        0     1738 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_validation_dismiss_response_200.py
+-rw-r--r--   0        0        0      159 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/delete_validation_dismiss_response_200_status.py
+-rw-r--r--   0        0        0     1931 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/email_one_time_password.py
+-rw-r--r--   0        0        0     2677 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/email_one_time_password_expiring.py
+-rw-r--r--   0        0        0     2281 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/email_status.py
+-rw-r--r--   0        0        0     2527 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/email_status_expiring.py
+-rw-r--r--   0        0        0     2757 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/email_status_expiring_otp.py
+-rw-r--r--   0        0        0     1898 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/email_status_otp.py
+-rw-r--r--   0        0        0     1574 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/filter_group_response_type_0.py
+-rw-r--r--   0        0        0     1584 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/filter_group_response_type_1.py
+-rw-r--r--   0        0        0     5812 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/filters.py
+-rw-r--r--   0        0        0     1561 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1571 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1546 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1556 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/filters_metrics_type_1.py
+-rw-r--r--   0        0        0     2098 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_csv_url_response_200.py
+-rw-r--r--   0        0        0     1598 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_csv_url_response_200_results.py
+-rw-r--r--   0        0        0      145 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_csv_url_response_200_status.py
+-rw-r--r--   0        0        0     2986 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_integration_settings_response_200.py
+-rw-r--r--   0        0        0     1798 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_integration_settings_response_200_results.py
+-rw-r--r--   0        0        0      166 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_integration_settings_response_200_status.py
+-rw-r--r--   0        0        0     2372 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_metrics_response_200.py
+-rw-r--r--   0        0        0     2467 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_metrics_response_200_results.py
+-rw-r--r--   0        0        0     2587 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_metrics_response_200_results_metrics_item.py
+-rw-r--r--   0        0        0      154 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_metrics_response_200_status.py
+-rw-r--r--   0        0        0     2517 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_email_verification_status_response_200.py
+-rw-r--r--   0        0        0     2914 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_email_verification_status_response_200_results.py
+-rw-r--r--   0        0        0     2894 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_email_verification_status_response_200_results_otp.py
+-rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_email_verification_status_response_200_status.py
+-rw-r--r--   0        0        0     2546 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_group_members_response_200.py
+-rw-r--r--   0        0        0     2236 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_group_members_response_200_results_item.py
+-rw-r--r--   0        0        0      151 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_group_members_response_200_status.py
+-rw-r--r--   0        0        0     2050 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_group_response_200.py
+-rw-r--r--   0        0        0     2292 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_group_response_200_results.py
+-rw-r--r--   0        0        0      144 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_group_response_200_status.py
+-rw-r--r--   0        0        0     5697 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200.py
+-rw-r--r--   0        0        0     7347 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0.py
+-rw-r--r--   0        0        0      385 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0_chart_type.py
+-rw-r--r--   0        0        0      303 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0_error_type.py
+-rw-r--r--   0        0        0      232 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0_source.py
+-rw-r--r--   0        0        0     6464 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1.py
+-rw-r--r--   0        0        0      303 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1_error_type.py
+-rw-r--r--   0        0        0      232 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1_source.py
+-rw-r--r--   0        0        0     4341 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2.py
+-rw-r--r--   0        0        0      303 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2_error_type.py
+-rw-r--r--   0        0        0      232 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2_source.py
+-rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_status.py
+-rw-r--r--   0        0        0     2293 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_my_organization_response_200.py
+-rw-r--r--   0        0        0     3277 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_my_organization_response_200_results.py
+-rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_my_organization_response_200_status.py
+-rw-r--r--   0        0        0     5193 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200.py
+-rw-r--r--   0        0        0     2499 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0.py
+-rw-r--r--   0        0        0     7259 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data.py
+-rw-r--r--   0        0        0     1319 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_updated_by_user.py
+-rw-r--r--   0        0        0     2268 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_validation_errors_item.py
+-rw-r--r--   0        0        0      178 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_type.py
+-rw-r--r--   0        0        0     2499 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1.py
+-rw-r--r--   0        0        0     8178 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data.py
+-rw-r--r--   0        0        0      377 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_chart_type.py
+-rw-r--r--   0        0        0     1319 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_updated_by_user.py
+-rw-r--r--   0        0        0     2268 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_validation_errors_item.py
+-rw-r--r--   0        0        0      170 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_type.py
+-rw-r--r--   0        0        0     2424 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_2.py
+-rw-r--r--   0        0        0     3910 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_2_data.py
+-rw-r--r--   0        0        0      170 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_2_type.py
+-rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_status.py
+-rw-r--r--   0        0        0     2637 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_access_list_response_200.py
+-rw-r--r--   0        0        0     2753 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_access_list_response_200_results_item.py
+-rw-r--r--   0        0        0      289 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_access_list_response_200_results_item_role.py
+-rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_access_list_response_200_status.py
+-rw-r--r--   0        0        0     2109 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200.py
+-rw-r--r--   0        0        0    21254 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results.py
+-rw-r--r--   0        0        0     3430 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0.py
+-rw-r--r--   0        0        0     1773 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0_environment_item.py
+-rw-r--r--   0        0        0      171 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0_type.py
+-rw-r--r--   0        0        0     2571 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_1.py
+-rw-r--r--   0        0        0      191 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_1_type.py
+-rw-r--r--   0        0        0     4057 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2.py
+-rw-r--r--   0        0        0     1773 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2_environment_item.py
+-rw-r--r--   0        0        0      177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2_type.py
+-rw-r--r--   0        0        0     4239 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3.py
+-rw-r--r--   0        0        0     1773 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3_environment_item.py
+-rw-r--r--   0        0        0      183 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3_type.py
+-rw-r--r--   0        0        0     4057 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4.py
+-rw-r--r--   0        0        0     1773 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4_environment_item.py
+-rw-r--r--   0        0        0      177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4_type.py
+-rw-r--r--   0        0        0     4150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5.py
+-rw-r--r--   0        0        0     1773 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5_environment_item.py
+-rw-r--r--   0        0        0      189 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5_type.py
+-rw-r--r--   0        0        0     3205 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6.py
+-rw-r--r--   0        0        0     1773 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6_environment_item.py
+-rw-r--r--   0        0        0      173 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6_type.py
+-rw-r--r--   0        0        0      185 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_type.py
+-rw-r--r--   0        0        0     5637 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0.py
+-rw-r--r--   0        0        0     1437 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0_start_of_week.py
+-rw-r--r--   0        0        0      189 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0_type.py
+-rw-r--r--   0        0        0     6943 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1.py
+-rw-r--r--   0        0        0     1437 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1_start_of_week.py
+-rw-r--r--   0        0        0      187 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1_type.py
+-rw-r--r--   0        0        0     7188 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2.py
+-rw-r--r--   0        0        0     1437 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2_start_of_week.py
+-rw-r--r--   0        0        0      187 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2_type.py
+-rw-r--r--   0        0        0     6229 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3.py
+-rw-r--r--   0        0        0      217 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_priority.py
+-rw-r--r--   0        0        0     1437 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_start_of_week.py
+-rw-r--r--   0        0        0      187 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_type.py
+-rw-r--r--   0        0        0     4320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4.py
+-rw-r--r--   0        0        0     1437 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4_start_of_week.py
+-rw-r--r--   0        0        0      191 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4_type.py
+-rw-r--r--   0        0        0     4257 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5.py
+-rw-r--r--   0        0        0     1437 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5_start_of_week.py
+-rw-r--r--   0        0        0      181 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5_type.py
+-rw-r--r--   0        0        0      146 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_status.py
+-rw-r--r--   0        0        0     2563 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduled_jobs_response_200.py
+-rw-r--r--   0        0        0     1729 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduled_jobs_response_200_results_item.py
+-rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduled_jobs_response_200_status.py
+-rw-r--r--   0        0        0     2334 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_job_status_response_200.py
+-rw-r--r--   0        0        0     1529 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_job_status_response_200_results.py
+-rw-r--r--   0        0        0      157 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_job_status_response_200_status.py
+-rw-r--r--   0        0        0     2243 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200.py
+-rw-r--r--   0        0        0     5924 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results.py
+-rw-r--r--   0        0        0     1795 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_charts_item.py
+-rw-r--r--   0        0        0     1797 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_dashboards_item.py
+-rw-r--r--   0        0        0     5953 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item.py
+-rw-r--r--   0        0        0     1410 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_details.py
+-rw-r--r--   0        0        0      253 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_status.py
+-rw-r--r--   0        0        0      197 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_target_type.py
+-rw-r--r--   0        0        0      473 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_task.py
+-rw-r--r--   0        0        0     4392 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item.py
+-rw-r--r--   0        0        0     2840 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_0.py
+-rw-r--r--   0        0        0     2860 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_1.py
+-rw-r--r--   0        0        0     1970 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_users_item.py
+-rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_status.py
+-rw-r--r--   0        0        0     2160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200.py
+-rw-r--r--   0        0        0     3838 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200_results.py
+-rw-r--r--   0        0        0     2741 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_0.py
+-rw-r--r--   0        0        0     2761 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_1.py
+-rw-r--r--   0        0        0      148 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200_status.py
+-rw-r--r--   0        0        0     2304 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_share_url_response_200.py
+-rw-r--r--   0        0        0     3513 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_share_url_response_200_results.py
+-rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_share_url_response_200_status.py
+-rw-r--r--   0        0        0     2563 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_slack_channels_response_200.py
+-rw-r--r--   0        0        0     1626 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_slack_channels_response_200_results_item.py
+-rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_slack_channels_response_200_status.py
+-rw-r--r--   0        0        0     2050 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200.py
+-rw-r--r--   0        0        0     5502 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results.py
+-rw-r--r--   0        0        0     2317 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_access_item.py
+-rw-r--r--   0        0        0      283 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_access_item_role.py
+-rw-r--r--   0        0        0     7565 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_dashboards_item.py
+-rw-r--r--   0        0        0     1293 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_dashboards_item_updated_by_user.py
+-rw-r--r--   0        0        0     2234 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_dashboards_item_validation_errors_item.py
+-rw-r--r--   0        0        0     7883 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_queries_item.py
+-rw-r--r--   0        0        0      369 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_queries_item_chart_type.py
+-rw-r--r--   0        0        0     1281 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_queries_item_updated_by_user.py
+-rw-r--r--   0        0        0     2219 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_queries_item_validation_errors_item.py
+-rw-r--r--   0        0        0      144 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_status.py
+-rw-r--r--   0        0        0     2051 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/grant_project_access_to_user_json_body.py
+-rw-r--r--   0        0        0      279 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/grant_project_access_to_user_json_body_role.py
+-rw-r--r--   0        0        0     2053 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/grant_project_access_to_user_response_200.py
+-rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/grant_project_access_to_user_response_200_status.py
+-rw-r--r--   0        0        0     2175 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/group.py
+-rw-r--r--   0        0        0     2091 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/group_member.py
+-rw-r--r--   0        0        0     1961 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/join_organization_response_200.py
+-rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/join_organization_response_200_status.py
+-rw-r--r--   0        0        0     2620 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_charts_in_project_response_200.py
+-rw-r--r--   0        0        0     4075 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_charts_in_project_response_200_results_item.py
+-rw-r--r--   0        0        0      249 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_charts_in_project_response_200_results_item_chart_type.py
+-rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_charts_in_project_response_200_status.py
+-rw-r--r--   0        0        0     2705 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_groups_in_organization_response_200.py
+-rw-r--r--   0        0        0     2401 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_groups_in_organization_response_200_results_item.py
+-rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_groups_in_organization_response_200_status.py
+-rw-r--r--   0        0        0     2773 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_my_available_organizations_response_200.py
+-rw-r--r--   0        0        0     2071 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_my_available_organizations_response_200_results_item.py
+-rw-r--r--   0        0        0      164 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_my_available_organizations_response_200_status.py
+-rw-r--r--   0        0        0     2453 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200.py
+-rw-r--r--   0        0        0     6137 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results.py
+-rw-r--r--   0        0        0     4306 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item.py
+-rw-r--r--   0        0        0      194 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item_role_type_0.py
+-rw-r--r--   0        0        0      218 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item_role_type_1.py
+-rw-r--r--   0        0        0      194 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item_role_type_2.py
+-rw-r--r--   0        0        0      182 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_role_type_0.py
+-rw-r--r--   0        0        0      206 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_role_type_1.py
+-rw-r--r--   0        0        0      182 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_role_type_2.py
+-rw-r--r--   0        0        0      182 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_role_type_3.py
+-rw-r--r--   0        0        0      164 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_status.py
+-rw-r--r--   0        0        0     2682 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_members_response_200.py
+-rw-r--r--   0        0        0     3732 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_members_response_200_results_item.py
+-rw-r--r--   0        0        0      314 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_members_response_200_results_item_role.py
+-rw-r--r--   0        0        0      159 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_members_response_200_status.py
+-rw-r--r--   0        0        0     2744 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_projects_response_200.py
+-rw-r--r--   0        0        0     2279 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_projects_response_200_results_item.py
+-rw-r--r--   0        0        0      203 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_projects_response_200_results_item_type.py
+-rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_organization_projects_response_200_status.py
+-rw-r--r--   0        0        0     2620 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_spaces_in_project_response_200.py
+-rw-r--r--   0        0        0     2553 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_spaces_in_project_response_200_results_item.py
+-rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/list_spaces_in_project_response_200_status.py
+-rw-r--r--   0        0        0     2133 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_filter_rule.py
+-rw-r--r--   0        0        0      639 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_filter_rule_operator.py
+-rw-r--r--   0        0        0     1463 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_filter_rule_target.py
+-rw-r--r--   0        0        0     5557 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response.py
+-rw-r--r--   0        0        0     7432 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item.py
+-rw-r--r--   0        0        0      265 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      305 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0     2769 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item.py
+-rw-r--r--   0        0        0      674 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item_operator.py
+-rw-r--r--   0        0        0     1653 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item_target.py
+-rw-r--r--   0        0        0      417 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     7034 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters.py
+-rw-r--r--   0        0        0     1665 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1675 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1650 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1660 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     1690 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_sorts_item.py
+-rw-r--r--   0        0        0     3183 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_table_calculations_item.py
+-rw-r--r--   0        0        0     4643 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_table_calculations_item_format.py
+-rw-r--r--   0        0        0      266 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_table_calculations_item_format_compact.py
+-rw-r--r--   0        0        0      324 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      251 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0      383 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/metric_type.py
+-rw-r--r--   0        0        0      284 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/number_separator.py
+-rw-r--r--   0        0        0     5630 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid.py
+-rw-r--r--   0        0        0     4125 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item.py
+-rw-r--r--   0        0        0      187 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item_role_type_0.py
+-rw-r--r--   0        0        0      211 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item_role_type_1.py
+-rw-r--r--   0        0        0      187 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item_role_type_2.py
+-rw-r--r--   0        0        0      175 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_role_type_0.py
+-rw-r--r--   0        0        0      199 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_role_type_1.py
+-rw-r--r--   0        0        0      175 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_role_type_2.py
+-rw-r--r--   0        0        0      175 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_role_type_3.py
+-rw-r--r--   0        0        0     6420 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0      224 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_priority.py
+-rw-r--r--   0        0        0     1469 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      194 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     4520 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1479 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      200 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     7338 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1469 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      194 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     7093 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1469 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      194 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     5805 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1474 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      197 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     4353 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1454 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      185 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     3794 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_validation_response_base_name.py
+-rw-r--r--   0        0        0      280 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_validation_response_base_name_error_type.py
+-rw-r--r--   0        0        0      209 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/omit_validation_response_base_name_source.py
+-rw-r--r--   0        0        0     3147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization.py
+-rw-r--r--   0        0        0     3507 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_profile.py
+-rw-r--r--   0        0        0      294 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_profile_role.py
+-rw-r--r--   0        0        0     1674 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_profile_update.py
+-rw-r--r--   0        0        0      300 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_profile_update_role.py
+-rw-r--r--   0        0        0      287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_role.py
+-rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_role_editor.py
+-rw-r--r--   0        0        0      190 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_role_interactiveviewer.py
+-rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_role_member.py
+-rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_member_role_viewer.py
+-rw-r--r--   0        0        0     1980 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_project.py
+-rw-r--r--   0        0        0      176 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/organization_project_type.py
+-rw-r--r--   0        0        0     2713 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py
+-rw-r--r--   0        0        0     6971 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py
+-rw-r--r--   0        0        0     5108 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item.py
+-rw-r--r--   0        0        0      218 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item_role_type_0.py
+-rw-r--r--   0        0        0      242 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item_role_type_1.py
+-rw-r--r--   0        0        0      218 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item_role_type_2.py
+-rw-r--r--   0        0        0      206 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_role_type_0.py
+-rw-r--r--   0        0        0      230 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_role_type_1.py
+-rw-r--r--   0        0        0      206 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_role_type_2.py
+-rw-r--r--   0        0        0      206 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_role_type_3.py
+-rw-r--r--   0        0        0     7661 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0      267 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_priority.py
+-rw-r--r--   0        0        0     1728 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      231 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     5374 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1748 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      245 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     1769 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py
+-rw-r--r--   0        0        0     1493 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_group_name.py
+-rw-r--r--   0        0        0     8285 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1728 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      231 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     8036 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1728 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      231 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     6654 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1738 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      235 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     5124 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names.py
+-rw-r--r--   0        0        0     1693 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py
+-rw-r--r--   0        0        0      219 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names_type.py
+-rw-r--r--   0        0        0     9895 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors.py
+-rw-r--r--   0        0        0     1834 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py
+-rw-r--r--   0        0        0     2946 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py
+-rw-r--r--   0        0        0     7951 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     1840 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py
+-rw-r--r--   0        0        0     1460 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_group_name.py
+-rw-r--r--   0        0        0     1494 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_organization_name.py
+-rw-r--r--   0        0        0     1926 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     3654 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py
+-rw-r--r--   0        0        0     5491 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py
+-rw-r--r--   0        0        0     1610 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py
+-rw-r--r--   0        0        0     1685 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_share_url_path_or_params.py
+-rw-r--r--   0        0        0     2537 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py
+-rw-r--r--   0        0        0     3330 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py
+-rw-r--r--   0        0        0    11635 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors.py
+-rw-r--r--   0        0        0      496 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_chart_type.py
+-rw-r--r--   0        0        0     1838 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py
+-rw-r--r--   0        0        0     2952 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py
+-rw-r--r--   0        0        0     1547 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_ssh_key_pair_public_key.py
+-rw-r--r--   0        0        0     4356 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py
+-rw-r--r--   0        0        0      314 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name_error_type.py
+-rw-r--r--   0        0        0      243 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name_source.py
+-rw-r--r--   0        0        0     2194 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py
+-rw-r--r--   0        0        0     1227 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_0_data_updated_by_user.py
+-rw-r--r--   0        0        0     2151 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_0_data_validation_errors_item.py
+-rw-r--r--   0        0        0      157 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_0_type.py
+-rw-r--r--   0        0        0      356 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_1_data_chart_type.py
+-rw-r--r--   0        0        0     1227 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_1_data_updated_by_user.py
+-rw-r--r--   0        0        0     2151 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_1_data_validation_errors_item.py
+-rw-r--r--   0        0        0      149 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_1_type.py
+-rw-r--r--   0        0        0     3793 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_2_data.py
+-rw-r--r--   0        0        0      149 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_2_type.py
+-rw-r--r--   0        0        0     2212 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body.py
+-rw-r--r--   0        0        0     7343 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters.py
+-rw-r--r--   0        0        0     1696 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1706 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1681 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1691 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     2243 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200.py
+-rw-r--r--   0        0        0     2220 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results.py
+-rw-r--r--   0        0        0     6589 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query.py
+-rw-r--r--   0        0        0     8425 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item.py
+-rw-r--r--   0        0        0      291 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      331 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0     3254 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item.py
+-rw-r--r--   0        0        0      700 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py
+-rw-r--r--   0        0        0     1822 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_target.py
+-rw-r--r--   0        0        0      443 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     8643 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters.py
+-rw-r--r--   0        0        0     1810 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1820 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1795 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1805 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     1835 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_sorts_item.py
+-rw-r--r--   0        0        0     3546 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item.py
+-rw-r--r--   0        0        0     5245 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format.py
+-rw-r--r--   0        0        0      292 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format_compact.py
+-rw-r--r--   0        0        0      350 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      277 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_status.py
+-rw-r--r--   0        0        0     5967 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body.py
+-rw-r--r--   0        0        0     7477 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item.py
+-rw-r--r--   0        0        0      266 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      306 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0     2795 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item.py
+-rw-r--r--   0        0        0      675 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item_operator.py
+-rw-r--r--   0        0        0     1664 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item_target.py
+-rw-r--r--   0        0        0      418 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     1855 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_filters.py
+-rw-r--r--   0        0        0     1701 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_sorts_item.py
+-rw-r--r--   0        0        0     3206 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_table_calculations_item.py
+-rw-r--r--   0        0        0     4677 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_table_calculations_item_format.py
+-rw-r--r--   0        0        0      267 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_table_calculations_item_format_compact.py
+-rw-r--r--   0        0        0      325 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      252 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0     2166 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200.py
+-rw-r--r--   0        0        0     2172 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results.py
+-rw-r--r--   0        0        0     6457 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query.py
+-rw-r--r--   0        0        0     8263 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item.py
+-rw-r--r--   0        0        0      287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      327 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0     3168 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item.py
+-rw-r--r--   0        0        0      696 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py
+-rw-r--r--   0        0        0     1802 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.py
+-rw-r--r--   0        0        0      439 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     8417 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters.py
+-rw-r--r--   0        0        0     1790 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1800 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1775 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1785 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     1815 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_sorts_item.py
+-rw-r--r--   0        0        0     3494 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item.py
+-rw-r--r--   0        0        0     5157 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format.py
+-rw-r--r--   0        0        0      288 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format_compact.py
+-rw-r--r--   0        0        0      346 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      273 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0      148 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_status.py
+-rw-r--r--   0        0        0     6528 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body.py
+-rw-r--r--   0        0        0     8001 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item.py
+-rw-r--r--   0        0        0      280 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0     3029 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item.py
+-rw-r--r--   0        0        0      689 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_operator.py
+-rw-r--r--   0        0        0     1740 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_target.py
+-rw-r--r--   0        0        0      432 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     1931 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_filters.py
+-rw-r--r--   0        0        0     1777 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_sorts_item.py
+-rw-r--r--   0        0        0     3398 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item.py
+-rw-r--r--   0        0        0     4997 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format.py
+-rw-r--r--   0        0        0      281 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format_compact.py
+-rw-r--r--   0        0        0      339 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      266 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0     2425 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200.py
+-rw-r--r--   0        0        0     2350 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results.py
+-rw-r--r--   0        0        0     7047 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query.py
+-rw-r--r--   0        0        0     8971 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item.py
+-rw-r--r--   0        0        0      301 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      341 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0     3456 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item.py
+-rw-r--r--   0        0        0      710 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py
+-rw-r--r--   0        0        0     1934 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.py
+-rw-r--r--   0        0        0      453 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     9367 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters.py
+-rw-r--r--   0        0        0     1890 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_0.py
+-rw-r--r--   0        0        0     1900 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_1.py
+-rw-r--r--   0        0        0     1875 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_0.py
+-rw-r--r--   0        0        0     1885 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_1.py
+-rw-r--r--   0        0        0     1891 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_sorts_item.py
+-rw-r--r--   0        0        0     3740 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item.py
+-rw-r--r--   0        0        0     5635 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format.py
+-rw-r--r--   0        0        0      302 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format_compact.py
+-rw-r--r--   0        0        0      360 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_status.py
+-rw-r--r--   0        0        0     6543 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/postgres_credentials.py
+-rw-r--r--   0        0        0     1251 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/postgres_credentials_start_of_week.py
+-rw-r--r--   0        0        0      154 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/postgres_credentials_type.py
+-rw-r--r--   0        0        0    17362 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project.py
+-rw-r--r--   0        0        0     3035 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_0.py
+-rw-r--r--   0        0        0     1656 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_0_environment_item.py
+-rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_0_type.py
+-rw-r--r--   0        0        0     2361 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_1.py
+-rw-r--r--   0        0        0      170 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_1_type.py
+-rw-r--r--   0        0        0     3662 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_2.py
+-rw-r--r--   0        0        0     1656 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_2_environment_item.py
+-rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_2_type.py
+-rw-r--r--   0        0        0     3844 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_3.py
+-rw-r--r--   0        0        0     1656 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_3_environment_item.py
+-rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_3_type.py
+-rw-r--r--   0        0        0     3662 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_4.py
+-rw-r--r--   0        0        0     1656 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_4_environment_item.py
+-rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_4_type.py
+-rw-r--r--   0        0        0     3755 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_5.py
+-rw-r--r--   0        0        0     1656 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_5_environment_item.py
+-rw-r--r--   0        0        0      168 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_5_type.py
+-rw-r--r--   0        0        0     2810 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_6.py
+-rw-r--r--   0        0        0     1656 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_6_environment_item.py
+-rw-r--r--   0        0        0      152 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_6_type.py
+-rw-r--r--   0        0        0     2504 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_member_profile.py
+-rw-r--r--   0        0        0      267 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_member_profile_role.py
+-rw-r--r--   0        0        0      260 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_member_role.py
+-rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_member_role_editor.py
+-rw-r--r--   0        0        0      185 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_member_role_interactiveviewer.py
+-rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_member_role_viewer.py
+-rw-r--r--   0        0        0      164 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_type.py
+-rw-r--r--   0        0        0     5235 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_0.py
+-rw-r--r--   0        0        0     1320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_0_start_of_week.py
+-rw-r--r--   0        0        0      168 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_0_type.py
+-rw-r--r--   0        0        0     6541 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_1.py
+-rw-r--r--   0        0        0     1320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_1_start_of_week.py
+-rw-r--r--   0        0        0      166 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_1_type.py
+-rw-r--r--   0        0        0     6786 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_2.py
+-rw-r--r--   0        0        0     1320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_2_start_of_week.py
+-rw-r--r--   0        0        0      166 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_2_type.py
+-rw-r--r--   0        0        0     5697 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_3.py
+-rw-r--r--   0        0        0      196 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_3_priority.py
+-rw-r--r--   0        0        0     1320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_3_start_of_week.py
+-rw-r--r--   0        0        0      166 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_3_type.py
+-rw-r--r--   0        0        0     3918 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_4.py
+-rw-r--r--   0        0        0     1320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_4_start_of_week.py
+-rw-r--r--   0        0        0      170 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_4_type.py
+-rw-r--r--   0        0        0     3855 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_5.py
+-rw-r--r--   0        0        0     1320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_5_start_of_week.py
+-rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_5_type.py
+-rw-r--r--   0        0        0     1222 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/record_string_any.py
+-rw-r--r--   0        0        0     6298 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/redshift_credentials.py
+-rw-r--r--   0        0        0     1251 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/redshift_credentials_start_of_week.py
+-rw-r--r--   0        0        0      154 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/redshift_credentials_type.py
+-rw-r--r--   0        0        0     1999 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/remove_user_from_group_response_200.py
+-rw-r--r--   0        0        0      155 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/remove_user_from_group_response_200_status.py
+-rw-r--r--   0        0        0     2066 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item.py
+-rw-r--r--   0        0        0     7618 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item_data.py
+-rw-r--r--   0        0        0      357 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item_data_chart_type.py
+-rw-r--r--   0        0        0     1229 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item_data_updated_by_user.py
+-rw-r--r--   0        0        0     2153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item_data_validation_errors_item.py
+-rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item_type.py
+-rw-r--r--   0        0        0     2159 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item.py
+-rw-r--r--   0        0        0     6904 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item_data.py
+-rw-r--r--   0        0        0     1245 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item_data_updated_by_user.py
+-rw-r--r--   0        0        0     2173 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item_data_validation_errors_item.py
+-rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item_type.py
+-rw-r--r--   0        0        0      193 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_item_type.py
+-rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_item_type_chart.py
+-rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_item_type_dashboard.py
+-rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_item_type_space.py
+-rw-r--r--   0        0        0     2003 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_space_item.py
+-rw-r--r--   0        0        0     3795 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_space_item_data.py
+-rw-r--r--   0        0        0      150 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/resource_view_space_item_type.py
+-rw-r--r--   0        0        0     2073 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/revoke_project_access_for_user_response_200.py
+-rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/revoke_project_access_for_user_response_200_status.py
+-rw-r--r--   0        0        0     2053 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/revoke_space_access_for_user_response_200.py
+-rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/revoke_space_access_for_user_response_200_status.py
+-rw-r--r--   0        0        0     5680 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request.py
+-rw-r--r--   0        0        0     7266 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item.py
+-rw-r--r--   0        0        0      261 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item_compact_type_0.py
+-rw-r--r--   0        0        0      301 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item_compact_type_1.py
+-rw-r--r--   0        0        0     2705 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item_filters_item.py
+-rw-r--r--   0        0        0      670 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item_filters_item_operator.py
+-rw-r--r--   0        0        0     1633 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item_filters_item_target.py
+-rw-r--r--   0        0        0      413 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item_type.py
+-rw-r--r--   0        0        0     1824 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_filters.py
+-rw-r--r--   0        0        0     1670 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_sorts_item.py
+-rw-r--r--   0        0        0     3131 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_table_calculations_item.py
+-rw-r--r--   0        0        0     4555 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_table_calculations_item_format.py
+-rw-r--r--   0        0        0      262 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_table_calculations_item_format_compact.py
+-rw-r--r--   0        0        0      320 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_table_calculations_item_format_separator.py
+-rw-r--r--   0        0        0      247 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_table_calculations_item_format_type.py
+-rw-r--r--   0        0        0     1589 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduled_jobs.py
+-rw-r--r--   0        0        0     3502 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_and_targets.py
+-rw-r--r--   0        0        0     2680 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_and_targets_targets_item_type_0.py
+-rw-r--r--   0        0        0     2700 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_and_targets_targets_item_type_1.py
+-rw-r--r--   0        0        0     4849 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_base.py
+-rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_base_format.py
+-rw-r--r--   0        0        0     2471 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_base_options_type_0.py
+-rw-r--r--   0        0        0      176 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_base_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1226 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_base_options_type_1.py
+-rw-r--r--   0        0        0     2376 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_csv_options.py
+-rw-r--r--   0        0        0      170 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_csv_options_limit_type_1.py
+-rw-r--r--   0        0        0     2613 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_email_target.py
+-rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_format.py
+-rw-r--r--   0        0        0     1200 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_image_options.py
+-rw-r--r--   0        0        0      223 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_job_status.py
+-rw-r--r--   0        0        0     4954 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_log.py
+-rw-r--r--   0        0        0     1242 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_log_details.py
+-rw-r--r--   0        0        0      223 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_log_status.py
+-rw-r--r--   0        0        0      167 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_log_target_type.py
+-rw-r--r--   0        0        0      443 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_log_task.py
+-rw-r--r--   0        0        0     2415 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_options_type_0.py
+-rw-r--r--   0        0        0      172 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1203 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_options_type_1.py
+-rw-r--r--   0        0        0     2593 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_slack_target.py
+-rw-r--r--   0        0        0      161 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_0_format.py
+-rw-r--r--   0        0        0     2488 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_0_options_type_0.py
+-rw-r--r--   0        0        0      177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_0_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1234 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_0_options_type_1.py
+-rw-r--r--   0        0        0      161 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_1_format.py
+-rw-r--r--   0        0        0     2488 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_1_options_type_0.py
+-rw-r--r--   0        0        0      177 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_1_options_type_0_limit_type_1.py
+-rw-r--r--   0        0        0     1234 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_1_options_type_1.py
+-rw-r--r--   0        0        0     5079 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs.py
+-rw-r--r--   0        0        0     1701 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_charts_item.py
+-rw-r--r--   0        0        0     1703 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_dashboards_item.py
+-rw-r--r--   0        0        0     5415 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_logs_item.py
+-rw-r--r--   0        0        0     1316 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_logs_item_details.py
+-rw-r--r--   0        0        0      236 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_logs_item_status.py
+-rw-r--r--   0        0        0      180 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_logs_item_target_type.py
+-rw-r--r--   0        0        0      456 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_logs_item_task.py
+-rw-r--r--   0        0        0     3862 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_schedulers_item.py
+-rw-r--r--   0        0        0     2746 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_0.py
+-rw-r--r--   0        0        0     2766 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_1.py
+-rw-r--r--   0        0        0     1876 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_users_item.py
+-rw-r--r--   0        0        0     3396 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/share_url.py
+-rw-r--r--   0        0        0     1481 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/slack_channel.py
+-rw-r--r--   0        0        0     5010 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/snowflake_credentials.py
+-rw-r--r--   0        0        0     1256 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/snowflake_credentials_start_of_week.py
+-rw-r--r--   0        0        0      157 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/snowflake_credentials_type.py
+-rw-r--r--   0        0        0     1586 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/sort_field.py
+-rw-r--r--   0        0        0     4794 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space.py
+-rw-r--r--   0        0        0     2082 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_access_item.py
+-rw-r--r--   0        0        0      262 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_access_item_role.py
+-rw-r--r--   0        0        0     6938 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_dashboard.py
+-rw-r--r--   0        0        0     1179 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_dashboard_updated_by_user.py
+-rw-r--r--   0        0        0     2089 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_dashboard_validation_errors_item.py
+-rw-r--r--   0        0        0     7087 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_dashboards_item.py
+-rw-r--r--   0        0        0     1201 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_dashboards_item_updated_by_user.py
+-rw-r--r--   0        0        0     2117 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_dashboards_item_validation_errors_item.py
+-rw-r--r--   0        0        0     7266 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_queries_item.py
+-rw-r--r--   0        0        0      348 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_queries_item_chart_type.py
+-rw-r--r--   0        0        0     1189 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_queries_item_updated_by_user.py
+-rw-r--r--   0        0        0     2102 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_queries_item_validation_errors_item.py
+-rw-r--r--   0        0        0     7060 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_query.py
+-rw-r--r--   0        0        0      342 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_query_chart_type.py
+-rw-r--r--   0        0        0     1163 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_query_updated_by_user.py
+-rw-r--r--   0        0        0     2069 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_query_validation_errors_item.py
+-rw-r--r--   0        0        0     2028 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_share.py
+-rw-r--r--   0        0        0      257 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_share_role.py
+-rw-r--r--   0        0        0     2390 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/space_summary.py
+-rw-r--r--   0        0        0      242 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/table_calculation_format_compact.py
+-rw-r--r--   0        0        0      300 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/table_calculation_format_separator.py
+-rw-r--r--   0        0        0      227 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/table_calculation_format_type.py
+-rw-r--r--   0        0        0     3516 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/trino_credentials.py
+-rw-r--r--   0        0        0     1236 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/trino_credentials_start_of_week.py
+-rw-r--r--   0        0        0      145 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/trino_credentials_type.py
+-rw-r--r--   0        0        0     5066 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains.py
+-rw-r--r--   0        0        0     3751 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_projects_item.py
+-rw-r--r--   0        0        0      173 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_projects_item_role_type_0.py
+-rw-r--r--   0        0        0      197 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_projects_item_role_type_1.py
+-rw-r--r--   0        0        0      173 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_projects_item_role_type_2.py
+-rw-r--r--   0        0        0      161 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_role_type_0.py
+-rw-r--r--   0        0        0      185 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_role_type_1.py
+-rw-r--r--   0        0        0      161 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_role_type_2.py
+-rw-r--r--   0        0        0      161 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_role_type_3.py
+-rw-r--r--   0        0        0     3040 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_dbt_cloud_integration_settings_response_200.py
+-rw-r--r--   0        0        0     1813 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_dbt_cloud_integration_settings_response_200_results.py
+-rw-r--r--   0        0        0      169 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_dbt_cloud_integration_settings_response_200_status.py
+-rw-r--r--   0        0        0     1447 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_group.py
+-rw-r--r--   0        0        0     1493 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_group_json_body.py
+-rw-r--r--   0        0        0     2126 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_group_response_200.py
+-rw-r--r--   0        0        0     2307 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_group_response_200_results.py
+-rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_group_response_200_status.py
+-rw-r--r--   0        0        0     2575 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_my_organization_json_body.py
+-rw-r--r--   0        0        0     2005 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_my_organization_response_200.py
+-rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_my_organization_response_200_status.py
+-rw-r--r--   0        0        0     2520 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization.py
+-rw-r--r--   0        0        0     5551 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body.py
+-rw-r--r--   0        0        0     4100 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_projects_item.py
+-rw-r--r--   0        0        0      186 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_projects_item_role_type_0.py
+-rw-r--r--   0        0        0      210 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_projects_item_role_type_1.py
+-rw-r--r--   0        0        0      186 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_projects_item_role_type_2.py
+-rw-r--r--   0        0        0      174 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_role_type_0.py
+-rw-r--r--   0        0        0      198 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_role_type_1.py
+-rw-r--r--   0        0        0      174 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_role_type_2.py
+-rw-r--r--   0        0        0      174 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_role_type_3.py
+-rw-r--r--   0        0        0     2487 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200.py
+-rw-r--r--   0        0        0     6215 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results.py
+-rw-r--r--   0        0        0     4356 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item.py
+-rw-r--r--   0        0        0      196 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item_role_type_0.py
+-rw-r--r--   0        0        0      220 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item_role_type_1.py
+-rw-r--r--   0        0        0      196 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item_role_type_2.py
+-rw-r--r--   0        0        0      184 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_role_type_0.py
+-rw-r--r--   0        0        0      208 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_role_type_1.py
+-rw-r--r--   0        0        0      184 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_role_type_2.py
+-rw-r--r--   0        0        0      184 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_role_type_3.py
+-rw-r--r--   0        0        0      166 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_status.py
+-rw-r--r--   0        0        0     1715 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_json_body.py
+-rw-r--r--   0        0        0      301 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_json_body_role.py
+-rw-r--r--   0        0        0     2430 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_response_200.py
+-rw-r--r--   0        0        0     3698 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_response_200_results.py
+-rw-r--r--   0        0        0      311 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_response_200_results_role.py
+-rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_response_200_status.py
+-rw-r--r--   0        0        0     2066 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_item_order.py
+-rw-r--r--   0        0        0     1798 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_item_order_data.py
+-rw-r--r--   0        0        0      198 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_item_order_type.py
+-rw-r--r--   0        0        0     2356 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_json_body_item.py
+-rw-r--r--   0        0        0     1872 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_json_body_item_data.py
+-rw-r--r--   0        0        0      211 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_json_body_item_type.py
+-rw-r--r--   0        0        0     5525 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200.py
+-rw-r--r--   0        0        0     2641 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0.py
+-rw-r--r--   0        0        0     7522 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data.py
+-rw-r--r--   0        0        0     1353 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_updated_by_user.py
+-rw-r--r--   0        0        0     2311 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_validation_errors_item.py
+-rw-r--r--   0        0        0      186 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_type.py
+-rw-r--r--   0        0        0     2641 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1.py
+-rw-r--r--   0        0        0     8490 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data.py
+-rw-r--r--   0        0        0      385 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_chart_type.py
+-rw-r--r--   0        0        0     1353 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_updated_by_user.py
+-rw-r--r--   0        0        0     2311 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_validation_errors_item.py
+-rw-r--r--   0        0        0      178 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_type.py
+-rw-r--r--   0        0        0     2566 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2.py
+-rw-r--r--   0        0        0     3953 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2_data.py
+-rw-r--r--   0        0        0      178 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2_type.py
+-rw-r--r--   0        0        0      158 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_status.py
+-rw-r--r--   0        0        0     1716 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_project_access_for_user_json_body.py
+-rw-r--r--   0        0        0      281 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_project_access_for_user_json_body_role.py
+-rw-r--r--   0        0        0     2073 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_project_access_for_user_response_200.py
+-rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_project_access_for_user_response_200_status.py
+-rw-r--r--   0        0        0     1541 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_project_member.py
+-rw-r--r--   0        0        0      266 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_project_member_role.py
+-rw-r--r--   0        0        0     2220 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201.py
+-rw-r--r--   0        0        0     3910 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201_results.py
+-rw-r--r--   0        0        0     2756 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_0.py
+-rw-r--r--   0        0        0     2776 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_1.py
+-rw-r--r--   0        0        0      151 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201_status.py
+-rw-r--r--   0        0        0     1556 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space.py
+-rw-r--r--   0        0        0     1602 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_json_body.py
+-rw-r--r--   0        0        0     2126 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200.py
+-rw-r--r--   0        0        0     5580 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results.py
+-rw-r--r--   0        0        0     2347 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_access_item.py
+-rw-r--r--   0        0        0      286 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_access_item_role.py
+-rw-r--r--   0        0        0     7625 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_dashboards_item.py
+-rw-r--r--   0        0        0     1305 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_dashboards_item_updated_by_user.py
+-rw-r--r--   0        0        0     2249 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_dashboards_item_validation_errors_item.py
+-rw-r--r--   0        0        0     7961 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_queries_item.py
+-rw-r--r--   0        0        0      372 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_queries_item_chart_type.py
+-rw-r--r--   0        0        0     1293 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_queries_item_updated_by_user.py
+-rw-r--r--   0        0        0     2234 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_queries_item_validation_errors_item.py
+-rw-r--r--   0        0        0      147 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_status.py
+-rw-r--r--   0        0        0     1119 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/updated_by_user.py
+-rw-r--r--   0        0        0     1921 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/user_allowed_organization.py
+-rw-r--r--   0        0        0     1837 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validate_project_json_body.py
+-rw-r--r--   0        0        0     2220 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validate_project_response_200.py
+-rw-r--r--   0        0        0     1491 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validate_project_response_200_results.py
+-rw-r--r--   0        0        0      151 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validate_project_response_200_status.py
+-rw-r--r--   0        0        0     6761 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_chart_response.py
+-rw-r--r--   0        0        0      360 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_chart_response_chart_type.py
+-rw-r--r--   0        0        0      278 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_chart_response_error_type.py
+-rw-r--r--   0        0        0      207 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_chart_response_source.py
+-rw-r--r--   0        0        0     6098 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_dashboard_response.py
+-rw-r--r--   0        0        0      282 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_dashboard_response_error_type.py
+-rw-r--r--   0        0        0      211 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_dashboard_response_source.py
+-rw-r--r--   0        0        0     3911 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_table_response.py
+-rw-r--r--   0        0        0      278 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_table_response_error_type.py
+-rw-r--r--   0        0        0      207 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_table_response_source.py
+-rw-r--r--   0        0        0      260 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_error_type.py
+-rw-r--r--   0        0        0     3711 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_base.py
+-rw-r--r--   0        0        0      272 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_base_error_type.py
+-rw-r--r--   0        0        0      201 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_base_source.py
+-rw-r--r--   0        0        0     6642 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_0.py
+-rw-r--r--   0        0        0      355 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_0_chart_type.py
+-rw-r--r--   0        0        0      273 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_0_error_type.py
+-rw-r--r--   0        0        0      202 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_0_source.py
+-rw-r--r--   0        0        0     5945 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_1.py
+-rw-r--r--   0        0        0      273 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_1_error_type.py
+-rw-r--r--   0        0        0      202 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_1_source.py
+-rw-r--r--   0        0        0     3822 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_2.py
+-rw-r--r--   0        0        0      273 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_2_error_type.py
+-rw-r--r--   0        0        0      202 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_2_source.py
+-rw-r--r--   0        0        0      193 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_source_type.py
+-rw-r--r--   0        0        0     1995 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/validation_summary.py
+-rw-r--r--   0        0        0     2525 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/view_statistics.py
+-rw-r--r--   0        0        0     1287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_0_start_of_week.py
+-rw-r--r--   0        0        0      162 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_0_type.py
+-rw-r--r--   0        0        0     1287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_1_start_of_week.py
+-rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_1_type.py
+-rw-r--r--   0        0        0     1287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_2_start_of_week.py
+-rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_2_type.py
+-rw-r--r--   0        0        0      190 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_3_priority.py
+-rw-r--r--   0        0        0     1287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_3_start_of_week.py
+-rw-r--r--   0        0        0      160 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_3_type.py
+-rw-r--r--   0        0        0     1287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_4_start_of_week.py
+-rw-r--r--   0        0        0      164 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_4_type.py
+-rw-r--r--   0        0        0     1287 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_5_start_of_week.py
+-rw-r--r--   0        0        0      154 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_5_type.py
+-rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_types_bigquery.py
+-rw-r--r--   0        0        0      159 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_types_databricks.py
+-rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_types_postgres.py
+-rw-r--r--   0        0        0      153 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_types_redshift.py
+-rw-r--r--   0        0        0      156 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_types_snowflake.py
+-rw-r--r--   0        0        0      144 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/warehouse_types_trino.py
+-rw-r--r--   0        0        0      225 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/models/week_day.py
+-rw-r--r--   0        0        0       26 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/py.typed
+-rw-r--r--   0        0        0      993 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/lightdash_client/types.py
+-rw-r--r--   0        0        0     1862 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/pyproject.toml
+-rw-r--r--   0        0        0      830 2023-07-11 01:36:57.000000 lightdash_client_python-0.651.2/setup.py
+-rw-r--r--   0        0        0     5168 1970-01-01 00:00:00.000000 lightdash_client_python-0.651.2/PKG-INFO
```

### Comparing `lightdash_client_python-0.640.1/.openapi-generator-ignore` & `lightdash_client_python-0.651.2/.openapi-generator-ignore`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/LICENSE` & `lightdash_client_python-0.651.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/README.md` & `lightdash_client_python-0.651.2/README.md`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/charts/post_chart_results.py` & `lightdash_client_python-0.651.2/lightdash_client/api/charts/post_chart_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/content/get_pinned_items.py` & `lightdash_client_python-0.651.2/lightdash_client/api/content/get_pinned_items.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/content/update_pinned_items_order.py` & `lightdash_client_python-0.651.2/lightdash_client/api/content/update_pinned_items_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/exploring/post_run_query.py` & `lightdash_client_python-0.651.2/lightdash_client/api/exploring/post_run_query.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/exploring/post_run_underlying_data_query.py` & `lightdash_client_python-0.651.2/lightdash_client/api/exploring/post_run_underlying_data_query.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/exports/get_csv_url.py` & `lightdash_client_python-0.651.2/lightdash_client/api/exports/get_csv_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.651.2/lightdash_client/api/integrations/delete_dbt_cloud_integration_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.651.2/lightdash_client/api/integrations/get_dbt_cloud_integration_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/integrations/get_dbt_cloud_metrics.py` & `lightdash_client_python-0.651.2/lightdash_client/api/integrations/get_dbt_cloud_metrics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/integrations/get_slack_channels.py` & `lightdash_client_python-0.651.2/lightdash_client/api/integrations/get_slack_channels.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.651.2/lightdash_client/api/integrations/update_dbt_cloud_integration_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/my_account/create_email_one_time_passcode.py` & `lightdash_client_python-0.651.2/lightdash_client/api/my_account/create_email_one_time_passcode.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/my_account/delete_me.py` & `lightdash_client_python-0.651.2/lightdash_client/api/my_account/delete_me.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/my_account/get_email_verification_status.py` & `lightdash_client_python-0.651.2/lightdash_client/api/my_account/get_email_verification_status.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/my_account/join_organization.py` & `lightdash_client_python-0.651.2/lightdash_client/api/my_account/join_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/my_account/list_my_available_organizations.py` & `lightdash_client_python-0.651.2/lightdash_client/api/my_account/list_my_available_organizations.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/organizations/create_group_in_organization.py` & `lightdash_client_python-0.651.2/lightdash_client/api/organizations/create_group_in_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/organizations/create_organization.py` & `lightdash_client_python-0.651.2/lightdash_client/api/organizations/create_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/organizations/delete_my_organization.py` & `lightdash_client_python-0.651.2/lightdash_client/api/organizations/delete_my_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/organizations/delete_organization_member.py` & `lightdash_client_python-0.651.2/lightdash_client/api/organizations/delete_organization_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/organizations/get_my_organization.py` & `lightdash_client_python-0.651.2/lightdash_client/api/organizations/get_my_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/organizations/list_groups_in_organization.py` & `lightdash_client_python-0.651.2/lightdash_client/api/organizations/list_groups_in_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/organizations/list_organization_email_domains.py` & `lightdash_client_python-0.651.2/lightdash_client/api/organizations/list_organization_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/organizations/list_organization_members.py` & `lightdash_client_python-0.651.2/lightdash_client/api/organizations/list_organization_members.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/organizations/list_organization_projects.py` & `lightdash_client_python-0.651.2/lightdash_client/api/organizations/list_organization_projects.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/organizations/update_my_organization.py` & `lightdash_client_python-0.651.2/lightdash_client/api/organizations/update_my_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/organizations/update_organization_email_domains.py` & `lightdash_client_python-0.651.2/lightdash_client/api/organizations/update_organization_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/projects/delete_validation_dismiss.py` & `lightdash_client_python-0.651.2/lightdash_client/api/projects/delete_validation_dismiss.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/projects/get_latest_validation_results.py` & `lightdash_client_python-0.651.2/lightdash_client/api/projects/get_latest_validation_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/projects/get_project.py` & `lightdash_client_python-0.651.2/lightdash_client/api/projects/get_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/projects/list_charts_in_project.py` & `lightdash_client_python-0.651.2/lightdash_client/api/projects/list_charts_in_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/projects/list_spaces_in_project.py` & `lightdash_client_python-0.651.2/lightdash_client/api/projects/list_spaces_in_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/projects/validate_project.py` & `lightdash_client_python-0.651.2/lightdash_client/api/projects/validate_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/add_space_share_to_user.py` & `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/add_space_share_to_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/create_space_in_project.py` & `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/create_space_in_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/get_project_access_list.py` & `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/get_project_access_list.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/grant_project_access_to_user.py` & `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/grant_project_access_to_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py` & `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/revoke_project_access_for_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py` & `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/revoke_space_access_for_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/update_organization_member.py` & `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/update_organization_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/update_project_access_for_user.py` & `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/update_project_access_for_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/roles_permissions/update_space.py` & `lightdash_client_python-0.651.2/lightdash_client/api/roles_permissions/update_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/schedulers/delete_scheduler.py` & `lightdash_client_python-0.651.2/lightdash_client/api/schedulers/delete_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/schedulers/get_scheduled_jobs.py` & `lightdash_client_python-0.651.2/lightdash_client/api/schedulers/get_scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/schedulers/get_scheduler.py` & `lightdash_client_python-0.651.2/lightdash_client/api/schedulers/get_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/schedulers/get_scheduler_job_status.py` & `lightdash_client_python-0.651.2/lightdash_client/api/schedulers/get_scheduler_job_status.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/schedulers/get_scheduler_logs.py` & `lightdash_client_python-0.651.2/lightdash_client/api/schedulers/get_scheduler_logs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/schedulers/update_scheduler.py` & `lightdash_client_python-0.651.2/lightdash_client/api/schedulers/update_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/share_links/create_share_url.py` & `lightdash_client_python-0.651.2/lightdash_client/api/share_links/create_share_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/share_links/get_share_url.py` & `lightdash_client_python-0.651.2/lightdash_client/api/share_links/get_share_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/spaces/delete_space.py` & `lightdash_client_python-0.651.2/lightdash_client/api/spaces/delete_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/spaces/get_space.py` & `lightdash_client_python-0.651.2/lightdash_client/api/spaces/get_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py` & `lightdash_client_python-0.651.2/lightdash_client/api/ssh_keypairs/create_ssh_key_pair.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/user_groups/add_user_to_group.py` & `lightdash_client_python-0.651.2/lightdash_client/api/user_groups/add_user_to_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/user_groups/delete_group.py` & `lightdash_client_python-0.651.2/lightdash_client/api/user_groups/delete_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/user_groups/get_group.py` & `lightdash_client_python-0.651.2/lightdash_client/api/user_groups/get_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/user_groups/get_group_members.py` & `lightdash_client_python-0.651.2/lightdash_client/api/user_groups/get_group_members.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/user_groups/remove_user_from_group.py` & `lightdash_client_python-0.651.2/lightdash_client/api/user_groups/remove_user_from_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/api/user_groups/update_group.py` & `lightdash_client_python-0.651.2/lightdash_client/api/user_groups/update_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/client.py` & `lightdash_client_python-0.651.2/lightdash_client/client.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/__init__.py` & `lightdash_client_python-0.651.2/lightdash_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """ Contains all the data models used in inputs/outputs """
+
 from .add_space_share import AddSpaceShare
 from .add_space_share_to_user_json_body import AddSpaceShareToUserJsonBody
 from .add_space_share_to_user_response_200 import AddSpaceShareToUserResponse200
 from .add_space_share_to_user_response_200_status import (
     AddSpaceShareToUserResponse200Status,
 )
 from .add_user_to_group_response_200 import AddUserToGroupResponse200
```

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/add_space_share.py` & `lightdash_client_python-0.651.2/lightdash_client/models/add_space_share.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/add_space_share_to_user_json_body.py` & `lightdash_client_python-0.651.2/lightdash_client/models/add_space_share_to_user_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/add_space_share_to_user_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/add_space_share_to_user_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/add_user_to_group_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/add_user_to_group_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/additional_metric.py` & `lightdash_client_python-0.651.2/lightdash_client/models/additional_metric.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/additional_metric_filters_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_filters_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/additional_metric_filters_item_operator.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from enum import Enum
 
 
-class AdditionalMetricFiltersItemOperator(str, Enum):
+class PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator(str, Enum):
     DOESNOTINCLUDE = "doesNotInclude"
     ENDSWITH = "endsWith"
     EQUALS = "equals"
     GREATERTHAN = "greaterThan"
     GREATERTHANOREQUAL = "greaterThanOrEqual"
     INBETWEEN = "inBetween"
     INCLUDE = "include"
     INTHECURRENT = "inTheCurrent"
     INTHENEXT = "inTheNext"
     INTHEPAST = "inThePast"
     ISNULL = "isNull"
     LESSTHAN = "lessThan"
     LESSTHANOREQUAL = "lessThanOrEqual"
     NOTEQUALS = "notEquals"
+    NOTINTHEPAST = "notInThePast"
     NOTNULL = "notNull"
     STARTSWITH = "startsWith"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/additional_metric_filters_item_target.py` & `lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_filters_item_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/allowed_email_domains.py` & `lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/allowed_email_domains_projects_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/allowed_email_domains_projects_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_chart_summary_list_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_chart_summary_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_chart_summary_list_response_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_chart_summary_list_response_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_csv_url_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_csv_url_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_csv_url_response_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_csv_url_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_dbt_cloud_integration_settings.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_integration_settings.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_dbt_cloud_integration_settings_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_integration_settings_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_dbt_cloud_metrics.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_metrics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_dbt_cloud_metrics_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_metrics_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_dbt_cloud_metrics_results_metrics_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_metrics_results_metrics_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_dbt_cloud_settings_delete_success.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_dbt_cloud_settings_delete_success.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_email_status_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_email_status_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_email_status_response_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_email_status_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_email_status_response_results_otp.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_email_status_response_results_otp.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_error_payload.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_error_payload.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_error_payload_error.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_error_payload_error.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_group_list_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_group_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_group_list_response_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_group_list_response_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_group_members_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_group_members_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_group_members_response_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_group_members_response_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_group_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_group_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_group_response_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_group_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_job_scheduled_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_job_scheduled_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_job_scheduled_response_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_job_scheduled_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_job_status_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_job_status_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_job_status_response_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_job_status_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_organization.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_organization_allowed_email_domains.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_organization_allowed_email_domains_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_allowed_email_domains_results_projects_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_organization_member_profile.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profile.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_organization_member_profile_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profile_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_organization_member_profiles.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profiles.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_organization_member_profiles_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_member_profiles_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_organization_projects.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_projects.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_organization_projects_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_projects_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_organization_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_organization_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_0_data.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_0_data_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_0_data_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_0_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_1_data.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_1_data_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_1_data_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_1_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_2.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_pinned_items_results_item_type_2_data.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_pinned_items_results_item_type_2_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_access_list_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_access_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_access_list_response_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_access_list_response_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_0_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_0_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_2.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_2_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_2_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_3.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_3.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_3_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_3_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_4.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_4.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_4_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_4_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_5.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_5.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_5_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_5_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_6.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_6.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_dbt_connection_type_6_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_dbt_connection_type_6_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_0_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_0_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_1_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_1_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_2.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_2_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_2_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_3.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_3.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_3_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_4.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_4.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_4_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_4_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_5.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_5.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_project_response_results_warehouse_connection_type_5_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_project_response_results_warehouse_connection_type_5_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item_operator.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from enum import Enum
 
 
-class ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemFiltersItemOperator(str, Enum):
+class PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator(str, Enum):
     DOESNOTINCLUDE = "doesNotInclude"
     ENDSWITH = "endsWith"
     EQUALS = "equals"
     GREATERTHAN = "greaterThan"
     GREATERTHANOREQUAL = "greaterThanOrEqual"
     INBETWEEN = "inBetween"
     INCLUDE = "include"
     INTHECURRENT = "inTheCurrent"
     INTHENEXT = "inTheNext"
     INTHEPAST = "inThePast"
     ISNULL = "isNull"
     LESSTHAN = "lessThan"
     LESSTHANOREQUAL = "lessThanOrEqual"
     NOTEQUALS = "notEquals"
+    NOTINTHEPAST = "notInThePast"
     NOTNULL = "notNull"
     STARTSWITH = "startsWith"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item_target.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_filters.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters_dimensions_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_filters_metrics_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_sorts_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_sorts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_table_calculations_item_format.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_scheduled_jobs_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduled_jobs_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_scheduled_jobs_response_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduled_jobs_response_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_and_targets_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_and_targets_response_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_and_targets_response_results_targets_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_charts_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_charts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_dashboards_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_dashboards_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_logs_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_logs_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_logs_item_details.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_logs_item_details.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_schedulers_item_targets_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_scheduler_logs_response_results_users_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_scheduler_logs_response_results_users_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_share_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_share_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_share_response_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_share_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_slack_channels_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_slack_channels_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_slack_channels_response_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_slack_channels_response_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_space_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results_access_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_access_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results_dashboards_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_dashboards_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results_dashboards_item_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_dashboards_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results_dashboards_item_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_dashboards_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results_queries_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_queries_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results_queries_item_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_queries_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_space_response_results_queries_item_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_space_response_results_queries_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_space_summary_list_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_space_summary_list_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_space_summary_list_response_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_space_summary_list_response_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_ssh_key_pair_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_ssh_key_pair_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_ssh_key_pair_response_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_ssh_key_pair_response_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_success_empty.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_success_empty.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_user_allowed_organizations_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_user_allowed_organizations_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_user_allowed_organizations_response_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_user_allowed_organizations_response_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_validate_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_validate_response_results_item_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_validate_response_results_item_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_validate_response_results_item_type_2.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_validate_response_results_item_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/api_validation_dismiss_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_validation_dismiss_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/bigquery_credentials.py` & `lightdash_client_python-0.651.2/lightdash_client/models/bigquery_credentials.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/bigquery_credentials_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/bigquery_credentials_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/chart_scheduler.py` & `lightdash_client_python-0.651.2/lightdash_client/models/chart_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/chart_scheduler_options_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/chart_scheduler_options_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/chart_scheduler_options_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/chart_scheduler_options_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/chart_summary.py` & `lightdash_client_python-0.651.2/lightdash_client/models/chart_summary.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/conditional_operator.py` & `lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item_filters_item_operator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from enum import Enum
 
 
-class ConditionalOperator(str, Enum):
+class RunQueryRequestAdditionalMetricsItemFiltersItemOperator(str, Enum):
     DOESNOTINCLUDE = "doesNotInclude"
     ENDSWITH = "endsWith"
     EQUALS = "equals"
     GREATERTHAN = "greaterThan"
     GREATERTHANOREQUAL = "greaterThanOrEqual"
     INBETWEEN = "inBetween"
     INCLUDE = "include"
     INTHECURRENT = "inTheCurrent"
     INTHENEXT = "inTheNext"
     INTHEPAST = "inThePast"
     ISNULL = "isNull"
     LESSTHAN = "lessThan"
     LESSTHANOREQUAL = "lessThanOrEqual"
     NOTEQUALS = "notEquals"
+    NOTINTHEPAST = "notInThePast"
     NOTNULL = "notNull"
     STARTSWITH = "startsWith"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_email_one_time_passcode_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_email_one_time_passcode_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_email_one_time_passcode_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_email_one_time_passcode_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_email_one_time_passcode_response_200_results_otp.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_email_one_time_passcode_response_200_results_otp.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_group_in_organization_json_body.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_group_in_organization_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_group_in_organization_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_group_in_organization_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_group_in_organization_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_group_in_organization_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_organization.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_organization_json_body.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_organization_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_organization_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_organization_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_project_member.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_project_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_share_url.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_share_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_share_url_json_body.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_share_url_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_share_url_response_201.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_share_url_response_201.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_share_url_response_201_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_share_url_response_201_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_space.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_space_access_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_space_access_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_json_body.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_json_body_access_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_json_body_access_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results_access_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_access_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_dashboards_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results_queries_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_queries_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results_queries_item_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_queries_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_space_in_project_response_200_results_queries_item_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_space_in_project_response_200_results_queries_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_ssh_key_pair_response_201.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_ssh_key_pair_response_201.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/create_ssh_key_pair_response_201_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/create_ssh_key_pair_response_201_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dashboard_basic_details.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dashboard_basic_details.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dashboard_basic_details_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dashboard_basic_details_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dashboard_basic_details_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dashboard_basic_details_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dashboard_scheduler.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dashboard_scheduler.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dashboard_scheduler_options_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dashboard_scheduler_options_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dashboard_scheduler_options_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dashboard_scheduler_options_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/databricks_credentials.py` & `lightdash_client_python-0.651.2/lightdash_client/models/databricks_credentials.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/databricks_credentials_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/databricks_credentials_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_azure_dev_ops_project_config.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_azure_dev_ops_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_azure_dev_ops_project_config_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_azure_dev_ops_project_config_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_bit_bucket_project_config.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_bit_bucket_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_bit_bucket_project_config_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_bit_bucket_project_config_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_cloud_ide_project_config.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_ide_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_cloud_integration.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_integration.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_cloud_metadata_response_metrics.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_metadata_response_metrics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_cloud_metadata_response_metrics_metrics_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_metadata_response_metrics_metrics_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_cloud_metric.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_cloud_metric.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_github_project_config.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_github_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_github_project_config_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_github_project_config_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_gitlab_project_config.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_gitlab_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_gitlab_project_config_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_gitlab_project_config_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_local_project_config.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_local_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_local_project_config_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_local_project_config_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_none_project_config.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_none_project_config.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_none_project_config_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_none_project_config_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_0_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_0_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_2_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_2_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_3_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_3_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_4_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_4_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_5_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_5_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_config_type_6_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_config_type_6_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/dbt_project_environment_variable.py` & `lightdash_client_python-0.651.2/lightdash_client/models/dbt_project_environment_variable.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/delete_dbt_cloud_integration_settings_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/delete_dbt_cloud_integration_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/delete_group_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/delete_group_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/delete_me_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/delete_me_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/delete_my_organization_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/delete_my_organization_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/delete_organization_member_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/delete_organization_member_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/delete_scheduler_response_201.py` & `lightdash_client_python-0.651.2/lightdash_client/models/delete_scheduler_response_201.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/delete_space_response_204.py` & `lightdash_client_python-0.651.2/lightdash_client/models/delete_space_response_204.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/delete_validation_dismiss_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/delete_validation_dismiss_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/email_one_time_password.py` & `lightdash_client_python-0.651.2/lightdash_client/models/email_one_time_password.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/email_one_time_password_expiring.py` & `lightdash_client_python-0.651.2/lightdash_client/models/email_one_time_password_expiring.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/email_status.py` & `lightdash_client_python-0.651.2/lightdash_client/models/email_status.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/email_status_expiring.py` & `lightdash_client_python-0.651.2/lightdash_client/models/email_status_expiring.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/email_status_expiring_otp.py` & `lightdash_client_python-0.651.2/lightdash_client/models/email_status_expiring_otp.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/email_status_otp.py` & `lightdash_client_python-0.651.2/lightdash_client/models/email_status_otp.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/filter_group_response_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/filter_group_response_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/filter_group_response_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/filter_group_response_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/filters.py` & `lightdash_client_python-0.651.2/lightdash_client/models/filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/filters_dimensions_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/filters_dimensions_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/filters_dimensions_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/filters_dimensions_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/filters_metrics_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/filters_metrics_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/filters_metrics_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/filters_metrics_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_csv_url_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_csv_url_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_csv_url_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_csv_url_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_dbt_cloud_integration_settings_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_integration_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_dbt_cloud_integration_settings_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_integration_settings_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_dbt_cloud_metrics_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_metrics_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_dbt_cloud_metrics_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_metrics_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_dbt_cloud_metrics_response_200_results_metrics_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_dbt_cloud_metrics_response_200_results_metrics_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_email_verification_status_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_email_verification_status_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_email_verification_status_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_email_verification_status_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_email_verification_status_response_200_results_otp.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_email_verification_status_response_200_results_otp.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_group_members_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_group_members_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_group_members_response_200_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_group_members_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_group_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_group_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_group_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_group_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_latest_validation_results_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_latest_validation_results_response_200_results_item_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_my_organization_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_my_organization_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_my_organization_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_my_organization_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_0_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_1_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_2.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_pinned_items_response_200_results_item_type_2_data.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_pinned_items_response_200_results_item_type_2_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_access_list_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_access_list_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_access_list_response_200_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_access_list_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_0_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_2_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_3_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_4_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_5_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_dbt_connection_type_6_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_0_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_1_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_2_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_3_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_4_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_project_response_200_results_warehouse_connection_type_5_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduled_jobs_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduled_jobs_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduled_jobs_response_200_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduled_jobs_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_job_status_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_job_status_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_job_status_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_job_status_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_charts_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_charts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_dashboards_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_dashboards_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_details.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_logs_item_details.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_schedulers_item_targets_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_logs_response_200_results_users_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_logs_response_200_results_users_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_scheduler_response_200_results_targets_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_share_url_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_share_url_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_share_url_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_share_url_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_slack_channels_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_slack_channels_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_slack_channels_response_200_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_slack_channels_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results_access_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_access_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results_dashboards_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_dashboards_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results_dashboards_item_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_dashboards_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results_dashboards_item_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_dashboards_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results_queries_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_queries_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results_queries_item_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_queries_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/get_space_response_200_results_queries_item_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/get_space_response_200_results_queries_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/grant_project_access_to_user_json_body.py` & `lightdash_client_python-0.651.2/lightdash_client/models/grant_project_access_to_user_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/grant_project_access_to_user_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/grant_project_access_to_user_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/group.py` & `lightdash_client_python-0.651.2/lightdash_client/models/group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/group_member.py` & `lightdash_client_python-0.651.2/lightdash_client/models/group_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/join_organization_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/join_organization_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/list_charts_in_project_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/list_charts_in_project_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/list_charts_in_project_response_200_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/list_charts_in_project_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/list_groups_in_organization_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/list_groups_in_organization_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/list_groups_in_organization_response_200_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/list_groups_in_organization_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/list_my_available_organizations_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/list_my_available_organizations_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/list_my_available_organizations_response_200_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/list_my_available_organizations_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/list_organization_email_domains_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/list_organization_email_domains_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/list_organization_email_domains_response_200_results_projects_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/list_organization_members_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/list_organization_members_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/list_organization_members_response_200_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/list_organization_members_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/list_organization_projects_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/list_organization_projects_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/list_organization_projects_response_200_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/list_organization_projects_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/list_spaces_in_project_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/list_spaces_in_project_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/list_spaces_in_project_response_200_results_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/list_spaces_in_project_response_200_results_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/metric_filter_rule.py` & `lightdash_client_python-0.651.2/lightdash_client/models/metric_filter_rule.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/metric_filter_rule_operator.py` & `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item_operator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from enum import Enum
 
 
-class MetricFilterRuleOperator(str, Enum):
+class MetricQueryResponseAdditionalMetricsItemFiltersItemOperator(str, Enum):
     DOESNOTINCLUDE = "doesNotInclude"
     ENDSWITH = "endsWith"
     EQUALS = "equals"
     GREATERTHAN = "greaterThan"
     GREATERTHANOREQUAL = "greaterThanOrEqual"
     INBETWEEN = "inBetween"
     INCLUDE = "include"
     INTHECURRENT = "inTheCurrent"
     INTHENEXT = "inTheNext"
     INTHEPAST = "inThePast"
     ISNULL = "isNull"
     LESSTHAN = "lessThan"
     LESSTHANOREQUAL = "lessThanOrEqual"
     NOTEQUALS = "notEquals"
+    NOTINTHEPAST = "notInThePast"
     NOTNULL = "notNull"
     STARTSWITH = "startsWith"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/metric_filter_rule_target.py` & `lightdash_client_python-0.651.2/lightdash_client/models/metric_filter_rule_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_additional_metrics_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item_operator.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_operator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from enum import Enum
 
 
-class MetricQueryResponseAdditionalMetricsItemFiltersItemOperator(str, Enum):
+class PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFiltersItemOperator(str, Enum):
     DOESNOTINCLUDE = "doesNotInclude"
     ENDSWITH = "endsWith"
     EQUALS = "equals"
     GREATERTHAN = "greaterThan"
     GREATERTHANOREQUAL = "greaterThanOrEqual"
     INBETWEEN = "inBetween"
     INCLUDE = "include"
     INTHECURRENT = "inTheCurrent"
     INTHENEXT = "inTheNext"
     INTHEPAST = "inThePast"
     ISNULL = "isNull"
     LESSTHAN = "lessThan"
     LESSTHANOREQUAL = "lessThanOrEqual"
     NOTEQUALS = "notEquals"
+    NOTINTHEPAST = "notInThePast"
     NOTNULL = "notNull"
     STARTSWITH = "startsWith"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item_target.py` & `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_additional_metrics_item_filters_item_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_filters.py` & `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_filters_dimensions_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters_dimensions_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_filters_dimensions_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters_dimensions_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_filters_metrics_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters_metrics_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_filters_metrics_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_filters_metrics_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_sorts_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_sorts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_table_calculations_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_table_calculations_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/metric_query_response_table_calculations_item_format.py` & `lightdash_client_python-0.651.2/lightdash_client/models/metric_query_response_table_calculations_item_format.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid.py` & `lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/omit_allowed_email_domains_organization_uuid_projects_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/omit_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/omit_validation_response_base_name.py` & `lightdash_client_python-0.651.2/lightdash_client/models/omit_validation_response_base_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/organization.py` & `lightdash_client_python-0.651.2/lightdash_client/models/organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/organization_member_profile.py` & `lightdash_client_python-0.651.2/lightdash_client/models/organization_member_profile.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/organization_member_profile_update.py` & `lightdash_client_python-0.651.2/lightdash_client/models/organization_member_profile_update.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/organization_project.py` & `lightdash_client_python-0.651.2/lightdash_client/models/organization_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py` & `lightdash_client_python-0.651.2/lightdash_client/models/partial_omit_organization_organization_uuid_or_needs_project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_allowed_email_domains_exclude_keyof_allowed_email_domains_organization_uuid_projects_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_bigquery_credentials_exclude_keyof_create_bigquery_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_databricks_credentials_exclude_keyof_create_databricks_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_dbt_cloud_integration_metrics_job_id.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_create_group_name.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_group_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_postgres_credentials_exclude_keyof_create_postgres_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_redshift_credentials_exclude_keyof_create_redshift_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_snowflake_credentials_exclude_keyof_create_snowflake_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_create_trino_credentials_exclude_keyof_create_trino_credentials_sensitive_credentials_field_names_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_basic_details_uuid_or_space_uuid_or_description_or_name_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_dashboard_uuid_or_name_or_description_or_updated_at_or_project_uuid_or_updated_by_user_or_organization_uuid_or_space_uuid_or_views_or_first_viewed_at_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_group_name.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_group_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_organization_name.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_organization_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_resource_view_item_at_data_uuid_or_pinned_list_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_description_or_space_name_or_space_uuid_or_project_uuid_or_organization_uuid_or_pinned_list_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_saved_chart_uuid_or_name_or_updated_at_or_updated_by_user_or_description_or_space_uuid_or_pinned_list_uuid_or_pinned_list_order_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_share_url_path_or_params.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_share_url_path_or_params.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_space_organization_uuid_or_project_uuid_or_uuid_or_name_or_is_private.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_space_project_uuid_or_uuid_or_name_or_is_private_or_pinned_list_uuid_or_pinned_list_order_or_organization_uuid.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_space_query_uuid_or_name_or_chart_type_or_first_viewed_at_or_views_or_pinned_list_uuid_or_pinned_list_order_or_space_uuid_or_description_or_updated_at_or_updated_by_user_or_validation_errors_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_ssh_key_pair_public_key.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_ssh_key_pair_public_key.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_validation_response_base_exclude_keyof_validation_response_base_name.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pick_validation_response_error_or_created_at_or_validation_id.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pinned_items_item_type_0_data_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_0_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pinned_items_item_type_0_data_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_0_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pinned_items_item_type_1_data_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_1_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pinned_items_item_type_1_data_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_1_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/pinned_items_item_type_2_data.py` & `lightdash_client_python-0.651.2/lightdash_client/models/pinned_items_item_type_2_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_json_body.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_json_body_filters.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters_dimensions_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_json_body_filters_metrics_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,12 +12,13 @@
     INTHECURRENT = "inTheCurrent"
     INTHENEXT = "inTheNext"
     INTHEPAST = "inThePast"
     ISNULL = "isNull"
     LESSTHAN = "lessThan"
     LESSTHANOREQUAL = "lessThanOrEqual"
     NOTEQUALS = "notEquals"
+    NOTINTHEPAST = "notInThePast"
     NOTNULL = "notNull"
     STARTSWITH = "startsWith"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_target.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_additional_metrics_item_filters_item_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_dimensions_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_filters_metrics_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_sorts_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_sorts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_chart_results_response_200_results_metric_query_table_calculations_item_format.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_additional_metrics_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item_operator.py` & `lightdash_client_python-0.651.2/lightdash_client/models/additional_metric_filters_item_operator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from enum import Enum
 
 
-class PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemOperator(str, Enum):
+class AdditionalMetricFiltersItemOperator(str, Enum):
     DOESNOTINCLUDE = "doesNotInclude"
     ENDSWITH = "endsWith"
     EQUALS = "equals"
     GREATERTHAN = "greaterThan"
     GREATERTHANOREQUAL = "greaterThanOrEqual"
     INBETWEEN = "inBetween"
     INCLUDE = "include"
     INTHECURRENT = "inTheCurrent"
     INTHENEXT = "inTheNext"
     INTHEPAST = "inThePast"
     ISNULL = "isNull"
     LESSTHAN = "lessThan"
     LESSTHANOREQUAL = "lessThanOrEqual"
     NOTEQUALS = "notEquals"
+    NOTINTHEPAST = "notInThePast"
     NOTNULL = "notNull"
     STARTSWITH = "startsWith"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item_target.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_filters.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_sorts_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_sorts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_table_calculations_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_table_calculations_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_json_body_table_calculations_item_format.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_table_calculations_item_format.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py` & `lightdash_client_python-0.651.2/lightdash_client/models/api_run_query_response_results_metric_query_additional_metrics_item_filters_item_operator.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from enum import Enum
 
 
-class PostRunQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator(str, Enum):
+class ApiRunQueryResponseResultsMetricQueryAdditionalMetricsItemFiltersItemOperator(str, Enum):
     DOESNOTINCLUDE = "doesNotInclude"
     ENDSWITH = "endsWith"
     EQUALS = "equals"
     GREATERTHAN = "greaterThan"
     GREATERTHANOREQUAL = "greaterThanOrEqual"
     INBETWEEN = "inBetween"
     INCLUDE = "include"
     INTHECURRENT = "inTheCurrent"
     INTHENEXT = "inTheNext"
     INTHEPAST = "inThePast"
     ISNULL = "isNull"
     LESSTHAN = "lessThan"
     LESSTHANOREQUAL = "lessThanOrEqual"
     NOTEQUALS = "notEquals"
+    NOTINTHEPAST = "notInThePast"
     NOTNULL = "notNull"
     STARTSWITH = "startsWith"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_filters.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_dimensions_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_dimensions_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_dimensions_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_dimensions_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_metrics_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_metrics_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_metrics_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_filters_metrics_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_sorts_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_sorts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_response_200_results_metric_query_table_calculations_item_format.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_operator.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_query_json_body_additional_metrics_item_filters_item_operator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from enum import Enum
 
 
-class PostRunUnderlyingDataQueryJsonBodyAdditionalMetricsItemFiltersItemOperator(str, Enum):
+class PostRunQueryJsonBodyAdditionalMetricsItemFiltersItemOperator(str, Enum):
     DOESNOTINCLUDE = "doesNotInclude"
     ENDSWITH = "endsWith"
     EQUALS = "equals"
     GREATERTHAN = "greaterThan"
     GREATERTHANOREQUAL = "greaterThanOrEqual"
     INBETWEEN = "inBetween"
     INCLUDE = "include"
     INTHECURRENT = "inTheCurrent"
     INTHENEXT = "inTheNext"
     INTHEPAST = "inThePast"
     ISNULL = "isNull"
     LESSTHAN = "lessThan"
     LESSTHANOREQUAL = "lessThanOrEqual"
     NOTEQUALS = "notEquals"
+    NOTINTHEPAST = "notInThePast"
     NOTNULL = "notNull"
     STARTSWITH = "startsWith"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_target.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_additional_metrics_item_filters_item_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_filters.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_sorts_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_sorts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_json_body_table_calculations_item_format.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item_operator.py` & `lightdash_client_python-0.651.2/lightdash_client/models/metric_filter_rule_operator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from enum import Enum
 
 
-class PostRunUnderlyingDataQueryResponse200ResultsMetricQueryAdditionalMetricsItemFiltersItemOperator(str, Enum):
+class MetricFilterRuleOperator(str, Enum):
     DOESNOTINCLUDE = "doesNotInclude"
     ENDSWITH = "endsWith"
     EQUALS = "equals"
     GREATERTHAN = "greaterThan"
     GREATERTHANOREQUAL = "greaterThanOrEqual"
     INBETWEEN = "inBetween"
     INCLUDE = "include"
     INTHECURRENT = "inTheCurrent"
     INTHENEXT = "inTheNext"
     INTHEPAST = "inThePast"
     ISNULL = "isNull"
     LESSTHAN = "lessThan"
     LESSTHANOREQUAL = "lessThanOrEqual"
     NOTEQUALS = "notEquals"
+    NOTINTHEPAST = "notInThePast"
     NOTNULL = "notNull"
     STARTSWITH = "startsWith"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_additional_metrics_item_filters_item_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_dimensions_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_filters_metrics_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_sorts_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_sorts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format.py` & `lightdash_client_python-0.651.2/lightdash_client/models/post_run_underlying_data_query_response_200_results_metric_query_table_calculations_item_format.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/postgres_credentials.py` & `lightdash_client_python-0.651.2/lightdash_client/models/postgres_credentials.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/postgres_credentials_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/postgres_credentials_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_0_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_0_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_2.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_2_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_2_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_3.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_3.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_3_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_3_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_4.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_4.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_4_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_4_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_5.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_5.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_5_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_5_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_6.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_6.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_dbt_connection_type_6_environment_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_dbt_connection_type_6_environment_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_member_profile.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_member_profile.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_0_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_0_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_1_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_1_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_2.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_2_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_2_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_3.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_3.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_3_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_3_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_4.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_4.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_4_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_4_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_5.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_5.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/project_warehouse_connection_type_5_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/project_warehouse_connection_type_5_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/record_string_any.py` & `lightdash_client_python-0.651.2/lightdash_client/models/record_string_any.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/redshift_credentials.py` & `lightdash_client_python-0.651.2/lightdash_client/models/redshift_credentials.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/redshift_credentials_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/redshift_credentials_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/remove_user_from_group_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/remove_user_from_group_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/resource_view_chart_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/resource_view_chart_item_data.py` & `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/resource_view_chart_item_data_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/resource_view_chart_item_data_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_chart_item_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/resource_view_dashboard_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/resource_view_dashboard_item_data.py` & `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/resource_view_dashboard_item_data_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/resource_view_dashboard_item_data_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_dashboard_item_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/resource_view_space_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_space_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/resource_view_space_item_data.py` & `lightdash_client_python-0.651.2/lightdash_client/models/resource_view_space_item_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/revoke_project_access_for_user_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/revoke_project_access_for_user_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/revoke_space_access_for_user_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/revoke_space_access_for_user_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/run_query_request.py` & `lightdash_client_python-0.651.2/lightdash_client/models/run_query_request.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_additional_metrics_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_additional_metrics_item_filters_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item_filters_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_additional_metrics_item_filters_item_operator.py` & `lightdash_client_python-0.651.2/lightdash_client/models/conditional_operator.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from enum import Enum
 
 
-class RunQueryRequestAdditionalMetricsItemFiltersItemOperator(str, Enum):
+class ConditionalOperator(str, Enum):
     DOESNOTINCLUDE = "doesNotInclude"
     ENDSWITH = "endsWith"
     EQUALS = "equals"
     GREATERTHAN = "greaterThan"
     GREATERTHANOREQUAL = "greaterThanOrEqual"
     INBETWEEN = "inBetween"
     INCLUDE = "include"
     INTHECURRENT = "inTheCurrent"
     INTHENEXT = "inTheNext"
     INTHEPAST = "inThePast"
     ISNULL = "isNull"
     LESSTHAN = "lessThan"
     LESSTHANOREQUAL = "lessThanOrEqual"
     NOTEQUALS = "notEquals"
+    NOTINTHEPAST = "notInThePast"
     NOTNULL = "notNull"
     STARTSWITH = "startsWith"
 
     def __str__(self) -> str:
         return str(self.value)
```

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_additional_metrics_item_filters_item_target.py` & `lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_additional_metrics_item_filters_item_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_filters.py` & `lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_filters.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_sorts_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_sorts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_table_calculations_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_table_calculations_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/run_query_request_table_calculations_item_format.py` & `lightdash_client_python-0.651.2/lightdash_client/models/run_query_request_table_calculations_item_format.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduled_jobs.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduled_jobs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_and_targets.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_and_targets.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_and_targets_targets_item_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_and_targets_targets_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_and_targets_targets_item_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_and_targets_targets_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_base.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_base.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_base_options_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_base_options_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_base_options_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_base_options_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_csv_options.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_csv_options.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_email_target.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_email_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_image_options.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_image_options.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_log.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_log.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_log_details.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_log_details.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_options_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_options_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_options_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_options_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_slack_target.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_slack_target.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_type_0_options_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_0_options_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_type_0_options_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_0_options_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_type_1_options_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_1_options_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_type_1_options_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_type_1_options_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_charts_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_charts_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_dashboards_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_dashboards_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_logs_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_logs_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_logs_item_details.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_logs_item_details.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_schedulers_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_schedulers_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_schedulers_item_targets_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/scheduler_with_logs_users_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/scheduler_with_logs_users_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/share_url.py` & `lightdash_client_python-0.651.2/lightdash_client/models/share_url.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/slack_channel.py` & `lightdash_client_python-0.651.2/lightdash_client/models/slack_channel.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/snowflake_credentials.py` & `lightdash_client_python-0.651.2/lightdash_client/models/snowflake_credentials.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/snowflake_credentials_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/snowflake_credentials_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/sort_field.py` & `lightdash_client_python-0.651.2/lightdash_client/models/sort_field.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/space.py` & `lightdash_client_python-0.651.2/lightdash_client/models/space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/space_access_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/space_access_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/space_dashboard.py` & `lightdash_client_python-0.651.2/lightdash_client/models/space_dashboard.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/space_dashboard_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/space_dashboard_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/space_dashboard_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/space_dashboard_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/space_dashboards_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/space_dashboards_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/space_dashboards_item_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/space_dashboards_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/space_dashboards_item_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/space_dashboards_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/space_queries_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/space_queries_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/space_queries_item_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/space_queries_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/space_queries_item_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/space_queries_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/space_query.py` & `lightdash_client_python-0.651.2/lightdash_client/models/space_query.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/space_query_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/space_query_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/space_query_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/space_query_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/space_share.py` & `lightdash_client_python-0.651.2/lightdash_client/models/space_share.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/space_summary.py` & `lightdash_client_python-0.651.2/lightdash_client/models/space_summary.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/trino_credentials.py` & `lightdash_client_python-0.651.2/lightdash_client/models/trino_credentials.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/trino_credentials_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/trino_credentials_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_allowed_email_domains.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_allowed_email_domains_projects_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_allowed_email_domains_projects_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_dbt_cloud_integration_settings_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_dbt_cloud_integration_settings_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_dbt_cloud_integration_settings_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_dbt_cloud_integration_settings_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_group.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_group.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_group_json_body.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_group_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_group_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_group_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_group_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_group_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_my_organization_json_body.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_my_organization_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_my_organization_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_my_organization_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_organization.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_json_body.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_json_body_projects_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_json_body_projects_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_organization_email_domains_response_200_results_projects_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_organization_member_json_body.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_organization_member_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_organization_member_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_organization_member_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_item_order.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_item_order.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_item_order_data.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_item_order_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_json_body_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_json_body_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_json_body_item_data.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_json_body_item_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_0_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_1_data_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2_data.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_pinned_items_order_response_200_results_item_type_2_data.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_project_access_for_user_json_body.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_project_access_for_user_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_project_access_for_user_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_project_access_for_user_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_project_member.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_project_member.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_scheduler_response_201.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_scheduler_response_201_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_scheduler_response_201_results_targets_item_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_space.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_space.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_space_json_body.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_space_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results_access_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_access_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results_dashboards_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_dashboards_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results_dashboards_item_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_dashboards_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results_dashboards_item_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_dashboards_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results_queries_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_queries_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results_queries_item_updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_queries_item_updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/update_space_response_200_results_queries_item_validation_errors_item.py` & `lightdash_client_python-0.651.2/lightdash_client/models/update_space_response_200_results_queries_item_validation_errors_item.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/updated_by_user.py` & `lightdash_client_python-0.651.2/lightdash_client/models/updated_by_user.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/user_allowed_organization.py` & `lightdash_client_python-0.651.2/lightdash_client/models/user_allowed_organization.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/validate_project_json_body.py` & `lightdash_client_python-0.651.2/lightdash_client/models/validate_project_json_body.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/validate_project_response_200.py` & `lightdash_client_python-0.651.2/lightdash_client/models/validate_project_response_200.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/validate_project_response_200_results.py` & `lightdash_client_python-0.651.2/lightdash_client/models/validate_project_response_200_results.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/validation_error_chart_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/validation_error_chart_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/validation_error_dashboard_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/validation_error_dashboard_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/validation_error_table_response.py` & `lightdash_client_python-0.651.2/lightdash_client/models/validation_error_table_response.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/validation_response_base.py` & `lightdash_client_python-0.651.2/lightdash_client/models/validation_response_base.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/validation_response_type_0.py` & `lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_0.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/validation_response_type_1.py` & `lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_1.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/validation_response_type_2.py` & `lightdash_client_python-0.651.2/lightdash_client/models/validation_response_type_2.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/validation_summary.py` & `lightdash_client_python-0.651.2/lightdash_client/models/validation_summary.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/view_statistics.py` & `lightdash_client_python-0.651.2/lightdash_client/models/view_statistics.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_0_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_0_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_1_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_1_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_2_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_2_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_3_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_3_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_4_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_4_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/models/warehouse_credentials_type_5_start_of_week.py` & `lightdash_client_python-0.651.2/lightdash_client/models/warehouse_credentials_type_5_start_of_week.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/lightdash_client/types.py` & `lightdash_client_python-0.651.2/lightdash_client/types.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/pyproject.toml` & `lightdash_client_python-0.651.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/setup.py` & `lightdash_client_python-0.651.2/setup.py`

 * *Files identical despite different names*

### Comparing `lightdash_client_python-0.640.1/PKG-INFO` & `lightdash_client_python-0.651.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightdash-client-python
-Version: 0.640.1
+Version: 0.651.2
 Summary: A client library for accessing Lightdash API 
 Author: yu-iskw
 Requires-Python: >=3.8.0,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
```

