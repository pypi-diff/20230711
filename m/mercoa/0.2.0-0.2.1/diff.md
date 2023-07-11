# Comparing `tmp/mercoa-0.2.0.tar.gz` & `tmp/mercoa-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercoa-0.2.0.tar", max compression
+gzip compressed data, was "mercoa-0.2.1.tar", max compression
```

## Comparing `mercoa-0.2.0.tar` & `mercoa-0.2.1.tar`

### file list

```diff
@@ -1,181 +1,183 @@
--rw-r--r--   0        0        0     1930 2023-07-08 22:39:19.354413 mercoa-0.2.0/README.md
--rw-r--r--   0        0        0      368 2023-07-08 22:39:19.354413 mercoa-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4199 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/__init__.py
--rw-r--r--   0        0        0     2384 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/client.py
--rw-r--r--   0        0        0      348 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      157 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/environment.py
--rw-r--r--   0        0        0        0 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/py.typed
--rw-r--r--   0        0        0     4280 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/__init__.py
--rw-r--r--   0        0        0      165 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/bank_lookup/__init__.py
--rw-r--r--   0        0        0     3801 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/bank_lookup/client.py
--rw-r--r--   0        0        0      205 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/bank_lookup/types/__init__.py
--rw-r--r--   0        0        0      960 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/bank_lookup/types/bank_address.py
--rw-r--r--   0        0        0      946 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
--rw-r--r--   0        0        0      814 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/__init__.py
--rw-r--r--   0        0        0      314 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/errors/__init__.py
--rw-r--r--   0        0        0      237 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/errors/auth_header_malformed_error.py
--rw-r--r--   0        0        0      221 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/errors/auth_header_missing_error.py
--rw-r--r--   0        0        0      225 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/errors/unauthorized.py
--rw-r--r--   0        0        0      947 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/__init__.py
--rw-r--r--   0        0        0     1093 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/address.py
--rw-r--r--   0        0        0       88 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/approval_policy_id.py
--rw-r--r--   0        0        0      824 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/birth_date.py
--rw-r--r--   0        0        0       81 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/comment_id.py
--rw-r--r--   0        0        0       80 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/entity_id.py
--rw-r--r--   0        0        0       84 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/entity_user_id.py
--rw-r--r--   0        0        0      994 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/full_name.py
--rw-r--r--   0        0        0      850 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/individual_government_id.py
--rw-r--r--   0        0        0       81 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/invoice_id.py
--rw-r--r--   0        0        0      857 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/itin.py
--rw-r--r--   0        0        0      441 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/order_direction.py
--rw-r--r--   0        0        0       87 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/payment_method_id.py
--rw-r--r--   0        0        0       93 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/payment_method_schema_id.py
--rw-r--r--   0        0        0      855 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/phone_number.py
--rw-r--r--   0        0        0      856 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/commons/types/ssn.py
--rw-r--r--   0        0        0     2246 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/__init__.py
--rw-r--r--   0        0        0    33504 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/client.py
--rw-r--r--   0        0        0     1593 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/__init__.py
--rw-r--r--   0        0        0      854 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/__init__.py
--rw-r--r--   0        0        0    17631 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/client.py
--rw-r--r--   0        0        0      305 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/errors/__init__.py
--rw-r--r--   0        0        0      242 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/errors/num_approver_less_than_one_error.py
--rw-r--r--   0        0        0      248 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/errors/num_approvers_user_list_mismatch_error.py
--rw-r--r--   0        0        0      854 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/__init__.py
--rw-r--r--   0        0        0      847 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/amount_trigger.py
--rw-r--r--   0        0        0     1120 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/approval_policy_request.py
--rw-r--r--   0        0        0     1056 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/approval_policy_response.py
--rw-r--r--   0        0        0     1087 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/approval_policy_update_request.py
--rw-r--r--   0        0        0      965 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/approver_rule.py
--rw-r--r--   0        0        0      651 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/identifier_list.py
--rw-r--r--   0        0        0      391 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/rule.py
--rw-r--r--   0        0        0      573 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/trigger.py
--rw-r--r--   0        0        0      199 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/counterparty/__init__.py
--rw-r--r--   0        0        0     4088 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/counterparty/client.py
--rw-r--r--   0        0        0      256 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/counterparty/types/__init__.py
--rw-r--r--   0        0        0     1020 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/counterparty/types/counterparty_response.py
--rw-r--r--   0        0        0     1448 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/counterparty/types/find_counterparties_response.py
--rw-r--r--   0        0        0      145 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/invoice/__init__.py
--rw-r--r--   0        0        0    11190 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/invoice/client.py
--rw-r--r--   0        0        0      164 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/invoice/types/__init__.py
--rw-r--r--   0        0        0     1070 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/invoice/types/invoice_metrics_response.py
--rw-r--r--   0        0        0       65 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/payment_method/__init__.py
--rw-r--r--   0        0        0    22264 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/payment_method/client.py
--rw-r--r--   0        0        0      269 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/__init__.py
--rw-r--r--   0        0        0    12714 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/client.py
--rw-r--r--   0        0        0      381 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/types/__init__.py
--rw-r--r--   0        0        0       88 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/types/representative_id.py
--rw-r--r--   0        0        0     1382 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/types/representative_request.py
--rw-r--r--   0        0        0     1547 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/types/representative_response.py
--rw-r--r--   0        0        0     1102 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/types/responsibilities.py
--rw-r--r--   0        0        0      177 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/user/__init__.py
--rw-r--r--   0        0        0    15285 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/user/client.py
--rw-r--r--   0        0        0      224 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/user/types/__init__.py
--rw-r--r--   0        0        0     1102 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/user/types/entity_user_request.py
--rw-r--r--   0        0        0     1244 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/resources/user/types/entity_user_response.py
--rw-r--r--   0        0        0     1148 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/__init__.py
--rw-r--r--   0        0        0      487 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/account_type.py
--rw-r--r--   0        0        0     1535 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/business_profile_request.py
--rw-r--r--   0        0        0     1492 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/business_profile_response.py
--rw-r--r--   0        0        0     1917 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/business_type.py
--rw-r--r--   0        0        0      741 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/ein.py
--rw-r--r--   0        0        0      930 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/entity_add_payees_request.py
--rw-r--r--   0        0        0     2432 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/entity_request.py
--rw-r--r--   0        0        0     1830 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/entity_response.py
--rw-r--r--   0        0        0     1084 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/entity_status.py
--rw-r--r--   0        0        0     2084 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/entity_update_request.py
--rw-r--r--   0        0        0     1372 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/individual_profile_request.py
--rw-r--r--   0        0        0     1206 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/individual_profile_response.py
--rw-r--r--   0        0        0      974 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/profile_request.py
--rw-r--r--   0        0        0      981 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/profile_response.py
--rw-r--r--   0        0        0      761 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/entity/types/tax_id.py
--rw-r--r--   0        0        0      867 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/invoice/__init__.py
--rw-r--r--   0        0        0    20763 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/invoice/client.py
--rw-r--r--   0        0        0      391 2023-07-08 22:39:19.354413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/__init__.py
--rw-r--r--   0        0        0      131 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/approval/__init__.py
--rw-r--r--   0        0        0     6536 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/approval/client.py
--rw-r--r--   0        0        0      142 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/approval/types/__init__.py
--rw-r--r--   0        0        0     1016 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/approval/types/approval_request.py
--rw-r--r--   0        0        0      165 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/comment/__init__.py
--rw-r--r--   0        0        0    15286 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/comment/client.py
--rw-r--r--   0        0        0      204 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/comment/types/__init__.py
--rw-r--r--   0        0        0      933 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/comment/types/comment_request.py
--rw-r--r--   0        0        0     1450 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/comment/types/comment_response.py
--rw-r--r--   0        0        0      133 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/document/__init__.py
--rw-r--r--   0        0        0     3847 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/document/client.py
--rw-r--r--   0        0        0      145 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/document/types/__init__.py
--rw-r--r--   0        0        0      853 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/resources/document/types/document_response.py
--rw-r--r--   0        0        0      877 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/__init__.py
--rw-r--r--   0        0        0      631 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/approver_action.py
--rw-r--r--   0        0        0      900 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/assigned_approver.py
--rw-r--r--   0        0        0      979 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/associated_approval_action.py
--rw-r--r--   0        0        0     1404 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_approver_response.py
--rw-r--r--   0        0        0     1325 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_line_item_request.py
--rw-r--r--   0        0        0     1252 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_line_item_response.py
--rw-r--r--   0        0        0      870 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_order_by_field.py
--rw-r--r--   0        0        0     3439 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_request.py
--rw-r--r--   0        0        0     4299 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_response.py
--rw-r--r--   0        0        0     1485 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_status.py
--rw-r--r--   0        0        0      155 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/ocr/__init__.py
--rw-r--r--   0        0        0     4419 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/ocr/client.py
--rw-r--r--   0        0        0      189 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/ocr/types/__init__.py
--rw-r--r--   0        0        0     1234 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/ocr/types/ocr_response.py
--rw-r--r--   0        0        0      642 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/ocr/types/vendor_network.py
--rw-r--r--   0        0        0      983 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/__init__.py
--rw-r--r--   0        0        0    10870 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/client.py
--rw-r--r--   0        0        0     1466 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/__init__.py
--rw-r--r--   0        0        0      948 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/color_scheme_request.py
--rw-r--r--   0        0        0      949 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/color_scheme_response.py
--rw-r--r--   0        0        0      981 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/email_log_response.py
--rw-r--r--   0        0        0      932 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/email_provider_request.py
--rw-r--r--   0        0        0      936 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/email_provider_response.py
--rw-r--r--   0        0        0      785 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/email_sender_provider.py
--rw-r--r--   0        0        0     1052 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/email_sender_request.py
--rw-r--r--   0        0        0     1044 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/email_sender_response.py
--rw-r--r--   0        0        0       86 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/organization_id.py
--rw-r--r--   0        0        0     1463 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/organization_request.py
--rw-r--r--   0        0        0     1579 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/organization_response.py
--rw-r--r--   0        0        0     1142 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/payment_methods_request.py
--rw-r--r--   0        0        0     1148 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/payment_methods_response.py
--rw-r--r--   0        0        0      849 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/payment_rail_markup.py
--rw-r--r--   0        0        0      482 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/payment_rail_markup_type.py
--rw-r--r--   0        0        0     1145 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/payment_rail_request.py
--rw-r--r--   0        0        0      843 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/organization/types/payment_rail_response.py
--rw-r--r--   0        0        0     1597 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/__init__.py
--rw-r--r--   0        0        0     2083 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/__init__.py
--rw-r--r--   0        0        0     1215 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/bank_account_request.py
--rw-r--r--   0        0        0     1478 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/bank_account_response.py
--rw-r--r--   0        0        0      960 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/bank_status.py
--rw-r--r--   0        0        0      632 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/bank_type.py
--rw-r--r--   0        0        0      819 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/card_brand.py
--rw-r--r--   0        0        0     1141 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/card_request.py
--rw-r--r--   0        0        0     1480 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/card_response.py
--rw-r--r--   0        0        0      750 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/card_type.py
--rw-r--r--   0        0        0     1152 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/check_request.py
--rw-r--r--   0        0        0     1506 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/check_response.py
--rw-r--r--   0        0        0    22179 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/currency_code.py
--rw-r--r--   0        0        0     1554 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/custom_payment_method_request.py
--rw-r--r--   0        0        0     2084 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/custom_payment_method_response.py
--rw-r--r--   0        0        0     1625 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/custom_payment_method_update_request.py
--rw-r--r--   0        0        0     1264 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/payment_method_request.py
--rw-r--r--   0        0        0     1298 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/payment_method_response.py
--rw-r--r--   0        0        0     1229 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/payment_method_type.py
--rw-r--r--   0        0        0      514 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method/types/payment_method_update_request.py
--rw-r--r--   0        0        0      369 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method_schema/__init__.py
--rw-r--r--   0        0        0    12318 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method_schema/client.py
--rw-r--r--   0        0        0      500 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/__init__.py
--rw-r--r--   0        0        0     1984 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py
--rw-r--r--   0        0        0      682 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py
--rw-r--r--   0        0        0     1604 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py
--rw-r--r--   0        0        0     1732 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py
--rw-r--r--   0        0        0      271 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/transaction/__init__.py
--rw-r--r--   0        0        0     6642 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/transaction/client.py
--rw-r--r--   0        0        0      386 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/transaction/types/__init__.py
--rw-r--r--   0        0        0       85 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/transaction/types/transaction_id.py
--rw-r--r--   0        0        0     1132 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/transaction/types/transaction_response.py
--rw-r--r--   0        0        0     1564 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/transaction/types/transaction_response_expanded.py
--rw-r--r--   0        0        0     1261 2023-07-08 22:39:19.358413 mercoa-0.2.0/src/mercoa/resources/transaction/types/transaction_status.py
--rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 mercoa-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1930 2023-07-11 00:12:39.048495 mercoa-0.2.1/README.md
+-rw-r--r--   0        0        0      368 2023-07-11 00:12:39.048495 mercoa-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     7261 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/__init__.py
+-rw-r--r--   0        0        0     2384 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/client.py
+-rw-r--r--   0        0        0      348 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      157 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/environment.py
+-rw-r--r--   0        0        0        0 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/py.typed
+-rw-r--r--   0        0        0     7370 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/__init__.py
+-rw-r--r--   0        0        0      165 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/bank_lookup/__init__.py
+-rw-r--r--   0        0        0     3801 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/bank_lookup/client.py
+-rw-r--r--   0        0        0      205 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/bank_lookup/types/__init__.py
+-rw-r--r--   0        0        0      960 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/bank_lookup/types/bank_address.py
+-rw-r--r--   0        0        0      946 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py
+-rw-r--r--   0        0        0      499 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/__init__.py
+-rw-r--r--   0        0        0      314 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/errors/__init__.py
+-rw-r--r--   0        0        0      237 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/errors/auth_header_malformed_error.py
+-rw-r--r--   0        0        0      221 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/errors/auth_header_missing_error.py
+-rw-r--r--   0        0        0      225 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/errors/unauthorized.py
+-rw-r--r--   0        0        0      469 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/__init__.py
+-rw-r--r--   0        0        0     1093 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/address.py
+-rw-r--r--   0        0        0      824 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/birth_date.py
+-rw-r--r--   0        0        0      994 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/full_name.py
+-rw-r--r--   0        0        0      850 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/individual_government_id.py
+-rw-r--r--   0        0        0      857 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/itin.py
+-rw-r--r--   0        0        0      441 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/order_direction.py
+-rw-r--r--   0        0        0      855 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/phone_number.py
+-rw-r--r--   0        0        0      856 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/commons/types/ssn.py
+-rw-r--r--   0        0        0      471 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/__init__.py
+-rw-r--r--   0        0        0    33579 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/client.py
+-rw-r--r--   0        0        0      453 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/__init__.py
+-rw-r--r--   0        0        0      228 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/approval_policy/__init__.py
+-rw-r--r--   0        0        0    17689 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/approval_policy/client.py
+-rw-r--r--   0        0        0      305 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/approval_policy/errors/__init__.py
+-rw-r--r--   0        0        0      242 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/approval_policy/errors/num_approver_less_than_one_error.py
+-rw-r--r--   0        0        0      248 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/approval_policy/errors/num_approvers_user_list_mismatch_error.py
+-rw-r--r--   0        0        0       65 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/counterparty/__init__.py
+-rw-r--r--   0        0        0     4109 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/counterparty/client.py
+-rw-r--r--   0        0        0       65 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    11242 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/invoice/client.py
+-rw-r--r--   0        0        0       65 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/payment_method/__init__.py
+-rw-r--r--   0        0        0    22306 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/payment_method/client.py
+-rw-r--r--   0        0        0       65 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/representative/__init__.py
+-rw-r--r--   0        0        0    12767 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/representative/client.py
+-rw-r--r--   0        0        0       65 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/user/__init__.py
+-rw-r--r--   0        0        0    15327 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity/resources/user/client.py
+-rw-r--r--   0        0        0     1911 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/__init__.py
+-rw-r--r--   0        0        0     2766 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/__init__.py
+-rw-r--r--   0        0        0      487 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/account_type.py
+-rw-r--r--   0        0        0      849 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/amount_trigger.py
+-rw-r--r--   0        0        0       88 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/approval_policy_id.py
+-rw-r--r--   0        0        0     1100 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/approval_policy_request.py
+-rw-r--r--   0        0        0     1036 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/approval_policy_response.py
+-rw-r--r--   0        0        0     1067 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/approval_policy_update_request.py
+-rw-r--r--   0        0        0      963 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/approver_rule.py
+-rw-r--r--   0        0        0     1535 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/business_profile_request.py
+-rw-r--r--   0        0        0     1492 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/business_profile_response.py
+-rw-r--r--   0        0        0     1917 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/business_type.py
+-rw-r--r--   0        0        0     1013 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/counterparty_response.py
+-rw-r--r--   0        0        0      741 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/ein.py
+-rw-r--r--   0        0        0      914 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_add_payees_request.py
+-rw-r--r--   0        0        0       80 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_id.py
+-rw-r--r--   0        0        0     2432 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_request.py
+-rw-r--r--   0        0        0     1814 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_response.py
+-rw-r--r--   0        0        0     1084 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_status.py
+-rw-r--r--   0        0        0     2084 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_update_request.py
+-rw-r--r--   0        0        0       84 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_user_id.py
+-rw-r--r--   0        0        0     1100 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_user_request.py
+-rw-r--r--   0        0        0     1224 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_user_response.py
+-rw-r--r--   0        0        0     1446 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/find_counterparties_response.py
+-rw-r--r--   0        0        0      633 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/identifier_list.py
+-rw-r--r--   0        0        0     1372 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/individual_profile_request.py
+-rw-r--r--   0        0        0     1206 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/individual_profile_response.py
+-rw-r--r--   0        0        0      974 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/profile_request.py
+-rw-r--r--   0        0        0      981 2023-07-11 00:12:39.048495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/profile_response.py
+-rw-r--r--   0        0        0       88 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/representative_id.py
+-rw-r--r--   0        0        0     1370 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/representative_request.py
+-rw-r--r--   0        0        0     1539 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/representative_response.py
+-rw-r--r--   0        0        0     1100 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/responsibilities.py
+-rw-r--r--   0        0        0      391 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/rule.py
+-rw-r--r--   0        0        0      761 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/tax_id.py
+-rw-r--r--   0        0        0      573 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/entity_types/types/trigger.py
+-rw-r--r--   0        0        0      163 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/__init__.py
+-rw-r--r--   0        0        0    20834 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/client.py
+-rw-r--r--   0        0        0      154 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/resources/approval/__init__.py
+-rw-r--r--   0        0        0     6559 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/resources/approval/client.py
+-rw-r--r--   0        0        0       65 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/resources/comment/__init__.py
+-rw-r--r--   0        0        0    15332 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/resources/comment/client.py
+-rw-r--r--   0        0        0       65 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/resources/document/__init__.py
+-rw-r--r--   0        0        0     3870 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice/resources/document/client.py
+-rw-r--r--   0        0        0      907 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/__init__.py
+-rw-r--r--   0        0        0     1346 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/__init__.py
+-rw-r--r--   0        0        0     1017 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/approval_request.py
+-rw-r--r--   0        0        0      631 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/approver_action.py
+-rw-r--r--   0        0        0      905 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/assigned_approver.py
+-rw-r--r--   0        0        0      984 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/associated_approval_action.py
+-rw-r--r--   0        0        0       81 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/comment_id.py
+-rw-r--r--   0        0        0      934 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/comment_request.py
+-rw-r--r--   0        0        0     1428 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/comment_response.py
+-rw-r--r--   0        0        0      851 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/document_response.py
+-rw-r--r--   0        0        0     1409 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_approver_response.py
+-rw-r--r--   0        0        0       81 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_id.py
+-rw-r--r--   0        0        0     1331 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py
+-rw-r--r--   0        0        0     1258 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py
+-rw-r--r--   0        0        0     1072 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py
+-rw-r--r--   0        0        0      870 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py
+-rw-r--r--   0        0        0     3439 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_request.py
+-rw-r--r--   0        0        0     4252 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_response.py
+-rw-r--r--   0        0        0     1485 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_status.py
+-rw-r--r--   0        0        0      155 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/ocr/__init__.py
+-rw-r--r--   0        0        0     4424 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/ocr/client.py
+-rw-r--r--   0        0        0      189 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/ocr/types/__init__.py
+-rw-r--r--   0        0        0     1258 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/ocr/types/ocr_response.py
+-rw-r--r--   0        0        0      642 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/ocr/types/vendor_network.py
+-rw-r--r--   0        0        0      983 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/__init__.py
+-rw-r--r--   0        0        0    10870 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/client.py
+-rw-r--r--   0        0        0     1466 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/__init__.py
+-rw-r--r--   0        0        0      948 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/color_scheme_request.py
+-rw-r--r--   0        0        0      949 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/color_scheme_response.py
+-rw-r--r--   0        0        0      981 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/email_log_response.py
+-rw-r--r--   0        0        0      932 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/email_provider_request.py
+-rw-r--r--   0        0        0      936 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/email_provider_response.py
+-rw-r--r--   0        0        0      785 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/email_sender_provider.py
+-rw-r--r--   0        0        0     1052 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/email_sender_request.py
+-rw-r--r--   0        0        0     1044 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/email_sender_response.py
+-rw-r--r--   0        0        0       86 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/organization_id.py
+-rw-r--r--   0        0        0     1463 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/organization_request.py
+-rw-r--r--   0        0        0     1579 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/organization_response.py
+-rw-r--r--   0        0        0     1142 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/payment_methods_request.py
+-rw-r--r--   0        0        0     1148 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/payment_methods_response.py
+-rw-r--r--   0        0        0      849 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/payment_rail_markup.py
+-rw-r--r--   0        0        0      482 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/payment_rail_markup_type.py
+-rw-r--r--   0        0        0     1151 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/payment_rail_request.py
+-rw-r--r--   0        0        0      843 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/organization/types/payment_rail_response.py
+-rw-r--r--   0        0        0       65 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_schema/__init__.py
+-rw-r--r--   0        0        0    12375 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_schema/client.py
+-rw-r--r--   0        0        0     2501 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/__init__.py
+-rw-r--r--   0        0        0     3514 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/__init__.py
+-rw-r--r--   0        0        0     1287 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py
+-rw-r--r--   0        0        0     1466 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py
+-rw-r--r--   0        0        0     1026 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_account_request.py
+-rw-r--r--   0        0        0     1014 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_account_response.py
+-rw-r--r--   0        0        0      960 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_status.py
+-rw-r--r--   0        0        0      632 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_type.py
+-rw-r--r--   0        0        0     1247 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_base_request.py
+-rw-r--r--   0        0        0     1468 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_base_response.py
+-rw-r--r--   0        0        0      819 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_brand.py
+-rw-r--r--   0        0        0      961 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_request.py
+-rw-r--r--   0        0        0      935 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_response.py
+-rw-r--r--   0        0        0      750 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_type.py
+-rw-r--r--   0        0        0     1258 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/check_base_request.py
+-rw-r--r--   0        0        0     1494 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/check_base_response.py
+-rw-r--r--   0        0        0      967 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/check_request.py
+-rw-r--r--   0        0        0      941 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/check_response.py
+-rw-r--r--   0        0        0    22179 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/currency_code.py
+-rw-r--r--   0        0        0     1607 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py
+-rw-r--r--   0        0        0     2026 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py
+-rw-r--r--   0        0        0     1040 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py
+-rw-r--r--   0        0        0     1028 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_response.py
+-rw-r--r--   0        0        0     1613 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py
+-rw-r--r--   0        0        0     1071 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_request.py
+-rw-r--r--   0        0        0       87 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_id.py
+-rw-r--r--   0        0        0     1264 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_request.py
+-rw-r--r--   0        0        0     1298 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_response.py
+-rw-r--r--   0        0        0     1984 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py
+-rw-r--r--   0        0        0      682 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py
+-rw-r--r--   0        0        0       93 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_id.py
+-rw-r--r--   0        0        0     1581 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py
+-rw-r--r--   0        0        0     1693 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py
+-rw-r--r--   0        0        0     1229 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_type.py
+-rw-r--r--   0        0        0      514 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py
+-rw-r--r--   0        0        0      271 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/transaction/__init__.py
+-rw-r--r--   0        0        0     6642 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/transaction/client.py
+-rw-r--r--   0        0        0      386 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/transaction/types/__init__.py
+-rw-r--r--   0        0        0       85 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/transaction/types/transaction_id.py
+-rw-r--r--   0        0        0     1138 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/transaction/types/transaction_response.py
+-rw-r--r--   0        0        0     1582 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/transaction/types/transaction_response_expanded.py
+-rw-r--r--   0        0        0     1261 2023-07-11 00:12:39.052495 mercoa-0.2.1/src/mercoa/resources/transaction/types/transaction_status.py
+-rw-r--r--   0        0        0     2433 1970-01-01 00:00:00.000000 mercoa-0.2.1/PKG-INFO
```

### Comparing `mercoa-0.2.0/README.md` & `mercoa-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/client.py` & `mercoa-0.2.1/src/mercoa/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/core/datetime_utils.py` & `mercoa-0.2.1/src/mercoa/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/core/jsonable_encoder.py` & `mercoa-0.2.1/src/mercoa/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/bank_lookup/client.py` & `mercoa-0.2.1/src/mercoa/resources/bank_lookup/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/bank_lookup/types/bank_address.py` & `mercoa-0.2.1/src/mercoa/resources/bank_lookup/types/bank_address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py` & `mercoa-0.2.1/src/mercoa/resources/bank_lookup/types/bank_lookup_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/commons/types/address.py` & `mercoa-0.2.1/src/mercoa/resources/commons/types/address.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/commons/types/birth_date.py` & `mercoa-0.2.1/src/mercoa/resources/commons/types/birth_date.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/commons/types/full_name.py` & `mercoa-0.2.1/src/mercoa/resources/commons/types/full_name.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/commons/types/individual_government_id.py` & `mercoa-0.2.1/src/mercoa/resources/commons/types/individual_government_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/commons/types/itin.py` & `mercoa-0.2.1/src/mercoa/resources/commons/types/itin.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/commons/types/phone_number.py` & `mercoa-0.2.1/src/mercoa/resources/commons/types/phone_number.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/commons/types/ssn.py` & `mercoa-0.2.1/src/mercoa/resources/commons/types/ssn.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/client.py` & `mercoa-0.2.1/src/mercoa/resources/entity/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
 from ..commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ..commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ..commons.errors.unauthorized import Unauthorized
