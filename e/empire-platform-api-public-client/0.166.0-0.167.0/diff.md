# Comparing `tmp/empire-platform-api-public-client-0.166.0.tar.gz` & `tmp/empire-platform-api-public-client-0.167.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empire-platform-api-public-client-0.166.0.tar", last modified: Wed Jul  5 11:59:34 2023, max compression
+gzip compressed data, was "empire-platform-api-public-client-0.167.0.tar", last modified: Tue Jul 11 11:17:52 2023, max compression
```

## Comparing `empire-platform-api-public-client-0.166.0.tar` & `empire-platform-api-public-client-0.167.0.tar`

### file list

```diff
@@ -1,716 +1,716 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 11:59:34.093738 empire-platform-api-public-client-0.166.0/
--rw-r--r--   0 root         (0) root         (0)      612 2023-07-05 11:59:34.093738 empire-platform-api-public-client-0.166.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    50302 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 11:59:34.023738 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/
--rw-r--r--   0 root         (0) root         (0)    41280 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 11:59:34.023738 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/
--rw-r--r--   0 root         (0) root         (0)     2193 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10382 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/attachment_api.py
--rw-r--r--   0 root         (0) root         (0)   116019 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/auction_api.py
--rw-r--r--   0 root         (0) root         (0)    17984 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/audit_log_api.py
--rw-r--r--   0 root         (0) root         (0)    15031 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/bidding_configuration_api.py
--rw-r--r--   0 root         (0) root         (0)    16899 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/buy_now_offers_api.py
--rw-r--r--   0 root         (0) root         (0)    71676 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/default_bid_api.py
--rw-r--r--   0 root         (0) root         (0)    46916 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/default_nomination_api.py
--rw-r--r--   0 root         (0) root         (0)    44696 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/finance_api.py
--rw-r--r--   0 root         (0) root         (0)     7766 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/finance_information_api.py
--rw-r--r--   0 root         (0) root         (0)    24412 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/manual_file_upload_api.py
--rw-r--r--   0 root         (0) root         (0)    31027 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/messages_api.py
--rw-r--r--   0 root         (0) root         (0)     6828 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/metadata_api.py
--rw-r--r--   0 root         (0) root         (0)    35670 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/nomination_api.py
--rw-r--r--   0 root         (0) root         (0)    19781 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/organisation_api.py
--rw-r--r--   0 root         (0) root         (0)    35124 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/organisation_document_api.py
--rw-r--r--   0 root         (0) root         (0)    72445 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/participant_dashboard_api.py
--rw-r--r--   0 root         (0) root         (0)     7810 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/participant_overview_api.py
--rw-r--r--   0 root         (0) root         (0)    55831 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/profile_api.py
--rw-r--r--   0 root         (0) root         (0)    21816 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/public_allocated_auction_api.py
--rw-r--r--   0 root         (0) root         (0)    67522 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/public_auction_api.py
--rw-r--r--   0 root         (0) root         (0)     8660 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/public_nominations_api.py
--rw-r--r--   0 root         (0) root         (0)    65136 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/reporting_api.py
--rw-r--r--   0 root         (0) root         (0)   212050 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/secondary_market_api.py
--rw-r--r--   0 root         (0) root         (0)    10353 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/transmission_right_api.py
--rw-r--r--   0 root         (0) root         (0)    36183 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/user_api.py
--rw-r--r--   0 root         (0) root         (0)    30336 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api_client.py
--rw-r--r--   0 root         (0) root         (0)      844 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api_response.py
--rw-r--r--   0 root         (0) root         (0)    16914 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/configuration.py
--rw-r--r--   0 root         (0) root         (0)     5334 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 11:59:34.053738 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/
--rw-r--r--   0 root         (0) root         (0)    38418 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2518 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/address.py
--rw-r--r--   0 root         (0) root         (0)     5328 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_allocated_auction.py
--rw-r--r--   0 root         (0) root         (0)     1084 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nomination_type.py
--rw-r--r--   0 root         (0) root         (0)     3172 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nominations.py
--rw-r--r--   0 root         (0) root         (0)     2935 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nominations_mns_or_gb.py
--rw-r--r--   0 root         (0) root         (0)     4362 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nominations_mns_or_gb_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     2690 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nominations_mtu_netted_nominations.py
--rw-r--r--   0 root         (0) root         (0)     2491 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nominations_mtu_value.py
--rw-r--r--   0 root         (0) root         (0)     2873 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nominations_nl.py
--rw-r--r--   0 root         (0) root         (0)     4961 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nominations_nl_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     2675 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nominations_nl_mtus_inner_eprogram_values.py
--rw-r--r--   0 root         (0) root         (0)     5292 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/allocated_auction.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/allocated_auction_batch.py
--rw-r--r--   0 root         (0) root         (0)     1480 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/allocated_auction_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     2645 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/api_key.py
--rw-r--r--   0 root         (0) root         (0)     2971 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/attachment.py
--rw-r--r--   0 root         (0) root         (0)     5818 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction.py
--rw-r--r--   0 root         (0) root         (0)     1063 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_allocation_resolution.py
--rw-r--r--   0 root         (0) root         (0)     2804 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_batch.py
--rw-r--r--   0 root         (0) root         (0)     2239 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_bid_participant.py
--rw-r--r--   0 root         (0) root         (0)     1050 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_bid_status.py
--rw-r--r--   0 root         (0) root         (0)     3086 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_bidding_configuration.py
--rw-r--r--   0 root         (0) root         (0)      944 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_bidding_mode.py
--rw-r--r--   0 root         (0) root         (0)     1114 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_intra_day_product_type.py
--rw-r--r--   0 root         (0) root         (0)     6510 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_process_steps_absolute.py
--rw-r--r--   0 root         (0) root         (0)     1715 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_product_type.py
--rw-r--r--   0 root         (0) root         (0)     2965 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_reduction_period.py
--rw-r--r--   0 root         (0) root         (0)     3122 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_result_congestion_rent.py
--rw-r--r--   0 root         (0) root         (0)     2707 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_result_participant.py
--rw-r--r--   0 root         (0) root         (0)     1533 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1318 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_status.py
--rw-r--r--   0 root         (0) root         (0)     1355 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_timescale.py
--rw-r--r--   0 root         (0) root         (0)     4663 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log.py
--rw-r--r--   0 root         (0) root         (0)     2709 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_api_key.py
--rw-r--r--   0 root         (0) root         (0)     2768 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_batch.py
--rw-r--r--   0 root         (0) root         (0)     1946 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_domain.py
--rw-r--r--   0 root         (0) root         (0)     2377 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_payload.py
--rw-r--r--   0 root         (0) root         (0)      964 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      934 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_status.py
--rw-r--r--   0 root         (0) root         (0)     8092 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_type.py
--rw-r--r--   0 root         (0) root         (0)     2817 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_user.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_user_organisation.py
--rw-r--r--   0 root         (0) root         (0)     2427 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/bid_value.py
--rw-r--r--   0 root         (0) root         (0)     3391 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/bidding_configuration.py
--rw-r--r--   0 root         (0) root         (0)     3112 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/bidding_configuration_per_direction.py
--rw-r--r--   0 root         (0) root         (0)     2541 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/bidding_configuration_secondary_market_notices.py
--rw-r--r--   0 root         (0) root         (0)     2828 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/bidding_configuration_values_inner.py
--rw-r--r--   0 root         (0) root         (0)      992 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/border_direction.py
--rw-r--r--   0 root         (0) root         (0)     1017 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/border_direction_with_both.py
--rw-r--r--   0 root         (0) root         (0)     1072 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/border_direction_with_both_and_none.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/buy_now_day_ahead_offer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     5708 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/buy_now_offer.py
--rw-r--r--   0 root         (0) root         (0)     3119 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/buy_now_offer_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)      999 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/buy_now_offer_status.py
--rw-r--r--   0 root         (0) root         (0)     2089 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_api_key_request.py
--rw-r--r--   0 root         (0) root         (0)     6802 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request.py
--rw-r--r--   0 root         (0) root         (0)     3028 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request_bids_inner.py
--rw-r--r--   0 root         (0) root         (0)     3410 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request_bids_inner_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     3752 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_default_nomination_request.py
--rw-r--r--   0 root         (0) root         (0)     6545 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_long_term_default_bid_request.py
--rw-r--r--   0 root         (0) root         (0)     2427 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_organisation_document_request.py
--rw-r--r--   0 root         (0) root         (0)     3790 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     4220 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_noticeboard_response.py
--rw-r--r--   0 root         (0) root         (0)     3945 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     3585 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_transfer_request_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     4215 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_secondary_market_long_term_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     4112 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_secondary_market_long_term_noticeboard_response.py
--rw-r--r--   0 root         (0) root         (0)     3383 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_secondary_market_long_term_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2844 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_secondary_market_return_request.py
--rw-r--r--   0 root         (0) root         (0)     2257 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_api_key.py
--rw-r--r--   0 root         (0) root         (0)     2129 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_default_bid.py
--rw-r--r--   0 root         (0) root         (0)     2185 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_default_nomination.py
--rw-r--r--   0 root         (0) root         (0)     2209 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_organisation_document.py
--rw-r--r--   0 root         (0) root         (0)     2441 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     2465 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_noticeboard_response.py
--rw-r--r--   0 root         (0) root         (0)     2433 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2361 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_secondary_market_long_term_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     2385 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_secondary_market_long_term_noticeboard_response.py
--rw-r--r--   0 root         (0) root         (0)     2353 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_secondary_market_long_term_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2353 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_secondary_market_return_request_identifier.py
--rw-r--r--   0 root         (0) root         (0)     4011 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/dashboard_next_nomination_gate.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/dashboard_next_nomination_gate_window.py
--rw-r--r--   0 root         (0) root         (0)     1043 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/dashboard_next_nomination_window_status.py
--rw-r--r--   0 root         (0) root         (0)     2524 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/date_period.py
--rw-r--r--   0 root         (0) root         (0)     3071 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/date_time_period.py
--rw-r--r--   0 root         (0) root         (0)     6273 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_auction.py
--rw-r--r--   0 root         (0) root         (0)     3470 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group.py
--rw-r--r--   0 root         (0) root         (0)     3074 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_batch.py
--rw-r--r--   0 root         (0) root         (0)     3654 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids_inner.py
--rw-r--r--   0 root         (0) root         (0)     3342 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids_inner_value.py
--rw-r--r--   0 root         (0) root         (0)     4615 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu.py
--rw-r--r--   0 root         (0) root         (0)     2845 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu_results.py
--rw-r--r--   0 root         (0) root         (0)     3090 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu_results_bids_inner.py
--rw-r--r--   0 root         (0) root         (0)     2941 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results.py
--rw-r--r--   0 root         (0) root         (0)     3774 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     3025 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results_mtus_inner_value.py
--rw-r--r--   0 root         (0) root         (0)     4161 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_results.py
--rw-r--r--   0 root         (0) root         (0)     5137 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_results_mtu.py
--rw-r--r--   0 root         (0) root         (0)     6843 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_default_bid.py
--rw-r--r--   0 root         (0) root         (0)     5979 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_bid.py
--rw-r--r--   0 root         (0) root         (0)     2792 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_bid_batch.py
--rw-r--r--   0 root         (0) root         (0)     2692 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_bid_options.py
--rw-r--r--   0 root         (0) root         (0)     1588 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_bid_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      942 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_bid_status.py
--rw-r--r--   0 root         (0) root         (0)     3399 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_nomination.py
--rw-r--r--   0 root         (0) root         (0)     2876 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_nomination_batch.py
--rw-r--r--   0 root         (0) root         (0)     1028 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_nomination_declaration_type.py
--rw-r--r--   0 root         (0) root         (0)     3849 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_nomination_details.py
--rw-r--r--   0 root         (0) root         (0)     3177 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_nomination_mtu.py
--rw-r--r--   0 root         (0) root         (0)     2710 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_nomination_options.py
--rw-r--r--   0 root         (0) root         (0)     1343 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_nomination_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_nomination_status.py
--rw-r--r--   0 root         (0) root         (0)     9333 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/error_code.py
--rw-r--r--   0 root         (0) root         (0)     3278 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/error_response.py
--rw-r--r--   0 root         (0) root         (0)     5902 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/finance_information.py
--rw-r--r--   0 root         (0) root         (0)     2752 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/finance_information_bank_deposits_inner.py
--rw-r--r--   0 root         (0) root         (0)     2895 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/finance_information_letter_of_credits_inner.py
--rw-r--r--   0 root         (0) root         (0)     2489 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/finance_information_lockable_amount.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/finance_information_lockable_date.py
--rw-r--r--   0 root         (0) root         (0)     3549 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/finance_information_lockable_period.py
--rw-r--r--   0 root         (0) root         (0)     2590 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/finance_information_market_vat_details.py
--rw-r--r--   0 root         (0) root         (0)     2344 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/finance_information_sage_settings.py
--rw-r--r--   0 root         (0) root         (0)     6273 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/intra_day_auction.py
--rw-r--r--   0 root         (0) root         (0)     4687 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_action_type.py
--rw-r--r--   0 root         (0) root         (0)     2755 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_batch.py
--rw-r--r--   0 root         (0) root         (0)     8176 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_details.py
--rw-r--r--   0 root         (0) root         (0)     3154 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_history.py
--rw-r--r--   0 root         (0) root         (0)     4434 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_line_item.py
--rw-r--r--   0 root         (0) root         (0)     2275 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_participant_details.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_status.py
--rw-r--r--   0 root         (0) root         (0)     3964 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_summary.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_vat_rate.py
--rw-r--r--   0 root         (0) root         (0)     6980 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_auction.py
--rw-r--r--   0 root         (0) root         (0)     3875 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_auction_bid.py
--rw-r--r--   0 root         (0) root         (0)     2890 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_auction_bid_batch.py
--rw-r--r--   0 root         (0) root         (0)     1080 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_auction_bid_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     4475 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_auction_results.py
--rw-r--r--   0 root         (0) root         (0)     3415 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_auction_results_allocated_capacity_inner.py
--rw-r--r--   0 root         (0) root         (0)     3407 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_bidding_results.py
--rw-r--r--   0 root         (0) root         (0)     6586 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_default_bid.py
--rw-r--r--   0 root         (0) root         (0)     2837 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_offered_capacity.py
--rw-r--r--   0 root         (0) root         (0)     2909 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_reserve_price.py
--rw-r--r--   0 root         (0) root         (0)     3043 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_reserve_price_steps_inner.py
--rw-r--r--   0 root         (0) root         (0)     2241 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/manual_file_upload_request.py
--rw-r--r--   0 root         (0) root         (0)      874 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/market.py
--rw-r--r--   0 root         (0) root         (0)     4125 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/message.py
--rw-r--r--   0 root         (0) root         (0)     2755 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/message_batch.py
--rw-r--r--   0 root         (0) root         (0)      979 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/message_category.py
--rw-r--r--   0 root         (0) root         (0)      919 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/message_sender.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/message_severity.py
--rw-r--r--   0 root         (0) root         (0)     1149 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/message_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1463 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/message_type.py
--rw-r--r--   0 root         (0) root         (0)     4139 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/mtu_period.py
--rw-r--r--   0 root         (0) root         (0)      967 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/mtu_size.py
--rw-r--r--   0 root         (0) root         (0)     2517 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/mtu_size_per_auction_product_type.py
--rw-r--r--   0 root         (0) root         (0)     2370 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/mtu_size_per_timescale.py
--rw-r--r--   0 root         (0) root         (0)     2276 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/nested_error.py
--rw-r--r--   0 root         (0) root         (0)     1015 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/nomination_restriction_type.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/noticeboard_entry_type.py
--rw-r--r--   0 root         (0) root         (0)     1008 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/noticeboard_entry_type_with_both.py
--rw-r--r--   0 root         (0) root         (0)     2119 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/notification_preference.py
--rw-r--r--   0 root         (0) root         (0)     2250 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/notification_preference_with_sms.py
--rw-r--r--   0 root         (0) root         (0)     3484 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/ntc_overview_mtu_data.py
--rw-r--r--   0 root         (0) root         (0)     1032 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/offered_capacity_setup.py
--rw-r--r--   0 root         (0) root         (0)     2969 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation.py
--rw-r--r--   0 root         (0) root         (0)      968 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_auth_method.py
--rw-r--r--   0 root         (0) root         (0)     2898 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_contact.py
--rw-r--r--   0 root         (0) root         (0)     3625 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_contact_information.py
--rw-r--r--   0 root         (0) root         (0)     4298 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document.py
--rw-r--r--   0 root         (0) root         (0)     2912 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_batch.py
--rw-r--r--   0 root         (0) root         (0)     1073 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_file_type.py
--rw-r--r--   0 root         (0) root         (0)     3068 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_options.py
--rw-r--r--   0 root         (0) root         (0)     2966 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_organisation.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_sort_by.py
--rw-r--r--   0 root         (0) root         (0)      996 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_status.py
--rw-r--r--   0 root         (0) root         (0)     2934 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_uploaded_by_user.py
--rw-r--r--   0 root         (0) root         (0)     2439 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_uploaded_by_user_organisation.py
--rw-r--r--   0 root         (0) root         (0)     2263 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_user.py
--rw-r--r--   0 root         (0) root         (0)     2326 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_file_settings.py
--rw-r--r--   0 root         (0) root         (0)     3906 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_market_settings.py
--rw-r--r--   0 root         (0) root         (0)     2995 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_market_settings_gb_nomination_settings.py
--rw-r--r--   0 root         (0) root         (0)     2791 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_market_settings_nl_nomination_settings.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_status.py
--rw-r--r--   0 root         (0) root         (0)      960 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_type.py
--rw-r--r--   0 root         (0) root         (0)     4588 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_user.py
--rw-r--r--   0 root         (0) root         (0)     2864 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_user_batch.py
--rw-r--r--   0 root         (0) root         (0)     1174 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     2170 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/other_party.py
--rw-r--r--   0 root         (0) root         (0)     2159 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant.py
--rw-r--r--   0 root         (0) root         (0)     2601 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_default_bids_and_nominations_data.py
--rw-r--r--   0 root         (0) root         (0)     3816 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_finance_overview_data.py
--rw-r--r--   0 root         (0) root         (0)     3598 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_finance_overview_invoice.py
--rw-r--r--   0 root         (0) root         (0)     3164 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data.py
--rw-r--r--   0 root         (0) root         (0)     4012 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     2971 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data_mtus_inner_values_inner.py
--rw-r--r--   0 root         (0) root         (0)     3035 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data.py
--rw-r--r--   0 root         (0) root         (0)     4869 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     2871 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_inner_netted_nominations.py
--rw-r--r--   0 root         (0) root         (0)     2819 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_inner_values_inner.py
--rw-r--r--   0 root         (0) root         (0)     3207 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_messages.py
--rw-r--r--   0 root         (0) root         (0)     3091 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data.py
--rw-r--r--   0 root         (0) root         (0)     4939 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     2867 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_inner_aggregated_nominations_inner.py
--rw-r--r--   0 root         (0) root         (0)     2791 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_inner_netted_nominations.py
--rw-r--r--   0 root         (0) root         (0)     4889 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_next_auction.py
--rw-r--r--   0 root         (0) root         (0)     4442 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_next_auctions_and_nomination_gates.py
--rw-r--r--   0 root         (0) root         (0)     3273 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data.py
--rw-r--r--   0 root         (0) root         (0)     4134 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     4163 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_inner_values_inner.py
--rw-r--r--   0 root         (0) root         (0)     3046 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_inner_values_inner_nomination_restriction.py
--rw-r--r--   0 root         (0) root         (0)     3157 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data.py
--rw-r--r--   0 root         (0) root         (0)     4195 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_inner_values_inner.py
--rw-r--r--   0 root         (0) root         (0)     4429 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_organisation_details.py
--rw-r--r--   0 root         (0) root         (0)     5035 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_overview_data.py
--rw-r--r--   0 root         (0) root         (0)     3713 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_overview_data_contact_information.py
--rw-r--r--   0 root         (0) root         (0)     3085 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_overview_data_finance_overview.py
--rw-r--r--   0 root         (0) root         (0)     2659 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_overview_data_organisation_members.py
--rw-r--r--   0 root         (0) root         (0)     6742 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/permission.py
--rw-r--r--   0 root         (0) root         (0)     1154 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/platform_appearance.py
--rw-r--r--   0 root         (0) root         (0)     3142 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/profile.py
--rw-r--r--   0 root         (0) root         (0)     3701 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/profile_details.py
--rw-r--r--   0 root         (0) root         (0)     3237 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/profile_user.py
--rw-r--r--   0 root         (0) root         (0)     2493 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/profile_user_organisation.py
--rw-r--r--   0 root         (0) root         (0)     3136 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response.py
--rw-r--r--   0 root         (0) root         (0)     4772 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     3062 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus_inner_values_inner.py
--rw-r--r--   0 root         (0) root         (0)     4460 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_auction.py
--rw-r--r--   0 root         (0) root         (0)     2828 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_auction_batch.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_auction_bid_status.py
--rw-r--r--   0 root         (0) root         (0)     1247 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_auction_status.py
--rw-r--r--   0 root         (0) root         (0)     5423 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_day_ahead_auction.py
--rw-r--r--   0 root         (0) root         (0)     2918 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_mtu_results.py
--rw-r--r--   0 root         (0) root         (0)     3157 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_mtu_results_bids_inner.py
--rw-r--r--   0 root         (0) root         (0)     3628 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_results.py
--rw-r--r--   0 root         (0) root         (0)     5423 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_intra_day_auction.py
--rw-r--r--   0 root         (0) root         (0)     6428 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_long_term_auction.py
--rw-r--r--   0 root         (0) root         (0)     3933 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_long_term_auction_results.py
--rw-r--r--   0 root         (0) root         (0)     2255 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/purchased_by_organisation.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/reserve_price_publish_type.py
--rw-r--r--   0 root         (0) root         (0)     3108 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/return_auction.py
--rw-r--r--   0 root         (0) root         (0)     5216 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/sage_code.py
--rw-r--r--   0 root         (0) root         (0)     3545 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_capacity_price_mtu.py
--rw-r--r--   0 root         (0) root         (0)     4592 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     4594 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_details.py
--rw-r--r--   0 root         (0) root         (0)     4952 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_matching.py
--rw-r--r--   0 root         (0) root         (0)     4761 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_response.py
--rw-r--r--   0 root         (0) root         (0)     3910 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_response_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     3139 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_options.py
--rw-r--r--   0 root         (0) root         (0)     3203 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_response_options.py
--rw-r--r--   0 root         (0) root         (0)     6570 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     3514 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     3257 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_options.py
--rw-r--r--   0 root         (0) root         (0)     3654 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_options_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     3560 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     4309 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry_details.py
--rw-r--r--   0 root         (0) root         (0)     4501 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry_response.py
--rw-r--r--   0 root         (0) root         (0)     2526 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_options.py
--rw-r--r--   0 root         (0) root         (0)     2590 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_response_options.py
--rw-r--r--   0 root         (0) root         (0)     2506 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_long_term_transfer_request_options.py
--rw-r--r--   0 root         (0) root         (0)     5332 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     3046 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_noticeboard_entry_batch.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_noticeboard_entry_status.py
--rw-r--r--   0 root         (0) root         (0)     4441 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_return_request.py
--rw-r--r--   0 root         (0) root         (0)     3010 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_return_request_batch.py
--rw-r--r--   0 root         (0) root         (0)     1114 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_return_request_status.py
--rw-r--r--   0 root         (0) root         (0)     6453 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     3034 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_transfer_request_batch.py
--rw-r--r--   0 root         (0) root         (0)     1122 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_transfer_request_status.py
--rw-r--r--   0 root         (0) root         (0)     1030 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_transfer_request_type.py
--rw-r--r--   0 root         (0) root         (0)     3546 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_transfer_transmission_rights_mtu.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/settlement.py
--rw-r--r--   0 root         (0) root         (0)     2739 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/settlement_item.py
--rw-r--r--   0 root         (0) root         (0)     3350 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/settlement_per_source.py
--rw-r--r--   0 root         (0) root         (0)     1038 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/settlement_source_type.py
--rw-r--r--   0 root         (0) root         (0)     2223 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/settlement_sub_source_type.py
--rw-r--r--   0 root         (0) root         (0)     3715 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/source_auction.py
--rw-r--r--   0 root         (0) root         (0)     2348 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/source_auction_display_data.py
--rw-r--r--   0 root         (0) root         (0)     2684 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/source_auction_result.py
--rw-r--r--   0 root         (0) root         (0)     3149 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request.py
--rw-r--r--   0 root         (0) root         (0)     3594 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request_bid_groups_inner.py
--rw-r--r--   0 root         (0) root         (0)     3617 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request_bid_groups_inner_bids_inner.py
--rw-r--r--   0 root         (0) root         (0)     2936 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/submit_long_term_bids_request.py
--rw-r--r--   0 root         (0) root         (0)     3087 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/submit_long_term_bids_request_bids_inner.py
--rw-r--r--   0 root         (0) root         (0)     3169 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/submit_nominations_mtu.py
--rw-r--r--   0 root         (0) root         (0)     2726 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/submit_timescale_nominations_request.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/system_message_category.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nomination_mtu_status.py
--rw-r--r--   0 root         (0) root         (0)     3262 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nomination_options.py
--rw-r--r--   0 root         (0) root         (0)     3150 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nomination_options_window_timing.py
--rw-r--r--   0 root         (0) root         (0)     1069 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nomination_status.py
--rw-r--r--   0 root         (0) root         (0)     1081 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nomination_type.py
--rw-r--r--   0 root         (0) root         (0)     1045 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nomination_window_status.py
--rw-r--r--   0 root         (0) root         (0)     2836 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nominations.py
--rw-r--r--   0 root         (0) root         (0)     4657 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nominations_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     3219 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nominations_mtus_inner_current_nomination.py
--rw-r--r--   0 root         (0) root         (0)     2732 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/transmission_rights_overview.py
--rw-r--r--   0 root         (0) root         (0)     3770 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/transmission_rights_overview_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     3960 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/transmission_rights_overview_mtus_inner_values_inner.py
--rw-r--r--   0 root         (0) root         (0)     2788 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/transmission_rights_overview_mtus_inner_values_inner_timescales_inner.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/uiosi_not_resold.py
--rw-r--r--   0 root         (0) root         (0)     2740 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/uiosi_overview.py
--rw-r--r--   0 root         (0) root         (0)     4347 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/uiosi_overview_per_mtu.py
--rw-r--r--   0 root         (0) root         (0)     2841 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/uiosi_resold.py
--rw-r--r--   0 root         (0) root         (0)     2206 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/unread_messages_response.py
--rw-r--r--   0 root         (0) root         (0)     6116 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/update_day_ahead_or_intra_day_default_bid_request.py
--rw-r--r--   0 root         (0) root         (0)     3318 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/update_default_nomination_request.py
--rw-r--r--   0 root         (0) root         (0)     5859 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/update_long_term_default_bid_request.py
--rw-r--r--   0 root         (0) root         (0)     2761 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/update_profile_details_request.py
--rw-r--r--   0 root         (0) root         (0)     2830 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/update_user_request.py
--rw-r--r--   0 root         (0) root         (0)     3904 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/user.py
--rw-r--r--   0 root         (0) root         (0)     2199 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/user_organisation.py
--rw-r--r--   0 root         (0) root         (0)     3545 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/user_preferences.py
--rw-r--r--   0 root         (0) root         (0)     3806 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/user_preferences_general_notifications.py
--rw-r--r--   0 root         (0) root         (0)     3409 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/user_preferences_subscription_notifications.py
--rw-r--r--   0 root         (0) root         (0)     1510 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/user_role.py
--rw-r--r--   0 root         (0) root         (0)      940 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/user_status.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/vat_rate_type.py
--rw-r--r--   0 root         (0) root         (0)     2005 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/version.py
--rw-r--r--   0 root         (0) root         (0)     2133 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/zendesk_chat_token_response.py
--rw-r--r--   0 root         (0) root         (0)    12999 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 11:59:34.023738 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)      612 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    43360 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       34 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/empire_platform_api_public_client.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      712 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-05 11:59:34.093738 empire-platform-api-public-client-0.166.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1597 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 11:59:34.093738 empire-platform-api-public-client-0.166.0/test/
--rw-r--r--   0 root         (0) root         (0)     1943 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_address.py
--rw-r--r--   0 root         (0) root         (0)     3195 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_aggregated_allocated_auction.py
--rw-r--r--   0 root         (0) root         (0)     1110 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_aggregated_nomination_type.py
--rw-r--r--   0 root         (0) root         (0)     8585 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_aggregated_nominations.py
--rw-r--r--   0 root         (0) root         (0)     3624 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_aggregated_nominations_mns_or_gb.py
--rw-r--r--   0 root         (0) root         (0)     3113 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_aggregated_nominations_mns_or_gb_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     2194 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_aggregated_nominations_mtu_netted_nominations.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_aggregated_nominations_mtu_value.py
--rw-r--r--   0 root         (0) root         (0)     4094 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_aggregated_nominations_nl.py
--rw-r--r--   0 root         (0) root         (0)     3558 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_aggregated_nominations_nl_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     2256 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_aggregated_nominations_nl_mtus_inner_eprogram_values.py
--rw-r--r--   0 root         (0) root         (0)     3110 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_allocated_auction.py
--rw-r--r--   0 root         (0) root         (0)     3956 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_allocated_auction_batch.py
--rw-r--r--   0 root         (0) root         (0)     1097 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_allocated_auction_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_api_key.py
--rw-r--r--   0 root         (0) root         (0)     2053 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_attachment.py
--rw-r--r--   0 root         (0) root         (0)     1112 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_attachment_api.py
--rw-r--r--   0 root         (0) root         (0)     3417 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_auction.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_auction_allocation_resolution.py
--rw-r--r--   0 root         (0) root         (0)     3000 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_auction_api.py
--rw-r--r--   0 root         (0) root         (0)     4242 2023-07-05 11:59:29.000000 empire-platform-api-public-client-0.166.0/test/test_auction_batch.py
--rw-r--r--   0 root         (0) root         (0)     1998 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_auction_bid_participant.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_auction_bid_status.py
--rw-r--r--   0 root         (0) root         (0)     2218 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_auction_bidding_configuration.py
--rw-r--r--   0 root         (0) root         (0)     1068 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_auction_bidding_mode.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_auction_intra_day_product_type.py
--rw-r--r--   0 root         (0) root         (0)     2738 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_auction_process_steps_absolute.py
--rw-r--r--   0 root         (0) root         (0)     1068 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_auction_product_type.py
--rw-r--r--   0 root         (0) root         (0)     2377 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_auction_reduction_period.py
--rw-r--r--   0 root         (0) root         (0)     2129 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_auction_result_congestion_rent.py
--rw-r--r--   0 root         (0) root         (0)     2129 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_auction_result_participant.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_auction_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1032 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_auction_status.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_auction_timescale.py
--rw-r--r--   0 root         (0) root         (0)     3927 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_audit_log.py
--rw-r--r--   0 root         (0) root         (0)     1212 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_audit_log_api.py
--rw-r--r--   0 root         (0) root         (0)     2017 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_audit_log_api_key.py
--rw-r--r--   0 root         (0) root         (0)     5328 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_audit_log_batch.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_audit_log_domain.py
--rw-r--r--   0 root         (0) root         (0)     1970 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_audit_log_payload.py
--rw-r--r--   0 root         (0) root         (0)     1041 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_audit_log_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1040 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_audit_log_status.py
--rw-r--r--   0 root         (0) root         (0)     1026 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_audit_log_type.py
--rw-r--r--   0 root         (0) root         (0)     2424 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_audit_log_user.py
--rw-r--r--   0 root         (0) root         (0)     2036 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_audit_log_user_organisation.py
--rw-r--r--   0 root         (0) root         (0)     1788 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_bid_value.py
--rw-r--r--   0 root         (0) root         (0)     3498 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_bidding_configuration.py
--rw-r--r--   0 root         (0) root         (0)     1320 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_bidding_configuration_api.py
--rw-r--r--   0 root         (0) root         (0)     2086 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_bidding_configuration_per_direction.py
--rw-r--r--   0 root         (0) root         (0)     2283 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_bidding_configuration_secondary_market_notices.py
--rw-r--r--   0 root         (0) root         (0)     2596 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_bidding_configuration_values_inner.py
--rw-r--r--   0 root         (0) root         (0)     1046 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_border_direction.py
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_border_direction_with_both.py
--rw-r--r--   0 root         (0) root         (0)     1155 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_border_direction_with_both_and_none.py
--rw-r--r--   0 root         (0) root         (0)     1121 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_buy_now_day_ahead_offer_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     3524 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_buy_now_offer.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_buy_now_offer_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     1062 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_buy_now_offer_status.py
--rw-r--r--   0 root         (0) root         (0)     1248 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_buy_now_offers_api.py
--rw-r--r--   0 root         (0) root         (0)     1853 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_create_api_key_request.py
--rw-r--r--   0 root         (0) root         (0)     4254 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_create_day_ahead_or_intra_day_default_bid_request.py
--rw-r--r--   0 root         (0) root         (0)     3127 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_create_day_ahead_or_intra_day_default_bid_request_bids_inner.py
--rw-r--r--   0 root         (0) root         (0)     2519 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_create_day_ahead_or_intra_day_default_bid_request_bids_inner_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     2877 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_create_default_nomination_request.py
--rw-r--r--   0 root         (0) root         (0)     3042 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_create_long_term_default_bid_request.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_create_organisation_document_request.py
--rw-r--r--   0 root         (0) root         (0)     3211 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_create_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     7394 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_create_secondary_market_day_ahead_or_intra_day_noticeboard_response.py
--rw-r--r--   0 root         (0) root         (0)     3369 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_create_secondary_market_day_ahead_or_intra_day_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2470 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_create_secondary_market_day_ahead_or_intra_day_transfer_request_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     2698 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_create_secondary_market_long_term_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     6807 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_create_secondary_market_long_term_noticeboard_response.py
--rw-r--r--   0 root         (0) root         (0)     2647 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_create_secondary_market_long_term_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2363 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_create_secondary_market_return_request.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_created_api_key.py
--rw-r--r--   0 root         (0) root         (0)     1895 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_created_default_bid.py
--rw-r--r--   0 root         (0) root         (0)     1979 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_created_default_nomination.py
--rw-r--r--   0 root         (0) root         (0)     2015 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_created_organisation_document.py
--rw-r--r--   0 root         (0) root         (0)     2377 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_created_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     2413 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_created_secondary_market_day_ahead_or_intra_day_noticeboard_response.py
--rw-r--r--   0 root         (0) root         (0)     2365 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_created_secondary_market_day_ahead_or_intra_day_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2251 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_created_secondary_market_long_term_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     2287 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_created_secondary_market_long_term_noticeboard_response.py
--rw-r--r--   0 root         (0) root         (0)     2239 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_created_secondary_market_long_term_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_created_secondary_market_return_request_identifier.py
--rw-r--r--   0 root         (0) root         (0)     3095 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_dashboard_next_nomination_gate.py
--rw-r--r--   0 root         (0) root         (0)     2164 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_dashboard_next_nomination_gate_window.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_dashboard_next_nomination_window_status.py
--rw-r--r--   0 root         (0) root         (0)     1908 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_date_period.py
--rw-r--r--   0 root         (0) root         (0)     1914 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_date_time_period.py
--rw-r--r--   0 root         (0) root         (0)     5555 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_day_ahead_auction.py
--rw-r--r--   0 root         (0) root         (0)     3780 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_bid_group.py
--rw-r--r--   0 root         (0) root         (0)     4794 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_bid_group_batch.py
--rw-r--r--   0 root         (0) root         (0)     2627 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_bid_group_bids_inner.py
--rw-r--r--   0 root         (0) root         (0)     2607 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_bid_group_bids_inner_value.py
--rw-r--r--   0 root         (0) root         (0)     2141 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_mtu.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_mtu_results.py
--rw-r--r--   0 root         (0) root         (0)     2560 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_mtu_results_bids_inner.py
--rw-r--r--   0 root         (0) root         (0)     3273 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_participant_results.py
--rw-r--r--   0 root         (0) root         (0)     2578 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_participant_results_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     2383 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_participant_results_mtus_inner_value.py
--rw-r--r--   0 root         (0) root         (0)     3985 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_results.py
--rw-r--r--   0 root         (0) root         (0)     2565 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_results_mtu.py
--rw-r--r--   0 root         (0) root         (0)     4217 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_default_bid.py
--rw-r--r--   0 root         (0) root         (0)     2470 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_default_bid.py
--rw-r--r--   0 root         (0) root         (0)     2188 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_default_bid_api.py
--rw-r--r--   0 root         (0) root         (0)     3128 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_default_bid_batch.py
--rw-r--r--   0 root         (0) root         (0)     2385 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_default_bid_options.py
--rw-r--r--   0 root         (0) root         (0)     1055 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_default_bid_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1054 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_default_bid_status.py
--rw-r--r--   0 root         (0) root         (0)     2352 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_default_nomination.py
--rw-r--r--   0 root         (0) root         (0)     1792 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_default_nomination_api.py
--rw-r--r--   0 root         (0) root         (0)     2956 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_default_nomination_batch.py
--rw-r--r--   0 root         (0) root         (0)     1167 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_default_nomination_declaration_type.py
--rw-r--r--   0 root         (0) root         (0)     2926 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_default_nomination_details.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_default_nomination_mtu.py
--rw-r--r--   0 root         (0) root         (0)     2377 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_default_nomination_options.py
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_default_nomination_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_default_nomination_status.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_error_code.py
--rw-r--r--   0 root         (0) root         (0)     2282 2023-07-05 11:59:30.000000 empire-platform-api-public-client-0.166.0/test/test_error_response.py
--rw-r--r--   0 root         (0) root         (0)     1612 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_finance_api.py
--rw-r--r--   0 root         (0) root         (0)     9977 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_finance_information.py
--rw-r--r--   0 root         (0) root         (0)     1174 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_finance_information_api.py
--rw-r--r--   0 root         (0) root         (0)     3836 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_finance_information_bank_deposits_inner.py
--rw-r--r--   0 root         (0) root         (0)     3941 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_finance_information_letter_of_credits_inner.py
--rw-r--r--   0 root         (0) root         (0)     2082 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_finance_information_lockable_amount.py
--rw-r--r--   0 root         (0) root         (0)     2112 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_finance_information_lockable_date.py
--rw-r--r--   0 root         (0) root         (0)     3323 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_finance_information_lockable_period.py
--rw-r--r--   0 root         (0) root         (0)     2197 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_finance_information_market_vat_details.py
--rw-r--r--   0 root         (0) root         (0)     2068 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_finance_information_sage_settings.py
--rw-r--r--   0 root         (0) root         (0)     5555 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_intra_day_auction.py
--rw-r--r--   0 root         (0) root         (0)     2990 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_invoice.py
--rw-r--r--   0 root         (0) root         (0)     1061 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_invoice_action_type.py
--rw-r--r--   0 root         (0) root         (0)     4006 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_invoice_batch.py
--rw-r--r--   0 root         (0) root         (0)     7368 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_invoice_details.py
--rw-r--r--   0 root         (0) root         (0)     2134 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_invoice_history.py
--rw-r--r--   0 root         (0) root         (0)     2436 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_invoice_line_item.py
--rw-r--r--   0 root         (0) root         (0)     2046 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_invoice_participant_details.py
--rw-r--r--   0 root         (0) root         (0)     1032 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_invoice_status.py
--rw-r--r--   0 root         (0) root         (0)     2146 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_invoice_summary.py
--rw-r--r--   0 root         (0) root         (0)     1872 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_invoice_vat_rate.py
--rw-r--r--   0 root         (0) root         (0)     6329 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_long_term_auction.py
--rw-r--r--   0 root         (0) root         (0)     2333 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_long_term_auction_bid.py
--rw-r--r--   0 root         (0) root         (0)     3236 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_long_term_auction_bid_batch.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_long_term_auction_bid_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     4438 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_long_term_auction_results.py
--rw-r--r--   0 root         (0) root         (0)     2772 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_long_term_auction_results_allocated_capacity_inner.py
--rw-r--r--   0 root         (0) root         (0)     2036 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_long_term_bidding_results.py
--rw-r--r--   0 root         (0) root         (0)     3005 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_long_term_default_bid.py
--rw-r--r--   0 root         (0) root         (0)     2019 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_long_term_offered_capacity.py
--rw-r--r--   0 root         (0) root         (0)     2522 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_long_term_reserve_price.py
--rw-r--r--   0 root         (0) root         (0)     2127 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_long_term_reserve_price_steps_inner.py
--rw-r--r--   0 root         (0) root         (0)     1432 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_manual_file_upload_api.py
--rw-r--r--   0 root         (0) root         (0)     1991 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_manual_file_upload_request.py
--rw-r--r--   0 root         (0) root         (0)      982 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_market.py
--rw-r--r--   0 root         (0) root         (0)     2658 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_message.py
--rw-r--r--   0 root         (0) root         (0)     3678 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_message_batch.py
--rw-r--r--   0 root         (0) root         (0)     1046 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_message_category.py
--rw-r--r--   0 root         (0) root         (0)     1032 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_message_sender.py
--rw-r--r--   0 root         (0) root         (0)     1046 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_message_severity.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_message_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_message_type.py
--rw-r--r--   0 root         (0) root         (0)     1362 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_messages_api.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_metadata_api.py
--rw-r--r--   0 root         (0) root         (0)     1884 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_mtu_period.py
--rw-r--r--   0 root         (0) root         (0)      990 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_mtu_size.py
--rw-r--r--   0 root         (0) root         (0)     2130 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_mtu_size_per_auction_product_type.py
--rw-r--r--   0 root         (0) root         (0)     1966 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_mtu_size_per_timescale.py
--rw-r--r--   0 root         (0) root         (0)     1818 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_nested_error.py
--rw-r--r--   0 root         (0) root         (0)     1522 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_nomination_api.py
--rw-r--r--   0 root         (0) root         (0)     1117 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_nomination_restriction_type.py
--rw-r--r--   0 root         (0) root         (0)     1082 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_noticeboard_entry_type.py
--rw-r--r--   0 root         (0) root         (0)     1140 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_noticeboard_entry_type_with_both.py
--rw-r--r--   0 root         (0) root         (0)     1891 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_notification_preference.py
--rw-r--r--   0 root         (0) root         (0)     2036 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_notification_preference_with_sms.py
--rw-r--r--   0 root         (0) root         (0)     2003 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_ntc_overview_mtu_data.py
--rw-r--r--   0 root         (0) root         (0)     1082 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_offered_capacity_setup.py
--rw-r--r--   0 root         (0) root         (0)     2147 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_api.py
--rw-r--r--   0 root         (0) root         (0)     1096 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_auth_method.py
--rw-r--r--   0 root         (0) root         (0)     6103 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_contact.py
--rw-r--r--   0 root         (0) root         (0)    11189 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_contact_information.py
--rw-r--r--   0 root         (0) root         (0)     3633 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_document.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_document_api.py
--rw-r--r--   0 root         (0) root         (0)     4658 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_document_batch.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_document_file_type.py
--rw-r--r--   0 root         (0) root         (0)     3268 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_document_options.py
--rw-r--r--   0 root         (0) root         (0)     2671 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_document_organisation.py
--rw-r--r--   0 root         (0) root         (0)     1125 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_document_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_document_status.py
--rw-r--r--   0 root         (0) root         (0)     2707 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_document_uploaded_by_user.py
--rw-r--r--   0 root         (0) root         (0)     2304 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_document_uploaded_by_user_organisation.py
--rw-r--r--   0 root         (0) root         (0)     2034 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_document_user.py
--rw-r--r--   0 root         (0) root         (0)     2014 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_file_settings.py
--rw-r--r--   0 root         (0) root         (0)     3505 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_market_settings.py
--rw-r--r--   0 root         (0) root         (0)     2375 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_market_settings_gb_nomination_settings.py
--rw-r--r--   0 root         (0) root         (0)     2325 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_market_settings_nl_nomination_settings.py
--rw-r--r--   0 root         (0) root         (0)     1067 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_status.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_type.py
--rw-r--r--   0 root         (0) root         (0)     6451 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_user.py
--rw-r--r--   0 root         (0) root         (0)     7158 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_user_batch.py
--rw-r--r--   0 root         (0) root         (0)     1097 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_organisation_user_sort_by.py
--rw-r--r--   0 root         (0) root         (0)     1864 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_other_party.py
--rw-r--r--   0 root         (0) root         (0)     1874 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant.py
--rw-r--r--   0 root         (0) root         (0)     2844 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_api.py
--rw-r--r--   0 root         (0) root         (0)     2352 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_default_bids_and_nominations_data.py
--rw-r--r--   0 root         (0) root         (0)     3986 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_finance_overview_data.py
--rw-r--r--   0 root         (0) root         (0)     2762 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_finance_overview_invoice.py
--rw-r--r--   0 root         (0) root         (0)     4166 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_interconnector_capacity_data.py
--rw-r--r--   0 root         (0) root         (0)     3568 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_interconnector_capacity_data_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     3000 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_interconnector_capacity_data_mtus_inner_values_inner.py
--rw-r--r--   0 root         (0) root         (0)     4255 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_interconnector_capacity_graph_data.py
--rw-r--r--   0 root         (0) root         (0)     3735 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     2636 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_inner_netted_nominations.py
--rw-r--r--   0 root         (0) root         (0)     2562 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_inner_values_inner.py
--rw-r--r--   0 root         (0) root         (0)     5714 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_messages.py
--rw-r--r--   0 root         (0) root         (0)     4190 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_netted_nominations_data.py
--rw-r--r--   0 root         (0) root         (0)     3627 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_netted_nominations_data_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     2626 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_netted_nominations_data_mtus_inner_aggregated_nominations_inner.py
--rw-r--r--   0 root         (0) root         (0)     2514 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_netted_nominations_data_mtus_inner_netted_nominations.py
--rw-r--r--   0 root         (0) root         (0)     3109 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_next_auction.py
--rw-r--r--   0 root         (0) root         (0)     7585 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_next_auctions_and_nomination_gates.py
--rw-r--r--   0 root         (0) root         (0)     4722 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_transmission_rights_and_nominations_data.py
--rw-r--r--   0 root         (0) root         (0)     4080 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     3097 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_inner_values_inner.py
--rw-r--r--   0 root         (0) root         (0)     2876 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_inner_values_inner_nomination_restriction.py
--rw-r--r--   0 root         (0) root         (0)     3907 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data.py
--rw-r--r--   0 root         (0) root         (0)     3376 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     2789 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_inner_values_inner.py
--rw-r--r--   0 root         (0) root         (0)    14117 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_organisation_details.py
--rw-r--r--   0 root         (0) root         (0)     1182 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_participant_overview_api.py
--rw-r--r--   0 root         (0) root         (0)    13510 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_overview_data.py
--rw-r--r--   0 root         (0) root         (0)    11325 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_overview_data_contact_information.py
--rw-r--r--   0 root         (0) root         (0)     2271 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_overview_data_finance_overview.py
--rw-r--r--   0 root         (0) root         (0)     2224 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_participant_overview_data_organisation_members.py
--rw-r--r--   0 root         (0) root         (0)     1010 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_permission.py
--rw-r--r--   0 root         (0) root         (0)     1067 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_platform_appearance.py
--rw-r--r--   0 root         (0) root         (0)     9781 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_profile.py
--rw-r--r--   0 root         (0) root         (0)     1946 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_profile_api.py
--rw-r--r--   0 root         (0) root         (0)     6754 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_profile_details.py
--rw-r--r--   0 root         (0) root         (0)     6669 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_profile_user.py
--rw-r--r--   0 root         (0) root         (0)     2107 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_profile_user_organisation.py
--rw-r--r--   0 root         (0) root         (0)     4256 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_public_aggregated_nominations_overview_response.py
--rw-r--r--   0 root         (0) root         (0)     3711 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_public_aggregated_nominations_overview_response_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     2555 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_public_aggregated_nominations_overview_response_mtus_inner_values_inner.py
--rw-r--r--   0 root         (0) root         (0)     1366 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_public_allocated_auction_api.py
--rw-r--r--   0 root         (0) root         (0)     3327 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_public_auction.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_public_auction_api.py
--rw-r--r--   0 root         (0) root         (0)     4016 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_public_auction_batch.py
--rw-r--r--   0 root         (0) root         (0)     1097 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_public_auction_bid_status.py
--rw-r--r--   0 root         (0) root         (0)     1075 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_public_auction_status.py
--rw-r--r--   0 root         (0) root         (0)     5300 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_public_day_ahead_auction.py
--rw-r--r--   0 root         (0) root         (0)     3087 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_public_day_ahead_or_intra_day_auction_mtu_results.py
--rw-r--r--   0 root         (0) root         (0)     2624 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_public_day_ahead_or_intra_day_auction_mtu_results_bids_inner.py
--rw-r--r--   0 root         (0) root         (0)     3790 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_public_day_ahead_or_intra_day_auction_results.py
--rw-r--r--   0 root         (0) root         (0)     5300 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_public_intra_day_auction.py
--rw-r--r--   0 root         (0) root         (0)     5794 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_public_long_term_auction.py
--rw-r--r--   0 root         (0) root         (0)     3693 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_public_long_term_auction_results.py
--rw-r--r--   0 root         (0) root         (0)     1206 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_public_nominations_api.py
--rw-r--r--   0 root         (0) root         (0)     2022 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_purchased_by_organisation.py
--rw-r--r--   0 root         (0) root         (0)     1988 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_reporting_api.py
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_reserve_price_publish_type.py
--rw-r--r--   0 root         (0) root         (0)     2543 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_return_auction.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_sage_code.py
--rw-r--r--   0 root         (0) root         (0)     5536 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_api.py
--rw-r--r--   0 root         (0) root         (0)     2095 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_capacity_price_mtu.py
--rw-r--r--   0 root         (0) root         (0)    11431 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     3472 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_details.py
--rw-r--r--   0 root         (0) root         (0)     3161 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_matching.py
--rw-r--r--   0 root         (0) root         (0)     7558 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_response.py
--rw-r--r--   0 root         (0) root         (0)     2627 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_response_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     2998 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_options.py
--rw-r--r--   0 root         (0) root         (0)     3096 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_response_options.py
--rw-r--r--   0 root         (0) root         (0)     4631 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     2442 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     3122 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_options.py
--rw-r--r--   0 root         (0) root         (0)     2585 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_options_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     8384 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_long_term_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     2822 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_long_term_noticeboard_entry_details.py
--rw-r--r--   0 root         (0) root         (0)     6775 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_long_term_noticeboard_entry_response.py
--rw-r--r--   0 root         (0) root         (0)     2171 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_long_term_noticeboard_options.py
--rw-r--r--   0 root         (0) root         (0)     2269 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_long_term_noticeboard_response_options.py
--rw-r--r--   0 root         (0) root         (0)     2199 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_long_term_transfer_request_options.py
--rw-r--r--   0 root         (0) root         (0)     3108 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_noticeboard_entry.py
--rw-r--r--   0 root         (0) root         (0)     3926 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_noticeboard_entry_batch.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_noticeboard_entry_status.py
--rw-r--r--   0 root         (0) root         (0)     3890 2023-07-05 11:59:31.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_return_request.py
--rw-r--r--   0 root         (0) root         (0)     4718 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_return_request_batch.py
--rw-r--r--   0 root         (0) root         (0)     1182 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_return_request_status.py
--rw-r--r--   0 root         (0) root         (0)     3940 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_transfer_request.py
--rw-r--r--   0 root         (0) root         (0)     4780 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_transfer_request_batch.py
--rw-r--r--   0 root         (0) root         (0)     1196 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_transfer_request_status.py
--rw-r--r--   0 root         (0) root         (0)     1182 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_transfer_request_type.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_secondary_market_transfer_transmission_rights_mtu.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_settlement.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_settlement_item.py
--rw-r--r--   0 root         (0) root         (0)     2636 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_settlement_per_source.py
--rw-r--r--   0 root         (0) root         (0)     1082 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_settlement_source_type.py
--rw-r--r--   0 root         (0) root         (0)     1104 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_settlement_sub_source_type.py
--rw-r--r--   0 root         (0) root         (0)     3103 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_source_auction.py
--rw-r--r--   0 root         (0) root         (0)     2104 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_source_auction_display_data.py
--rw-r--r--   0 root         (0) root         (0)     1980 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_source_auction_result.py
--rw-r--r--   0 root         (0) root         (0)     3820 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_submit_day_ahead_or_intra_day_bids_request.py
--rw-r--r--   0 root         (0) root         (0)     3197 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_submit_day_ahead_or_intra_day_bids_request_bid_groups_inner.py
--rw-r--r--   0 root         (0) root         (0)     2531 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_submit_day_ahead_or_intra_day_bids_request_bid_groups_inner_bids_inner.py
--rw-r--r--   0 root         (0) root         (0)     2906 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_submit_long_term_bids_request.py
--rw-r--r--   0 root         (0) root         (0)     2365 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_submit_long_term_bids_request_bids_inner.py
--rw-r--r--   0 root         (0) root         (0)     1924 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_submit_nominations_mtu.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_submit_timescale_nominations_request.py
--rw-r--r--   0 root         (0) root         (0)     1089 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_system_message_category.py
--rw-r--r--   0 root         (0) root         (0)     1139 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_timescale_nomination_mtu_status.py
--rw-r--r--   0 root         (0) root         (0)     2339 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_timescale_nomination_options.py
--rw-r--r--   0 root         (0) root         (0)     2220 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_timescale_nomination_options_window_timing.py
--rw-r--r--   0 root         (0) root         (0)     1117 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_timescale_nomination_status.py
--rw-r--r--   0 root         (0) root         (0)     1103 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_timescale_nomination_type.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_timescale_nomination_window_status.py
--rw-r--r--   0 root         (0) root         (0)     3328 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_timescale_nominations.py
--rw-r--r--   0 root         (0) root         (0)     2552 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_timescale_nominations_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     2308 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_timescale_nominations_mtus_inner_current_nomination.py
--rw-r--r--   0 root         (0) root         (0)     1186 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_transmission_right_api.py
--rw-r--r--   0 root         (0) root         (0)     4087 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_transmission_rights_overview.py
--rw-r--r--   0 root         (0) root         (0)     3610 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_transmission_rights_overview_mtus_inner.py
--rw-r--r--   0 root         (0) root         (0)     2983 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_transmission_rights_overview_mtus_inner_values_inner.py
--rw-r--r--   0 root         (0) root         (0)     2424 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_transmission_rights_overview_mtus_inner_values_inner_timescales_inner.py
--rw-r--r--   0 root         (0) root         (0)     1878 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_uiosi_not_resold.py
--rw-r--r--   0 root         (0) root         (0)     3364 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_uiosi_overview.py
--rw-r--r--   0 root         (0) root         (0)     2881 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_uiosi_overview_per_mtu.py
--rw-r--r--   0 root         (0) root         (0)     1937 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_uiosi_resold.py
--rw-r--r--   0 root         (0) root         (0)     1887 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_unread_messages_response.py
--rw-r--r--   0 root         (0) root         (0)     3945 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_update_day_ahead_or_intra_day_default_bid_request.py
--rw-r--r--   0 root         (0) root         (0)     2705 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_update_default_nomination_request.py
--rw-r--r--   0 root         (0) root         (0)     2733 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_update_long_term_default_bid_request.py
--rw-r--r--   0 root         (0) root         (0)     2079 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_update_profile_details_request.py
--rw-r--r--   0 root         (0) root         (0)     2038 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_update_user_request.py
--rw-r--r--   0 root         (0) root         (0)     6660 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_user.py
--rw-r--r--   0 root         (0) root         (0)     1446 2023-07-05 11:59:33.000000 empire-platform-api-public-client-0.166.0/test/test_user_api.py
--rw-r--r--   0 root         (0) root         (0)     1936 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_user_organisation.py
--rw-r--r--   0 root         (0) root         (0)     4381 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_user_preferences.py
--rw-r--r--   0 root         (0) root         (0)     3318 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_user_preferences_general_notifications.py
--rw-r--r--   0 root         (0) root         (0)     2750 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_user_preferences_subscription_notifications.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_user_role.py
--rw-r--r--   0 root         (0) root         (0)     1011 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_user_status.py
--rw-r--r--   0 root         (0) root         (0)     1019 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_vat_rate_type.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_version.py
--rw-r--r--   0 root         (0) root         (0)     1915 2023-07-05 11:59:32.000000 empire-platform-api-public-client-0.166.0/test/test_zendesk_chat_token_response.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:17:52.915233 empire-platform-api-public-client-0.167.0/
+-rw-r--r--   0 root         (0) root         (0)      612 2023-07-11 11:17:52.915233 empire-platform-api-public-client-0.167.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    50302 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:17:52.845234 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/
+-rw-r--r--   0 root         (0) root         (0)    41280 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:17:52.855234 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/
+-rw-r--r--   0 root         (0) root         (0)     2193 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10382 2023-07-11 11:17:51.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/attachment_api.py
+-rw-r--r--   0 root         (0) root         (0)   116019 2023-07-11 11:17:51.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/auction_api.py
+-rw-r--r--   0 root         (0) root         (0)    17984 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/audit_log_api.py
+-rw-r--r--   0 root         (0) root         (0)    15031 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/bidding_configuration_api.py
+-rw-r--r--   0 root         (0) root         (0)    16899 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/buy_now_offers_api.py
+-rw-r--r--   0 root         (0) root         (0)    71676 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/default_bid_api.py
+-rw-r--r--   0 root         (0) root         (0)    46916 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/default_nomination_api.py
+-rw-r--r--   0 root         (0) root         (0)    44696 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/finance_api.py
+-rw-r--r--   0 root         (0) root         (0)     7766 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/finance_information_api.py
+-rw-r--r--   0 root         (0) root         (0)    24412 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/manual_file_upload_api.py
+-rw-r--r--   0 root         (0) root         (0)    31027 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/messages_api.py
+-rw-r--r--   0 root         (0) root         (0)     6828 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)    35670 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/nomination_api.py
+-rw-r--r--   0 root         (0) root         (0)    19781 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/organisation_api.py
+-rw-r--r--   0 root         (0) root         (0)    35124 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/organisation_document_api.py
+-rw-r--r--   0 root         (0) root         (0)    72445 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/participant_dashboard_api.py
+-rw-r--r--   0 root         (0) root         (0)     7810 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/participant_overview_api.py
+-rw-r--r--   0 root         (0) root         (0)    55831 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/profile_api.py
+-rw-r--r--   0 root         (0) root         (0)    21816 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/public_allocated_auction_api.py
+-rw-r--r--   0 root         (0) root         (0)    67522 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/public_auction_api.py
+-rw-r--r--   0 root         (0) root         (0)     8660 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/public_nominations_api.py
+-rw-r--r--   0 root         (0) root         (0)    65136 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/reporting_api.py
+-rw-r--r--   0 root         (0) root         (0)   212050 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/secondary_market_api.py
+-rw-r--r--   0 root         (0) root         (0)    10353 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/transmission_right_api.py
+-rw-r--r--   0 root         (0) root         (0)    36183 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/user_api.py
+-rw-r--r--   0 root         (0) root         (0)    30336 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api_client.py
+-rw-r--r--   0 root         (0) root         (0)      844 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api_response.py
+-rw-r--r--   0 root         (0) root         (0)    16914 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     5334 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:17:52.885233 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/
+-rw-r--r--   0 root         (0) root         (0)    38418 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2518 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/address.py
+-rw-r--r--   0 root         (0) root         (0)     5328 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_allocated_auction.py
+-rw-r--r--   0 root         (0) root         (0)     1084 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nomination_type.py
+-rw-r--r--   0 root         (0) root         (0)     3172 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nominations_mns_or_gb.py
+-rw-r--r--   0 root         (0) root         (0)     4362 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nominations_mns_or_gb_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2690 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nominations_mtu_netted_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     2491 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nominations_mtu_value.py
+-rw-r--r--   0 root         (0) root         (0)     2873 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nominations_nl.py
+-rw-r--r--   0 root         (0) root         (0)     4961 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nominations_nl_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2675 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nominations_nl_mtus_inner_eprogram_values.py
+-rw-r--r--   0 root         (0) root         (0)     5292 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/allocated_auction.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/allocated_auction_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1480 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/allocated_auction_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     2645 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/api_key.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/attachment.py
+-rw-r--r--   0 root         (0) root         (0)     5818 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_allocation_resolution.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_batch.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_bid_participant.py
+-rw-r--r--   0 root         (0) root         (0)     1050 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_bid_status.py
+-rw-r--r--   0 root         (0) root         (0)     3086 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_bidding_configuration.py
+-rw-r--r--   0 root         (0) root         (0)      944 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_bidding_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_intra_day_product_type.py
+-rw-r--r--   0 root         (0) root         (0)     6510 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_process_steps_absolute.py
+-rw-r--r--   0 root         (0) root         (0)     1715 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_product_type.py
+-rw-r--r--   0 root         (0) root         (0)     2965 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_reduction_period.py
+-rw-r--r--   0 root         (0) root         (0)     3122 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_result_congestion_rent.py
+-rw-r--r--   0 root         (0) root         (0)     2707 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_result_participant.py
+-rw-r--r--   0 root         (0) root         (0)     1533 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_status.py
+-rw-r--r--   0 root         (0) root         (0)     1355 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_timescale.py
+-rw-r--r--   0 root         (0) root         (0)     4663 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     2709 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_api_key.py
+-rw-r--r--   0 root         (0) root         (0)     2768 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_domain.py
+-rw-r--r--   0 root         (0) root         (0)     2377 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_payload.py
+-rw-r--r--   0 root         (0) root         (0)      964 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      934 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_status.py
+-rw-r--r--   0 root         (0) root         (0)     8092 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_type.py
+-rw-r--r--   0 root         (0) root         (0)     2817 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_user.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_user_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/bid_value.py
+-rw-r--r--   0 root         (0) root         (0)     3391 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/bidding_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     3112 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/bidding_configuration_per_direction.py
+-rw-r--r--   0 root         (0) root         (0)     2541 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/bidding_configuration_secondary_market_notices.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/bidding_configuration_values_inner.py
+-rw-r--r--   0 root         (0) root         (0)      992 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/border_direction.py
+-rw-r--r--   0 root         (0) root         (0)     1017 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/border_direction_with_both.py
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/border_direction_with_both_and_none.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/buy_now_day_ahead_offer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     5708 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/buy_now_offer.py
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/buy_now_offer_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)      999 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/buy_now_offer_status.py
+-rw-r--r--   0 root         (0) root         (0)     2089 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_api_key_request.py
+-rw-r--r--   0 root         (0) root         (0)     6802 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request.py
+-rw-r--r--   0 root         (0) root         (0)     3028 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request_bids_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3410 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request_bids_inner_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3752 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_default_nomination_request.py
+-rw-r--r--   0 root         (0) root         (0)     6545 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_long_term_default_bid_request.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_organisation_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4220 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_noticeboard_response.py
+-rw-r--r--   0 root         (0) root         (0)     3945 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     3585 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_transfer_request_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4215 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_secondary_market_long_term_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4112 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_secondary_market_long_term_noticeboard_response.py
+-rw-r--r--   0 root         (0) root         (0)     3383 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_secondary_market_long_term_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_secondary_market_return_request.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_api_key.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_default_bid.py
+-rw-r--r--   0 root         (0) root         (0)     2185 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_default_nomination.py
+-rw-r--r--   0 root         (0) root         (0)     2209 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_organisation_document.py
+-rw-r--r--   0 root         (0) root         (0)     2441 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2465 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_noticeboard_response.py
+-rw-r--r--   0 root         (0) root         (0)     2433 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2361 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_secondary_market_long_term_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_secondary_market_long_term_noticeboard_response.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_secondary_market_long_term_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_secondary_market_return_request_identifier.py
+-rw-r--r--   0 root         (0) root         (0)     4011 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/dashboard_next_nomination_gate.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/dashboard_next_nomination_gate_window.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/dashboard_next_nomination_window_status.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/date_period.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/date_time_period.py
+-rw-r--r--   0 root         (0) root         (0)     6273 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_auction.py
+-rw-r--r--   0 root         (0) root         (0)     3470 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group.py
+-rw-r--r--   0 root         (0) root         (0)     3074 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_batch.py
+-rw-r--r--   0 root         (0) root         (0)     3654 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3342 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids_inner_value.py
+-rw-r--r--   0 root         (0) root         (0)     4615 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     2845 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu_results.py
+-rw-r--r--   0 root         (0) root         (0)     3090 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu_results_bids_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2941 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results.py
+-rw-r--r--   0 root         (0) root         (0)     3774 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3025 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results_mtus_inner_value.py
+-rw-r--r--   0 root         (0) root         (0)     4161 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_results.py
+-rw-r--r--   0 root         (0) root         (0)     5137 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_results_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     6843 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_default_bid.py
+-rw-r--r--   0 root         (0) root         (0)     5979 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_bid.py
+-rw-r--r--   0 root         (0) root         (0)     2792 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_bid_batch.py
+-rw-r--r--   0 root         (0) root         (0)     2692 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_bid_options.py
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_bid_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      942 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_bid_status.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_nomination.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_nomination_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_nomination_declaration_type.py
+-rw-r--r--   0 root         (0) root         (0)     3849 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_nomination_details.py
+-rw-r--r--   0 root         (0) root         (0)     3177 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_nomination_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_nomination_options.py
+-rw-r--r--   0 root         (0) root         (0)     1343 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_nomination_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_nomination_status.py
+-rw-r--r--   0 root         (0) root         (0)     9333 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/error_code.py
+-rw-r--r--   0 root         (0) root         (0)     3278 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/error_response.py
+-rw-r--r--   0 root         (0) root         (0)     5902 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/finance_information.py
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/finance_information_bank_deposits_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2895 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/finance_information_letter_of_credits_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2489 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/finance_information_lockable_amount.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/finance_information_lockable_date.py
+-rw-r--r--   0 root         (0) root         (0)     3549 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/finance_information_lockable_period.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/finance_information_market_vat_details.py
+-rw-r--r--   0 root         (0) root         (0)     2344 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/finance_information_sage_settings.py
+-rw-r--r--   0 root         (0) root         (0)     6273 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/intra_day_auction.py
+-rw-r--r--   0 root         (0) root         (0)     4687 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_action_type.py
+-rw-r--r--   0 root         (0) root         (0)     2755 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_batch.py
+-rw-r--r--   0 root         (0) root         (0)     8176 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_details.py
+-rw-r--r--   0 root         (0) root         (0)     3154 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_history.py
+-rw-r--r--   0 root         (0) root         (0)     4434 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_line_item.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_participant_details.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_status.py
+-rw-r--r--   0 root         (0) root         (0)     3964 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_summary.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_vat_rate.py
+-rw-r--r--   0 root         (0) root         (0)     6980 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_auction.py
+-rw-r--r--   0 root         (0) root         (0)     3875 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_auction_bid.py
+-rw-r--r--   0 root         (0) root         (0)     2890 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_auction_bid_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1080 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_auction_bid_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     4475 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_auction_results.py
+-rw-r--r--   0 root         (0) root         (0)     3415 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_auction_results_allocated_capacity_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3407 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_bidding_results.py
+-rw-r--r--   0 root         (0) root         (0)     6586 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_default_bid.py
+-rw-r--r--   0 root         (0) root         (0)     2837 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_offered_capacity.py
+-rw-r--r--   0 root         (0) root         (0)     2909 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_reserve_price.py
+-rw-r--r--   0 root         (0) root         (0)     3043 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_reserve_price_steps_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/manual_file_upload_request.py
+-rw-r--r--   0 root         (0) root         (0)      874 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/market.py
+-rw-r--r--   0 root         (0) root         (0)     4125 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/message.py
+-rw-r--r--   0 root         (0) root         (0)     2755 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/message_batch.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/message_category.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/message_sender.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/message_severity.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/message_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/message_type.py
+-rw-r--r--   0 root         (0) root         (0)     4139 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/mtu_period.py
+-rw-r--r--   0 root         (0) root         (0)      967 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/mtu_size.py
+-rw-r--r--   0 root         (0) root         (0)     2517 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/mtu_size_per_auction_product_type.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/mtu_size_per_timescale.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/nested_error.py
+-rw-r--r--   0 root         (0) root         (0)     1015 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/nomination_restriction_type.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/noticeboard_entry_type.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/noticeboard_entry_type_with_both.py
+-rw-r--r--   0 root         (0) root         (0)     2119 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/notification_preference.py
+-rw-r--r--   0 root         (0) root         (0)     2250 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/notification_preference_with_sms.py
+-rw-r--r--   0 root         (0) root         (0)     3484 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/ntc_overview_mtu_data.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/offered_capacity_setup.py
+-rw-r--r--   0 root         (0) root         (0)     2969 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation.py
+-rw-r--r--   0 root         (0) root         (0)      968 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_auth_method.py
+-rw-r--r--   0 root         (0) root         (0)     2898 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_contact.py
+-rw-r--r--   0 root         (0) root         (0)     3625 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_contact_information.py
+-rw-r--r--   0 root         (0) root         (0)     4298 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document.py
+-rw-r--r--   0 root         (0) root         (0)     2912 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_file_type.py
+-rw-r--r--   0 root         (0) root         (0)     3068 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_options.py
+-rw-r--r--   0 root         (0) root         (0)     2966 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)      996 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_status.py
+-rw-r--r--   0 root         (0) root         (0)     2934 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_uploaded_by_user.py
+-rw-r--r--   0 root         (0) root         (0)     2439 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_uploaded_by_user_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_user.py
+-rw-r--r--   0 root         (0) root         (0)     2326 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_file_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3906 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_market_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2995 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_market_settings_gb_nomination_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_market_settings_nl_nomination_settings.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_status.py
+-rw-r--r--   0 root         (0) root         (0)      960 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_type.py
+-rw-r--r--   0 root         (0) root         (0)     4588 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_user.py
+-rw-r--r--   0 root         (0) root         (0)     2864 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_user_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     2170 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/other_party.py
+-rw-r--r--   0 root         (0) root         (0)     2159 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant.py
+-rw-r--r--   0 root         (0) root         (0)     2601 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_default_bids_and_nominations_data.py
+-rw-r--r--   0 root         (0) root         (0)     3816 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_finance_overview_data.py
+-rw-r--r--   0 root         (0) root         (0)     3598 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_finance_overview_invoice.py
+-rw-r--r--   0 root         (0) root         (0)     3164 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data.py
+-rw-r--r--   0 root         (0) root         (0)     4012 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data_mtus_inner_values_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data.py
+-rw-r--r--   0 root         (0) root         (0)     4869 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2871 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_inner_netted_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_inner_values_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3207 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_messages.py
+-rw-r--r--   0 root         (0) root         (0)     3091 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data.py
+-rw-r--r--   0 root         (0) root         (0)     4939 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2867 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_inner_aggregated_nominations_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2791 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_inner_netted_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     4889 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_next_auction.py
+-rw-r--r--   0 root         (0) root         (0)     4442 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_next_auctions_and_nomination_gates.py
+-rw-r--r--   0 root         (0) root         (0)     3273 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data.py
+-rw-r--r--   0 root         (0) root         (0)     4134 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4163 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_inner_values_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_inner_values_inner_nomination_restriction.py
+-rw-r--r--   0 root         (0) root         (0)     3157 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data.py
+-rw-r--r--   0 root         (0) root         (0)     4195 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_inner_values_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4429 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_organisation_details.py
+-rw-r--r--   0 root         (0) root         (0)     5035 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_overview_data.py
+-rw-r--r--   0 root         (0) root         (0)     3713 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_overview_data_contact_information.py
+-rw-r--r--   0 root         (0) root         (0)     3085 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_overview_data_finance_overview.py
+-rw-r--r--   0 root         (0) root         (0)     2659 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_overview_data_organisation_members.py
+-rw-r--r--   0 root         (0) root         (0)     6742 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/permission.py
+-rw-r--r--   0 root         (0) root         (0)     1154 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/platform_appearance.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/profile.py
+-rw-r--r--   0 root         (0) root         (0)     3701 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/profile_details.py
+-rw-r--r--   0 root         (0) root         (0)     3237 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/profile_user.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/profile_user_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     3136 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response.py
+-rw-r--r--   0 root         (0) root         (0)     4772 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3062 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus_inner_values_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4460 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_auction.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_auction_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_auction_bid_status.py
+-rw-r--r--   0 root         (0) root         (0)     1247 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_auction_status.py
+-rw-r--r--   0 root         (0) root         (0)     5423 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_day_ahead_auction.py
+-rw-r--r--   0 root         (0) root         (0)     2918 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_mtu_results.py
+-rw-r--r--   0 root         (0) root         (0)     3157 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_mtu_results_bids_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3628 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_results.py
+-rw-r--r--   0 root         (0) root         (0)     5423 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_intra_day_auction.py
+-rw-r--r--   0 root         (0) root         (0)     6428 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_long_term_auction.py
+-rw-r--r--   0 root         (0) root         (0)     3933 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_long_term_auction_results.py
+-rw-r--r--   0 root         (0) root         (0)     2255 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/purchased_by_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/reserve_price_publish_type.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/return_auction.py
+-rw-r--r--   0 root         (0) root         (0)     5216 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/sage_code.py
+-rw-r--r--   0 root         (0) root         (0)     3545 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_capacity_price_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     4592 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4594 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_details.py
+-rw-r--r--   0 root         (0) root         (0)     4952 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_matching.py
+-rw-r--r--   0 root         (0) root         (0)     4761 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_response.py
+-rw-r--r--   0 root         (0) root         (0)     3910 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_response_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3139 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_options.py
+-rw-r--r--   0 root         (0) root         (0)     3203 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_response_options.py
+-rw-r--r--   0 root         (0) root         (0)     6570 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     3514 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3257 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_options.py
+-rw-r--r--   0 root         (0) root         (0)     3654 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_options_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3560 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4309 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry_details.py
+-rw-r--r--   0 root         (0) root         (0)     4501 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry_response.py
+-rw-r--r--   0 root         (0) root         (0)     2526 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_options.py
+-rw-r--r--   0 root         (0) root         (0)     2590 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_response_options.py
+-rw-r--r--   0 root         (0) root         (0)     2506 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_long_term_transfer_request_options.py
+-rw-r--r--   0 root         (0) root         (0)     5332 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3046 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_noticeboard_entry_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_noticeboard_entry_status.py
+-rw-r--r--   0 root         (0) root         (0)     4441 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_return_request.py
+-rw-r--r--   0 root         (0) root         (0)     3010 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_return_request_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_return_request_status.py
+-rw-r--r--   0 root         (0) root         (0)     6453 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     3034 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_transfer_request_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1122 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_transfer_request_status.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_transfer_request_type.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_transfer_transmission_rights_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/settlement.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/settlement_item.py
+-rw-r--r--   0 root         (0) root         (0)     3350 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/settlement_per_source.py
+-rw-r--r--   0 root         (0) root         (0)     1038 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/settlement_source_type.py
+-rw-r--r--   0 root         (0) root         (0)     2223 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/settlement_sub_source_type.py
+-rw-r--r--   0 root         (0) root         (0)     3715 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/source_auction.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/source_auction_display_data.py
+-rw-r--r--   0 root         (0) root         (0)     2684 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/source_auction_result.py
+-rw-r--r--   0 root         (0) root         (0)     2935 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request.py
+-rw-r--r--   0 root         (0) root         (0)     3594 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request_bid_groups_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3617 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request_bid_groups_inner_bids_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2722 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/submit_long_term_bids_request.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/submit_long_term_bids_request_bids_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3169 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/submit_nominations_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     2726 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/submit_timescale_nominations_request.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/system_message_category.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nomination_mtu_status.py
+-rw-r--r--   0 root         (0) root         (0)     3262 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nomination_options.py
+-rw-r--r--   0 root         (0) root         (0)     3150 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nomination_options_window_timing.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nomination_status.py
+-rw-r--r--   0 root         (0) root         (0)     1081 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nomination_type.py
+-rw-r--r--   0 root         (0) root         (0)     1045 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nomination_window_status.py
+-rw-r--r--   0 root         (0) root         (0)     2836 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     5393 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nominations_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3219 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nominations_mtus_inner_current_nomination.py
+-rw-r--r--   0 root         (0) root         (0)     2732 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/transmission_rights_overview.py
+-rw-r--r--   0 root         (0) root         (0)     3770 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/transmission_rights_overview_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3960 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/transmission_rights_overview_mtus_inner_values_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/transmission_rights_overview_mtus_inner_values_inner_timescales_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/uiosi_not_resold.py
+-rw-r--r--   0 root         (0) root         (0)     2740 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/uiosi_overview.py
+-rw-r--r--   0 root         (0) root         (0)     4347 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/uiosi_overview_per_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     2841 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/uiosi_resold.py
+-rw-r--r--   0 root         (0) root         (0)     2206 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/unread_messages_response.py
+-rw-r--r--   0 root         (0) root         (0)     6116 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/update_day_ahead_or_intra_day_default_bid_request.py
+-rw-r--r--   0 root         (0) root         (0)     3318 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/update_default_nomination_request.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/update_long_term_default_bid_request.py
+-rw-r--r--   0 root         (0) root         (0)     2761 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/update_profile_details_request.py
+-rw-r--r--   0 root         (0) root         (0)     2830 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/update_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     3904 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/user.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/user_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     3545 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/user_preferences.py
+-rw-r--r--   0 root         (0) root         (0)     3806 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/user_preferences_general_notifications.py
+-rw-r--r--   0 root         (0) root         (0)     3409 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/user_preferences_subscription_notifications.py
+-rw-r--r--   0 root         (0) root         (0)     1510 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/user_role.py
+-rw-r--r--   0 root         (0) root         (0)      940 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/user_status.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/vat_rate_type.py
+-rw-r--r--   0 root         (0) root         (0)     2005 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/version.py
+-rw-r--r--   0 root         (0) root         (0)     2133 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/zendesk_chat_token_response.py
+-rw-r--r--   0 root         (0) root         (0)    12999 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:17:52.845234 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      612 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    43360 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       34 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/empire_platform_api_public_client.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      712 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-11 11:17:52.915233 empire-platform-api-public-client-0.167.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 11:17:52.915233 empire-platform-api-public-client-0.167.0/test/
+-rw-r--r--   0 root         (0) root         (0)     1943 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_address.py
+-rw-r--r--   0 root         (0) root         (0)     3195 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_aggregated_allocated_auction.py
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_aggregated_nomination_type.py
+-rw-r--r--   0 root         (0) root         (0)     8585 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_aggregated_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     3624 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_aggregated_nominations_mns_or_gb.py
+-rw-r--r--   0 root         (0) root         (0)     3113 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_aggregated_nominations_mns_or_gb_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_aggregated_nominations_mtu_netted_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_aggregated_nominations_mtu_value.py
+-rw-r--r--   0 root         (0) root         (0)     4094 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_aggregated_nominations_nl.py
+-rw-r--r--   0 root         (0) root         (0)     3558 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_aggregated_nominations_nl_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_aggregated_nominations_nl_mtus_inner_eprogram_values.py
+-rw-r--r--   0 root         (0) root         (0)     3110 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_allocated_auction.py
+-rw-r--r--   0 root         (0) root         (0)     3956 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_allocated_auction_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_allocated_auction_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_api_key.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_attachment.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2023-07-11 11:17:51.000000 empire-platform-api-public-client-0.167.0/test/test_attachment_api.py
+-rw-r--r--   0 root         (0) root         (0)     3417 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_auction.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_auction_allocation_resolution.py
+-rw-r--r--   0 root         (0) root         (0)     3000 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_auction_api.py
+-rw-r--r--   0 root         (0) root         (0)     4242 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_auction_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1998 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_auction_bid_participant.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_auction_bid_status.py
+-rw-r--r--   0 root         (0) root         (0)     2218 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_auction_bidding_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_auction_bidding_mode.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_auction_intra_day_product_type.py
+-rw-r--r--   0 root         (0) root         (0)     2738 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_auction_process_steps_absolute.py
+-rw-r--r--   0 root         (0) root         (0)     1068 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_auction_product_type.py
+-rw-r--r--   0 root         (0) root         (0)     2377 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_auction_reduction_period.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_auction_result_congestion_rent.py
+-rw-r--r--   0 root         (0) root         (0)     2129 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_auction_result_participant.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_auction_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_auction_status.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_auction_timescale.py
+-rw-r--r--   0 root         (0) root         (0)     3927 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_audit_log.py
+-rw-r--r--   0 root         (0) root         (0)     1212 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_audit_log_api.py
+-rw-r--r--   0 root         (0) root         (0)     2017 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_audit_log_api_key.py
+-rw-r--r--   0 root         (0) root         (0)     5328 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_audit_log_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_audit_log_domain.py
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_audit_log_payload.py
+-rw-r--r--   0 root         (0) root         (0)     1041 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_audit_log_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1040 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_audit_log_status.py
+-rw-r--r--   0 root         (0) root         (0)     1026 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_audit_log_type.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_audit_log_user.py
+-rw-r--r--   0 root         (0) root         (0)     2036 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_audit_log_user_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_bid_value.py
+-rw-r--r--   0 root         (0) root         (0)     3498 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_bidding_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     1320 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_bidding_configuration_api.py
+-rw-r--r--   0 root         (0) root         (0)     2086 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_bidding_configuration_per_direction.py
+-rw-r--r--   0 root         (0) root         (0)     2283 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_bidding_configuration_secondary_market_notices.py
+-rw-r--r--   0 root         (0) root         (0)     2596 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_bidding_configuration_values_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_border_direction.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_border_direction_with_both.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_border_direction_with_both_and_none.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_buy_now_day_ahead_offer_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_buy_now_offer.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_buy_now_offer_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1062 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_buy_now_offer_status.py
+-rw-r--r--   0 root         (0) root         (0)     1248 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_buy_now_offers_api.py
+-rw-r--r--   0 root         (0) root         (0)     1853 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_create_api_key_request.py
+-rw-r--r--   0 root         (0) root         (0)     4254 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_create_day_ahead_or_intra_day_default_bid_request.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_create_day_ahead_or_intra_day_default_bid_request_bids_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2519 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_create_day_ahead_or_intra_day_default_bid_request_bids_inner_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2877 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_create_default_nomination_request.py
+-rw-r--r--   0 root         (0) root         (0)     3042 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_create_long_term_default_bid_request.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_create_organisation_document_request.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_create_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     7394 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_create_secondary_market_day_ahead_or_intra_day_noticeboard_response.py
+-rw-r--r--   0 root         (0) root         (0)     3369 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_create_secondary_market_day_ahead_or_intra_day_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2470 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_create_secondary_market_day_ahead_or_intra_day_transfer_request_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2698 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_create_secondary_market_long_term_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     6807 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_create_secondary_market_long_term_noticeboard_response.py
+-rw-r--r--   0 root         (0) root         (0)     2647 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_create_secondary_market_long_term_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2363 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_create_secondary_market_return_request.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_created_api_key.py
+-rw-r--r--   0 root         (0) root         (0)     1895 2023-07-11 11:17:48.000000 empire-platform-api-public-client-0.167.0/test/test_created_default_bid.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_created_default_nomination.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_created_organisation_document.py
+-rw-r--r--   0 root         (0) root         (0)     2377 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_created_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2413 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_created_secondary_market_day_ahead_or_intra_day_noticeboard_response.py
+-rw-r--r--   0 root         (0) root         (0)     2365 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_created_secondary_market_day_ahead_or_intra_day_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_created_secondary_market_long_term_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_created_secondary_market_long_term_noticeboard_response.py
+-rw-r--r--   0 root         (0) root         (0)     2239 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_created_secondary_market_long_term_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_created_secondary_market_return_request_identifier.py
+-rw-r--r--   0 root         (0) root         (0)     3095 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_dashboard_next_nomination_gate.py
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_dashboard_next_nomination_gate_window.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_dashboard_next_nomination_window_status.py
+-rw-r--r--   0 root         (0) root         (0)     1908 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_date_period.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_date_time_period.py
+-rw-r--r--   0 root         (0) root         (0)     5555 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_day_ahead_auction.py
+-rw-r--r--   0 root         (0) root         (0)     3780 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_bid_group.py
+-rw-r--r--   0 root         (0) root         (0)     4794 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_bid_group_batch.py
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_bid_group_bids_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2607 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_bid_group_bids_inner_value.py
+-rw-r--r--   0 root         (0) root         (0)     2141 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_mtu_results.py
+-rw-r--r--   0 root         (0) root         (0)     2560 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_mtu_results_bids_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3273 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_participant_results.py
+-rw-r--r--   0 root         (0) root         (0)     2578 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_participant_results_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2383 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_participant_results_mtus_inner_value.py
+-rw-r--r--   0 root         (0) root         (0)     3985 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_results.py
+-rw-r--r--   0 root         (0) root         (0)     2565 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_results_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     4217 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_default_bid.py
+-rw-r--r--   0 root         (0) root         (0)     2470 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_default_bid.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_default_bid_api.py
+-rw-r--r--   0 root         (0) root         (0)     3128 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_default_bid_batch.py
+-rw-r--r--   0 root         (0) root         (0)     2385 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_default_bid_options.py
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_default_bid_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1054 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_default_bid_status.py
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_default_nomination.py
+-rw-r--r--   0 root         (0) root         (0)     1792 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_default_nomination_api.py
+-rw-r--r--   0 root         (0) root         (0)     2956 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_default_nomination_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_default_nomination_declaration_type.py
+-rw-r--r--   0 root         (0) root         (0)     2926 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_default_nomination_details.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_default_nomination_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     2377 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_default_nomination_options.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_default_nomination_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_default_nomination_status.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_error_code.py
+-rw-r--r--   0 root         (0) root         (0)     2282 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_error_response.py
+-rw-r--r--   0 root         (0) root         (0)     1612 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_finance_api.py
+-rw-r--r--   0 root         (0) root         (0)     9977 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_finance_information.py
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_finance_information_api.py
+-rw-r--r--   0 root         (0) root         (0)     3836 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_finance_information_bank_deposits_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3941 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_finance_information_letter_of_credits_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2082 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_finance_information_lockable_amount.py
+-rw-r--r--   0 root         (0) root         (0)     2112 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_finance_information_lockable_date.py
+-rw-r--r--   0 root         (0) root         (0)     3323 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_finance_information_lockable_period.py
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_finance_information_market_vat_details.py
+-rw-r--r--   0 root         (0) root         (0)     2068 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_finance_information_sage_settings.py
+-rw-r--r--   0 root         (0) root         (0)     5555 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_intra_day_auction.py
+-rw-r--r--   0 root         (0) root         (0)     2990 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_invoice.py
+-rw-r--r--   0 root         (0) root         (0)     1061 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_invoice_action_type.py
+-rw-r--r--   0 root         (0) root         (0)     4006 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_invoice_batch.py
+-rw-r--r--   0 root         (0) root         (0)     7368 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_invoice_details.py
+-rw-r--r--   0 root         (0) root         (0)     2134 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_invoice_history.py
+-rw-r--r--   0 root         (0) root         (0)     2436 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_invoice_line_item.py
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_invoice_participant_details.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_invoice_status.py
+-rw-r--r--   0 root         (0) root         (0)     2146 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_invoice_summary.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_invoice_vat_rate.py
+-rw-r--r--   0 root         (0) root         (0)     6329 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_long_term_auction.py
+-rw-r--r--   0 root         (0) root         (0)     2333 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_long_term_auction_bid.py
+-rw-r--r--   0 root         (0) root         (0)     3236 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_long_term_auction_bid_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_long_term_auction_bid_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     4438 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_long_term_auction_results.py
+-rw-r--r--   0 root         (0) root         (0)     2772 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_long_term_auction_results_allocated_capacity_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2036 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_long_term_bidding_results.py
+-rw-r--r--   0 root         (0) root         (0)     3005 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_long_term_default_bid.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_long_term_offered_capacity.py
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_long_term_reserve_price.py
+-rw-r--r--   0 root         (0) root         (0)     2127 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_long_term_reserve_price_steps_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_manual_file_upload_api.py
+-rw-r--r--   0 root         (0) root         (0)     1991 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_manual_file_upload_request.py
+-rw-r--r--   0 root         (0) root         (0)      982 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_market.py
+-rw-r--r--   0 root         (0) root         (0)     2658 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_message.py
+-rw-r--r--   0 root         (0) root         (0)     3678 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_message_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_message_category.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_message_sender.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_message_severity.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_message_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_message_type.py
+-rw-r--r--   0 root         (0) root         (0)     1362 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_messages_api.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_metadata_api.py
+-rw-r--r--   0 root         (0) root         (0)     1884 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_mtu_period.py
+-rw-r--r--   0 root         (0) root         (0)      990 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_mtu_size.py
+-rw-r--r--   0 root         (0) root         (0)     2130 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_mtu_size_per_auction_product_type.py
+-rw-r--r--   0 root         (0) root         (0)     1966 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_mtu_size_per_timescale.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_nested_error.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_nomination_api.py
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_nomination_restriction_type.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_noticeboard_entry_type.py
+-rw-r--r--   0 root         (0) root         (0)     1140 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_noticeboard_entry_type_with_both.py
+-rw-r--r--   0 root         (0) root         (0)     1891 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_notification_preference.py
+-rw-r--r--   0 root         (0) root         (0)     2036 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_notification_preference_with_sms.py
+-rw-r--r--   0 root         (0) root         (0)     2003 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_ntc_overview_mtu_data.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_offered_capacity_setup.py
+-rw-r--r--   0 root         (0) root         (0)     2147 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_api.py
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_auth_method.py
+-rw-r--r--   0 root         (0) root         (0)     6103 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_contact.py
+-rw-r--r--   0 root         (0) root         (0)    11189 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_contact_information.py
+-rw-r--r--   0 root         (0) root         (0)     3633 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_document.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_document_api.py
+-rw-r--r--   0 root         (0) root         (0)     4658 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_document_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_document_file_type.py
+-rw-r--r--   0 root         (0) root         (0)     3268 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_document_options.py
+-rw-r--r--   0 root         (0) root         (0)     2671 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_document_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     1125 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_document_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_document_status.py
+-rw-r--r--   0 root         (0) root         (0)     2707 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_document_uploaded_by_user.py
+-rw-r--r--   0 root         (0) root         (0)     2304 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_document_uploaded_by_user_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     2034 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_document_user.py
+-rw-r--r--   0 root         (0) root         (0)     2014 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_file_settings.py
+-rw-r--r--   0 root         (0) root         (0)     3505 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_market_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_market_settings_gb_nomination_settings.py
+-rw-r--r--   0 root         (0) root         (0)     2325 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_market_settings_nl_nomination_settings.py
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_status.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_type.py
+-rw-r--r--   0 root         (0) root         (0)     6451 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_user.py
+-rw-r--r--   0 root         (0) root         (0)     7158 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_user_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_organisation_user_sort_by.py
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_other_party.py
+-rw-r--r--   0 root         (0) root         (0)     1874 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_participant.py
+-rw-r--r--   0 root         (0) root         (0)     2844 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_api.py
+-rw-r--r--   0 root         (0) root         (0)     2352 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_default_bids_and_nominations_data.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2023-07-11 11:17:49.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_finance_overview_data.py
+-rw-r--r--   0 root         (0) root         (0)     2762 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_finance_overview_invoice.py
+-rw-r--r--   0 root         (0) root         (0)     4166 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_interconnector_capacity_data.py
+-rw-r--r--   0 root         (0) root         (0)     3568 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_interconnector_capacity_data_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3000 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_interconnector_capacity_data_mtus_inner_values_inner.py
+-rw-r--r--   0 root         (0) root         (0)     4255 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_interconnector_capacity_graph_data.py
+-rw-r--r--   0 root         (0) root         (0)     3735 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_inner_netted_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_inner_values_inner.py
+-rw-r--r--   0 root         (0) root         (0)     5714 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_messages.py
+-rw-r--r--   0 root         (0) root         (0)     4190 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_netted_nominations_data.py
+-rw-r--r--   0 root         (0) root         (0)     3627 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_netted_nominations_data_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_netted_nominations_data_mtus_inner_aggregated_nominations_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2514 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_netted_nominations_data_mtus_inner_netted_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_next_auction.py
+-rw-r--r--   0 root         (0) root         (0)     7585 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_next_auctions_and_nomination_gates.py
+-rw-r--r--   0 root         (0) root         (0)     4722 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_transmission_rights_and_nominations_data.py
+-rw-r--r--   0 root         (0) root         (0)     4080 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3097 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_inner_values_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2876 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_inner_values_inner_nomination_restriction.py
+-rw-r--r--   0 root         (0) root         (0)     3907 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data.py
+-rw-r--r--   0 root         (0) root         (0)     3376 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2789 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_inner_values_inner.py
+-rw-r--r--   0 root         (0) root         (0)    14117 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_organisation_details.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_participant_overview_api.py
+-rw-r--r--   0 root         (0) root         (0)    13510 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_overview_data.py
+-rw-r--r--   0 root         (0) root         (0)    11325 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_overview_data_contact_information.py
+-rw-r--r--   0 root         (0) root         (0)     2271 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_overview_data_finance_overview.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_participant_overview_data_organisation_members.py
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_permission.py
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_platform_appearance.py
+-rw-r--r--   0 root         (0) root         (0)     9781 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_profile.py
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_profile_api.py
+-rw-r--r--   0 root         (0) root         (0)     6754 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_profile_details.py
+-rw-r--r--   0 root         (0) root         (0)     6669 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_profile_user.py
+-rw-r--r--   0 root         (0) root         (0)     2107 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_profile_user_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     4256 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_public_aggregated_nominations_overview_response.py
+-rw-r--r--   0 root         (0) root         (0)     3711 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_public_aggregated_nominations_overview_response_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2555 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_public_aggregated_nominations_overview_response_mtus_inner_values_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_public_allocated_auction_api.py
+-rw-r--r--   0 root         (0) root         (0)     3327 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_public_auction.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_public_auction_api.py
+-rw-r--r--   0 root         (0) root         (0)     4016 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_public_auction_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1097 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_public_auction_bid_status.py
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_public_auction_status.py
+-rw-r--r--   0 root         (0) root         (0)     5300 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_public_day_ahead_auction.py
+-rw-r--r--   0 root         (0) root         (0)     3087 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_public_day_ahead_or_intra_day_auction_mtu_results.py
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_public_day_ahead_or_intra_day_auction_mtu_results_bids_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3790 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_public_day_ahead_or_intra_day_auction_results.py
+-rw-r--r--   0 root         (0) root         (0)     5300 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_public_intra_day_auction.py
+-rw-r--r--   0 root         (0) root         (0)     5794 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_public_long_term_auction.py
+-rw-r--r--   0 root         (0) root         (0)     3693 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_public_long_term_auction_results.py
+-rw-r--r--   0 root         (0) root         (0)     1206 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_public_nominations_api.py
+-rw-r--r--   0 root         (0) root         (0)     2022 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_purchased_by_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     1988 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_reporting_api.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_reserve_price_publish_type.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_return_auction.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_sage_code.py
+-rw-r--r--   0 root         (0) root         (0)     5536 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_api.py
+-rw-r--r--   0 root         (0) root         (0)     2095 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_capacity_price_mtu.py
+-rw-r--r--   0 root         (0) root         (0)    11431 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3472 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_details.py
+-rw-r--r--   0 root         (0) root         (0)     3161 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_matching.py
+-rw-r--r--   0 root         (0) root         (0)     7558 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_response.py
+-rw-r--r--   0 root         (0) root         (0)     2627 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_response_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2998 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_options.py
+-rw-r--r--   0 root         (0) root         (0)     3096 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_response_options.py
+-rw-r--r--   0 root         (0) root         (0)     4631 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     2442 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     3122 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_options.py
+-rw-r--r--   0 root         (0) root         (0)     2585 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_options_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     8384 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_long_term_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_long_term_noticeboard_entry_details.py
+-rw-r--r--   0 root         (0) root         (0)     6775 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_long_term_noticeboard_entry_response.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_long_term_noticeboard_options.py
+-rw-r--r--   0 root         (0) root         (0)     2269 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_long_term_noticeboard_response_options.py
+-rw-r--r--   0 root         (0) root         (0)     2199 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_long_term_transfer_request_options.py
+-rw-r--r--   0 root         (0) root         (0)     3108 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_noticeboard_entry.py
+-rw-r--r--   0 root         (0) root         (0)     3926 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_noticeboard_entry_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_noticeboard_entry_status.py
+-rw-r--r--   0 root         (0) root         (0)     3890 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_return_request.py
+-rw-r--r--   0 root         (0) root         (0)     4718 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_return_request_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_return_request_status.py
+-rw-r--r--   0 root         (0) root         (0)     3940 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_transfer_request.py
+-rw-r--r--   0 root         (0) root         (0)     4780 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_transfer_request_batch.py
+-rw-r--r--   0 root         (0) root         (0)     1196 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_transfer_request_status.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_transfer_request_type.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_secondary_market_transfer_transmission_rights_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_settlement.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_settlement_item.py
+-rw-r--r--   0 root         (0) root         (0)     2636 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_settlement_per_source.py
+-rw-r--r--   0 root         (0) root         (0)     1082 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_settlement_source_type.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_settlement_sub_source_type.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_source_auction.py
+-rw-r--r--   0 root         (0) root         (0)     2104 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_source_auction_display_data.py
+-rw-r--r--   0 root         (0) root         (0)     1980 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_source_auction_result.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_submit_day_ahead_or_intra_day_bids_request.py
+-rw-r--r--   0 root         (0) root         (0)     3197 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_submit_day_ahead_or_intra_day_bids_request_bid_groups_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_submit_day_ahead_or_intra_day_bids_request_bid_groups_inner_bids_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2759 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_submit_long_term_bids_request.py
+-rw-r--r--   0 root         (0) root         (0)     2365 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_submit_long_term_bids_request_bids_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_submit_nominations_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     2455 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_submit_timescale_nominations_request.py
+-rw-r--r--   0 root         (0) root         (0)     1089 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_system_message_category.py
+-rw-r--r--   0 root         (0) root         (0)     1139 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_timescale_nomination_mtu_status.py
+-rw-r--r--   0 root         (0) root         (0)     2339 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_timescale_nomination_options.py
+-rw-r--r--   0 root         (0) root         (0)     2220 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_timescale_nomination_options_window_timing.py
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_timescale_nomination_status.py
+-rw-r--r--   0 root         (0) root         (0)     1103 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_timescale_nomination_type.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_timescale_nomination_window_status.py
+-rw-r--r--   0 root         (0) root         (0)     3328 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_timescale_nominations.py
+-rw-r--r--   0 root         (0) root         (0)     2552 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_timescale_nominations_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_timescale_nominations_mtus_inner_current_nomination.py
+-rw-r--r--   0 root         (0) root         (0)     1186 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_transmission_right_api.py
+-rw-r--r--   0 root         (0) root         (0)     4087 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_transmission_rights_overview.py
+-rw-r--r--   0 root         (0) root         (0)     3610 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_transmission_rights_overview_mtus_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2983 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_transmission_rights_overview_mtus_inner_values_inner.py
+-rw-r--r--   0 root         (0) root         (0)     2424 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_transmission_rights_overview_mtus_inner_values_inner_timescales_inner.py
+-rw-r--r--   0 root         (0) root         (0)     1878 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_uiosi_not_resold.py
+-rw-r--r--   0 root         (0) root         (0)     3364 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_uiosi_overview.py
+-rw-r--r--   0 root         (0) root         (0)     2881 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_uiosi_overview_per_mtu.py
+-rw-r--r--   0 root         (0) root         (0)     1937 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_uiosi_resold.py
+-rw-r--r--   0 root         (0) root         (0)     1887 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_unread_messages_response.py
+-rw-r--r--   0 root         (0) root         (0)     3945 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_update_day_ahead_or_intra_day_default_bid_request.py
+-rw-r--r--   0 root         (0) root         (0)     2705 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_update_default_nomination_request.py
+-rw-r--r--   0 root         (0) root         (0)     2733 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_update_long_term_default_bid_request.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_update_profile_details_request.py
+-rw-r--r--   0 root         (0) root         (0)     2038 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_update_user_request.py
+-rw-r--r--   0 root         (0) root         (0)     6660 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_user.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2023-07-11 11:17:52.000000 empire-platform-api-public-client-0.167.0/test/test_user_api.py
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_user_organisation.py
+-rw-r--r--   0 root         (0) root         (0)     4381 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_user_preferences.py
+-rw-r--r--   0 root         (0) root         (0)     3318 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_user_preferences_general_notifications.py
+-rw-r--r--   0 root         (0) root         (0)     2750 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_user_preferences_subscription_notifications.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_user_role.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_user_status.py
+-rw-r--r--   0 root         (0) root         (0)     1019 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_vat_rate_type.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_version.py
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-07-11 11:17:50.000000 empire-platform-api-public-client-0.167.0/test/test_zendesk_chat_token_response.py
```

### Comparing `empire-platform-api-public-client-0.166.0/PKG-INFO` & `empire-platform-api-public-client-0.167.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empire-platform-api-public-client
-Version: 0.166.0
+Version: 0.167.0
 Summary: Empire - Platform API
 Home-page: UNKNOWN
 Author: BritNed
 Author-email: britned.info@britned.com
 License: UNKNOWN
 Description:     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ &#x3D;&gt; kW (integers)   * _dates and local times_ &#x3D;&gt; System Time   * _currencies_ &#x3D;&gt; EUR   # noqa: E501
