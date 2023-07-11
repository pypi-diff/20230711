# Comparing `tmp/types-braintree-4.20.0.0.tar.gz` & `tmp/types-braintree-4.21.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-braintree-4.20.0.0.tar", last modified: Tue May 23 09:14:52 2023, max compression
+gzip compressed data, was "types-braintree-4.21.0.0.tar", last modified: Tue Jul 11 09:16:21 2023, max compression
```

## Comparing `types-braintree-4.20.0.0.tar` & `types-braintree-4.21.0.0.tar`

### file list

```diff
@@ -1,172 +1,172 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:14:52.416328 types-braintree-4.20.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-23 09:14:49.000000 types-braintree-4.20.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-23 09:14:49.000000 types-braintree-4.20.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-23 09:14:52.416328 types-braintree-4.20.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:14:52.408328 types-braintree-4.20.0.0/braintree-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-23 09:14:49.000000 types-braintree-4.20.0.0/braintree-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/account_updater_daily_report.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/ach_mandate.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/add_on.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/add_on_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/address.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/address_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/amex_express_checkout_card.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/android_pay_card.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/apple_pay_card.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/apple_pay_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/apple_pay_options.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/attribute_getter.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/authorization_adjustment.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/bin_data.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/braintree_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/client_token.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/client_token_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/configuration.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/connected_merchant_paypal_status_changed.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/connected_merchant_status_transitioned.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/credentials_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/credit_card.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/credit_card_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/credit_card_verification.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/credit_card_verification_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/credit_card_verification_search.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/customer.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/customer_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/customer_search.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/descriptor.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/disbursement.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/disbursement_detail.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/discount.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/discount_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/dispute.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:14:52.412328 types-braintree-4.20.0.0/braintree-stubs/dispute_details/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/dispute_details/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/dispute_details/evidence.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/dispute_details/paypal_message.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/dispute_details/status_history.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/dispute_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/dispute_search.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/document_upload.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/document_upload_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/environment.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29247 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/error_codes.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/error_result.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/europe_bank_account.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:14:52.412328 types-braintree-4.20.0.0/braintree-stubs/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/authentication_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/authorization_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/braintree_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/configuration_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/gateway_timeout_error.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:14:52.412328 types-braintree-4.20.0.0/braintree-stubs/exceptions/http/
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/http/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/http/connection_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/http/invalid_response_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/http/timeout_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/invalid_challenge_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/invalid_signature_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/not_found_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/request_timeout_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/server_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/service_unavailable_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/too_many_requests_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/unexpected_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/exceptions/upgrade_required_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/facilitated_details.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/facilitator_details.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/granted_payment_instrument_update.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/iban_bank_account.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/ids_search.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/local_payment.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/local_payment_completed.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/local_payment_reversed.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/masterpass_card.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/merchant.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:14:52.416328 types-braintree-4.20.0.0/braintree-stubs/merchant_account/
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/merchant_account/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/merchant_account/address_details.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/merchant_account/business_details.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/merchant_account/funding_details.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/merchant_account/individual_details.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/merchant_account/merchant_account.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/merchant_account_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/merchant_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/modification.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/oauth_access_revocation.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/oauth_credentials.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/oauth_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/paginated_collection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/paginated_result.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/partner_merchant.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/payment_instrument_type.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/payment_method.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/payment_method_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/payment_method_nonce.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/payment_method_nonce_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/payment_method_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/paypal_account.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/paypal_account_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/paypal_here.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/plan.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/plan_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/processor_response_types.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/resource_collection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/revoked_payment_method_metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/risk_data.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/samsung_pay_card.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/search.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/settlement_batch_summary.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/settlement_batch_summary_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/signature_service.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/status_event.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/subscription.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/subscription_details.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/subscription_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/subscription_search.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/subscription_status_event.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/successful_result.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/testing_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/three_d_secure_info.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/transaction.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/transaction_amounts.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/transaction_details.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/transaction_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/transaction_line_item.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/transaction_line_item_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/transaction_search.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/unknown_payment_method.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/us_bank_account.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/us_bank_account_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/us_bank_account_verification.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/us_bank_account_verification_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/us_bank_account_verification_search.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:14:52.416328 types-braintree-4.20.0.0/braintree-stubs/util/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/util/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/util/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/util/crypto.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/util/datetime_parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/util/generator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/util/graphql_client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/util/http.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/util/parser.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/util/xml_util.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/validation_error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/validation_error_collection.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/venmo_account.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/visa_checkout_card.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/webhook_notification.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/webhook_notification_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/webhook_testing.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-23 09:14:32.000000 types-braintree-4.20.0.0/braintree-stubs/webhook_testing_gateway.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 09:14:52.416328 types-braintree-4.20.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5973 2023-05-23 09:14:49.000000 types-braintree-4.20.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 09:14:52.416328 types-braintree-4.20.0.0/types_braintree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-23 09:14:52.000000 types-braintree-4.20.0.0/types_braintree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-05-23 09:14:52.000000 types-braintree-4.20.0.0/types_braintree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 09:14:52.000000 types-braintree-4.20.0.0/types_braintree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-23 09:14:52.000000 types-braintree-4.20.0.0/types_braintree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:16:21.177629 types-braintree-4.21.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2268 2023-07-11 09:16:20.000000 types-braintree-4.21.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-11 09:16:20.000000 types-braintree-4.21.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-11 09:16:21.177629 types-braintree-4.21.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:16:21.173629 types-braintree-4.21.0.0/braintree-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-11 09:16:20.000000 types-braintree-4.21.0.0/braintree-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6001 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/account_updater_daily_report.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/ach_mandate.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/add_on.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/add_on_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/address.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/address_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/amex_express_checkout_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/android_pay_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/apple_pay_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/apple_pay_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/apple_pay_options.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/attribute_getter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/authorization_adjustment.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/bin_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/braintree_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/client_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/client_token_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/configuration.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/connected_merchant_paypal_status_changed.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/connected_merchant_status_transitioned.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/credentials_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/credit_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/credit_card_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/credit_card_verification.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/credit_card_verification_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/credit_card_verification_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2344 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/customer.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/customer_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/customer_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/descriptor.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/disbursement.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/disbursement_detail.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/discount.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/discount_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/dispute.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:16:21.173629 types-braintree-4.21.0.0/braintree-stubs/dispute_details/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/dispute_details/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/dispute_details/evidence.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/dispute_details/paypal_message.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/dispute_details/status_history.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/dispute_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/dispute_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/document_upload.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/document_upload_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29247 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/error_codes.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/error_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/europe_bank_account.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:16:21.173629 types-braintree-4.21.0.0/braintree-stubs/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/authentication_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/authorization_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/braintree_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/configuration_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/gateway_timeout_error.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:16:21.177629 types-braintree-4.21.0.0/braintree-stubs/exceptions/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/http/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/http/connection_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/http/invalid_response_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/http/timeout_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/invalid_challenge_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/invalid_signature_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/not_found_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/request_timeout_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/server_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/service_unavailable_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/too_many_requests_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/unexpected_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/exceptions/upgrade_required_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/facilitated_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/facilitator_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/granted_payment_instrument_update.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/iban_bank_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/ids_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/local_payment.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/local_payment_completed.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/local_payment_reversed.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/masterpass_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/merchant.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:16:21.177629 types-braintree-4.21.0.0/braintree-stubs/merchant_account/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/merchant_account/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/merchant_account/address_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/merchant_account/business_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/merchant_account/funding_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/merchant_account/individual_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/merchant_account/merchant_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/merchant_account_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/merchant_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/modification.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/oauth_access_revocation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/oauth_credentials.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/oauth_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/paginated_collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/paginated_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/partner_merchant.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/payment_instrument_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/payment_method.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/payment_method_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/payment_method_nonce.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/payment_method_nonce_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/payment_method_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/paypal_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/paypal_account_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/paypal_here.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/plan.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/plan_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/processor_response_types.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/resource_collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/revoked_payment_method_metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/risk_data.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/samsung_pay_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/search.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/settlement_batch_summary.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/settlement_batch_summary_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/signature_service.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/status_event.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/subscription.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/subscription_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/subscription_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/subscription_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/subscription_status_event.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/successful_result.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/testing_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/three_d_secure_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6491 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/transaction.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/transaction_amounts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/transaction_details.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/transaction_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/transaction_line_item.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/transaction_line_item_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/transaction_search.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/unknown_payment_method.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/us_bank_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/us_bank_account_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/us_bank_account_verification.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/us_bank_account_verification_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/us_bank_account_verification_search.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:16:21.177629 types-braintree-4.21.0.0/braintree-stubs/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/util/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/util/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/util/crypto.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/util/datetime_parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/util/generator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/util/graphql_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2298 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/util/http.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/util/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/util/xml_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/validation_error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/validation_error_collection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/venmo_account.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/visa_checkout_card.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/webhook_notification.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/webhook_notification_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/webhook_testing.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-07-11 09:16:02.000000 types-braintree-4.21.0.0/braintree-stubs/webhook_testing_gateway.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 09:16:21.177629 types-braintree-4.21.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6246 2023-07-11 09:16:20.000000 types-braintree-4.21.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 09:16:21.177629 types-braintree-4.21.0.0/types_braintree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-07-11 09:16:21.000000 types-braintree-4.21.0.0/types_braintree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6518 2023-07-11 09:16:21.000000 types-braintree-4.21.0.0/types_braintree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 09:16:21.000000 types-braintree-4.21.0.0/types_braintree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-11 09:16:21.000000 types-braintree-4.21.0.0/types_braintree.egg-info/top_level.txt
```

### Comparing `types-braintree-4.20.0.0/CHANGELOG.md` & `types-braintree-4.21.0.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## 4.21.0.0 (2023-07-11)
+
+[stubsabot] Bump braintree to 4.21.* (#10433)
+
+Release: https://pypi.org/pypi/braintree/4.21.0
+Homepage: https://developer.paypal.com/braintree/docs/reference/overview
+
 ## 4.20.0.0 (2023-05-23)
 
 [stubsabot] Bump braintree to 4.20.* (#10198)
 
 Release: https://pypi.org/pypi/braintree/4.20.0
 Homepage: https://developer.paypal.com/braintree/docs/reference/overview
```

### Comparing `types-braintree-4.20.0.0/PKG-INFO` & `types-braintree-4.21.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-braintree
-Version: 4.20.0.0
+Version: 4.21.0.0
 Summary: Typing stubs for braintree
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/braintree.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `braintree`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/braintree. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e821090926dcb06d5b53e0a81f29508bbe3a911b`.
+This package was generated from typeshed commit `d14ab09375120199eb9cbf775cb44951b26dc1b1` and was tested
+with mypy 1.4.1, pyright 1.1.316, and
+pytype 2023.6.16.
```

### Comparing `types-braintree-4.20.0.0/braintree-stubs/__init__.pyi` & `types-braintree-4.21.0.0/braintree-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/address.pyi` & `types-braintree-4.21.0.0/braintree-stubs/address.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/address_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/address_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/apple_pay_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/apple_pay_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/braintree_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/braintree_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/configuration.pyi` & `types-braintree-4.21.0.0/braintree-stubs/configuration.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/credentials_parser.pyi` & `types-braintree-4.21.0.0/braintree-stubs/credentials_parser.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/credit_card.pyi` & `types-braintree-4.21.0.0/braintree-stubs/credit_card.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/credit_card_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/credit_card_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/credit_card_verification.pyi` & `types-braintree-4.21.0.0/braintree-stubs/credit_card_verification.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/credit_card_verification_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/credit_card_verification_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/credit_card_verification_search.pyi` & `types-braintree-4.21.0.0/braintree-stubs/credit_card_verification_search.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/customer.pyi` & `types-braintree-4.21.0.0/braintree-stubs/customer.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/customer_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/customer_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/customer_search.pyi` & `types-braintree-4.21.0.0/braintree-stubs/customer_search.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/dispute.pyi` & `types-braintree-4.21.0.0/braintree-stubs/dispute.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/dispute_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/dispute_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/environment.pyi` & `types-braintree-4.21.0.0/braintree-stubs/environment.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/error_codes.pyi` & `types-braintree-4.21.0.0/braintree-stubs/error_codes.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/exceptions/__init__.pyi` & `types-braintree-4.21.0.0/braintree-stubs/exceptions/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/merchant_account/merchant_account.pyi` & `types-braintree-4.21.0.0/braintree-stubs/merchant_account/merchant_account.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/merchant_account_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/merchant_account_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/merchant_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/merchant_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/oauth_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/oauth_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/payment_method.pyi` & `types-braintree-4.21.0.0/braintree-stubs/payment_method.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/payment_method_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/payment_method_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/payment_method_nonce.pyi` & `types-braintree-4.21.0.0/braintree-stubs/payment_method_nonce.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/payment_method_nonce_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/payment_method_nonce_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/payment_method_parser.pyi` & `types-braintree-4.21.0.0/braintree-stubs/payment_method_parser.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/paypal_account.pyi` & `types-braintree-4.21.0.0/braintree-stubs/paypal_account.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/paypal_account_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/paypal_account_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/plan.pyi` & `types-braintree-4.21.0.0/braintree-stubs/plan.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/plan_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/plan_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/search.pyi` & `types-braintree-4.21.0.0/braintree-stubs/search.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/settlement_batch_summary.pyi` & `types-braintree-4.21.0.0/braintree-stubs/settlement_batch_summary.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/settlement_batch_summary_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/settlement_batch_summary_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/subscription.pyi` & `types-braintree-4.21.0.0/braintree-stubs/subscription.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/subscription_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/subscription_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/testing_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/testing_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/transaction.pyi` & `types-braintree-4.21.0.0/braintree-stubs/transaction.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/transaction_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/transaction_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/transaction_line_item_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/transaction_line_item_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/transaction_search.pyi` & `types-braintree-4.21.0.0/braintree-stubs/transaction_search.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/us_bank_account.pyi` & `types-braintree-4.21.0.0/braintree-stubs/us_bank_account.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/us_bank_account_verification.pyi` & `types-braintree-4.21.0.0/braintree-stubs/us_bank_account_verification.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/us_bank_account_verification_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/us_bank_account_verification_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/us_bank_account_verification_search.pyi` & `types-braintree-4.21.0.0/braintree-stubs/us_bank_account_verification_search.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/util/graphql_client.pyi` & `types-braintree-4.21.0.0/braintree-stubs/util/graphql_client.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/util/http.pyi` & `types-braintree-4.21.0.0/braintree-stubs/util/http.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/validation_error_collection.pyi` & `types-braintree-4.21.0.0/braintree-stubs/validation_error_collection.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/webhook_notification.pyi` & `types-braintree-4.21.0.0/braintree-stubs/webhook_notification.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/braintree-stubs/webhook_notification_gateway.pyi` & `types-braintree-4.21.0.0/braintree-stubs/webhook_notification_gateway.pyi`

 * *Files identical despite different names*

### Comparing `types-braintree-4.20.0.0/setup.py` & `types-braintree-4.21.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,33 +11,39 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `braintree`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/braintree. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e821090926dcb06d5b53e0a81f29508bbe3a911b`.
+This package was generated from typeshed commit `d14ab09375120199eb9cbf775cb44951b26dc1b1` and was tested
+with mypy 1.4.1, pyright 1.1.316, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="4.20.0.0",
+      version="4.21.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/braintree.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['braintree-stubs'],
-      package_data={'braintree-stubs': ['__init__.pyi', 'account_updater_daily_report.pyi', 'ach_mandate.pyi', 'add_on.pyi', 'add_on_gateway.pyi', 'address.pyi', 'address_gateway.pyi', 'amex_express_checkout_card.pyi', 'android_pay_card.pyi', 'apple_pay_card.pyi', 'apple_pay_gateway.pyi', 'apple_pay_options.pyi', 'attribute_getter.pyi', 'authorization_adjustment.pyi', 'bin_data.pyi', 'braintree_gateway.pyi', 'client_token.pyi', 'client_token_gateway.pyi', 'configuration.pyi', 'connected_merchant_paypal_status_changed.pyi', 'connected_merchant_status_transitioned.pyi', 'credentials_parser.pyi', 'credit_card.pyi', 'credit_card_gateway.pyi', 'credit_card_verification.pyi', 'credit_card_verification_gateway.pyi', 'credit_card_verification_search.pyi', 'customer.pyi', 'customer_gateway.pyi', 'customer_search.pyi', 'descriptor.pyi', 'disbursement.pyi', 'disbursement_detail.pyi', 'discount.pyi', 'discount_gateway.pyi', 'dispute.pyi', 'dispute_details/__init__.pyi', 'dispute_details/evidence.pyi', 'dispute_details/paypal_message.pyi', 'dispute_details/status_history.pyi', 'dispute_gateway.pyi', 'dispute_search.pyi', 'document_upload.pyi', 'document_upload_gateway.pyi', 'environment.pyi', 'error_codes.pyi', 'error_result.pyi', 'errors.pyi', 'europe_bank_account.pyi', 'exceptions/__init__.pyi', 'exceptions/authentication_error.pyi', 'exceptions/authorization_error.pyi', 'exceptions/braintree_error.pyi', 'exceptions/configuration_error.pyi', 'exceptions/gateway_timeout_error.pyi', 'exceptions/http/__init__.pyi', 'exceptions/http/connection_error.pyi', 'exceptions/http/invalid_response_error.pyi', 'exceptions/http/timeout_error.pyi', 'exceptions/invalid_challenge_error.pyi', 'exceptions/invalid_signature_error.pyi', 'exceptions/not_found_error.pyi', 'exceptions/request_timeout_error.pyi', 'exceptions/server_error.pyi', 'exceptions/service_unavailable_error.pyi', 'exceptions/too_many_requests_error.pyi', 'exceptions/unexpected_error.pyi', 'exceptions/upgrade_required_error.pyi', 'facilitated_details.pyi', 'facilitator_details.pyi', 'granted_payment_instrument_update.pyi', 'iban_bank_account.pyi', 'ids_search.pyi', 'local_payment.pyi', 'local_payment_completed.pyi', 'local_payment_reversed.pyi', 'masterpass_card.pyi', 'merchant.pyi', 'merchant_account/__init__.pyi', 'merchant_account/address_details.pyi', 'merchant_account/business_details.pyi', 'merchant_account/funding_details.pyi', 'merchant_account/individual_details.pyi', 'merchant_account/merchant_account.pyi', 'merchant_account_gateway.pyi', 'merchant_gateway.pyi', 'modification.pyi', 'oauth_access_revocation.pyi', 'oauth_credentials.pyi', 'oauth_gateway.pyi', 'paginated_collection.pyi', 'paginated_result.pyi', 'partner_merchant.pyi', 'payment_instrument_type.pyi', 'payment_method.pyi', 'payment_method_gateway.pyi', 'payment_method_nonce.pyi', 'payment_method_nonce_gateway.pyi', 'payment_method_parser.pyi', 'paypal_account.pyi', 'paypal_account_gateway.pyi', 'paypal_here.pyi', 'plan.pyi', 'plan_gateway.pyi', 'processor_response_types.pyi', 'resource.pyi', 'resource_collection.pyi', 'revoked_payment_method_metadata.pyi', 'risk_data.pyi', 'samsung_pay_card.pyi', 'search.pyi', 'settlement_batch_summary.pyi', 'settlement_batch_summary_gateway.pyi', 'signature_service.pyi', 'status_event.pyi', 'subscription.pyi', 'subscription_details.pyi', 'subscription_gateway.pyi', 'subscription_search.pyi', 'subscription_status_event.pyi', 'successful_result.pyi', 'testing_gateway.pyi', 'three_d_secure_info.pyi', 'transaction.pyi', 'transaction_amounts.pyi', 'transaction_details.pyi', 'transaction_gateway.pyi', 'transaction_line_item.pyi', 'transaction_line_item_gateway.pyi', 'transaction_search.pyi', 'unknown_payment_method.pyi', 'us_bank_account.pyi', 'us_bank_account_gateway.pyi', 'us_bank_account_verification.pyi', 'us_bank_account_verification_gateway.pyi', 'us_bank_account_verification_search.pyi', 'util/__init__.pyi', 'util/constants.pyi', 'util/crypto.pyi', 'util/datetime_parser.pyi', 'util/generator.pyi', 'util/graphql_client.pyi', 'util/http.pyi', 'util/parser.pyi', 'util/xml_util.pyi', 'validation_error.pyi', 'validation_error_collection.pyi', 'venmo_account.pyi', 'version.pyi', 'visa_checkout_card.pyi', 'webhook_notification.pyi', 'webhook_notification_gateway.pyi', 'webhook_testing.pyi', 'webhook_testing_gateway.pyi', 'METADATA.toml']},
+      package_data={'braintree-stubs': ['__init__.pyi', 'account_updater_daily_report.pyi', 'ach_mandate.pyi', 'add_on.pyi', 'add_on_gateway.pyi', 'address.pyi', 'address_gateway.pyi', 'amex_express_checkout_card.pyi', 'android_pay_card.pyi', 'apple_pay_card.pyi', 'apple_pay_gateway.pyi', 'apple_pay_options.pyi', 'attribute_getter.pyi', 'authorization_adjustment.pyi', 'bin_data.pyi', 'braintree_gateway.pyi', 'client_token.pyi', 'client_token_gateway.pyi', 'configuration.pyi', 'connected_merchant_paypal_status_changed.pyi', 'connected_merchant_status_transitioned.pyi', 'credentials_parser.pyi', 'credit_card.pyi', 'credit_card_gateway.pyi', 'credit_card_verification.pyi', 'credit_card_verification_gateway.pyi', 'credit_card_verification_search.pyi', 'customer.pyi', 'customer_gateway.pyi', 'customer_search.pyi', 'descriptor.pyi', 'disbursement.pyi', 'disbursement_detail.pyi', 'discount.pyi', 'discount_gateway.pyi', 'dispute.pyi', 'dispute_details/__init__.pyi', 'dispute_details/evidence.pyi', 'dispute_details/paypal_message.pyi', 'dispute_details/status_history.pyi', 'dispute_gateway.pyi', 'dispute_search.pyi', 'document_upload.pyi', 'document_upload_gateway.pyi', 'environment.pyi', 'error_codes.pyi', 'error_result.pyi', 'errors.pyi', 'europe_bank_account.pyi', 'exceptions/__init__.pyi', 'exceptions/authentication_error.pyi', 'exceptions/authorization_error.pyi', 'exceptions/braintree_error.pyi', 'exceptions/configuration_error.pyi', 'exceptions/gateway_timeout_error.pyi', 'exceptions/http/__init__.pyi', 'exceptions/http/connection_error.pyi', 'exceptions/http/invalid_response_error.pyi', 'exceptions/http/timeout_error.pyi', 'exceptions/invalid_challenge_error.pyi', 'exceptions/invalid_signature_error.pyi', 'exceptions/not_found_error.pyi', 'exceptions/request_timeout_error.pyi', 'exceptions/server_error.pyi', 'exceptions/service_unavailable_error.pyi', 'exceptions/too_many_requests_error.pyi', 'exceptions/unexpected_error.pyi', 'exceptions/upgrade_required_error.pyi', 'facilitated_details.pyi', 'facilitator_details.pyi', 'granted_payment_instrument_update.pyi', 'iban_bank_account.pyi', 'ids_search.pyi', 'local_payment.pyi', 'local_payment_completed.pyi', 'local_payment_reversed.pyi', 'masterpass_card.pyi', 'merchant.pyi', 'merchant_account/__init__.pyi', 'merchant_account/address_details.pyi', 'merchant_account/business_details.pyi', 'merchant_account/funding_details.pyi', 'merchant_account/individual_details.pyi', 'merchant_account/merchant_account.pyi', 'merchant_account_gateway.pyi', 'merchant_gateway.pyi', 'modification.pyi', 'oauth_access_revocation.pyi', 'oauth_credentials.pyi', 'oauth_gateway.pyi', 'paginated_collection.pyi', 'paginated_result.pyi', 'partner_merchant.pyi', 'payment_instrument_type.pyi', 'payment_method.pyi', 'payment_method_gateway.pyi', 'payment_method_nonce.pyi', 'payment_method_nonce_gateway.pyi', 'payment_method_parser.pyi', 'paypal_account.pyi', 'paypal_account_gateway.pyi', 'paypal_here.pyi', 'plan.pyi', 'plan_gateway.pyi', 'processor_response_types.pyi', 'resource.pyi', 'resource_collection.pyi', 'revoked_payment_method_metadata.pyi', 'risk_data.pyi', 'samsung_pay_card.pyi', 'search.pyi', 'settlement_batch_summary.pyi', 'settlement_batch_summary_gateway.pyi', 'signature_service.pyi', 'status_event.pyi', 'subscription.pyi', 'subscription_details.pyi', 'subscription_gateway.pyi', 'subscription_search.pyi', 'subscription_status_event.pyi', 'successful_result.pyi', 'testing_gateway.pyi', 'three_d_secure_info.pyi', 'transaction.pyi', 'transaction_amounts.pyi', 'transaction_details.pyi', 'transaction_gateway.pyi', 'transaction_line_item.pyi', 'transaction_line_item_gateway.pyi', 'transaction_search.pyi', 'unknown_payment_method.pyi', 'us_bank_account.pyi', 'us_bank_account_gateway.pyi', 'us_bank_account_verification.pyi', 'us_bank_account_verification_gateway.pyi', 'us_bank_account_verification_search.pyi', 'util/__init__.pyi', 'util/constants.pyi', 'util/crypto.pyi', 'util/datetime_parser.pyi', 'util/generator.pyi', 'util/graphql_client.pyi', 'util/http.pyi', 'util/parser.pyi', 'util/xml_util.pyi', 'validation_error.pyi', 'validation_error_collection.pyi', 'venmo_account.pyi', 'version.pyi', 'visa_checkout_card.pyi', 'webhook_notification.pyi', 'webhook_notification_gateway.pyi', 'webhook_testing.pyi', 'webhook_testing_gateway.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-braintree-4.20.0.0/types_braintree.egg-info/PKG-INFO` & `types-braintree-4.21.0.0/types_braintree.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-braintree
-Version: 4.20.0.0
+Version: 4.21.0.0
 Summary: Typing stubs for braintree
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/braintree.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `braintree`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/braintree. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `e821090926dcb06d5b53e0a81f29508bbe3a911b`.
+This package was generated from typeshed commit `d14ab09375120199eb9cbf775cb44951b26dc1b1` and was tested
+with mypy 1.4.1, pyright 1.1.316, and
+pytype 2023.6.16.
```

### Comparing `types-braintree-4.20.0.0/types_braintree.egg-info/SOURCES.txt` & `types-braintree-4.21.0.0/types_braintree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