-from ..commons.types.entity_id import EntityId
+from ..entity_types.types.entity_add_payees_request import EntityAddPayeesRequest
+from ..entity_types.types.entity_id import EntityId
+from ..entity_types.types.entity_request import EntityRequest
+from ..entity_types.types.entity_response import EntityResponse
+from ..entity_types.types.entity_status import EntityStatus
+from ..entity_types.types.entity_update_request import EntityUpdateRequest
 from .resources.approval_policy.client import ApprovalPolicyClient, AsyncApprovalPolicyClient
 from .resources.counterparty.client import AsyncCounterpartyClient, CounterpartyClient
 from .resources.invoice.client import AsyncInvoiceClient, InvoiceClient
 from .resources.payment_method.client import AsyncPaymentMethodClient, PaymentMethodClient
 from .resources.representative.client import AsyncRepresentativeClient, RepresentativeClient
 from .resources.user.client import AsyncUserClient, UserClient
-from .types.entity_add_payees_request import EntityAddPayeesRequest
-from .types.entity_request import EntityRequest
-from .types.entity_response import EntityResponse
-from .types.entity_status import EntityStatus
-from .types.entity_update_request import EntityUpdateRequest
 
 
 class EntityClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
         self.approval_policy = ApprovalPolicyClient(environment=self._environment, token=self._token)
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/client.py` & `mercoa-0.2.1/src/mercoa/resources/entity/resources/approval_policy/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 from .....core.api_error import ApiError
 from .....core.jsonable_encoder import jsonable_encoder
 from .....core.remove_none_from_headers import remove_none_from_headers
 from .....environment import MercoaEnvironment
 from ....commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ....commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ....commons.errors.unauthorized import Unauthorized