```

### Comparing `empire-platform-api-public-client-0.166.0/README.md` & `empire-platform-api-public-client-0.167.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
   * _capacity values_ => kW (integers)
   * _dates and local times_ => System Time
   * _currencies_ => EUR
 
 
 This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:
 
-- API version: 0.166.0
-- Package version: 0.166.0
+- API version: 0.167.0
+- Package version: 0.167.0
 - Build package: org.openapitools.codegen.languages.PythonNextgenClientCodegen
 For more information, please visit [https://www.britned.com](https://www.britned.com)
 
 ## Requirements.
 
 Python 3.7+
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/__init__.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # flake8: noqa
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-__version__ = "0.166.0"
+__version__ = "0.167.0"
 
 # import apis into sdk package
 from empire_platform_api_public_client.api.attachment_api import AttachmentApi
 from empire_platform_api_public_client.api.auction_api import AuctionApi
 from empire_platform_api_public_client.api.audit_log_api import AuditLogApi
 from empire_platform_api_public_client.api.bidding_configuration_api import BiddingConfigurationApi
 from empire_platform_api_public_client.api.buy_now_offers_api import BuyNowOffersApi
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/__init__.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/__init__.py`

 * *Files identical despite different names*

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/attachment_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/attachment_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/auction_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/auction_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/audit_log_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/audit_log_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/bidding_configuration_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/bidding_configuration_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/buy_now_offers_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/buy_now_offers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/default_bid_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/default_bid_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/default_nomination_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/default_nomination_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/finance_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/finance_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/finance_information_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/finance_information_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/manual_file_upload_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/manual_file_upload_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/messages_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/messages_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/metadata_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/nomination_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/nomination_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/organisation_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/organisation_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/organisation_document_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/organisation_document_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/participant_dashboard_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/participant_dashboard_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/participant_overview_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/participant_overview_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/profile_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/profile_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/public_allocated_auction_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/public_allocated_auction_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/public_auction_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/public_auction_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/public_nominations_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/public_nominations_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/reporting_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/reporting_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/secondary_market_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/secondary_market_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/transmission_right_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/transmission_right_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api/user_api.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api/user_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api_client.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -73,15 +73,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/0.166.0/python'
+        self.user_agent = 'OpenAPI-Generator/0.167.0/python'
         self.client_side_validation = configuration.client_side_validation
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/api_response.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/api_response.py`

 * *Files identical despite different names*

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/configuration.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -404,16 +404,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.166.0\n"\
-               "SDK Package Version: 0.166.0".\
+               "Version of the API: 0.167.0\n"\
+               "SDK Package Version: 0.167.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/exceptions.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/__init__.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/address.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_allocated_auction.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_allocated_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nomination_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nomination_type.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nominations.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nominations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nominations_mns_or_gb.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nominations_mns_or_gb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nominations_mns_or_gb_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nominations_mns_or_gb_mtus_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nominations_mtu_netted_nominations.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nominations_mtu_netted_nominations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nominations_mtu_value.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nominations_mtu_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nominations_nl.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nominations_nl.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nominations_nl_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nominations_nl_mtus_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/aggregated_nominations_nl_mtus_inner_eprogram_values.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/aggregated_nominations_nl_mtus_inner_eprogram_values.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/allocated_auction.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/allocated_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/allocated_auction_batch.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/allocated_auction_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/allocated_auction_sort_by.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/allocated_auction_sort_by.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/api_key.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/api_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/attachment.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/attachment.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_allocation_resolution.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_allocation_resolution.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_batch.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_bid_participant.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_bid_participant.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_bid_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_bid_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_bidding_configuration.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_bidding_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_bidding_mode.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/user_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,24 +18,25 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class AuctionBiddingMode(str, Enum):
+class UserStatus(str, Enum):
     """
-    AuctionBiddingMode
+    UserStatus
     """
 
     """
     allowed enum values
     """
-    OPEN = 'OPEN'
-    CLOSE = 'CLOSE'
+    ACTIVE = 'ACTIVE'
+    INVITED = 'INVITED'
+    SUSPENDED = 'SUSPENDED'
 
     @classmethod
-    def from_json(cls, json_str: str) -> AuctionBiddingMode:
-        """Create an instance of AuctionBiddingMode from a JSON string"""
-        return AuctionBiddingMode(json.loads(json_str))
+    def from_json(cls, json_str: str) -> UserStatus:
+        """Create an instance of UserStatus from a JSON string"""
+        return UserStatus(json.loads(json_str))
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_intra_day_product_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_intra_day_product_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_process_steps_absolute.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_process_steps_absolute.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_product_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_product_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_reduction_period.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_reduction_period.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_result_congestion_rent.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_result_congestion_rent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_result_participant.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_result_participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_sort_by.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_sort_by.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/auction_timescale.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/auction_timescale.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_api_key.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_api_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_batch.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_domain.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_domain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_payload.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_payload.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_sort_by.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/market.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,24 +18,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class AuditLogSortBy(str, Enum):
+class Market(str, Enum):
     """
-    AuditLogSortBy
+    Market
     """
 
     """
     allowed enum values
     """
-    CREATED_AT_ASC = 'CREATED_AT_ASC'
-    CREATED_AT_DESC = 'CREATED_AT_DESC'
+    GB = 'GB'
+    NL = 'NL'
 
     @classmethod
-    def from_json(cls, json_str: str) -> AuditLogSortBy:
-        """Create an instance of AuditLogSortBy from a JSON string"""
-        return AuditLogSortBy(json.loads(json_str))
+    def from_json(cls, json_str: str) -> Market:
+        """Create an instance of Market from a JSON string"""
+        return Market(json.loads(json_str))
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_status.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_user.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/audit_log_user_organisation.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_user_organisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/bid_value.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/bid_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/bidding_configuration.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/bidding_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/bidding_configuration_per_direction.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/bidding_configuration_per_direction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/bidding_configuration_secondary_market_notices.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/bidding_configuration_secondary_market_notices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/bidding_configuration_values_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/bidding_configuration_values_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/border_direction.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/border_direction.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/border_direction_with_both.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/border_direction_with_both.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/border_direction_with_both_and_none.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/border_direction_with_both_and_none.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/buy_now_day_ahead_offer_sort_by.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/buy_now_day_ahead_offer_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/buy_now_offer.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/buy_now_offer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/buy_now_offer_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/buy_now_offer_mtus_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/buy_now_offer_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/buy_now_offer_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_api_key_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_api_key_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request_bids_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request_bids_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request_bids_inner_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_day_ahead_or_intra_day_default_bid_request_bids_inner_mtus_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_default_nomination_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_default_nomination_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_long_term_default_bid_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_long_term_default_bid_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_organisation_document_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_organisation_document_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_noticeboard_response.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_noticeboard_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_transfer_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_transfer_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_transfer_request_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_secondary_market_day_ahead_or_intra_day_transfer_request_mtus_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_secondary_market_long_term_noticeboard_entry.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_secondary_market_long_term_noticeboard_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_secondary_market_long_term_noticeboard_response.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_secondary_market_long_term_noticeboard_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_secondary_market_long_term_transfer_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_secondary_market_long_term_transfer_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/create_secondary_market_return_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/create_secondary_market_return_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_api_key.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_api_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_default_bid.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_default_bid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_default_nomination.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_default_nomination.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_organisation_document.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_organisation_document.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_noticeboard_response.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_noticeboard_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_transfer_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_secondary_market_day_ahead_or_intra_day_transfer_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_secondary_market_long_term_noticeboard_entry.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_secondary_market_long_term_noticeboard_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_secondary_market_long_term_noticeboard_response.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_secondary_market_long_term_noticeboard_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_secondary_market_long_term_transfer_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_secondary_market_long_term_transfer_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/created_secondary_market_return_request_identifier.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/created_secondary_market_return_request_identifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/dashboard_next_nomination_gate.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/dashboard_next_nomination_gate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/dashboard_next_nomination_gate_window.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/dashboard_next_nomination_gate_window.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/dashboard_next_nomination_window_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/dashboard_next_nomination_window_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/date_period.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/date_period.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/date_time_period.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/date_time_period.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_auction.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_batch.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids_inner_value.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_bid_group_bids_inner_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu_results.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu_results.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu_results_bids_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_mtu_results_bids_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results_mtus_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results_mtus_inner_value.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_participant_results_mtus_inner_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_results.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_results_mtu.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_auction_results_mtu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_default_bid.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/day_ahead_or_intra_day_default_bid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_bid.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_bid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_bid_batch.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_bid_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_bid_options.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_bid_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_bid_sort_by.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_bid_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_bid_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_bid_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_nomination.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_nomination.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_nomination_batch.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_nomination_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_nomination_declaration_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_nomination_declaration_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_nomination_details.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_nomination_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_nomination_mtu.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_nomination_mtu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_nomination_options.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_nomination_options.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_nomination_sort_by.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_nomination_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/default_nomination_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/default_nomination_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/error_code.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/error_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/error_response.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/error_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/finance_information.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/finance_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/finance_information_bank_deposits_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/finance_information_bank_deposits_inner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/finance_information_letter_of_credits_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/finance_information_letter_of_credits_inner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/finance_information_lockable_amount.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/finance_information_lockable_amount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/finance_information_lockable_date.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/finance_information_lockable_date.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/finance_information_lockable_period.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/finance_information_lockable_period.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/finance_information_market_vat_details.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/finance_information_market_vat_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/finance_information_sage_settings.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/finance_information_sage_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/intra_day_auction.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/intra_day_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_action_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_action_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_batch.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_details.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_history.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_history.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_line_item.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_line_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_participant_details.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_participant_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_summary.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/invoice_vat_rate.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/invoice_vat_rate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_auction.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_auction_bid.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_auction_bid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_auction_bid_batch.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_auction_bid_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_auction_bid_sort_by.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_auction_bid_sort_by.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_auction_results.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_auction_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_auction_results_allocated_capacity_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_auction_results_allocated_capacity_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_bidding_results.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_bidding_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_default_bid.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_default_bid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_offered_capacity.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_offered_capacity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_reserve_price.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_reserve_price.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/long_term_reserve_price_steps_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/long_term_reserve_price_steps_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/manual_file_upload_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/manual_file_upload_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/market.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,24 +18,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class Market(str, Enum):
+class OrganisationDocumentStatus(str, Enum):
     """
-    Market
+    OrganisationDocumentStatus
     """
 
     """
     allowed enum values
     """
-    GB = 'GB'
-    NL = 'NL'
+    UPLOADED = 'UPLOADED'
+    DELETED = 'DELETED'
 
     @classmethod
-    def from_json(cls, json_str: str) -> Market:
-        """Create an instance of Market from a JSON string"""
-        return Market(json.loads(json_str))
+    def from_json(cls, json_str: str) -> OrganisationDocumentStatus:
+        """Create an instance of OrganisationDocumentStatus from a JSON string"""
+        return OrganisationDocumentStatus(json.loads(json_str))
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/message.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/message_batch.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/message_batch.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/message_category.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/message_category.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/message_sender.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/message_sender.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/message_severity.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/message_severity.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/message_sort_by.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/message_sort_by.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/message_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/message_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/mtu_period.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/mtu_period.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/mtu_size.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/mtu_size.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/mtu_size_per_auction_product_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/mtu_size_per_auction_product_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/mtu_size_per_timescale.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/mtu_size_per_timescale.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/nested_error.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/nested_error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/nomination_restriction_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/nomination_restriction_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/noticeboard_entry_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/noticeboard_entry_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/noticeboard_entry_type_with_both.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/noticeboard_entry_type_with_both.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/notification_preference.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/notification_preference.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/notification_preference_with_sms.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/notification_preference_with_sms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/ntc_overview_mtu_data.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/ntc_overview_mtu_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/offered_capacity_setup.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/offered_capacity_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_auth_method.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_auth_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_contact.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_contact.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_contact_information.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_contact_information.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_batch.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_file_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_file_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_options.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_organisation.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_organisation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_sort_by.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_status.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_document_status.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,37 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
-import json
-import pprint
-import re  # noqa: F401
-from aenum import Enum, no_arg
+import unittest
+import datetime
 
+import empire_platform_api_public_client
+from empire_platform_api_public_client.models.organisation_document_status import OrganisationDocumentStatus  # noqa: E501
+from empire_platform_api_public_client.rest import ApiException
 
+class TestOrganisationDocumentStatus(unittest.TestCase):
+    """OrganisationDocumentStatus unit test stubs"""
 
+    def setUp(self):
+        pass
 
+    def tearDown(self):
+        pass
 
-class OrganisationDocumentStatus(str, Enum):
-    """
-    OrganisationDocumentStatus
-    """
-
-    """
-    allowed enum values
-    """
-    UPLOADED = 'UPLOADED'
-    DELETED = 'DELETED'
-
-    @classmethod
-    def from_json(cls, json_str: str) -> OrganisationDocumentStatus:
-        """Create an instance of OrganisationDocumentStatus from a JSON string"""
-        return OrganisationDocumentStatus(json.loads(json_str))
-
+    def testOrganisationDocumentStatus(self):
+        """Test OrganisationDocumentStatus"""
+        # inst = OrganisationDocumentStatus()
 
+if __name__ == '__main__':
+    unittest.main()
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_uploaded_by_user.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_uploaded_by_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_uploaded_by_user_organisation.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_uploaded_by_user_organisation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_document_user.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_document_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_file_settings.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_file_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_market_settings.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_market_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_market_settings_gb_nomination_settings.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_market_settings_gb_nomination_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_market_settings_nl_nomination_settings.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_market_settings_nl_nomination_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_status.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_user.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_user_batch.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_user_batch.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/organisation_user_sort_by.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/organisation_user_sort_by.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/other_party.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/other_party.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_default_bids_and_nominations_data.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_default_bids_and_nominations_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_finance_overview_data.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_finance_overview_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_finance_overview_invoice.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_finance_overview_invoice.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data_mtus_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data_mtus_inner_values_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_data_mtus_inner_values_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_inner_netted_nominations.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_inner_netted_nominations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_inner_values_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_interconnector_capacity_graph_data_mtus_inner_values_inner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_messages.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_inner_aggregated_nominations_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_inner_aggregated_nominations_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_inner_netted_nominations.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_netted_nominations_data_mtus_inner_netted_nominations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_next_auction.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_next_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_next_auctions_and_nomination_gates.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_next_auctions_and_nomination_gates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_inner_values_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_inner_values_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_inner_values_inner_nomination_restriction.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_data_mtus_inner_values_inner_nomination_restriction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_inner_values_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_inner_values_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_organisation_details.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_organisation_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_overview_data.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_overview_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_overview_data_contact_information.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_overview_data_contact_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_overview_data_finance_overview.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_overview_data_finance_overview.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/participant_overview_data_organisation_members.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/participant_overview_data_organisation_members.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/permission.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/permission.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/platform_appearance.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/platform_appearance.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/profile.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/profile_details.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/profile_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/profile_user.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/profile_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/profile_user_organisation.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/profile_user_organisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus_inner_values_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_aggregated_nominations_overview_response_mtus_inner_values_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_auction.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_auction_batch.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_auction_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_auction_bid_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_auction_bid_status.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_auction_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_auction_status.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_day_ahead_auction.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_day_ahead_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_mtu_results.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_mtu_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_mtu_results_bids_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_mtu_results_bids_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_results.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_day_ahead_or_intra_day_auction_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_intra_day_auction.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_intra_day_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_long_term_auction.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_long_term_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/public_long_term_auction_results.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/public_long_term_auction_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/purchased_by_organisation.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/purchased_by_organisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/reserve_price_publish_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/reserve_price_publish_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/return_auction.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/return_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/sage_code.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/sage_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_capacity_price_mtu.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_capacity_price_mtu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_details.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_matching.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_matching.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_response.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_response_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_entry_response_mtus_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_options.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_response_options.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_noticeboard_response_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_mtus_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_options.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_options_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_day_ahead_or_intra_day_transfer_request_options_mtus_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry_details.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry_response.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_entry_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_options.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_response_options.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_long_term_noticeboard_response_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_long_term_transfer_request_options.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_long_term_transfer_request_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_noticeboard_entry.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_noticeboard_entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_noticeboard_entry_batch.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_noticeboard_entry_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_noticeboard_entry_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_noticeboard_entry_status.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_return_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_return_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_return_request_batch.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_return_request_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_return_request_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_return_request_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_transfer_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_transfer_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_transfer_request_batch.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_transfer_request_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_transfer_request_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_transfer_request_status.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_transfer_request_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_transfer_request_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/secondary_market_transfer_transmission_rights_mtu.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/secondary_market_transfer_transmission_rights_mtu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/settlement.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/settlement.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/settlement_item.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/settlement_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/settlement_per_source.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/settlement_per_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/settlement_source_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/settlement_source_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/settlement_sub_source_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/settlement_sub_source_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/source_auction.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/source_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/source_auction_display_data.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/source_auction_display_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/source_auction_result.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/source_auction_result.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic import BaseModel, Field, conlist
 from empire_platform_api_public_client.models.submit_day_ahead_or_intra_day_bids_request_bid_groups_inner import SubmitDayAheadOrIntraDayBidsRequestBidGroupsInner
 
 class SubmitDayAheadOrIntraDayBidsRequest(BaseModel):
     """
     SubmitDayAheadOrIntraDayBidsRequest
     """
-    participant_id: StrictStr = Field(..., alias="participantId", description="Unique identifier for the record in UUID4 format")
     bid_groups: conlist(SubmitDayAheadOrIntraDayBidsRequestBidGroupsInner) = Field(..., alias="bidGroups")
-    __properties = ["participantId", "bidGroups"]
+    __properties = ["bidGroups"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -70,12 +69,11 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return SubmitDayAheadOrIntraDayBidsRequest.parse_obj(obj)
 
         _obj = SubmitDayAheadOrIntraDayBidsRequest.parse_obj({
-            "participant_id": obj.get("participantId"),
             "bid_groups": [SubmitDayAheadOrIntraDayBidsRequestBidGroupsInner.from_dict(_item) for _item in obj.get("bidGroups")] if obj.get("bidGroups") is not None else None
         })
         return _obj
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request_bid_groups_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request_bid_groups_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request_bid_groups_inner_bids_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/submit_day_ahead_or_intra_day_bids_request_bid_groups_inner_bids_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/submit_long_term_bids_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/submit_long_term_bids_request.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 from __future__ import annotations
 import pprint
 import re  # noqa: F401
 import json
 
 
 from typing import List
-from pydantic import BaseModel, Field, StrictStr, conlist
+from pydantic import BaseModel, Field, conlist
 from empire_platform_api_public_client.models.submit_long_term_bids_request_bids_inner import SubmitLongTermBidsRequestBidsInner
 
 class SubmitLongTermBidsRequest(BaseModel):
     """
     SubmitLongTermBidsRequest
     """
-    participant_id: StrictStr = Field(..., alias="participantId", description="Unique identifier for the record in UUID4 format")
     bids: conlist(SubmitLongTermBidsRequestBidsInner) = Field(...)
-    __properties = ["participantId", "bids"]
+    __properties = ["bids"]
 
     class Config:
         """Pydantic configuration"""
         allow_population_by_field_name = True
         validate_assignment = True
 
     def to_str(self) -> str:
@@ -70,12 +69,11 @@
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return SubmitLongTermBidsRequest.parse_obj(obj)
 
         _obj = SubmitLongTermBidsRequest.parse_obj({
-            "participant_id": obj.get("participantId"),
             "bids": [SubmitLongTermBidsRequestBidsInner.from_dict(_item) for _item in obj.get("bids")] if obj.get("bids") is not None else None
         })
         return _obj
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/submit_long_term_bids_request_bids_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/submit_long_term_bids_request_bids_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/submit_nominations_mtu.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/submit_nominations_mtu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/submit_timescale_nominations_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/submit_timescale_nominations_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/system_message_category.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/system_message_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nomination_mtu_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nomination_mtu_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nomination_options.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nomination_options.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nomination_options_window_timing.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nomination_options_window_timing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nomination_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nomination_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nomination_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nomination_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nomination_window_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nomination_window_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nominations.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nominations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nominations_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nominations_mtus_inner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -22,15 +22,15 @@
 from typing import Optional
 from pydantic import BaseModel, Field, StrictInt
 from empire_platform_api_public_client.models.timescale_nomination_mtu_status import TimescaleNominationMtuStatus
 from empire_platform_api_public_client.models.timescale_nominations_mtus_inner_current_nomination import TimescaleNominationsMtusInnerCurrentNomination
 
 class TimescaleNominationsMtusInner(BaseModel):
     """
-    * `totalTrs` - Total value of Transmission Rights in kilowatts * `currentNomination.value` - Current value of Nominations in kilowatts * `notNominatedTrs` - Difference between total TRs and currentNomination.value 
+    * `mtuStatus`   - LOCKED => if either of the following cases are true for the MTU:     - the MTU nomination window for the selected timescale is closed     - the MTU was curtailed     - every MTU is by definition LOCKED if       - the specified Participant has `ableToNominate = FALSE` AND       - does not have an `onBehalfParticipantId` specified       - **in eihter markets**   - EDITABLE => if either of the following cases are true for the MTU:     - MTU nom window for the selected timescale is either not yet open or currently open     - There was no curtailment for the MTU   - NO_TR => if either of the following cases are true for the MTU:     - the user has no TR for the specific MTU, therefore there is nothing to nominate * `totalTrs` - Total value of Transmission Rights in kilowatts * `currentNomination.value` - Current value of Nominations in kilowatts * `notNominatedTrs` - Difference between total TRs and currentNomination.value 
     """
     mtu: datetime = Field(..., description="The first moment (inclusive) of an MTU period  - theoretically can be sent and received with any zone offset (until it marks the desired **absolute MTU start point** on the timeline) - in practice it is advised to transfer it in UTC timezone (with Z offset, \"Zulu time\") - ISO 8601 compliant string in `yyyy-mm-ddThh:mm:ss.SSSZ` format - only with `XX:00:00`, `XX:15:00`, `XX:30:00` and `XX:45:00` time parts are valid values (depending on MTU size) ")
     mtu_status: TimescaleNominationMtuStatus = Field(..., alias="mtuStatus")
     total_trs: StrictInt = Field(..., alias="totalTrs", description="Capacity value in kilowatts (kW) - the required system precision allows for handling capacity values as integers")
     current_nomination: Optional[TimescaleNominationsMtusInnerCurrentNomination] = Field(None, alias="currentNomination")
     not_nominated_trs: StrictInt = Field(..., alias="notNominatedTrs", description="Capacity value in kilowatts (kW) - the required system precision allows for handling capacity values as integers")
     __properties = ["mtu", "mtuStatus", "totalTrs", "currentNomination", "notNominatedTrs"]
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/timescale_nominations_mtus_inner_current_nomination.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/timescale_nominations_mtus_inner_current_nomination.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/transmission_rights_overview.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/transmission_rights_overview.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/transmission_rights_overview_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/transmission_rights_overview_mtus_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/transmission_rights_overview_mtus_inner_values_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/transmission_rights_overview_mtus_inner_values_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/transmission_rights_overview_mtus_inner_values_inner_timescales_inner.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/transmission_rights_overview_mtus_inner_values_inner_timescales_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/uiosi_not_resold.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/uiosi_not_resold.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/uiosi_overview.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/uiosi_overview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/uiosi_overview_per_mtu.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/uiosi_overview_per_mtu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/uiosi_resold.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/uiosi_resold.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/unread_messages_response.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/unread_messages_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/update_day_ahead_or_intra_day_default_bid_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/update_day_ahead_or_intra_day_default_bid_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/update_default_nomination_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/update_default_nomination_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/update_long_term_default_bid_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/update_long_term_default_bid_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/update_profile_details_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/update_profile_details_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/update_user_request.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/update_user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/user.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/user_organisation.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/user_organisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/user_preferences.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/user_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/user_preferences_general_notifications.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/user_preferences_general_notifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/user_preferences_subscription_notifications.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/user_preferences_subscription_notifications.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/user_role.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/user_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/user_status.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/audit_log_sort_by.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,25 +18,24 @@
 import re  # noqa: F401
 from aenum import Enum, no_arg
 
 
 
 
 
-class UserStatus(str, Enum):
+class AuditLogSortBy(str, Enum):
     """
-    UserStatus
+    AuditLogSortBy
     """
 
     """
     allowed enum values
     """
-    ACTIVE = 'ACTIVE'
-    INVITED = 'INVITED'
-    SUSPENDED = 'SUSPENDED'
+    CREATED_AT_ASC = 'CREATED_AT_ASC'
+    CREATED_AT_DESC = 'CREATED_AT_DESC'
 
     @classmethod
-    def from_json(cls, json_str: str) -> UserStatus:
-        """Create an instance of UserStatus from a JSON string"""
-        return UserStatus(json.loads(json_str))
+    def from_json(cls, json_str: str) -> AuditLogSortBy:
+        """Create an instance of AuditLogSortBy from a JSON string"""
+        return AuditLogSortBy(json.loads(json_str))
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/vat_rate_type.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/vat_rate_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/version.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/models/zendesk_chat_token_response.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/models/zendesk_chat_token_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client/rest.py` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client.egg-info/PKG-INFO` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empire-platform-api-public-client
-Version: 0.166.0
+Version: 0.167.0
 Summary: Empire - Platform API
 Home-page: UNKNOWN
 Author: BritNed
 Author-email: britned.info@britned.com
 License: UNKNOWN
 Description:     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ &#x3D;&gt; kW (integers)   * _dates and local times_ &#x3D;&gt; System Time   * _currencies_ &#x3D;&gt; EUR   # noqa: E501
```

### Comparing `empire-platform-api-public-client-0.166.0/empire_platform_api_public_client.egg-info/SOURCES.txt` & `empire-platform-api-public-client-0.167.0/empire_platform_api_public_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `empire-platform-api-public-client-0.166.0/setup.py` & `empire-platform-api-public-client-0.167.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -18,15 +18,15 @@
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 NAME = "empire-platform-api-public-client"
-VERSION = "0.166.0"
+VERSION = "0.167.0"
 PYTHON_REQUIRES = ">=3.7"
 REQUIRES = [
     "urllib3 >= 1.25.3",
     "python-dateutil",
     "pydantic >= 1.10.5, < 2",
     "aenum"
 ]
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_address.py` & `empire-platform-api-public-client-0.167.0/test/test_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_aggregated_allocated_auction.py` & `empire-platform-api-public-client-0.167.0/test/test_aggregated_allocated_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_aggregated_nomination_type.py` & `empire-platform-api-public-client-0.167.0/test/test_aggregated_nomination_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_aggregated_nominations.py` & `empire-platform-api-public-client-0.167.0/test/test_aggregated_nominations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_aggregated_nominations_mns_or_gb.py` & `empire-platform-api-public-client-0.167.0/test/test_aggregated_nominations_mns_or_gb.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_aggregated_nominations_mns_or_gb_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_aggregated_nominations_mns_or_gb_mtus_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_aggregated_nominations_mtu_netted_nominations.py` & `empire-platform-api-public-client-0.167.0/test/test_aggregated_nominations_mtu_netted_nominations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_aggregated_nominations_mtu_value.py` & `empire-platform-api-public-client-0.167.0/test/test_aggregated_nominations_mtu_value.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_aggregated_nominations_nl.py` & `empire-platform-api-public-client-0.167.0/test/test_aggregated_nominations_nl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_aggregated_nominations_nl_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_aggregated_nominations_nl_mtus_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_aggregated_nominations_nl_mtus_inner_eprogram_values.py` & `empire-platform-api-public-client-0.167.0/test/test_aggregated_nominations_nl_mtus_inner_eprogram_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_allocated_auction.py` & `empire-platform-api-public-client-0.167.0/test/test_allocated_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_allocated_auction_batch.py` & `empire-platform-api-public-client-0.167.0/test/test_allocated_auction_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_allocated_auction_sort_by.py` & `empire-platform-api-public-client-0.167.0/test/test_allocated_auction_sort_by.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_api_key.py` & `empire-platform-api-public-client-0.167.0/test/test_api_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_attachment.py` & `empire-platform-api-public-client-0.167.0/test/test_attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_attachment_api.py` & `empire-platform-api-public-client-0.167.0/test/test_attachment_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_auction.py` & `empire-platform-api-public-client-0.167.0/test/test_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_auction_allocation_resolution.py` & `empire-platform-api-public-client-0.167.0/test/test_auction_allocation_resolution.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_auction_api.py` & `empire-platform-api-public-client-0.167.0/test/test_auction_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_auction_batch.py` & `empire-platform-api-public-client-0.167.0/test/test_auction_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_auction_bid_participant.py` & `empire-platform-api-public-client-0.167.0/test/test_auction_bid_participant.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_auction_bid_status.py` & `empire-platform-api-public-client-0.167.0/test/test_auction_bid_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_auction_bidding_configuration.py` & `empire-platform-api-public-client-0.167.0/test/test_auction_bidding_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_auction_bidding_mode.py` & `empire-platform-api-public-client-0.167.0/test/test_auction_bidding_mode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_auction_intra_day_product_type.py` & `empire-platform-api-public-client-0.167.0/test/test_auction_intra_day_product_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_auction_process_steps_absolute.py` & `empire-platform-api-public-client-0.167.0/test/test_auction_process_steps_absolute.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_auction_product_type.py` & `empire-platform-api-public-client-0.167.0/test/test_auction_product_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_auction_reduction_period.py` & `empire-platform-api-public-client-0.167.0/test/test_auction_reduction_period.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_auction_result_congestion_rent.py` & `empire-platform-api-public-client-0.167.0/test/test_auction_result_congestion_rent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_auction_result_participant.py` & `empire-platform-api-public-client-0.167.0/test/test_auction_result_participant.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_auction_sort_by.py` & `empire-platform-api-public-client-0.167.0/test/test_auction_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_auction_status.py` & `empire-platform-api-public-client-0.167.0/test/test_auction_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_auction_timescale.py` & `empire-platform-api-public-client-0.167.0/test/test_auction_timescale.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_audit_log.py` & `empire-platform-api-public-client-0.167.0/test/test_audit_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_audit_log_api.py` & `empire-platform-api-public-client-0.167.0/test/test_audit_log_api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_audit_log_api_key.py` & `empire-platform-api-public-client-0.167.0/test/test_audit_log_api_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_audit_log_batch.py` & `empire-platform-api-public-client-0.167.0/test/test_audit_log_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_audit_log_domain.py` & `empire-platform-api-public-client-0.167.0/test/test_audit_log_domain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_audit_log_payload.py` & `empire-platform-api-public-client-0.167.0/test/test_audit_log_payload.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_audit_log_sort_by.py` & `empire-platform-api-public-client-0.167.0/test/test_audit_log_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_audit_log_status.py` & `empire-platform-api-public-client-0.167.0/test/test_audit_log_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_audit_log_type.py` & `empire-platform-api-public-client-0.167.0/test/test_audit_log_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_audit_log_user.py` & `empire-platform-api-public-client-0.167.0/test/test_audit_log_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_audit_log_user_organisation.py` & `empire-platform-api-public-client-0.167.0/test/test_audit_log_user_organisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_bid_value.py` & `empire-platform-api-public-client-0.167.0/test/test_bid_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_bidding_configuration.py` & `empire-platform-api-public-client-0.167.0/test/test_bidding_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_bidding_configuration_api.py` & `empire-platform-api-public-client-0.167.0/test/test_bidding_configuration_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_bidding_configuration_per_direction.py` & `empire-platform-api-public-client-0.167.0/test/test_bidding_configuration_per_direction.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_bidding_configuration_secondary_market_notices.py` & `empire-platform-api-public-client-0.167.0/test/test_bidding_configuration_secondary_market_notices.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_bidding_configuration_values_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_bidding_configuration_values_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_border_direction.py` & `empire-platform-api-public-client-0.167.0/test/test_border_direction.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_border_direction_with_both.py` & `empire-platform-api-public-client-0.167.0/test/test_border_direction_with_both.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_border_direction_with_both_and_none.py` & `empire-platform-api-public-client-0.167.0/test/test_border_direction_with_both_and_none.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_buy_now_day_ahead_offer_sort_by.py` & `empire-platform-api-public-client-0.167.0/test/test_buy_now_day_ahead_offer_sort_by.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_buy_now_offer.py` & `empire-platform-api-public-client-0.167.0/test/test_buy_now_offer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_buy_now_offer_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_buy_now_offer_mtus_inner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_buy_now_offer_status.py` & `empire-platform-api-public-client-0.167.0/test/test_buy_now_offer_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_buy_now_offers_api.py` & `empire-platform-api-public-client-0.167.0/test/test_buy_now_offers_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_create_api_key_request.py` & `empire-platform-api-public-client-0.167.0/test/test_create_api_key_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_create_day_ahead_or_intra_day_default_bid_request.py` & `empire-platform-api-public-client-0.167.0/test/test_create_day_ahead_or_intra_day_default_bid_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_create_day_ahead_or_intra_day_default_bid_request_bids_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_create_day_ahead_or_intra_day_default_bid_request_bids_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_create_day_ahead_or_intra_day_default_bid_request_bids_inner_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_create_day_ahead_or_intra_day_default_bid_request_bids_inner_mtus_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_create_default_nomination_request.py` & `empire-platform-api-public-client-0.167.0/test/test_create_default_nomination_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_create_long_term_default_bid_request.py` & `empire-platform-api-public-client-0.167.0/test/test_create_long_term_default_bid_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_create_organisation_document_request.py` & `empire-platform-api-public-client-0.167.0/test/test_create_organisation_document_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_create_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py` & `empire-platform-api-public-client-0.167.0/test/test_create_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_create_secondary_market_day_ahead_or_intra_day_noticeboard_response.py` & `empire-platform-api-public-client-0.167.0/test/test_create_secondary_market_day_ahead_or_intra_day_noticeboard_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_create_secondary_market_day_ahead_or_intra_day_transfer_request.py` & `empire-platform-api-public-client-0.167.0/test/test_create_secondary_market_day_ahead_or_intra_day_transfer_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_create_secondary_market_day_ahead_or_intra_day_transfer_request_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_create_secondary_market_day_ahead_or_intra_day_transfer_request_mtus_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_create_secondary_market_long_term_noticeboard_entry.py` & `empire-platform-api-public-client-0.167.0/test/test_create_secondary_market_long_term_noticeboard_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_create_secondary_market_long_term_noticeboard_response.py` & `empire-platform-api-public-client-0.167.0/test/test_create_secondary_market_long_term_noticeboard_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_create_secondary_market_long_term_transfer_request.py` & `empire-platform-api-public-client-0.167.0/test/test_create_secondary_market_long_term_transfer_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_create_secondary_market_return_request.py` & `empire-platform-api-public-client-0.167.0/test/test_create_secondary_market_return_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_created_api_key.py` & `empire-platform-api-public-client-0.167.0/test/test_created_api_key.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_created_default_bid.py` & `empire-platform-api-public-client-0.167.0/test/test_created_default_bid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_created_default_nomination.py` & `empire-platform-api-public-client-0.167.0/test/test_created_default_nomination.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_created_organisation_document.py` & `empire-platform-api-public-client-0.167.0/test/test_created_organisation_document.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_created_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py` & `empire-platform-api-public-client-0.167.0/test/test_created_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_created_secondary_market_day_ahead_or_intra_day_noticeboard_response.py` & `empire-platform-api-public-client-0.167.0/test/test_created_secondary_market_day_ahead_or_intra_day_noticeboard_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_created_secondary_market_day_ahead_or_intra_day_transfer_request.py` & `empire-platform-api-public-client-0.167.0/test/test_created_secondary_market_day_ahead_or_intra_day_transfer_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_created_secondary_market_long_term_noticeboard_entry.py` & `empire-platform-api-public-client-0.167.0/test/test_created_secondary_market_long_term_noticeboard_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_created_secondary_market_long_term_noticeboard_response.py` & `empire-platform-api-public-client-0.167.0/test/test_created_secondary_market_long_term_noticeboard_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_created_secondary_market_long_term_transfer_request.py` & `empire-platform-api-public-client-0.167.0/test/test_created_secondary_market_long_term_transfer_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_created_secondary_market_return_request_identifier.py` & `empire-platform-api-public-client-0.167.0/test/test_created_secondary_market_return_request_identifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_dashboard_next_nomination_gate.py` & `empire-platform-api-public-client-0.167.0/test/test_dashboard_next_nomination_gate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_dashboard_next_nomination_gate_window.py` & `empire-platform-api-public-client-0.167.0/test/test_dashboard_next_nomination_gate_window.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_dashboard_next_nomination_window_status.py` & `empire-platform-api-public-client-0.167.0/test/test_dashboard_next_nomination_window_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_date_period.py` & `empire-platform-api-public-client-0.167.0/test/test_date_period.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_date_time_period.py` & `empire-platform-api-public-client-0.167.0/test/test_date_time_period.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_day_ahead_auction.py` & `empire-platform-api-public-client-0.167.0/test/test_day_ahead_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_bid_group.py` & `empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_bid_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_bid_group_batch.py` & `empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_bid_group_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_bid_group_bids_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_bid_group_bids_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_bid_group_bids_inner_value.py` & `empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_bid_group_bids_inner_value.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_mtu.py` & `empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_mtu.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_mtu_results.py` & `empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_mtu_results.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_mtu_results_bids_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_mtu_results_bids_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_participant_results.py` & `empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_participant_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_participant_results_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_participant_results_mtus_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_participant_results_mtus_inner_value.py` & `empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_participant_results_mtus_inner_value.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_results.py` & `empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_auction_results_mtu.py` & `empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_auction_results_mtu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_day_ahead_or_intra_day_default_bid.py` & `empire-platform-api-public-client-0.167.0/test/test_day_ahead_or_intra_day_default_bid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_default_bid.py` & `empire-platform-api-public-client-0.167.0/test/test_default_bid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_default_bid_api.py` & `empire-platform-api-public-client-0.167.0/test/test_default_bid_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_default_bid_batch.py` & `empire-platform-api-public-client-0.167.0/test/test_default_bid_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_default_bid_options.py` & `empire-platform-api-public-client-0.167.0/test/test_default_bid_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_default_bid_sort_by.py` & `empire-platform-api-public-client-0.167.0/test/test_default_bid_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_default_bid_status.py` & `empire-platform-api-public-client-0.167.0/test/test_default_bid_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_default_nomination.py` & `empire-platform-api-public-client-0.167.0/test/test_default_nomination.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_default_nomination_api.py` & `empire-platform-api-public-client-0.167.0/test/test_default_nomination_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_default_nomination_batch.py` & `empire-platform-api-public-client-0.167.0/test/test_default_nomination_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_default_nomination_declaration_type.py` & `empire-platform-api-public-client-0.167.0/test/test_default_nomination_declaration_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_default_nomination_details.py` & `empire-platform-api-public-client-0.167.0/test/test_default_nomination_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_default_nomination_mtu.py` & `empire-platform-api-public-client-0.167.0/test/test_default_nomination_mtu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_default_nomination_options.py` & `empire-platform-api-public-client-0.167.0/test/test_default_nomination_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_default_nomination_sort_by.py` & `empire-platform-api-public-client-0.167.0/test/test_default_nomination_sort_by.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_default_nomination_status.py` & `empire-platform-api-public-client-0.167.0/test/test_default_nomination_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_error_code.py` & `empire-platform-api-public-client-0.167.0/test/test_error_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_error_response.py` & `empire-platform-api-public-client-0.167.0/test/test_error_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_finance_api.py` & `empire-platform-api-public-client-0.167.0/test/test_finance_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_finance_information.py` & `empire-platform-api-public-client-0.167.0/test/test_finance_information.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_finance_information_api.py` & `empire-platform-api-public-client-0.167.0/test/test_finance_information_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_finance_information_bank_deposits_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_finance_information_bank_deposits_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_finance_information_letter_of_credits_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_finance_information_letter_of_credits_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_finance_information_lockable_amount.py` & `empire-platform-api-public-client-0.167.0/test/test_finance_information_lockable_amount.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_finance_information_lockable_date.py` & `empire-platform-api-public-client-0.167.0/test/test_finance_information_lockable_date.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_finance_information_lockable_period.py` & `empire-platform-api-public-client-0.167.0/test/test_finance_information_lockable_period.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_finance_information_market_vat_details.py` & `empire-platform-api-public-client-0.167.0/test/test_finance_information_market_vat_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_finance_information_sage_settings.py` & `empire-platform-api-public-client-0.167.0/test/test_finance_information_sage_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_intra_day_auction.py` & `empire-platform-api-public-client-0.167.0/test/test_intra_day_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_invoice.py` & `empire-platform-api-public-client-0.167.0/test/test_invoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_invoice_action_type.py` & `empire-platform-api-public-client-0.167.0/test/test_invoice_action_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_invoice_batch.py` & `empire-platform-api-public-client-0.167.0/test/test_invoice_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_invoice_details.py` & `empire-platform-api-public-client-0.167.0/test/test_invoice_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_invoice_history.py` & `empire-platform-api-public-client-0.167.0/test/test_invoice_history.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_invoice_line_item.py` & `empire-platform-api-public-client-0.167.0/test/test_invoice_line_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_invoice_participant_details.py` & `empire-platform-api-public-client-0.167.0/test/test_invoice_participant_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_invoice_status.py` & `empire-platform-api-public-client-0.167.0/test/test_market.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
 import datetime
 
 import empire_platform_api_public_client
-from empire_platform_api_public_client.models.invoice_status import InvoiceStatus  # noqa: E501
+from empire_platform_api_public_client.models.market import Market  # noqa: E501
 from empire_platform_api_public_client.rest import ApiException
 
-class TestInvoiceStatus(unittest.TestCase):
-    """InvoiceStatus unit test stubs"""
+class TestMarket(unittest.TestCase):
+    """Market unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testInvoiceStatus(self):
-        """Test InvoiceStatus"""
-        # inst = InvoiceStatus()
+    def testMarket(self):
+        """Test Market"""
+        # inst = Market()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_invoice_summary.py` & `empire-platform-api-public-client-0.167.0/test/test_invoice_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_invoice_vat_rate.py` & `empire-platform-api-public-client-0.167.0/test/test_invoice_vat_rate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_long_term_auction.py` & `empire-platform-api-public-client-0.167.0/test/test_long_term_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_long_term_auction_bid.py` & `empire-platform-api-public-client-0.167.0/test/test_long_term_auction_bid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_long_term_auction_bid_batch.py` & `empire-platform-api-public-client-0.167.0/test/test_long_term_auction_bid_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_long_term_auction_bid_sort_by.py` & `empire-platform-api-public-client-0.167.0/test/test_long_term_auction_bid_sort_by.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_long_term_auction_results.py` & `empire-platform-api-public-client-0.167.0/test/test_long_term_auction_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_long_term_auction_results_allocated_capacity_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_long_term_auction_results_allocated_capacity_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_long_term_bidding_results.py` & `empire-platform-api-public-client-0.167.0/test/test_long_term_bidding_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_long_term_default_bid.py` & `empire-platform-api-public-client-0.167.0/test/test_long_term_default_bid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_long_term_offered_capacity.py` & `empire-platform-api-public-client-0.167.0/test/test_long_term_offered_capacity.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_long_term_reserve_price.py` & `empire-platform-api-public-client-0.167.0/test/test_long_term_reserve_price.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_long_term_reserve_price_steps_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_long_term_reserve_price_steps_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_manual_file_upload_api.py` & `empire-platform-api-public-client-0.167.0/test/test_manual_file_upload_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_manual_file_upload_request.py` & `empire-platform-api-public-client-0.167.0/test/test_manual_file_upload_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_market.py` & `empire-platform-api-public-client-0.167.0/test/test_permission.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
 import datetime
 
 import empire_platform_api_public_client
-from empire_platform_api_public_client.models.market import Market  # noqa: E501
+from empire_platform_api_public_client.models.permission import Permission  # noqa: E501
 from empire_platform_api_public_client.rest import ApiException
 
-class TestMarket(unittest.TestCase):
-    """Market unit test stubs"""
+class TestPermission(unittest.TestCase):
+    """Permission unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMarket(self):
-        """Test Market"""
-        # inst = Market()
+    def testPermission(self):
+        """Test Permission"""
+        # inst = Permission()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_message.py` & `empire-platform-api-public-client-0.167.0/test/test_message.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_message_batch.py` & `empire-platform-api-public-client-0.167.0/test/test_message_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_message_category.py` & `empire-platform-api-public-client-0.167.0/test/test_message_category.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_message_sender.py` & `empire-platform-api-public-client-0.167.0/test/test_message_sender.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_message_severity.py` & `empire-platform-api-public-client-0.167.0/test/test_message_severity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_message_sort_by.py` & `empire-platform-api-public-client-0.167.0/test/test_message_sort_by.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_message_type.py` & `empire-platform-api-public-client-0.167.0/test/test_message_type.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_messages_api.py` & `empire-platform-api-public-client-0.167.0/test/test_messages_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_metadata_api.py` & `empire-platform-api-public-client-0.167.0/test/test_metadata_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_mtu_period.py` & `empire-platform-api-public-client-0.167.0/test/test_mtu_period.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_mtu_size.py` & `empire-platform-api-public-client-0.167.0/test/test_mtu_size.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_mtu_size_per_auction_product_type.py` & `empire-platform-api-public-client-0.167.0/test/test_mtu_size_per_auction_product_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_mtu_size_per_timescale.py` & `empire-platform-api-public-client-0.167.0/test/test_mtu_size_per_timescale.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_nested_error.py` & `empire-platform-api-public-client-0.167.0/test/test_nested_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_nomination_api.py` & `empire-platform-api-public-client-0.167.0/test/test_nomination_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_nomination_restriction_type.py` & `empire-platform-api-public-client-0.167.0/test/test_nomination_restriction_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_noticeboard_entry_type.py` & `empire-platform-api-public-client-0.167.0/test/test_noticeboard_entry_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_noticeboard_entry_type_with_both.py` & `empire-platform-api-public-client-0.167.0/test/test_noticeboard_entry_type_with_both.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_notification_preference.py` & `empire-platform-api-public-client-0.167.0/test/test_notification_preference.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_notification_preference_with_sms.py` & `empire-platform-api-public-client-0.167.0/test/test_notification_preference_with_sms.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_ntc_overview_mtu_data.py` & `empire-platform-api-public-client-0.167.0/test/test_ntc_overview_mtu_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_offered_capacity_setup.py` & `empire-platform-api-public-client-0.167.0/test/test_offered_capacity_setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_api.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_auth_method.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_auth_method.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_contact.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_contact.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_contact_information.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_contact_information.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_document.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_document_api.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_document_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_document_batch.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_document_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_document_file_type.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_document_file_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_document_options.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_document_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_document_organisation.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_document_organisation.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_document_sort_by.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_document_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_document_status.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_transfer_request_status.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
 import datetime
 
 import empire_platform_api_public_client
-from empire_platform_api_public_client.models.organisation_document_status import OrganisationDocumentStatus  # noqa: E501
+from empire_platform_api_public_client.models.secondary_market_transfer_request_status import SecondaryMarketTransferRequestStatus  # noqa: E501
 from empire_platform_api_public_client.rest import ApiException
 
-class TestOrganisationDocumentStatus(unittest.TestCase):
-    """OrganisationDocumentStatus unit test stubs"""
+class TestSecondaryMarketTransferRequestStatus(unittest.TestCase):
+    """SecondaryMarketTransferRequestStatus unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testOrganisationDocumentStatus(self):
-        """Test OrganisationDocumentStatus"""
-        # inst = OrganisationDocumentStatus()
+    def testSecondaryMarketTransferRequestStatus(self):
+        """Test SecondaryMarketTransferRequestStatus"""
+        # inst = SecondaryMarketTransferRequestStatus()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_document_uploaded_by_user.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_document_uploaded_by_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_document_uploaded_by_user_organisation.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_document_uploaded_by_user_organisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_document_user.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_document_user.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_file_settings.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_file_settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_market_settings.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_market_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_market_settings_gb_nomination_settings.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_market_settings_gb_nomination_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_market_settings_nl_nomination_settings.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_market_settings_nl_nomination_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_status.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_type.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_user.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_user_batch.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_user_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_organisation_user_sort_by.py` & `empire-platform-api-public-client-0.167.0/test/test_organisation_user_sort_by.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_other_party.py` & `empire-platform-api-public-client-0.167.0/test/test_other_party.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant.py` & `empire-platform-api-public-client-0.167.0/test/test_participant.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_api.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_default_bids_and_nominations_data.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_default_bids_and_nominations_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_finance_overview_data.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_finance_overview_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_finance_overview_invoice.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_finance_overview_invoice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_interconnector_capacity_data.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_interconnector_capacity_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_interconnector_capacity_data_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_interconnector_capacity_data_mtus_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_interconnector_capacity_data_mtus_inner_values_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_interconnector_capacity_data_mtus_inner_values_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_interconnector_capacity_graph_data.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_interconnector_capacity_graph_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_inner_netted_nominations.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_inner_netted_nominations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_inner_values_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_interconnector_capacity_graph_data_mtus_inner_values_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_messages.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_messages.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_netted_nominations_data.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_netted_nominations_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_netted_nominations_data_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_netted_nominations_data_mtus_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_netted_nominations_data_mtus_inner_aggregated_nominations_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_netted_nominations_data_mtus_inner_aggregated_nominations_inner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_netted_nominations_data_mtus_inner_netted_nominations.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_netted_nominations_data_mtus_inner_netted_nominations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_next_auction.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_next_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_next_auctions_and_nomination_gates.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_next_auctions_and_nomination_gates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_transmission_rights_and_nominations_data.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_transmission_rights_and_nominations_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_inner_values_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_inner_values_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_inner_values_inner_nomination_restriction.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_transmission_rights_and_nominations_data_mtus_inner_values_inner_nomination_restriction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_inner_values_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_dashboard_transmission_rights_and_nominations_graph_data_mtus_inner_values_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_organisation_details.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_organisation_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_overview_api.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_overview_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_overview_data.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_overview_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_overview_data_contact_information.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_overview_data_contact_information.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_overview_data_finance_overview.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_overview_data_finance_overview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_participant_overview_data_organisation_members.py` & `empire-platform-api-public-client-0.167.0/test/test_participant_overview_data_organisation_members.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_permission.py` & `empire-platform-api-public-client-0.167.0/test/test_vat_rate_type.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
 import datetime
 
 import empire_platform_api_public_client
-from empire_platform_api_public_client.models.permission import Permission  # noqa: E501
+from empire_platform_api_public_client.models.vat_rate_type import VatRateType  # noqa: E501
 from empire_platform_api_public_client.rest import ApiException
 
-class TestPermission(unittest.TestCase):
-    """Permission unit test stubs"""
+class TestVatRateType(unittest.TestCase):
+    """VatRateType unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPermission(self):
-        """Test Permission"""
-        # inst = Permission()
+    def testVatRateType(self):
+        """Test VatRateType"""
+        # inst = VatRateType()
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_platform_appearance.py` & `empire-platform-api-public-client-0.167.0/test/test_platform_appearance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_profile.py` & `empire-platform-api-public-client-0.167.0/test/test_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_profile_api.py` & `empire-platform-api-public-client-0.167.0/test/test_profile_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_profile_details.py` & `empire-platform-api-public-client-0.167.0/test/test_profile_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_profile_user.py` & `empire-platform-api-public-client-0.167.0/test/test_profile_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_profile_user_organisation.py` & `empire-platform-api-public-client-0.167.0/test/test_profile_user_organisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_public_aggregated_nominations_overview_response.py` & `empire-platform-api-public-client-0.167.0/test/test_public_aggregated_nominations_overview_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_public_aggregated_nominations_overview_response_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_public_aggregated_nominations_overview_response_mtus_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_public_aggregated_nominations_overview_response_mtus_inner_values_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_public_aggregated_nominations_overview_response_mtus_inner_values_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_public_allocated_auction_api.py` & `empire-platform-api-public-client-0.167.0/test/test_public_allocated_auction_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_public_auction.py` & `empire-platform-api-public-client-0.167.0/test/test_public_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_public_auction_api.py` & `empire-platform-api-public-client-0.167.0/test/test_public_auction_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_public_auction_batch.py` & `empire-platform-api-public-client-0.167.0/test/test_public_auction_batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_public_auction_bid_status.py` & `empire-platform-api-public-client-0.167.0/test/test_public_auction_bid_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_public_auction_status.py` & `empire-platform-api-public-client-0.167.0/test/test_public_auction_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_public_day_ahead_auction.py` & `empire-platform-api-public-client-0.167.0/test/test_public_day_ahead_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_public_day_ahead_or_intra_day_auction_mtu_results.py` & `empire-platform-api-public-client-0.167.0/test/test_public_day_ahead_or_intra_day_auction_mtu_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_public_day_ahead_or_intra_day_auction_mtu_results_bids_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_public_day_ahead_or_intra_day_auction_mtu_results_bids_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_public_day_ahead_or_intra_day_auction_results.py` & `empire-platform-api-public-client-0.167.0/test/test_public_day_ahead_or_intra_day_auction_results.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_public_intra_day_auction.py` & `empire-platform-api-public-client-0.167.0/test/test_public_intra_day_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_public_long_term_auction.py` & `empire-platform-api-public-client-0.167.0/test/test_public_long_term_auction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_public_long_term_auction_results.py` & `empire-platform-api-public-client-0.167.0/test/test_public_long_term_auction_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_public_nominations_api.py` & `empire-platform-api-public-client-0.167.0/test/test_public_nominations_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_purchased_by_organisation.py` & `empire-platform-api-public-client-0.167.0/test/test_purchased_by_organisation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_reporting_api.py` & `empire-platform-api-public-client-0.167.0/test/test_reporting_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_reserve_price_publish_type.py` & `empire-platform-api-public-client-0.167.0/test/test_reserve_price_publish_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_return_auction.py` & `empire-platform-api-public-client-0.167.0/test/test_return_auction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_sage_code.py` & `empire-platform-api-public-client-0.167.0/test/test_sage_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_api.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_capacity_price_mtu.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_capacity_price_mtu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_details.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_matching.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_matching.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_response.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_response_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_entry_response_mtus_inner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_options.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_response_options.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_noticeboard_response_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_transfer_request.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_transfer_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_mtus_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_options.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_options_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_day_ahead_or_intra_day_transfer_request_options_mtus_inner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_long_term_noticeboard_entry.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_long_term_noticeboard_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_long_term_noticeboard_entry_details.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_long_term_noticeboard_entry_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_long_term_noticeboard_entry_response.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_long_term_noticeboard_entry_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_long_term_noticeboard_options.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_long_term_noticeboard_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_long_term_noticeboard_response_options.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_long_term_noticeboard_response_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_long_term_transfer_request_options.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_long_term_transfer_request_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_noticeboard_entry.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_noticeboard_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_noticeboard_entry_batch.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_noticeboard_entry_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_noticeboard_entry_status.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_noticeboard_entry_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_return_request.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_return_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_return_request_batch.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_return_request_batch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_return_request_status.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_return_request_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_transfer_request.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_transfer_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_transfer_request_batch.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_transfer_request_batch.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_transfer_request_type.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_transfer_request_type.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_secondary_market_transfer_transmission_rights_mtu.py` & `empire-platform-api-public-client-0.167.0/test/test_secondary_market_transfer_transmission_rights_mtu.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_settlement.py` & `empire-platform-api-public-client-0.167.0/test/test_settlement.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_settlement_item.py` & `empire-platform-api-public-client-0.167.0/test/test_settlement_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_settlement_per_source.py` & `empire-platform-api-public-client-0.167.0/test/test_settlement_per_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_settlement_source_type.py` & `empire-platform-api-public-client-0.167.0/test/test_settlement_source_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_settlement_sub_source_type.py` & `empire-platform-api-public-client-0.167.0/test/test_settlement_sub_source_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_source_auction.py` & `empire-platform-api-public-client-0.167.0/test/test_source_auction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_source_auction_display_data.py` & `empire-platform-api-public-client-0.167.0/test/test_source_auction_display_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_source_auction_result.py` & `empire-platform-api-public-client-0.167.0/test/test_source_auction_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_submit_day_ahead_or_intra_day_bids_request.py` & `empire-platform-api-public-client-0.167.0/test/test_submit_day_ahead_or_intra_day_bids_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
@@ -35,30 +35,28 @@
             params are included, when True both required and
             optional params are included """
         # uncomment below to create an instance of `SubmitDayAheadOrIntraDayBidsRequest`
         """
         model = empire_platform_api_public_client.models.submit_day_ahead_or_intra_day_bids_request.SubmitDayAheadOrIntraDayBidsRequest()  # noqa: E501
         if include_optional :
             return SubmitDayAheadOrIntraDayBidsRequest(
-                participant_id = '8d3787bb-b9ce-4d75-9a75-074ddd5d1e09', 
                 bid_groups = [
                     empire_platform_api_public_client.models.submit_day_ahead_or_intra_day_bids_request_bid_groups_inner.SubmitDayAheadOrIntraDayBidsRequest_bidGroups_inner(
                         id = '8d3787bb-b9ce-4d75-9a75-074ddd5d1e09', 
                         bids = [
                             empire_platform_api_public_client.models.submit_day_ahead_or_intra_day_bids_request_bid_groups_inner_bids_inner.SubmitDayAheadOrIntraDayBidsRequest_bidGroups_inner_bids_inner(
                                 mtu = '2022-01-04T10:00Z', 
                                 value = empire_platform_api_public_client.models.bid_value.BidValue(
                                     price = 1.337, 
                                     capacity = 56, ), )
                             ], )
                     ]
             )
         else :
             return SubmitDayAheadOrIntraDayBidsRequest(
-                participant_id = '8d3787bb-b9ce-4d75-9a75-074ddd5d1e09',
                 bid_groups = [
                     empire_platform_api_public_client.models.submit_day_ahead_or_intra_day_bids_request_bid_groups_inner.SubmitDayAheadOrIntraDayBidsRequest_bidGroups_inner(
                         id = '8d3787bb-b9ce-4d75-9a75-074ddd5d1e09', 
                         bids = [
                             empire_platform_api_public_client.models.submit_day_ahead_or_intra_day_bids_request_bid_groups_inner_bids_inner.SubmitDayAheadOrIntraDayBidsRequest_bidGroups_inner_bids_inner(
                                 mtu = '2022-01-04T10:00Z', 
                                 value = empire_platform_api_public_client.models.bid_value.BidValue(
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_submit_day_ahead_or_intra_day_bids_request_bid_groups_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_submit_day_ahead_or_intra_day_bids_request_bid_groups_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_submit_day_ahead_or_intra_day_bids_request_bid_groups_inner_bids_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_submit_day_ahead_or_intra_day_bids_request_bid_groups_inner_bids_inner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_submit_long_term_bids_request.py` & `empire-platform-api-public-client-0.167.0/test/test_update_user_request.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,70 +1,61 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
 import datetime
 
 import empire_platform_api_public_client
-from empire_platform_api_public_client.models.submit_long_term_bids_request import SubmitLongTermBidsRequest  # noqa: E501
+from empire_platform_api_public_client.models.update_user_request import UpdateUserRequest  # noqa: E501
 from empire_platform_api_public_client.rest import ApiException
 
-class TestSubmitLongTermBidsRequest(unittest.TestCase):
-    """SubmitLongTermBidsRequest unit test stubs"""
+class TestUpdateUserRequest(unittest.TestCase):
+    """UpdateUserRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test SubmitLongTermBidsRequest
+        """Test UpdateUserRequest
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `SubmitLongTermBidsRequest`
+        # uncomment below to create an instance of `UpdateUserRequest`
         """
-        model = empire_platform_api_public_client.models.submit_long_term_bids_request.SubmitLongTermBidsRequest()  # noqa: E501
+        model = empire_platform_api_public_client.models.update_user_request.UpdateUserRequest()  # noqa: E501
         if include_optional :
-            return SubmitLongTermBidsRequest(
-                participant_id = '8d3787bb-b9ce-4d75-9a75-074ddd5d1e09', 
-                bids = [
-                    empire_platform_api_public_client.models.submit_long_term_bids_request_bids_inner.SubmitLongTermBidsRequest_bids_inner(
-                        id = '8d3787bb-b9ce-4d75-9a75-074ddd5d1e09', 
-                        value = empire_platform_api_public_client.models.bid_value.BidValue(
-                            price = 1.337, 
-                            capacity = 56, ), )
-                    ]
+            return UpdateUserRequest(
+                name = '', 
+                phone_number = '+480728880015', 
+                role = 'ICO_ADMIN_BDL', 
+                job_title = ''
             )
         else :
-            return SubmitLongTermBidsRequest(
-                participant_id = '8d3787bb-b9ce-4d75-9a75-074ddd5d1e09',
-                bids = [
-                    empire_platform_api_public_client.models.submit_long_term_bids_request_bids_inner.SubmitLongTermBidsRequest_bids_inner(
-                        id = '8d3787bb-b9ce-4d75-9a75-074ddd5d1e09', 
-                        value = empire_platform_api_public_client.models.bid_value.BidValue(
-                            price = 1.337, 
-                            capacity = 56, ), )
-                    ],
+            return UpdateUserRequest(
+                name = '',
+                phone_number = '+480728880015',
+                role = 'ICO_ADMIN_BDL',
         )
         """
 
-    def testSubmitLongTermBidsRequest(self):
-        """Test SubmitLongTermBidsRequest"""
+    def testUpdateUserRequest(self):
+        """Test UpdateUserRequest"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_submit_long_term_bids_request_bids_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_submit_long_term_bids_request_bids_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_submit_nominations_mtu.py` & `empire-platform-api-public-client-0.167.0/test/test_submit_nominations_mtu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_submit_timescale_nominations_request.py` & `empire-platform-api-public-client-0.167.0/test/test_submit_timescale_nominations_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_system_message_category.py` & `empire-platform-api-public-client-0.167.0/test/test_system_message_category.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_timescale_nomination_mtu_status.py` & `empire-platform-api-public-client-0.167.0/test/test_timescale_nomination_mtu_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_timescale_nomination_options.py` & `empire-platform-api-public-client-0.167.0/test/test_timescale_nomination_options.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_timescale_nomination_options_window_timing.py` & `empire-platform-api-public-client-0.167.0/test/test_timescale_nomination_options_window_timing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_timescale_nomination_status.py` & `empire-platform-api-public-client-0.167.0/test/test_timescale_nomination_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_timescale_nomination_type.py` & `empire-platform-api-public-client-0.167.0/test/test_timescale_nomination_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_timescale_nomination_window_status.py` & `empire-platform-api-public-client-0.167.0/test/test_timescale_nomination_window_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_timescale_nominations.py` & `empire-platform-api-public-client-0.167.0/test/test_timescale_nominations.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_timescale_nominations_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_timescale_nominations_mtus_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_timescale_nominations_mtus_inner_current_nomination.py` & `empire-platform-api-public-client-0.167.0/test/test_timescale_nominations_mtus_inner_current_nomination.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_transmission_right_api.py` & `empire-platform-api-public-client-0.167.0/test/test_transmission_right_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_transmission_rights_overview.py` & `empire-platform-api-public-client-0.167.0/test/test_transmission_rights_overview.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_transmission_rights_overview_mtus_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_transmission_rights_overview_mtus_inner.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_transmission_rights_overview_mtus_inner_values_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_transmission_rights_overview_mtus_inner_values_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_transmission_rights_overview_mtus_inner_values_inner_timescales_inner.py` & `empire-platform-api-public-client-0.167.0/test/test_transmission_rights_overview_mtus_inner_values_inner_timescales_inner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_uiosi_not_resold.py` & `empire-platform-api-public-client-0.167.0/test/test_uiosi_not_resold.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_uiosi_overview.py` & `empire-platform-api-public-client-0.167.0/test/test_uiosi_overview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_uiosi_overview_per_mtu.py` & `empire-platform-api-public-client-0.167.0/test/test_uiosi_overview_per_mtu.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_uiosi_resold.py` & `empire-platform-api-public-client-0.167.0/test/test_uiosi_resold.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_unread_messages_response.py` & `empire-platform-api-public-client-0.167.0/test/test_unread_messages_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_update_day_ahead_or_intra_day_default_bid_request.py` & `empire-platform-api-public-client-0.167.0/test/test_update_day_ahead_or_intra_day_default_bid_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_update_default_nomination_request.py` & `empire-platform-api-public-client-0.167.0/test/test_update_default_nomination_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_update_long_term_default_bid_request.py` & `empire-platform-api-public-client-0.167.0/test/test_update_long_term_default_bid_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_update_profile_details_request.py` & `empire-platform-api-public-client-0.167.0/test/test_update_profile_details_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_update_user_request.py` & `empire-platform-api-public-client-0.167.0/test/test_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,56 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
 import datetime
 
 import empire_platform_api_public_client
-from empire_platform_api_public_client.models.update_user_request import UpdateUserRequest  # noqa: E501
+from empire_platform_api_public_client.models.version import Version  # noqa: E501
 from empire_platform_api_public_client.rest import ApiException
 
-class TestUpdateUserRequest(unittest.TestCase):
-    """UpdateUserRequest unit test stubs"""
+class TestVersion(unittest.TestCase):
+    """Version unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test UpdateUserRequest
+        """Test Version
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `UpdateUserRequest`
+        # uncomment below to create an instance of `Version`
         """
-        model = empire_platform_api_public_client.models.update_user_request.UpdateUserRequest()  # noqa: E501
+        model = empire_platform_api_public_client.models.version.Version()  # noqa: E501
         if include_optional :
-            return UpdateUserRequest(
-                name = '', 
-                phone_number = '+480728880015', 
-                role = 'ICO_ADMIN_BDL', 
-                job_title = ''
+            return Version(
+                version = ''
             )
         else :
-            return UpdateUserRequest(
-                name = '',
-                phone_number = '+480728880015',
-                role = 'ICO_ADMIN_BDL',
+            return Version(
+                version = '',
         )
         """
 
-    def testUpdateUserRequest(self):
-        """Test UpdateUserRequest"""
+    def testVersion(self):
+        """Test Version"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_user.py` & `empire-platform-api-public-client-0.167.0/test/test_user.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_user_api.py` & `empire-platform-api-public-client-0.167.0/test/test_user_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_user_organisation.py` & `empire-platform-api-public-client-0.167.0/test/test_user_organisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_user_preferences.py` & `empire-platform-api-public-client-0.167.0/test/test_user_preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_user_preferences_general_notifications.py` & `empire-platform-api-public-client-0.167.0/test/test_user_preferences_general_notifications.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_user_preferences_subscription_notifications.py` & `empire-platform-api-public-client-0.167.0/test/test_user_preferences_subscription_notifications.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_user_role.py` & `empire-platform-api-public-client-0.167.0/test/test_user_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_user_status.py` & `empire-platform-api-public-client-0.167.0/test/test_user_status.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
```

### Comparing `empire-platform-api-public-client-0.166.0/test/test_version.py` & `empire-platform-api-public-client-0.167.0/test/test_zendesk_chat_token_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 # coding: utf-8
 
 """
     Empire - Platform API
 
     OpenAPI specification for the Platform REST API of Empire  **System Time:** Europe/Amsterdam  **General data formats:**   * _capacity values_ => kW (integers)   * _dates and local times_ => System Time   * _currencies_ => EUR   # noqa: E501
 
-    The version of the OpenAPI document: 0.166.0
+    The version of the OpenAPI document: 0.167.0
     Contact: britned.info@britned.com
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """
 
 
 import unittest
 import datetime
 
 import empire_platform_api_public_client
-from empire_platform_api_public_client.models.version import Version  # noqa: E501
+from empire_platform_api_public_client.models.zendesk_chat_token_response import ZendeskChatTokenResponse  # noqa: E501
 from empire_platform_api_public_client.rest import ApiException
 
-class TestVersion(unittest.TestCase):
-    """Version unit test stubs"""
+class TestZendeskChatTokenResponse(unittest.TestCase):
+    """ZendeskChatTokenResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
     def make_instance(self, include_optional):
-        """Test Version
+        """Test ZendeskChatTokenResponse
             include_option is a boolean, when False only required
             params are included, when True both required and
             optional params are included """
-        # uncomment below to create an instance of `Version`
+        # uncomment below to create an instance of `ZendeskChatTokenResponse`
         """
-        model = empire_platform_api_public_client.models.version.Version()  # noqa: E501
+        model = empire_platform_api_public_client.models.zendesk_chat_token_response.ZendeskChatTokenResponse()  # noqa: E501
         if include_optional :
-            return Version(
-                version = ''
+            return ZendeskChatTokenResponse(
+                token = ''
             )
         else :
-            return Version(
-                version = '',
+            return ZendeskChatTokenResponse(
+                token = '',
         )
         """
 
-    def testVersion(self):
-        """Test Version"""
+    def testZendeskChatTokenResponse(self):
+        """Test ZendeskChatTokenResponse"""
         # inst_req_only = self.make_instance(include_optional=False)
         # inst_req_and_optional = self.make_instance(include_optional=True)
 
 if __name__ == '__main__':
     unittest.main()
```