-from ....commons.types.approval_policy_id import ApprovalPolicyId
-from ....commons.types.entity_id import EntityId
+from ....entity_types.types.approval_policy_id import ApprovalPolicyId
+from ....entity_types.types.approval_policy_request import ApprovalPolicyRequest
+from ....entity_types.types.approval_policy_response import ApprovalPolicyResponse
+from ....entity_types.types.approval_policy_update_request import ApprovalPolicyUpdateRequest
+from ....entity_types.types.entity_id import EntityId
 from .errors.num_approver_less_than_one_error import NumApproverLessThanOneError
 from .errors.num_approvers_user_list_mismatch_error import NumApproversUserListMismatchError
-from .types.approval_policy_request import ApprovalPolicyRequest
-from .types.approval_policy_response import ApprovalPolicyResponse
-from .types.approval_policy_update_request import ApprovalPolicyUpdateRequest
 
 
 class ApprovalPolicyClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/amount_trigger.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/amount_trigger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
-from .....payment_method.types.currency_code import CurrencyCode
+from ....core.datetime_utils import serialize_datetime
+from ...payment_method_types.types.currency_code import CurrencyCode
 
 
 class AmountTrigger(pydantic.BaseModel):
     amount: float
     currency: CurrencyCode
 
     def json(self, **kwargs: typing.Any) -> str:
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/approval_policy_request.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/approval_policy_request.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
-from .....commons.types.approval_policy_id import ApprovalPolicyId
+from ....core.datetime_utils import serialize_datetime
+from .approval_policy_id import ApprovalPolicyId
 from .rule import Rule
 from .trigger import Trigger
 
 
 class ApprovalPolicyRequest(pydantic.BaseModel):
     trigger: Trigger
     rule: Rule
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/approval_policy_response.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/approval_policy_update_request.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
-from .....commons.types.approval_policy_id import ApprovalPolicyId
+from ....core.datetime_utils import serialize_datetime
+from .approval_policy_id import ApprovalPolicyId
 from .rule import Rule
 from .trigger import Trigger
 
 
-class ApprovalPolicyResponse(pydantic.BaseModel):
-    id: ApprovalPolicyId
-    trigger: Trigger
-    rule: Rule
-    upstream_policy_id: ApprovalPolicyId = pydantic.Field(alias="upstreamPolicyId")
+class ApprovalPolicyUpdateRequest(pydantic.BaseModel):
+    trigger: typing.Optional[Trigger]
+    rule: typing.Optional[Rule]
+    upstream_policy_id: typing.Optional[ApprovalPolicyId] = pydantic.Field(alias="upstreamPolicyId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/approval_policy_update_request.py` & `mercoa-0.2.1/src/mercoa/resources/organization/types/color_scheme_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
-from .....commons.types.approval_policy_id import ApprovalPolicyId
-from .rule import Rule
-from .trigger import Trigger
+from ....core.datetime_utils import serialize_datetime
 
 
-class ApprovalPolicyUpdateRequest(pydantic.BaseModel):
-    trigger: typing.Optional[Trigger]
-    rule: typing.Optional[Rule]
-    upstream_policy_id: typing.Optional[ApprovalPolicyId] = pydantic.Field(alias="upstreamPolicyId")
+class ColorSchemeResponse(pydantic.BaseModel):
+    primary_color: typing.Optional[str] = pydantic.Field(alias="primaryColor")
+    secondary_color: typing.Optional[str] = pydantic.Field(alias="secondaryColor")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/approver_rule.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/approver_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
+from ....core.datetime_utils import serialize_datetime
 from .identifier_list import IdentifierList
 
 
 class ApproverRule(pydantic.BaseModel):
     num_approvers: int = pydantic.Field(alias="numApprovers")
     identifier_list: IdentifierList = pydantic.Field(alias="identifierList")
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/identifier_list.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/identifier_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 import typing
 
 import pydantic
 import typing_extensions
 
-from .....commons.types.entity_user_id import EntityUserId
+from .entity_user_id import EntityUserId
 
 
 class IdentifierList_RolesList(pydantic.BaseModel):
     type: typing_extensions.Literal["rolesList"]
     value: typing.List[str]
 
     class Config:
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/approval_policy/types/trigger.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/trigger.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/counterparty/client.py` & `mercoa-0.2.1/src/mercoa/resources/entity/resources/counterparty/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 from .....core.api_error import ApiError
 from .....core.remove_none_from_headers import remove_none_from_headers
 from .....environment import MercoaEnvironment
 from ....commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ....commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ....commons.errors.unauthorized import Unauthorized
-from ....commons.types.entity_id import EntityId
-from .types.find_counterparties_response import FindCounterpartiesResponse
+from ....entity_types.types.entity_id import EntityId
+from ....entity_types.types.find_counterparties_response import FindCounterpartiesResponse
 
 
 class CounterpartyClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/counterparty/types/counterparty_response.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/counterparty_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
-from .....payment_method.types.payment_method_response import PaymentMethodResponse
-from ....types.entity_response import EntityResponse
+from ....core.datetime_utils import serialize_datetime
+from ...payment_method_types.types.payment_method_response import PaymentMethodResponse
+from .entity_response import EntityResponse
 
 
 class CounterpartyResponse(EntityResponse):
     payment_methods: typing.List[PaymentMethodResponse] = pydantic.Field(alias="paymentMethods")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/counterparty/types/find_counterparties_response.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/find_counterparties_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
+from ....core.datetime_utils import serialize_datetime
 from .counterparty_response import CounterpartyResponse
 
 
 class FindCounterpartiesResponse(pydantic.BaseModel):
     entity_counterparties: typing.List[CounterpartyResponse] = pydantic.Field(
         alias="entityCounterparties", description=("Counterparties that have been paid by this entity\n")
     )
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/invoice/client.py` & `mercoa-0.2.1/src/mercoa/resources/entity/resources/invoice/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 from .....core.api_error import ApiError
 from .....core.datetime_utils import serialize_datetime
 from .....core.remove_none_from_headers import remove_none_from_headers
 from .....environment import MercoaEnvironment
 from ....commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ....commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ....commons.errors.unauthorized import Unauthorized
-from ....commons.types.entity_id import EntityId
-from ....commons.types.invoice_id import InvoiceId
 from ....commons.types.order_direction import OrderDirection
-from ....invoice.types.invoice_order_by_field import InvoiceOrderByField
-from ....invoice.types.invoice_response import InvoiceResponse
-from ....invoice.types.invoice_status import InvoiceStatus
-from ....payment_method.types.currency_code import CurrencyCode
-from .types.invoice_metrics_response import InvoiceMetricsResponse
+from ....entity_types.types.entity_id import EntityId
+from ....invoice_types.types.invoice_id import InvoiceId
+from ....invoice_types.types.invoice_metrics_response import InvoiceMetricsResponse
+from ....invoice_types.types.invoice_order_by_field import InvoiceOrderByField
+from ....invoice_types.types.invoice_response import InvoiceResponse
+from ....invoice_types.types.invoice_status import InvoiceStatus
+from ....payment_method_types.types.currency_code import CurrencyCode
 
 
 class InvoiceClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/invoice/types/invoice_metrics_response.py` & `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_metrics_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
-from .....payment_method.types.currency_code import CurrencyCode
+from ....core.datetime_utils import serialize_datetime
+from ...payment_method_types.types.currency_code import CurrencyCode
 
 
 class InvoiceMetricsResponse(pydantic.BaseModel):
     total_amount: float = pydantic.Field(alias="totalAmount")
     total_count: int = pydantic.Field(alias="totalCount")
     average_amount: float = pydantic.Field(alias="averageAmount")
     currency: CurrencyCode
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/payment_method/client.py` & `mercoa-0.2.1/src/mercoa/resources/entity/resources/payment_method/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 from .....core.api_error import ApiError
 from .....core.jsonable_encoder import jsonable_encoder
 from .....core.remove_none_from_headers import remove_none_from_headers
 from .....environment import MercoaEnvironment
 from ....commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ....commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ....commons.errors.unauthorized import Unauthorized
-from ....commons.types.entity_id import EntityId
-from ....commons.types.payment_method_id import PaymentMethodId
-from ....payment_method.types.payment_method_request import PaymentMethodRequest
-from ....payment_method.types.payment_method_response import PaymentMethodResponse
-from ....payment_method.types.payment_method_type import PaymentMethodType
-from ....payment_method.types.payment_method_update_request import PaymentMethodUpdateRequest
+from ....entity_types.types.entity_id import EntityId
+from ....payment_method_types.types.payment_method_id import PaymentMethodId
+from ....payment_method_types.types.payment_method_request import PaymentMethodRequest
+from ....payment_method_types.types.payment_method_response import PaymentMethodResponse
+from ....payment_method_types.types.payment_method_type import PaymentMethodType
+from ....payment_method_types.types.payment_method_update_request import PaymentMethodUpdateRequest
 
 
 class PaymentMethodClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/client.py` & `mercoa-0.2.1/src/mercoa/resources/entity/resources/representative/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from .....core.api_error import ApiError
 from .....core.jsonable_encoder import jsonable_encoder
 from .....core.remove_none_from_headers import remove_none_from_headers
 from .....environment import MercoaEnvironment
 from ....commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ....commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ....commons.errors.unauthorized import Unauthorized
-from ....commons.types.entity_id import EntityId
-from .types.representative_id import RepresentativeId
-from .types.representative_request import RepresentativeRequest
-from .types.representative_response import RepresentativeResponse
+from ....entity_types.types.entity_id import EntityId
+from ....entity_types.types.representative_id import RepresentativeId
+from ....entity_types.types.representative_request import RepresentativeRequest
+from ....entity_types.types.representative_response import RepresentativeResponse
 
 
 class RepresentativeClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/types/representative_request.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/representative_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
-from .....commons.types.address import Address
-from .....commons.types.birth_date import BirthDate
-from .....commons.types.full_name import FullName
-from .....commons.types.individual_government_id import IndividualGovernmentId
-from .....commons.types.phone_number import PhoneNumber
+from ....core.datetime_utils import serialize_datetime
+from ...commons.types.address import Address
+from ...commons.types.birth_date import BirthDate
+from ...commons.types.full_name import FullName
+from ...commons.types.individual_government_id import IndividualGovernmentId
+from ...commons.types.phone_number import PhoneNumber
 from .responsibilities import Responsibilities
 
 
 class RepresentativeRequest(pydantic.BaseModel):
     name: FullName
     phone: PhoneNumber
     email: str
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/types/representative_response.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/representative_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
-from .....commons.types.address import Address
-from .....commons.types.full_name import FullName
-from .....commons.types.phone_number import PhoneNumber
+from ....core.datetime_utils import serialize_datetime
+from ...commons.types.address import Address
+from ...commons.types.full_name import FullName
+from ...commons.types.phone_number import PhoneNumber
 from .representative_id import RepresentativeId
 from .responsibilities import Responsibilities
 
 
 class RepresentativeResponse(pydantic.BaseModel):
     id: RepresentativeId
     name: FullName
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/representative/types/responsibilities.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/responsibilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
+from ....core.datetime_utils import serialize_datetime
 
 
 class Responsibilities(pydantic.BaseModel):
     job_title: typing.Optional[str] = pydantic.Field(alias="jobTitle")
     is_controller: typing.Optional[bool] = pydantic.Field(alias="isController")
     is_owner: typing.Optional[bool] = pydantic.Field(alias="isOwner")
     ownership_percentage: typing.Optional[float] = pydantic.Field(alias="ownershipPercentage")
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/user/client.py` & `mercoa-0.2.1/src/mercoa/resources/entity/resources/user/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from .....core.api_error import ApiError
 from .....core.jsonable_encoder import jsonable_encoder
 from .....core.remove_none_from_headers import remove_none_from_headers
 from .....environment import MercoaEnvironment
 from ....commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ....commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ....commons.errors.unauthorized import Unauthorized
-from ....commons.types.entity_id import EntityId
-from ....commons.types.entity_user_id import EntityUserId
-from .types.entity_user_request import EntityUserRequest
-from .types.entity_user_response import EntityUserResponse
+from ....entity_types.types.entity_id import EntityId
+from ....entity_types.types.entity_user_id import EntityUserId
+from ....entity_types.types.entity_user_request import EntityUserRequest
+from ....entity_types.types.entity_user_response import EntityUserResponse
 
 
 class UserClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/user/types/entity_user_request.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
+from ....core.datetime_utils import serialize_datetime
 
 
 class EntityUserRequest(pydantic.BaseModel):
     foreign_id: typing.Optional[str] = pydantic.Field(alias="foreignId")
     email: typing.Optional[str]
     name: typing.Optional[str]
     roles: typing.Optional[typing.List[str]] = pydantic.Field(
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/resources/user/types/entity_user_response.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_user_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
-from .....commons.types.entity_user_id import EntityUserId
+from ....core.datetime_utils import serialize_datetime
+from .entity_user_id import EntityUserId
 
 
 class EntityUserResponse(pydantic.BaseModel):
     id: EntityUserId
     foreign_id: typing.Optional[str] = pydantic.Field(
         alias="foreignId", description=("Id from external auth provider or your auth system\n")
     )
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/types/business_profile_request.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/business_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/types/business_profile_response.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/business_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/types/business_type.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/business_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/types/ein.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/ein.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/types/entity_add_payees_request.py` & `mercoa-0.2.1/src/mercoa/resources/organization/types/email_provider_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.entity_id import EntityId
+from .email_sender_response import EmailSenderResponse
 
 
-class EntityAddPayeesRequest(pydantic.BaseModel):
-    payees: typing.List[EntityId] = pydantic.Field(
-        description=("List of payee entity IDs to associate with the entity\n")
-    )
+class EmailProviderResponse(pydantic.BaseModel):
+    sender: EmailSenderResponse
+    inbox_domain: str = pydantic.Field(alias="inboxDomain")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/types/entity_request.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/types/entity_response.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.entity_id import EntityId
 from .account_type import AccountType
+from .entity_id import EntityId
 from .entity_status import EntityStatus
 from .profile_response import ProfileResponse
 
 
 class EntityResponse(pydantic.BaseModel):
     id: EntityId
     foreign_id: typing.Optional[str] = pydantic.Field(alias="foreignId")
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/types/entity_status.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/types/entity_update_request.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/entity_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/types/individual_profile_request.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/individual_profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/types/individual_profile_response.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/individual_profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/types/profile_request.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/profile_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/types/profile_response.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/profile_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/entity/types/tax_id.py` & `mercoa-0.2.1/src/mercoa/resources/entity_types/types/tax_id.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/__init__.py` & `mercoa-0.2.1/src/mercoa/resources/invoice_types/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 # This file was auto-generated by Fern from our API Definition.
 
-from .resources import ApprovalRequest, CommentRequest, CommentResponse, DocumentResponse, approval, comment, document
 from .types import (
+    ApprovalRequest,
     ApproverAction,
     AssignedApprover,
     AssociatedApprovalAction,
+    CommentId,
+    CommentRequest,
+    CommentResponse,
+    DocumentResponse,
     InvoiceApproverResponse,
+    InvoiceId,
     InvoiceLineItemRequest,
     InvoiceLineItemResponse,
+    InvoiceMetricsResponse,
     InvoiceOrderByField,
     InvoiceRequest,
     InvoiceResponse,
     InvoiceStatus,
 )
 
 __all__ = [
     "ApprovalRequest",
     "ApproverAction",
     "AssignedApprover",
     "AssociatedApprovalAction",
+    "CommentId",
     "CommentRequest",
     "CommentResponse",
     "DocumentResponse",
     "InvoiceApproverResponse",
+    "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
+    "InvoiceMetricsResponse",
     "InvoiceOrderByField",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
-    "approval",
-    "comment",
-    "document",
 ]
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/client.py` & `mercoa-0.2.1/src/mercoa/resources/invoice/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,24 +12,24 @@
 from ...core.datetime_utils import serialize_datetime
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
 from ..commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ..commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ..commons.errors.unauthorized import Unauthorized
-from ..commons.types.entity_id import EntityId
-from ..commons.types.invoice_id import InvoiceId
 from ..commons.types.order_direction import OrderDirection
+from ..entity_types.types.entity_id import EntityId
+from ..invoice_types.types.invoice_id import InvoiceId
+from ..invoice_types.types.invoice_order_by_field import InvoiceOrderByField
+from ..invoice_types.types.invoice_request import InvoiceRequest
+from ..invoice_types.types.invoice_response import InvoiceResponse
+from ..invoice_types.types.invoice_status import InvoiceStatus
 from .resources.approval.client import ApprovalClient, AsyncApprovalClient
 from .resources.comment.client import AsyncCommentClient, CommentClient
 from .resources.document.client import AsyncDocumentClient, DocumentClient
-from .types.invoice_order_by_field import InvoiceOrderByField
-from .types.invoice_request import InvoiceRequest
-from .types.invoice_response import InvoiceResponse
-from .types.invoice_status import InvoiceStatus
 
 
 class InvoiceClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
         self.approval = ApprovalClient(environment=self._environment, token=self._token)
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/resources/approval/client.py` & `mercoa-0.2.1/src/mercoa/resources/invoice/resources/approval/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from .....core.api_error import ApiError
 from .....core.jsonable_encoder import jsonable_encoder
 from .....core.remove_none_from_headers import remove_none_from_headers
 from .....environment import MercoaEnvironment
 from ....commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ....commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ....commons.errors.unauthorized import Unauthorized
-from ....commons.types.invoice_id import InvoiceId
-from .types.approval_request import ApprovalRequest
+from ....invoice_types.types.approval_request import ApprovalRequest
+from ....invoice_types.types.invoice_id import InvoiceId
 
 
 class ApprovalClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/resources/approval/types/approval_request.py` & `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/approval_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
-from .....commons.types.entity_user_id import EntityUserId
+from ....core.datetime_utils import serialize_datetime
+from ...entity_types.types.entity_user_id import EntityUserId
 
 
 class ApprovalRequest(pydantic.BaseModel):
     text: typing.Optional[str] = pydantic.Field(description=("Comment associated with this approval action.\n"))
     user_id: EntityUserId = pydantic.Field(alias="userId")
 
     def json(self, **kwargs: typing.Any) -> str:
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/resources/comment/client.py` & `mercoa-0.2.1/src/mercoa/resources/invoice/resources/comment/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from .....core.api_error import ApiError
 from .....core.jsonable_encoder import jsonable_encoder
 from .....core.remove_none_from_headers import remove_none_from_headers
 from .....environment import MercoaEnvironment
 from ....commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ....commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ....commons.errors.unauthorized import Unauthorized
-from ....commons.types.comment_id import CommentId
-from ....commons.types.invoice_id import InvoiceId
-from .types.comment_request import CommentRequest
-from .types.comment_response import CommentResponse
+from ....invoice_types.types.comment_id import CommentId
+from ....invoice_types.types.comment_request import CommentRequest
+from ....invoice_types.types.comment_response import CommentResponse
+from ....invoice_types.types.invoice_id import InvoiceId
 
 
 class CommentClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/resources/comment/types/comment_request.py` & `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/comment_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
-from .....commons.types.entity_user_id import EntityUserId
+from ....core.datetime_utils import serialize_datetime
+from ...entity_types.types.entity_user_id import EntityUserId
 
 
 class CommentRequest(pydantic.BaseModel):
     text: str
     user_id: typing.Optional[EntityUserId] = pydantic.Field(alias="userId")
 
     def json(self, **kwargs: typing.Any) -> str:
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/resources/comment/types/comment_response.py` & `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/comment_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
-from .....entity.resources.user.types.entity_user_response import EntityUserResponse
-from ....types.associated_approval_action import AssociatedApprovalAction
+from ....core.datetime_utils import serialize_datetime
+from ...entity_types.types.entity_user_response import EntityUserResponse
+from .associated_approval_action import AssociatedApprovalAction
 
 
 class CommentResponse(pydantic.BaseModel):
     id: str
     text: str
     user: typing.Optional[EntityUserResponse]
     associated_approval_action: typing.Optional[AssociatedApprovalAction] = pydantic.Field(
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/resources/document/client.py` & `mercoa-0.2.1/src/mercoa/resources/invoice/resources/document/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 from .....core.api_error import ApiError
 from .....core.remove_none_from_headers import remove_none_from_headers
 from .....environment import MercoaEnvironment
 from ....commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ....commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ....commons.errors.unauthorized import Unauthorized
-from ....commons.types.invoice_id import InvoiceId
-from .types.document_response import DocumentResponse
+from ....invoice_types.types.document_response import DocumentResponse
+from ....invoice_types.types.invoice_id import InvoiceId
 
 
 class DocumentClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/resources/document/types/document_response.py` & `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/document_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 import pydantic
 
-from ......core.datetime_utils import serialize_datetime
+from ....core.datetime_utils import serialize_datetime
 
 
 class DocumentResponse(pydantic.BaseModel):
     mime_type: str = pydantic.Field(alias="mimeType")
     uri: str
 
     def json(self, **kwargs: typing.Any) -> str:
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/types/__init__.py` & `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,39 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from .approval_request import ApprovalRequest
 from .approver_action import ApproverAction
 from .assigned_approver import AssignedApprover
 from .associated_approval_action import AssociatedApprovalAction
+from .comment_id import CommentId
+from .comment_request import CommentRequest
+from .comment_response import CommentResponse
+from .document_response import DocumentResponse
 from .invoice_approver_response import InvoiceApproverResponse
+from .invoice_id import InvoiceId
 from .invoice_line_item_request import InvoiceLineItemRequest
 from .invoice_line_item_response import InvoiceLineItemResponse
+from .invoice_metrics_response import InvoiceMetricsResponse
 from .invoice_order_by_field import InvoiceOrderByField
 from .invoice_request import InvoiceRequest
 from .invoice_response import InvoiceResponse
 from .invoice_status import InvoiceStatus
 
 __all__ = [
+    "ApprovalRequest",
     "ApproverAction",
     "AssignedApprover",
     "AssociatedApprovalAction",
+    "CommentId",
+    "CommentRequest",
+    "CommentResponse",
+    "DocumentResponse",
     "InvoiceApproverResponse",
+    "InvoiceId",
     "InvoiceLineItemRequest",
     "InvoiceLineItemResponse",
+    "InvoiceMetricsResponse",
     "InvoiceOrderByField",
     "InvoiceRequest",
     "InvoiceResponse",
     "InvoiceStatus",
 ]
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/types/approver_action.py` & `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/approver_action.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/types/assigned_approver.py` & `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/assigned_approver.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.entity_user_id import EntityUserId
+from ...entity_types.types.entity_user_id import EntityUserId
 
 
 class AssignedApprover(pydantic.BaseModel):
     user_id: EntityUserId = pydantic.Field(alias="userId")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/types/associated_approval_action.py` & `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/associated_approval_action.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.entity_user_id import EntityUserId
+from ...entity_types.types.entity_user_id import EntityUserId
 from .approver_action import ApproverAction
 
 
 class AssociatedApprovalAction(pydantic.BaseModel):
     user_id: EntityUserId = pydantic.Field(alias="userId")
     action: ApproverAction
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_approver_response.py` & `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_approver_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.entity_user_id import EntityUserId
+from ...entity_types.types.entity_user_id import EntityUserId
 from .approver_action import ApproverAction
 
 
 class InvoiceApproverResponse(pydantic.BaseModel):
     assigned_user_id: typing.Optional[EntityUserId] = pydantic.Field(alias="assignedUserId")
     action: ApproverAction
     eligible_roles: typing.List[str] = pydantic.Field(alias="eligibleRoles")
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_line_item_request.py` & `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_line_item_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...payment_method.types.currency_code import CurrencyCode
+from ...payment_method_types.types.currency_code import CurrencyCode
 
 
 class InvoiceLineItemRequest(pydantic.BaseModel):
     id: typing.Optional[str] = pydantic.Field(
         description=(
             "If provided, will overwrite line item on the invoice with this ID. If not provided, will create a new line item.\n"
         )
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_line_item_response.py` & `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_line_item_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...payment_method.types.currency_code import CurrencyCode
+from ...payment_method_types.types.currency_code import CurrencyCode
 
 
 class InvoiceLineItemResponse(pydantic.BaseModel):
     id: str
     amount: typing.Optional[float]
     currency: typing.Optional[CurrencyCode]
     description: typing.Optional[str]
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_order_by_field.py` & `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_order_by_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_request.py` & `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.entity_id import EntityId
-from ...commons.types.entity_user_id import EntityUserId
-from ...commons.types.invoice_id import InvoiceId
-from ...payment_method.types.currency_code import CurrencyCode
+from ...entity_types.types.entity_id import EntityId
+from ...entity_types.types.entity_user_id import EntityUserId
+from ...payment_method_types.types.currency_code import CurrencyCode
 from .assigned_approver import AssignedApprover
+from .invoice_id import InvoiceId
 from .invoice_line_item_request import InvoiceLineItemRequest
 from .invoice_status import InvoiceStatus
 
 
 class InvoiceRequest(pydantic.BaseModel):
     status: typing.Optional[InvoiceStatus]
     amount: typing.Optional[float]
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_response.py` & `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.entity_id import EntityId
-from ...commons.types.invoice_id import InvoiceId
-from ...entity.resources.approval_policy.types.approval_policy_response import ApprovalPolicyResponse
-from ...entity.resources.user.types.entity_user_response import EntityUserResponse
-from ...entity.types.entity_response import EntityResponse
-from ...payment_method.types.currency_code import CurrencyCode
-from ...payment_method.types.payment_method_response import PaymentMethodResponse
+from ...entity_types.types.approval_policy_response import ApprovalPolicyResponse
+from ...entity_types.types.entity_id import EntityId
+from ...entity_types.types.entity_response import EntityResponse
+from ...entity_types.types.entity_user_response import EntityUserResponse
+from ...payment_method_types.types.currency_code import CurrencyCode
+from ...payment_method_types.types.payment_method_response import PaymentMethodResponse
 from ...transaction.types.transaction_response import TransactionResponse
-from ..resources.comment.types.comment_response import CommentResponse
+from .comment_response import CommentResponse
 from .invoice_approver_response import InvoiceApproverResponse
+from .invoice_id import InvoiceId
 from .invoice_line_item_response import InvoiceLineItemResponse
 from .invoice_status import InvoiceStatus
 
 
 class InvoiceResponse(pydantic.BaseModel):
     id: InvoiceId
     status: InvoiceStatus
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/invoice/types/invoice_status.py` & `mercoa-0.2.1/src/mercoa/resources/invoice_types/types/invoice_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/ocr/client.py` & `mercoa-0.2.1/src/mercoa/resources/ocr/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
 from ..commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ..commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ..commons.errors.unauthorized import Unauthorized
-from ..commons.types.entity_id import EntityId
+from ..entity_types.types.entity_id import EntityId
 from .types.ocr_response import OcrResponse
 from .types.vendor_network import VendorNetwork
 
 
 class OcrClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/ocr/types/ocr_response.py` & `mercoa-0.2.1/src/mercoa/resources/ocr/types/ocr_response.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...entity.types.entity_response import EntityResponse
-from ...invoice.types.invoice_response import InvoiceResponse
-from ...payment_method.types.bank_account_response import BankAccountResponse
-from ...payment_method.types.check_response import CheckResponse
+from ...entity_types.types.entity_response import EntityResponse
+from ...invoice_types.types.invoice_response import InvoiceResponse
+from ...payment_method_types.types.bank_account_response import BankAccountResponse
+from ...payment_method_types.types.check_response import CheckResponse
 
 
 class OcrResponse(pydantic.BaseModel):
     invoice: InvoiceResponse
     vendor: EntityResponse
     check: typing.Optional[CheckResponse]
     bank_account: typing.Optional[BankAccountResponse] = pydantic.Field(alias="bankAccount")
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/ocr/types/vendor_network.py` & `mercoa-0.2.1/src/mercoa/resources/ocr/types/vendor_network.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/__init__.py` & `mercoa-0.2.1/src/mercoa/resources/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/client.py` & `mercoa-0.2.1/src/mercoa/resources/organization/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/types/__init__.py` & `mercoa-0.2.1/src/mercoa/resources/organization/types/__init__.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/types/color_scheme_request.py` & `mercoa-0.2.1/src/mercoa/resources/organization/types/color_scheme_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/types/color_scheme_response.py` & `mercoa-0.2.1/src/mercoa/resources/organization/types/email_log_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 
 
-class ColorSchemeResponse(pydantic.BaseModel):
-    primary_color: typing.Optional[str] = pydantic.Field(alias="primaryColor")
-    secondary_color: typing.Optional[str] = pydantic.Field(alias="secondaryColor")
+class EmailLogResponse(pydantic.BaseModel):
+    from_: str = pydantic.Field(alias="from")
+    to: str
+    subject: str
+    raw_content: str = pydantic.Field(alias="rawContent")
+    created_at: dt.datetime = pydantic.Field(alias="createdAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/types/email_log_response.py` & `mercoa-0.2.1/src/mercoa/resources/organization/types/email_sender_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from .email_sender_provider import EmailSenderProvider
 
 
-class EmailLogResponse(pydantic.BaseModel):
-    from_: str = pydantic.Field(alias="from")
-    to: str
-    subject: str
-    raw_content: str = pydantic.Field(alias="rawContent")
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
+class EmailSenderRequest(pydantic.BaseModel):
+    provider: EmailSenderProvider
+    from_email: str = pydantic.Field(alias="fromEmail")
+    from_name: str = pydantic.Field(alias="fromName")
+    api_key: typing.Optional[str] = pydantic.Field(alias="apiKey")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/types/email_provider_request.py` & `mercoa-0.2.1/src/mercoa/resources/organization/types/email_provider_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/types/email_provider_response.py` & `mercoa-0.2.1/src/mercoa/resources/organization/types/payment_methods_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .email_sender_response import EmailSenderResponse
+from .payment_rail_response import PaymentRailResponse
 
 
-class EmailProviderResponse(pydantic.BaseModel):
-    sender: EmailSenderResponse
-    inbox_domain: str = pydantic.Field(alias="inboxDomain")
+class PaymentMethodsResponse(pydantic.BaseModel):
+    payer_payments: typing.List[PaymentRailResponse] = pydantic.Field(alias="payerPayments")
+    backup_disbursements: typing.List[PaymentRailResponse] = pydantic.Field(alias="backupDisbursements")
+    vendor_disbursements: typing.List[PaymentRailResponse] = pydantic.Field(alias="vendorDisbursements")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/types/email_sender_provider.py` & `mercoa-0.2.1/src/mercoa/resources/organization/types/email_sender_provider.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/types/email_sender_request.py` & `mercoa-0.2.1/src/mercoa/resources/organization/types/payment_rail_request.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .email_sender_provider import EmailSenderProvider
+from ...payment_method_types.types.payment_method_type import PaymentMethodType
+from .payment_rail_markup import PaymentRailMarkup
 
 
-class EmailSenderRequest(pydantic.BaseModel):
-    provider: EmailSenderProvider
-    from_email: str = pydantic.Field(alias="fromEmail")
-    from_name: str = pydantic.Field(alias="fromName")
-    api_key: typing.Optional[str] = pydantic.Field(alias="apiKey")
+class PaymentRailRequest(pydantic.BaseModel):
+    type: PaymentMethodType
+    name: str = pydantic.Field(
+        description=("Name of the payment method. For custom payment methods, this is the ID of the schema.\n")
+    )
+    markup: typing.Optional[PaymentRailMarkup]
+    description: typing.Optional[str]
+    active: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
-        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/types/email_sender_response.py` & `mercoa-0.2.1/src/mercoa/resources/organization/types/email_sender_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/types/organization_request.py` & `mercoa-0.2.1/src/mercoa/resources/organization/types/organization_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/types/organization_response.py` & `mercoa-0.2.1/src/mercoa/resources/organization/types/organization_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/types/payment_methods_request.py` & `mercoa-0.2.1/src/mercoa/resources/organization/types/payment_methods_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/types/payment_methods_response.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_response.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,21 +2,34 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from .payment_rail_response import PaymentRailResponse
-
-
-class PaymentMethodsResponse(pydantic.BaseModel):
-    payer_payments: typing.List[PaymentRailResponse] = pydantic.Field(alias="payerPayments")
-    backup_disbursements: typing.List[PaymentRailResponse] = pydantic.Field(alias="backupDisbursements")
-    vendor_disbursements: typing.List[PaymentRailResponse] = pydantic.Field(alias="vendorDisbursements")
+from .currency_code import CurrencyCode
+from .payment_method_schema_field import PaymentMethodSchemaField
+from .payment_method_schema_id import PaymentMethodSchemaId
+
+
+class PaymentMethodSchemaResponse(pydantic.BaseModel):
+    id: PaymentMethodSchemaId
+    name: str
+    is_source: bool = pydantic.Field(
+        alias="isSource", description=("This payment method can be used as a payment source for an invoice\n")
+    )
+    is_destination: bool = pydantic.Field(
+        alias="isDestination", description=("This payment method can be used as a payment destination for an invoice\n")
+    )
+    supported_currencies: typing.List[CurrencyCode] = pydantic.Field(
+        alias="supportedCurrencies", description=("List of currencies that this payment method supports.\n")
+    )
+    fields: typing.List[PaymentMethodSchemaField]
+    created_at: dt.datetime = pydantic.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/types/payment_rail_markup.py` & `mercoa-0.2.1/src/mercoa/resources/organization/types/payment_rail_markup.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/types/payment_rail_request.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_request.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,31 +2,27 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...payment_method.types.payment_method_type import PaymentMethodType
-from .payment_rail_markup import PaymentRailMarkup
+from .custom_payment_method_base_request import CustomPaymentMethodBaseRequest
 
 
-class PaymentRailRequest(pydantic.BaseModel):
-    type: PaymentMethodType
-    name: str = pydantic.Field(
-        description=("Name of the payment method. For custom payment methods, this is the ID of the schema.\n")
+class CustomPaymentMethodRequest(CustomPaymentMethodBaseRequest):
+    custom: typing.Optional[CustomPaymentMethodBaseRequest] = pydantic.Field(
+        description=("DEPRECATED DO NOT USE. WILL BE REMOVED SOON.\n")
     )
-    markup: typing.Optional[PaymentRailMarkup]
-    description: typing.Optional[str]
-    active: bool
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().dict(**kwargs_with_defaults)
 
     class Config:
         frozen = True
+        allow_population_by_field_name = True
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/organization/types/payment_rail_response.py` & `mercoa-0.2.1/src/mercoa/resources/organization/types/payment_rail_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/__init__.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,61 +1,91 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .types import (
+    BankAccountBaseRequest,
+    BankAccountBaseResponse,
     BankAccountRequest,
     BankAccountResponse,
     BankStatus,
     BankType,
+    CardBaseRequest,
+    CardBaseResponse,
     CardBrand,
     CardRequest,
     CardResponse,
     CardType,
+    CheckBaseRequest,
+    CheckBaseResponse,
     CheckRequest,
     CheckResponse,
     CurrencyCode,
+    CustomPaymentMethodBaseRequest,
+    CustomPaymentMethodBaseResponse,
     CustomPaymentMethodRequest,
     CustomPaymentMethodResponse,
+    CustomPaymentMethodUpdateBaseRequest,
     CustomPaymentMethodUpdateRequest,
+    PaymentMethodId,
     PaymentMethodRequest,
     PaymentMethodRequest_BankAccount,
     PaymentMethodRequest_Card,
     PaymentMethodRequest_Check,
     PaymentMethodRequest_Custom,
     PaymentMethodResponse,
     PaymentMethodResponse_BankAccount,
     PaymentMethodResponse_Card,
     PaymentMethodResponse_Check,
     PaymentMethodResponse_Custom,
+    PaymentMethodSchemaField,
+    PaymentMethodSchemaFieldType,
+    PaymentMethodSchemaId,
+    PaymentMethodSchemaRequest,
+    PaymentMethodSchemaResponse,
     PaymentMethodType,
     PaymentMethodUpdateRequest,
     PaymentMethodUpdateRequest_Custom,
 )
 
 __all__ = [
+    "BankAccountBaseRequest",
+    "BankAccountBaseResponse",
     "BankAccountRequest",
     "BankAccountResponse",
     "BankStatus",
     "BankType",
+    "CardBaseRequest",
+    "CardBaseResponse",
     "CardBrand",
     "CardRequest",
     "CardResponse",
     "CardType",
+    "CheckBaseRequest",
+    "CheckBaseResponse",
     "CheckRequest",
     "CheckResponse",
     "CurrencyCode",
+    "CustomPaymentMethodBaseRequest",
+    "CustomPaymentMethodBaseResponse",
     "CustomPaymentMethodRequest",
     "CustomPaymentMethodResponse",
+    "CustomPaymentMethodUpdateBaseRequest",
     "CustomPaymentMethodUpdateRequest",
+    "PaymentMethodId",
     "PaymentMethodRequest",
     "PaymentMethodRequest_BankAccount",
     "PaymentMethodRequest_Card",
     "PaymentMethodRequest_Check",
     "PaymentMethodRequest_Custom",
     "PaymentMethodResponse",
     "PaymentMethodResponse_BankAccount",
     "PaymentMethodResponse_Card",
     "PaymentMethodResponse_Check",
     "PaymentMethodResponse_Custom",
+    "PaymentMethodSchemaField",
+    "PaymentMethodSchemaFieldType",
+    "PaymentMethodSchemaId",
+    "PaymentMethodSchemaRequest",
+    "PaymentMethodSchemaResponse",
     "PaymentMethodType",
     "PaymentMethodUpdateRequest",
     "PaymentMethodUpdateRequest_Custom",
 ]
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/__init__.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,62 +1,92 @@
 # This file was auto-generated by Fern from our API Definition.
 
+from .bank_account_base_request import BankAccountBaseRequest
+from .bank_account_base_response import BankAccountBaseResponse
 from .bank_account_request import BankAccountRequest
 from .bank_account_response import BankAccountResponse
 from .bank_status import BankStatus
 from .bank_type import BankType
+from .card_base_request import CardBaseRequest
+from .card_base_response import CardBaseResponse
 from .card_brand import CardBrand
 from .card_request import CardRequest
 from .card_response import CardResponse
 from .card_type import CardType
+from .check_base_request import CheckBaseRequest
+from .check_base_response import CheckBaseResponse
 from .check_request import CheckRequest
 from .check_response import CheckResponse
 from .currency_code import CurrencyCode
+from .custom_payment_method_base_request import CustomPaymentMethodBaseRequest
+from .custom_payment_method_base_response import CustomPaymentMethodBaseResponse
 from .custom_payment_method_request import CustomPaymentMethodRequest
 from .custom_payment_method_response import CustomPaymentMethodResponse
+from .custom_payment_method_update_base_request import CustomPaymentMethodUpdateBaseRequest
 from .custom_payment_method_update_request import CustomPaymentMethodUpdateRequest
+from .payment_method_id import PaymentMethodId
 from .payment_method_request import (
     PaymentMethodRequest,
     PaymentMethodRequest_BankAccount,
     PaymentMethodRequest_Card,
     PaymentMethodRequest_Check,
     PaymentMethodRequest_Custom,
 )
 from .payment_method_response import (
     PaymentMethodResponse,
     PaymentMethodResponse_BankAccount,
     PaymentMethodResponse_Card,
     PaymentMethodResponse_Check,
     PaymentMethodResponse_Custom,
 )
+from .payment_method_schema_field import PaymentMethodSchemaField
+from .payment_method_schema_field_type import PaymentMethodSchemaFieldType
+from .payment_method_schema_id import PaymentMethodSchemaId
+from .payment_method_schema_request import PaymentMethodSchemaRequest
+from .payment_method_schema_response import PaymentMethodSchemaResponse
 from .payment_method_type import PaymentMethodType
 from .payment_method_update_request import PaymentMethodUpdateRequest, PaymentMethodUpdateRequest_Custom
 
 __all__ = [
+    "BankAccountBaseRequest",
+    "BankAccountBaseResponse",
     "BankAccountRequest",
     "BankAccountResponse",
     "BankStatus",
     "BankType",
+    "CardBaseRequest",
+    "CardBaseResponse",
     "CardBrand",
     "CardRequest",
     "CardResponse",
     "CardType",
+    "CheckBaseRequest",
+    "CheckBaseResponse",
     "CheckRequest",
     "CheckResponse",
     "CurrencyCode",
+    "CustomPaymentMethodBaseRequest",
+    "CustomPaymentMethodBaseResponse",
     "CustomPaymentMethodRequest",
     "CustomPaymentMethodResponse",
+    "CustomPaymentMethodUpdateBaseRequest",
     "CustomPaymentMethodUpdateRequest",
+    "PaymentMethodId",
     "PaymentMethodRequest",
     "PaymentMethodRequest_BankAccount",
     "PaymentMethodRequest_Card",
     "PaymentMethodRequest_Check",
     "PaymentMethodRequest_Custom",
     "PaymentMethodResponse",
     "PaymentMethodResponse_BankAccount",
     "PaymentMethodResponse_Card",
     "PaymentMethodResponse_Check",
     "PaymentMethodResponse_Custom",
+    "PaymentMethodSchemaField",
+    "PaymentMethodSchemaFieldType",
+    "PaymentMethodSchemaId",
+    "PaymentMethodSchemaRequest",
+    "PaymentMethodSchemaResponse",
     "PaymentMethodType",
     "PaymentMethodUpdateRequest",
     "PaymentMethodUpdateRequest_Custom",
 ]
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/bank_account_request.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_account_base_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from .bank_type import BankType
 
 
-class BankAccountRequest(pydantic.BaseModel):
-    bank_name: str = pydantic.Field(alias="bankName")
-    routing_number: str = pydantic.Field(alias="routingNumber")
-    account_number: str = pydantic.Field(alias="accountNumber")
+class BankAccountBaseRequest(pydantic.BaseModel):
+    bank_name: typing.Optional[str] = pydantic.Field(alias="bankName")
+    routing_number: typing.Optional[str] = pydantic.Field(alias="routingNumber")
+    account_number: typing.Optional[str] = pydantic.Field(alias="accountNumber")
     plaid_public_token: typing.Optional[str] = pydantic.Field(
         alias="plaidPublicToken", description=("Public token from Plaid Link\n")
     )
-    account_type: BankType = pydantic.Field(alias="accountType")
+    account_type: typing.Optional[BankType] = pydantic.Field(alias="accountType")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/bank_account_response.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_account_base_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.payment_method_id import PaymentMethodId
 from .bank_status import BankStatus
 from .bank_type import BankType
 from .currency_code import CurrencyCode
+from .payment_method_id import PaymentMethodId
 
 
-class BankAccountResponse(pydantic.BaseModel):
+class BankAccountBaseResponse(pydantic.BaseModel):
     id: PaymentMethodId
     bank_name: str = pydantic.Field(alias="bankName")
     routing_number: str = pydantic.Field(alias="routingNumber")
     account_number: str = pydantic.Field(alias="accountNumber")
     account_type: BankType = pydantic.Field(alias="accountType")
     status: BankStatus
     supported_currencies: typing.List[CurrencyCode] = pydantic.Field(alias="supportedCurrencies")
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/bank_status.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/bank_type.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/bank_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/card_brand.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_brand.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/card_request.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_base_request.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
 from .card_brand import CardBrand
 from .card_type import CardType
 
 
-class CardRequest(pydantic.BaseModel):
-    card_type: CardType = pydantic.Field(alias="cardType")
-    card_brand: CardBrand = pydantic.Field(alias="cardBrand")
-    last_four: str = pydantic.Field(alias="lastFour")
-    exp_month: str = pydantic.Field(alias="expMonth")
-    exp_year: str = pydantic.Field(alias="expYear")
-    token: str
+class CardBaseRequest(pydantic.BaseModel):
+    card_type: typing.Optional[CardType] = pydantic.Field(alias="cardType")
+    card_brand: typing.Optional[CardBrand] = pydantic.Field(alias="cardBrand")
+    last_four: typing.Optional[str] = pydantic.Field(alias="lastFour")
+    exp_month: typing.Optional[str] = pydantic.Field(alias="expMonth")
+    exp_year: typing.Optional[str] = pydantic.Field(alias="expYear")
+    token: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/card_response.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_base_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.payment_method_id import PaymentMethodId
 from .card_brand import CardBrand
 from .card_type import CardType
 from .currency_code import CurrencyCode
+from .payment_method_id import PaymentMethodId
 
 
-class CardResponse(pydantic.BaseModel):
+class CardBaseResponse(pydantic.BaseModel):
     id: PaymentMethodId
     card_type: CardType = pydantic.Field(alias="cardType")
     card_brand: CardBrand = pydantic.Field(alias="cardBrand")
     last_four: str = pydantic.Field(alias="lastFour")
     exp_month: str = pydantic.Field(alias="expMonth")
     exp_year: str = pydantic.Field(alias="expYear")
     supported_currencies: typing.List[CurrencyCode] = pydantic.Field(alias="supportedCurrencies")
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/card_type.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/check_request.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/check_base_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,24 +2,30 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
+from .currency_code import CurrencyCode
+from .payment_method_id import PaymentMethodId
 
 
-class CheckRequest(pydantic.BaseModel):
+class CheckBaseResponse(pydantic.BaseModel):
+    id: PaymentMethodId
     pay_to_the_order_of: str = pydantic.Field(alias="payToTheOrderOf")
     address_line_1: str = pydantic.Field(alias="addressLine1")
     address_line_2: typing.Optional[str] = pydantic.Field(alias="addressLine2")
     city: str
     state_or_province: str = pydantic.Field(alias="stateOrProvince")
     postal_code: str = pydantic.Field(alias="postalCode")
     country: str
+    supported_currencies: typing.List[CurrencyCode] = pydantic.Field(alias="supportedCurrencies")
+    created_at: dt.datetime = pydantic.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/check_response.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/check_base_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,30 +2,24 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.payment_method_id import PaymentMethodId
-from .currency_code import CurrencyCode
 
 
-class CheckResponse(pydantic.BaseModel):
-    id: PaymentMethodId
-    pay_to_the_order_of: str = pydantic.Field(alias="payToTheOrderOf")
-    address_line_1: str = pydantic.Field(alias="addressLine1")
+class CheckBaseRequest(pydantic.BaseModel):
+    pay_to_the_order_of: typing.Optional[str] = pydantic.Field(alias="payToTheOrderOf")
+    address_line_1: typing.Optional[str] = pydantic.Field(alias="addressLine1")
     address_line_2: typing.Optional[str] = pydantic.Field(alias="addressLine2")
-    city: str
-    state_or_province: str = pydantic.Field(alias="stateOrProvince")
-    postal_code: str = pydantic.Field(alias="postalCode")
-    country: str
-    supported_currencies: typing.List[CurrencyCode] = pydantic.Field(alias="supportedCurrencies")
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
+    city: typing.Optional[str]
+    state_or_province: typing.Optional[str] = pydantic.Field(alias="stateOrProvince")
+    postal_code: typing.Optional[str] = pydantic.Field(alias="postalCode")
+    country: typing.Optional[str]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/currency_code.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/currency_code.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/custom_payment_method_request.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,30 +2,38 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.payment_method_schema_id import PaymentMethodSchemaId
+from .currency_code import CurrencyCode
+from .payment_method_id import PaymentMethodId
+from .payment_method_schema_id import PaymentMethodSchemaId
+from .payment_method_schema_response import PaymentMethodSchemaResponse
 
 
-class CustomPaymentMethodRequest(pydantic.BaseModel):
+class CustomPaymentMethodBaseResponse(pydantic.BaseModel):
+    id: PaymentMethodId
     foreign_id: str = pydantic.Field(alias="foreignId", description=("ID for this payment method in your system\n"))
     account_name: typing.Optional[str] = pydantic.Field(alias="accountName")
     account_number: typing.Optional[str] = pydantic.Field(alias="accountNumber")
     schema_id: PaymentMethodSchemaId = pydantic.Field(
         alias="schemaId",
         description=(
             "Payment method schema used for this payment method. Defines the fields that this payment method contains.\n"
         ),
     )
+    schema_: PaymentMethodSchemaResponse = pydantic.Field(alias="schema")
     data: typing.Dict[str, str] = pydantic.Field(
         description=("Object of key/value pairs that matches the keys in the linked payment method schema.\n")
     )
+    supported_currencies: typing.List[CurrencyCode] = pydantic.Field(alias="supportedCurrencies")
+    created_at: dt.datetime = pydantic.Field(alias="createdAt")
+    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/custom_payment_method_response.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_update_base_request.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,38 +2,32 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.payment_method_id import PaymentMethodId
-from ...commons.types.payment_method_schema_id import PaymentMethodSchemaId
-from ...payment_method_schema.types.payment_method_schema_response import PaymentMethodSchemaResponse
-from .currency_code import CurrencyCode
+from .payment_method_schema_id import PaymentMethodSchemaId
 
 
-class CustomPaymentMethodResponse(pydantic.BaseModel):
-    id: PaymentMethodId
-    foreign_id: str = pydantic.Field(alias="foreignId", description=("ID for this payment method in your system\n"))
+class CustomPaymentMethodUpdateBaseRequest(pydantic.BaseModel):
+    foreign_id: typing.Optional[str] = pydantic.Field(
+        alias="foreignId", description=("ID for this payment method in your system\n")
+    )
     account_name: typing.Optional[str] = pydantic.Field(alias="accountName")
     account_number: typing.Optional[str] = pydantic.Field(alias="accountNumber")
-    schema_id: PaymentMethodSchemaId = pydantic.Field(
+    schema_id: typing.Optional[PaymentMethodSchemaId] = pydantic.Field(
         alias="schemaId",
         description=(
             "Payment method schema used for this payment method. Defines the fields that this payment method contains.\n"
         ),
     )
-    schema_: PaymentMethodSchemaResponse = pydantic.Field(alias="schema")
-    data: typing.Dict[str, str] = pydantic.Field(
+    data: typing.Optional[typing.Dict[str, str]] = pydantic.Field(
         description=("Object of key/value pairs that matches the keys in the linked payment method schema.\n")
     )
-    supported_currencies: typing.List[CurrencyCode] = pydantic.Field(alias="supportedCurrencies")
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/custom_payment_method_update_request.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/custom_payment_method_base_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,18 +2,18 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.payment_method_schema_id import PaymentMethodSchemaId
+from .payment_method_schema_id import PaymentMethodSchemaId
 
 
-class CustomPaymentMethodUpdateRequest(pydantic.BaseModel):
+class CustomPaymentMethodBaseRequest(pydantic.BaseModel):
     foreign_id: typing.Optional[str] = pydantic.Field(
         alias="foreignId", description=("ID for this payment method in your system\n")
     )
     account_name: typing.Optional[str] = pydantic.Field(alias="accountName")
     account_number: typing.Optional[str] = pydantic.Field(alias="accountNumber")
     schema_id: typing.Optional[PaymentMethodSchemaId] = pydantic.Field(
         alias="schemaId",
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/payment_method_request.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/payment_method_response.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_response.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/payment_method_type.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method/types/payment_method_update_request.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_update_request.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method_schema/client.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_schema/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 from ...core.api_error import ApiError
 from ...core.jsonable_encoder import jsonable_encoder
 from ...core.remove_none_from_headers import remove_none_from_headers
 from ...environment import MercoaEnvironment
 from ..commons.errors.auth_header_malformed_error import AuthHeaderMalformedError
 from ..commons.errors.auth_header_missing_error import AuthHeaderMissingError
 from ..commons.errors.unauthorized import Unauthorized
-from ..commons.types.payment_method_schema_id import PaymentMethodSchemaId
-from .types.payment_method_schema_request import PaymentMethodSchemaRequest
-from .types.payment_method_schema_response import PaymentMethodSchemaResponse
+from ..payment_method_types.types.payment_method_schema_id import PaymentMethodSchemaId
+from ..payment_method_types.types.payment_method_schema_request import PaymentMethodSchemaRequest
+from ..payment_method_types.types.payment_method_schema_response import PaymentMethodSchemaResponse
 
 
 class PaymentMethodSchemaClient:
     def __init__(self, *, environment: MercoaEnvironment = MercoaEnvironment.PRODUCTION, token: str):
         self._environment = environment
         self._token = token
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_field.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_field_type.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_field_type.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_request.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/payment_method_schema_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...payment_method.types.currency_code import CurrencyCode
+from .currency_code import CurrencyCode
 from .payment_method_schema_field import PaymentMethodSchemaField
 
 
 class PaymentMethodSchemaRequest(pydantic.BaseModel):
     name: str
     is_source: bool = pydantic.Field(
         alias="isSource", description=("This payment method can be used as a payment source for an invoice\n")
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/payment_method_schema/types/payment_method_schema_response.py` & `mercoa-0.2.1/src/mercoa/resources/transaction/types/transaction_response_expanded.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,34 +2,28 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.payment_method_schema_id import PaymentMethodSchemaId
-from ...payment_method.types.currency_code import CurrencyCode
-from .payment_method_schema_field import PaymentMethodSchemaField
-
-
-class PaymentMethodSchemaResponse(pydantic.BaseModel):
-    id: PaymentMethodSchemaId
-    name: str
-    is_source: bool = pydantic.Field(
-        alias="isSource", description=("This payment method can be used as a payment source for an invoice\n")
-    )
-    is_destination: bool = pydantic.Field(
-        alias="isDestination", description=("This payment method can be used as a payment destination for an invoice\n")
-    )
-    supported_currencies: typing.List[CurrencyCode] = pydantic.Field(
-        alias="supportedCurrencies", description=("List of currencies that this payment method supports.\n")
-    )
-    fields: typing.List[PaymentMethodSchemaField]
-    created_at: dt.datetime = pydantic.Field(alias="createdAt")
-    updated_at: dt.datetime = pydantic.Field(alias="updatedAt")
+from ...entity_types.types.entity_response import EntityResponse
+from ...invoice_types.types.invoice_id import InvoiceId
+from ...payment_method_types.types.payment_method_response import PaymentMethodResponse
+from .transaction_response import TransactionResponse
+
+
+class TransactionResponseExpanded(TransactionResponse):
+    invoice_id: InvoiceId = pydantic.Field(alias="invoiceId")
+    deduction_date: typing.Optional[dt.datetime] = pydantic.Field(alias="deductionDate")
+    due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate")
+    payer: typing.Optional[EntityResponse]
+    vendor: typing.Optional[EntityResponse]
+    payment_source: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentSource")
+    payment_destination: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentDestination")
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/transaction/client.py` & `mercoa-0.2.1/src/mercoa/resources/transaction/client.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/src/mercoa/resources/transaction/types/transaction_response.py` & `mercoa-0.2.1/src/mercoa/resources/transaction/types/transaction_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...payment_method.types.currency_code import CurrencyCode
+from ...payment_method_types.types.currency_code import CurrencyCode
 from .transaction_status import TransactionStatus
 
 
 class TransactionResponse(pydantic.BaseModel):
     id: str
     status: TransactionStatus
     amount: float
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/transaction/types/transaction_response_expanded.py` & `mercoa-0.2.1/src/mercoa/resources/payment_method_types/types/card_request.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,28 +2,21 @@
 
 import datetime as dt
 import typing
 
 import pydantic
 
 from ....core.datetime_utils import serialize_datetime
-from ...commons.types.invoice_id import InvoiceId
-from ...entity.types.entity_response import EntityResponse
-from ...payment_method.types.payment_method_response import PaymentMethodResponse
-from .transaction_response import TransactionResponse
+from .card_base_request import CardBaseRequest
 
 
-class TransactionResponseExpanded(TransactionResponse):
-    invoice_id: InvoiceId = pydantic.Field(alias="invoiceId")
-    deduction_date: typing.Optional[dt.datetime] = pydantic.Field(alias="deductionDate")
-    due_date: typing.Optional[dt.datetime] = pydantic.Field(alias="dueDate")
-    payer: typing.Optional[EntityResponse]
-    vendor: typing.Optional[EntityResponse]
-    payment_source: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentSource")
-    payment_destination: typing.Optional[PaymentMethodResponse] = pydantic.Field(alias="paymentDestination")
+class CardRequest(CardBaseRequest):
+    card: typing.Optional[CardBaseRequest] = pydantic.Field(
+        description=("DEPRECATED DO NOT USE. WILL BE REMOVED SOON.\n")
+    )
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
```

### Comparing `mercoa-0.2.0/src/mercoa/resources/transaction/types/transaction_status.py` & `mercoa-0.2.1/src/mercoa/resources/transaction/types/transaction_status.py`

 * *Files identical despite different names*

### Comparing `mercoa-0.2.0/PKG-INFO` & `mercoa-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercoa
-Version: 0.2.0
+Version: 0.2.1
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

