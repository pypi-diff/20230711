# Comparing `tmp/mypy-boto3-cognito-idp-1.28.0.tar.gz` & `tmp/mypy-boto3-cognito-idp-1.28.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-cognito-idp-1.28.0.tar", last modified: Thu Jul  6 20:59:16 2023, max compression
+gzip compressed data, was "mypy-boto3-cognito-idp-1.28.2.tar", last modified: Tue Jul 11 06:09:51 2023, max compression
```

## Comparing `mypy-boto3-cognito-idp-1.28.0.tar` & `mypy-boto3-cognito-idp-1.28.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:16.282259 mypy-boto3-cognito-idp-1.28.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-06 20:36:22.000000 mypy-boto3-cognito-idp-1.28.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-07-06 20:59:16.282259 mypy-boto3-cognito-idp-1.28.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    23665 2023-07-06 20:36:22.000000 mypy-boto3-cognito-idp-1.28.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:16.278259 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-06 20:36:23.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-06 20:36:23.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-06 20:36:23.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    78755 2023-07-06 20:36:23.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    78638 2023-07-06 20:36:23.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-07-06 20:36:24.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-06 20:36:24.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    11066 2023-07-06 20:36:23.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11055 2023-07-06 20:36:23.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 20:36:23.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    97444 2023-07-06 20:36:28.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    97305 2023-07-06 20:36:25.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-06 20:36:23.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 20:59:16.282259 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-07-06 20:59:16.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-06 20:59:16.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:16.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 20:59:16.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-06 20:59:16.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-06 20:59:16.000000 mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 20:59:16.282259 mypy-boto3-cognito-idp-1.28.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-06 20:36:22.000000 mypy-boto3-cognito-idp-1.28.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:09:51.558497 mypy-boto3-cognito-idp-1.28.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-07-11 06:09:51.558497 mypy-boto3-cognito-idp-1.28.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23665 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:09:51.558497 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78755 2023-07-11 06:09:40.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78638 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    13623 2023-07-11 06:09:40.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13621 2023-07-11 06:09:40.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11048 2023-07-11 06:09:40.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11037 2023-07-11 06:09:40.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    97304 2023-07-11 06:09:42.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97165 2023-07-11 06:09:41.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:09:51.558497 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25178 2023-07-11 06:09:51.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-07-11 06:09:51.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 06:09:51.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 06:09:51.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-11 06:09:51.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-11 06:09:51.000000 mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 06:09:51.558497 mypy-boto3-cognito-idp-1.28.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-11 06:09:39.000000 mypy-boto3-cognito-idp-1.28.2/setup.py
```

### Comparing `mypy-boto3-cognito-idp-1.28.0/LICENSE` & `mypy-boto3-cognito-idp-1.28.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.0/PKG-INFO` & `mypy-boto3-cognito-idp-1.28.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-idp
-Version: 1.28.0
-Summary: Type annotations for boto3.CognitoIdentityProvider 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.2
+Summary: Type annotations for boto3.CognitoIdentityProvider 1.28.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-idp?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentityProvider 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[boto3.CognitoIdentityProvider 1.28.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -400,62 +400,59 @@
 from mypy_boto3_cognito_idp.type_defs import (
     RecoveryOptionTypeTypeDef,
     AccountTakeoverActionTypeTypeDef,
     AdminAddUserToGroupRequestRequestTypeDef,
     AdminConfirmSignUpRequestRequestTypeDef,
     MessageTemplateTypeTypeDef,
     AttributeTypeTypeDef,
+    ResponseMetadataTypeDef,
     AdminDeleteUserAttributesRequestRequestTypeDef,
     AdminDeleteUserRequestRequestTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     AdminDisableUserRequestRequestTypeDef,
     AdminEnableUserRequestRequestTypeDef,
     AdminForgetDeviceRequestRequestTypeDef,
     AdminGetDeviceRequestRequestTypeDef,
     AdminGetUserRequestRequestTypeDef,
     MFAOptionTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AdminListDevicesRequestRequestTypeDef,
-    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    PaginatorConfigTypeDef,
     AdminListGroupsForUserRequestRequestTypeDef,
     GroupTypeTypeDef,
-    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
     AdminListUserAuthEventsRequestRequestTypeDef,
     AdminRemoveUserFromGroupRequestRequestTypeDef,
     AdminResetUserPasswordRequestRequestTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
     AdminSetUserPasswordRequestRequestTypeDef,
     AdminUpdateAuthEventFeedbackRequestRequestTypeDef,
     AdminUpdateDeviceStatusRequestRequestTypeDef,
     AdminUserGlobalSignOutRequestRequestTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AssociateSoftwareTokenRequestRequestTypeDef,
-    AssociateSoftwareTokenResponseTypeDef,
     ChallengeResponseTypeTypeDef,
     EventContextDataTypeTypeDef,
     EventFeedbackTypeTypeDef,
     EventRiskTypeTypeDef,
     NewDeviceMetadataTypeTypeDef,
     ChangePasswordRequestRequestTypeDef,
     CodeDeliveryDetailsTypeTypeDef,
     CompromisedCredentialsActionsTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
-    ConfirmDeviceResponseTypeDef,
     UserContextDataTypeTypeDef,
     HttpHeaderTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
     IdentityProviderTypeTypeDef,
     ResourceServerScopeTypeTypeDef,
     CreateUserImportJobRequestRequestTypeDef,
     UserImportJobTypeTypeDef,
     TokenValidityUnitsTypeTypeDef,
     CustomDomainConfigTypeTypeDef,
-    CreateUserPoolDomainResponseTypeDef,
     DeviceConfigurationTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     SmsConfigurationTypeTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
@@ -472,85 +469,88 @@
     DescribeIdentityProviderRequestRequestTypeDef,
     DescribeResourceServerRequestRequestTypeDef,
     DescribeRiskConfigurationRequestRequestTypeDef,
     DescribeUserImportJobRequestRequestTypeDef,
     DescribeUserPoolClientRequestRequestTypeDef,
     DescribeUserPoolDomainRequestRequestTypeDef,
     DescribeUserPoolRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ForgetDeviceRequestRequestTypeDef,
     GetCSVHeaderRequestRequestTypeDef,
-    GetCSVHeaderResponseTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GetIdentityProviderByIdentifierRequestRequestTypeDef,
     GetSigningCertificateRequestRequestTypeDef,
-    GetSigningCertificateResponseTypeDef,
     GetUICustomizationRequestRequestTypeDef,
     UICustomizationTypeTypeDef,
     GetUserAttributeVerificationCodeRequestRequestTypeDef,
     GetUserPoolMfaConfigRequestRequestTypeDef,
     SoftwareTokenMfaConfigTypeTypeDef,
     GetUserRequestRequestTypeDef,
     GlobalSignOutRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     ProviderDescriptionTypeDef,
-    ListResourceServersRequestListResourceServersPaginateTypeDef,
     ListResourceServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListUserImportJobsRequestRequestTypeDef,
-    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
     ListUserPoolClientsRequestRequestTypeDef,
     UserPoolClientDescriptionTypeDef,
-    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
     ListUserPoolsRequestRequestTypeDef,
-    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
     ListUsersInGroupRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     NotifyEmailTypeTypeDef,
     NumberAttributeConstraintsTypeTypeDef,
-    PaginatorConfigTypeDef,
     PasswordPolicyTypeTypeDef,
-    ResponseMetadataTypeDef,
     RevokeTokenRequestRequestTypeDef,
     RiskExceptionConfigurationTypeTypeDef,
     StringAttributeConstraintsTypeTypeDef,
     SetUICustomizationRequestRequestTypeDef,
     StartUserImportJobRequestRequestTypeDef,
     StopUserImportJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthEventFeedbackRequestRequestTypeDef,
     UpdateDeviceStatusRequestRequestTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
-    UpdateUserPoolDomainResponseTypeDef,
     VerifySoftwareTokenRequestRequestTypeDef,
-    VerifySoftwareTokenResponseTypeDef,
     VerifyUserAttributeRequestRequestTypeDef,
     AccountRecoverySettingTypeTypeDef,
     AccountTakeoverActionsTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserRequestRequestTypeDef,
     AdminUpdateUserAttributesRequestRequestTypeDef,
     DeviceTypeTypeDef,
     UpdateUserAttributesRequestRequestTypeDef,
+    AssociateSoftwareTokenResponseTypeDef,
+    ConfirmDeviceResponseTypeDef,
+    CreateUserPoolDomainResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCSVHeaderResponseTypeDef,
+    GetSigningCertificateResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateUserPoolDomainResponseTypeDef,
+    VerifySoftwareTokenResponseTypeDef,
     AdminDisableProviderForUserRequestRequestTypeDef,
     AdminLinkProviderForUserRequestRequestTypeDef,
     AdminGetUserResponseTypeDef,
     AdminSetUserSettingsRequestRequestTypeDef,
     GetUserResponseTypeDef,
     SetUserSettingsRequestRequestTypeDef,
     UserTypeTypeDef,
+    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    ListResourceServersRequestListResourceServersPaginateTypeDef,
+    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
+    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     AdminListGroupsForUserResponseTypeDef,
     CreateGroupResponseTypeDef,
     GetGroupResponseTypeDef,
     ListGroupsResponseTypeDef,
     UpdateGroupResponseTypeDef,
     AdminSetUserMFAPreferenceRequestRequestTypeDef,
     SetUserMFAPreferenceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-cognito-idp-1.28.0/README.md` & `mypy-boto3-cognito-idp-1.28.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-idp?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentityProvider 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[boto3.CognitoIdentityProvider 1.28.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -368,62 +368,59 @@
 from mypy_boto3_cognito_idp.type_defs import (
     RecoveryOptionTypeTypeDef,
     AccountTakeoverActionTypeTypeDef,
     AdminAddUserToGroupRequestRequestTypeDef,
     AdminConfirmSignUpRequestRequestTypeDef,
     MessageTemplateTypeTypeDef,
     AttributeTypeTypeDef,
+    ResponseMetadataTypeDef,
     AdminDeleteUserAttributesRequestRequestTypeDef,
     AdminDeleteUserRequestRequestTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     AdminDisableUserRequestRequestTypeDef,
     AdminEnableUserRequestRequestTypeDef,
     AdminForgetDeviceRequestRequestTypeDef,
     AdminGetDeviceRequestRequestTypeDef,
     AdminGetUserRequestRequestTypeDef,
     MFAOptionTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AdminListDevicesRequestRequestTypeDef,
-    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    PaginatorConfigTypeDef,
     AdminListGroupsForUserRequestRequestTypeDef,
     GroupTypeTypeDef,
-    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
     AdminListUserAuthEventsRequestRequestTypeDef,
     AdminRemoveUserFromGroupRequestRequestTypeDef,
     AdminResetUserPasswordRequestRequestTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
     AdminSetUserPasswordRequestRequestTypeDef,
     AdminUpdateAuthEventFeedbackRequestRequestTypeDef,
     AdminUpdateDeviceStatusRequestRequestTypeDef,
     AdminUserGlobalSignOutRequestRequestTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AssociateSoftwareTokenRequestRequestTypeDef,
-    AssociateSoftwareTokenResponseTypeDef,
     ChallengeResponseTypeTypeDef,
     EventContextDataTypeTypeDef,
     EventFeedbackTypeTypeDef,
     EventRiskTypeTypeDef,
     NewDeviceMetadataTypeTypeDef,
     ChangePasswordRequestRequestTypeDef,
     CodeDeliveryDetailsTypeTypeDef,
     CompromisedCredentialsActionsTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
-    ConfirmDeviceResponseTypeDef,
     UserContextDataTypeTypeDef,
     HttpHeaderTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
     IdentityProviderTypeTypeDef,
     ResourceServerScopeTypeTypeDef,
     CreateUserImportJobRequestRequestTypeDef,
     UserImportJobTypeTypeDef,
     TokenValidityUnitsTypeTypeDef,
     CustomDomainConfigTypeTypeDef,
-    CreateUserPoolDomainResponseTypeDef,
     DeviceConfigurationTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     SmsConfigurationTypeTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
@@ -440,85 +437,88 @@
     DescribeIdentityProviderRequestRequestTypeDef,
     DescribeResourceServerRequestRequestTypeDef,
     DescribeRiskConfigurationRequestRequestTypeDef,
     DescribeUserImportJobRequestRequestTypeDef,
     DescribeUserPoolClientRequestRequestTypeDef,
     DescribeUserPoolDomainRequestRequestTypeDef,
     DescribeUserPoolRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ForgetDeviceRequestRequestTypeDef,
     GetCSVHeaderRequestRequestTypeDef,
-    GetCSVHeaderResponseTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GetIdentityProviderByIdentifierRequestRequestTypeDef,
     GetSigningCertificateRequestRequestTypeDef,
-    GetSigningCertificateResponseTypeDef,
     GetUICustomizationRequestRequestTypeDef,
     UICustomizationTypeTypeDef,
     GetUserAttributeVerificationCodeRequestRequestTypeDef,
     GetUserPoolMfaConfigRequestRequestTypeDef,
     SoftwareTokenMfaConfigTypeTypeDef,
     GetUserRequestRequestTypeDef,
     GlobalSignOutRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     ProviderDescriptionTypeDef,
-    ListResourceServersRequestListResourceServersPaginateTypeDef,
     ListResourceServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListUserImportJobsRequestRequestTypeDef,
-    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
     ListUserPoolClientsRequestRequestTypeDef,
     UserPoolClientDescriptionTypeDef,
-    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
     ListUserPoolsRequestRequestTypeDef,
-    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
     ListUsersInGroupRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     NotifyEmailTypeTypeDef,
     NumberAttributeConstraintsTypeTypeDef,
-    PaginatorConfigTypeDef,
     PasswordPolicyTypeTypeDef,
-    ResponseMetadataTypeDef,
     RevokeTokenRequestRequestTypeDef,
     RiskExceptionConfigurationTypeTypeDef,
     StringAttributeConstraintsTypeTypeDef,
     SetUICustomizationRequestRequestTypeDef,
     StartUserImportJobRequestRequestTypeDef,
     StopUserImportJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthEventFeedbackRequestRequestTypeDef,
     UpdateDeviceStatusRequestRequestTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
-    UpdateUserPoolDomainResponseTypeDef,
     VerifySoftwareTokenRequestRequestTypeDef,
-    VerifySoftwareTokenResponseTypeDef,
     VerifyUserAttributeRequestRequestTypeDef,
     AccountRecoverySettingTypeTypeDef,
     AccountTakeoverActionsTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserRequestRequestTypeDef,
     AdminUpdateUserAttributesRequestRequestTypeDef,
     DeviceTypeTypeDef,
     UpdateUserAttributesRequestRequestTypeDef,
+    AssociateSoftwareTokenResponseTypeDef,
+    ConfirmDeviceResponseTypeDef,
+    CreateUserPoolDomainResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCSVHeaderResponseTypeDef,
+    GetSigningCertificateResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateUserPoolDomainResponseTypeDef,
+    VerifySoftwareTokenResponseTypeDef,
     AdminDisableProviderForUserRequestRequestTypeDef,
     AdminLinkProviderForUserRequestRequestTypeDef,
     AdminGetUserResponseTypeDef,
     AdminSetUserSettingsRequestRequestTypeDef,
     GetUserResponseTypeDef,
     SetUserSettingsRequestRequestTypeDef,
     UserTypeTypeDef,
+    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    ListResourceServersRequestListResourceServersPaginateTypeDef,
+    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
+    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     AdminListGroupsForUserResponseTypeDef,
     CreateGroupResponseTypeDef,
     GetGroupResponseTypeDef,
     ListGroupsResponseTypeDef,
     UpdateGroupResponseTypeDef,
     AdminSetUserMFAPreferenceRequestRequestTypeDef,
     SetUserMFAPreferenceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/__init__.py` & `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/__init__.pyi` & `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/__main__.py` & `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.CognitoIdentityProvider 1.28.0\nVersion:        "
-        " 1.28.0\nBuilder version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.CognitoIdentityProvider 1.28.2\nVersion:        "
+        " 1.28.2\nBuilder version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.28.0")
+    print("1.28.2")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/client.py` & `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/client.pyi` & `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/literals.py` & `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/literals.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/literals.pyi` & `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/literals.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/paginator.py` & `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/paginator.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,105 +78,105 @@
 class AdminListGroupsForUserPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
     """
 
     def paginate(
-        self, *, Username: str, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Username: str, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[AdminListGroupsForUserResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
         """
 
 
 class AdminListUserAuthEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistuserautheventspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, Username: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, Username: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[AdminListUserAuthEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistuserautheventspaginator)
         """
 
 
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listgroupspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listgroupspaginator)
         """
 
 
 class ListIdentityProvidersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listidentityproviderspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIdentityProvidersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listidentityproviderspaginator)
         """
 
 
 class ListResourceServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listresourceserverspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listresourceserverspaginator)
         """
 
 
 class ListUserPoolClientsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolclientspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUserPoolClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolclientspaginator)
         """
 
 
 class ListUserPoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUserPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolspaginator)
         """
 
 
@@ -188,28 +188,28 @@
 
     def paginate(
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Filter: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserspaginator)
         """
 
 
 class ListUsersInGroupPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listusersingrouppaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, GroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsersInGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listusersingrouppaginator)
         """
```

### Comparing `mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/paginator.pyi` & `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/paginator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -75,99 +75,99 @@
 class AdminListGroupsForUserPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
     """
 
     def paginate(
-        self, *, Username: str, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, Username: str, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[AdminListGroupsForUserResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListGroupsForUser.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistgroupsforuserpaginator)
         """
 
 class AdminListUserAuthEventsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistuserautheventspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, Username: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, Username: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[AdminListUserAuthEventsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.AdminListUserAuthEvents.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#adminlistuserautheventspaginator)
         """
 
 class ListGroupsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listgroupspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListGroupsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListGroups.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listgroupspaginator)
         """
 
 class ListIdentityProvidersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listidentityproviderspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListIdentityProvidersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListIdentityProviders.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listidentityproviderspaginator)
         """
 
 class ListResourceServersPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listresourceserverspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListResourceServersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListResourceServers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listresourceserverspaginator)
         """
 
 class ListUserPoolClientsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolclientspaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUserPoolClientsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPoolClients.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolclientspaginator)
         """
 
 class ListUserPoolsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolspaginator)
     """
 
     def paginate(
-        self, *, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUserPoolsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUserPools.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserpoolspaginator)
         """
 
 class ListUsersPaginator(Paginator):
@@ -178,27 +178,27 @@
 
     def paginate(
         self,
         *,
         UserPoolId: str,
         AttributesToGet: Sequence[str] = ...,
         Filter: str = ...,
-        PaginationConfig: "PaginatorConfigTypeDef" = ...
+        PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsersResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsers.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listuserspaginator)
         """
 
 class ListUsersInGroupPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listusersingrouppaginator)
     """
 
     def paginate(
-        self, *, UserPoolId: str, GroupName: str, PaginationConfig: "PaginatorConfigTypeDef" = ...
+        self, *, UserPoolId: str, GroupName: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListUsersInGroupResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider.Paginator.ListUsersInGroup.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/paginators/#listusersingrouppaginator)
         """
```

### Comparing `mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/type_defs.py` & `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -68,62 +68,59 @@
 __all__ = (
     "RecoveryOptionTypeTypeDef",
     "AccountTakeoverActionTypeTypeDef",
     "AdminAddUserToGroupRequestRequestTypeDef",
     "AdminConfirmSignUpRequestRequestTypeDef",
     "MessageTemplateTypeTypeDef",
     "AttributeTypeTypeDef",
+    "ResponseMetadataTypeDef",
     "AdminDeleteUserAttributesRequestRequestTypeDef",
     "AdminDeleteUserRequestRequestTypeDef",
     "ProviderUserIdentifierTypeTypeDef",
     "AdminDisableUserRequestRequestTypeDef",
     "AdminEnableUserRequestRequestTypeDef",
     "AdminForgetDeviceRequestRequestTypeDef",
     "AdminGetDeviceRequestRequestTypeDef",
     "AdminGetUserRequestRequestTypeDef",
     "MFAOptionTypeTypeDef",
     "AnalyticsMetadataTypeTypeDef",
     "AdminListDevicesRequestRequestTypeDef",
-    "AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "AdminListGroupsForUserRequestRequestTypeDef",
     "GroupTypeTypeDef",
-    "AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
     "AdminListUserAuthEventsRequestRequestTypeDef",
     "AdminRemoveUserFromGroupRequestRequestTypeDef",
     "AdminResetUserPasswordRequestRequestTypeDef",
     "SMSMfaSettingsTypeTypeDef",
     "SoftwareTokenMfaSettingsTypeTypeDef",
     "AdminSetUserPasswordRequestRequestTypeDef",
     "AdminUpdateAuthEventFeedbackRequestRequestTypeDef",
     "AdminUpdateDeviceStatusRequestRequestTypeDef",
     "AdminUserGlobalSignOutRequestRequestTypeDef",
     "AnalyticsConfigurationTypeTypeDef",
     "AssociateSoftwareTokenRequestRequestTypeDef",
-    "AssociateSoftwareTokenResponseTypeDef",
     "ChallengeResponseTypeTypeDef",
     "EventContextDataTypeTypeDef",
     "EventFeedbackTypeTypeDef",
     "EventRiskTypeTypeDef",
     "NewDeviceMetadataTypeTypeDef",
     "ChangePasswordRequestRequestTypeDef",
     "CodeDeliveryDetailsTypeTypeDef",
     "CompromisedCredentialsActionsTypeTypeDef",
     "DeviceSecretVerifierConfigTypeTypeDef",
-    "ConfirmDeviceResponseTypeDef",
     "UserContextDataTypeTypeDef",
     "HttpHeaderTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
     "IdentityProviderTypeTypeDef",
     "ResourceServerScopeTypeTypeDef",
     "CreateUserImportJobRequestRequestTypeDef",
     "UserImportJobTypeTypeDef",
     "TokenValidityUnitsTypeTypeDef",
     "CustomDomainConfigTypeTypeDef",
-    "CreateUserPoolDomainResponseTypeDef",
     "DeviceConfigurationTypeTypeDef",
     "EmailConfigurationTypeTypeDef",
     "SmsConfigurationTypeTypeDef",
     "UserAttributeUpdateSettingsTypeTypeDef",
     "UserPoolAddOnsTypeTypeDef",
     "UsernameConfigurationTypeTypeDef",
     "VerificationMessageTemplateTypeTypeDef",
@@ -140,85 +137,88 @@
     "DescribeIdentityProviderRequestRequestTypeDef",
     "DescribeResourceServerRequestRequestTypeDef",
     "DescribeRiskConfigurationRequestRequestTypeDef",
     "DescribeUserImportJobRequestRequestTypeDef",
     "DescribeUserPoolClientRequestRequestTypeDef",
     "DescribeUserPoolDomainRequestRequestTypeDef",
     "DescribeUserPoolRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ForgetDeviceRequestRequestTypeDef",
     "GetCSVHeaderRequestRequestTypeDef",
-    "GetCSVHeaderResponseTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GetIdentityProviderByIdentifierRequestRequestTypeDef",
     "GetSigningCertificateRequestRequestTypeDef",
-    "GetSigningCertificateResponseTypeDef",
     "GetUICustomizationRequestRequestTypeDef",
     "UICustomizationTypeTypeDef",
     "GetUserAttributeVerificationCodeRequestRequestTypeDef",
     "GetUserPoolMfaConfigRequestRequestTypeDef",
     "SoftwareTokenMfaConfigTypeTypeDef",
     "GetUserRequestRequestTypeDef",
     "GlobalSignOutRequestRequestTypeDef",
     "ListDevicesRequestRequestTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
     "ProviderDescriptionTypeDef",
-    "ListResourceServersRequestListResourceServersPaginateTypeDef",
     "ListResourceServersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListUserImportJobsRequestRequestTypeDef",
-    "ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
     "ListUserPoolClientsRequestRequestTypeDef",
     "UserPoolClientDescriptionTypeDef",
-    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
     "ListUserPoolsRequestRequestTypeDef",
-    "ListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
     "ListUsersInGroupRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "NotifyEmailTypeTypeDef",
     "NumberAttributeConstraintsTypeTypeDef",
-    "PaginatorConfigTypeDef",
     "PasswordPolicyTypeTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeTokenRequestRequestTypeDef",
     "RiskExceptionConfigurationTypeTypeDef",
     "StringAttributeConstraintsTypeTypeDef",
     "SetUICustomizationRequestRequestTypeDef",
     "StartUserImportJobRequestRequestTypeDef",
     "StopUserImportJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuthEventFeedbackRequestRequestTypeDef",
     "UpdateDeviceStatusRequestRequestTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
-    "UpdateUserPoolDomainResponseTypeDef",
     "VerifySoftwareTokenRequestRequestTypeDef",
-    "VerifySoftwareTokenResponseTypeDef",
     "VerifyUserAttributeRequestRequestTypeDef",
     "AccountRecoverySettingTypeTypeDef",
     "AccountTakeoverActionsTypeTypeDef",
     "AdminCreateUserConfigTypeTypeDef",
     "AdminCreateUserRequestRequestTypeDef",
     "AdminUpdateUserAttributesRequestRequestTypeDef",
     "DeviceTypeTypeDef",
     "UpdateUserAttributesRequestRequestTypeDef",
+    "AssociateSoftwareTokenResponseTypeDef",
+    "ConfirmDeviceResponseTypeDef",
+    "CreateUserPoolDomainResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCSVHeaderResponseTypeDef",
+    "GetSigningCertificateResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateUserPoolDomainResponseTypeDef",
+    "VerifySoftwareTokenResponseTypeDef",
     "AdminDisableProviderForUserRequestRequestTypeDef",
     "AdminLinkProviderForUserRequestRequestTypeDef",
     "AdminGetUserResponseTypeDef",
     "AdminSetUserSettingsRequestRequestTypeDef",
     "GetUserResponseTypeDef",
     "SetUserSettingsRequestRequestTypeDef",
     "UserTypeTypeDef",
+    "AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    "AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    "ListResourceServersRequestListResourceServersPaginateTypeDef",
+    "ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
+    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
+    "ListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "AdminListGroupsForUserResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "GetGroupResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "UpdateGroupResponseTypeDef",
     "AdminSetUserMFAPreferenceRequestRequestTypeDef",
     "SetUserMFAPreferenceRequestRequestTypeDef",
@@ -379,14 +379,25 @@
 )
 
 
 class AttributeTypeTypeDef(_RequiredAttributeTypeTypeDef, _OptionalAttributeTypeTypeDef):
     pass
 
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 AdminDeleteUserAttributesRequestRequestTypeDef = TypedDict(
     "AdminDeleteUserAttributesRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
         "UserAttributeNames": Sequence[str],
     },
@@ -488,37 +499,24 @@
 
 class AdminListDevicesRequestRequestTypeDef(
     _RequiredAdminListDevicesRequestRequestTypeDef, _OptionalAdminListDevicesRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
-    "_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
-    {
-        "Username": str,
-        "UserPoolId": str,
-    },
-)
-_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
-    "_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-
-class AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef(
-    _RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
-    _OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
-):
-    pass
-
-
 _RequiredAdminListGroupsForUserRequestRequestTypeDef = TypedDict(
     "_RequiredAdminListGroupsForUserRequestRequestTypeDef",
     {
         "Username": str,
         "UserPoolId": str,
     },
 )
@@ -549,37 +547,14 @@
         "Precedence": int,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
     total=False,
 )
 
-_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
-    "_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-        "Username": str,
-    },
-)
-_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
-    "_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef(
-    _RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
-    _OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredAdminListUserAuthEventsRequestRequestTypeDef = TypedDict(
     "_RequiredAdminListUserAuthEventsRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
     },
 )
@@ -733,23 +708,14 @@
     {
         "AccessToken": str,
         "Session": str,
     },
     total=False,
 )
 
-AssociateSoftwareTokenResponseTypeDef = TypedDict(
-    "AssociateSoftwareTokenResponseTypeDef",
-    {
-        "SecretCode": str,
-        "Session": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ChallengeResponseTypeTypeDef = TypedDict(
     "ChallengeResponseTypeTypeDef",
     {
         "ChallengeName": ChallengeNameType,
         "ChallengeResponse": ChallengeResponseType,
     },
     total=False,
@@ -839,22 +805,14 @@
     {
         "PasswordVerifier": str,
         "Salt": str,
     },
     total=False,
 )
 
-ConfirmDeviceResponseTypeDef = TypedDict(
-    "ConfirmDeviceResponseTypeDef",
-    {
-        "UserConfirmationNecessary": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UserContextDataTypeTypeDef = TypedDict(
     "UserContextDataTypeTypeDef",
     {
         "IpAddress": str,
         "EncodedData": str,
     },
     total=False,
@@ -984,22 +942,14 @@
 CustomDomainConfigTypeTypeDef = TypedDict(
     "CustomDomainConfigTypeTypeDef",
     {
         "CertificateArn": str,
     },
 )
 
-CreateUserPoolDomainResponseTypeDef = TypedDict(
-    "CreateUserPoolDomainResponseTypeDef",
-    {
-        "CloudFrontDomain": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceConfigurationTypeTypeDef = TypedDict(
     "DeviceConfigurationTypeTypeDef",
     {
         "ChallengeRequiredOnNewDevice": bool,
         "DeviceOnlyRememberedOnUserPrompt": bool,
     },
     total=False,
@@ -1216,21 +1166,14 @@
 DescribeUserPoolRequestRequestTypeDef = TypedDict(
     "DescribeUserPoolRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredForgetDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredForgetDeviceRequestRequestTypeDef",
     {
         "DeviceKey": str,
     },
 )
 _OptionalForgetDeviceRequestRequestTypeDef = TypedDict(
@@ -1251,23 +1194,14 @@
 GetCSVHeaderRequestRequestTypeDef = TypedDict(
     "GetCSVHeaderRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
-GetCSVHeaderResponseTypeDef = TypedDict(
-    "GetCSVHeaderResponseTypeDef",
-    {
-        "UserPoolId": str,
-        "CSVHeader": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeviceRequestRequestTypeDef",
     {
         "DeviceKey": str,
     },
 )
 _OptionalGetDeviceRequestRequestTypeDef = TypedDict(
@@ -1304,22 +1238,14 @@
 GetSigningCertificateRequestRequestTypeDef = TypedDict(
     "GetSigningCertificateRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
-GetSigningCertificateResponseTypeDef = TypedDict(
-    "GetSigningCertificateResponseTypeDef",
-    {
-        "Certificate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetUICustomizationRequestRequestTypeDef = TypedDict(
     "_RequiredGetUICustomizationRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalGetUICustomizationRequestRequestTypeDef = TypedDict(
@@ -1422,36 +1348,14 @@
 
 class ListDevicesRequestRequestTypeDef(
     _RequiredListDevicesRequestRequestTypeDef, _OptionalListDevicesRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListGroupsRequestListGroupsPaginateTypeDef(
-    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
-    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupsRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListGroupsRequestRequestTypeDef = TypedDict(
@@ -1466,36 +1370,14 @@
 
 class ListGroupsRequestRequestTypeDef(
     _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef(
-    _RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    _OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListIdentityProvidersRequestRequestTypeDef = TypedDict(
     "_RequiredListIdentityProvidersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListIdentityProvidersRequestRequestTypeDef = TypedDict(
@@ -1522,36 +1404,14 @@
         "ProviderType": IdentityProviderTypeTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
     total=False,
 )
 
-_RequiredListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
-    "_RequiredListResourceServersRequestListResourceServersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
-    "_OptionalListResourceServersRequestListResourceServersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListResourceServersRequestListResourceServersPaginateTypeDef(
-    _RequiredListResourceServersRequestListResourceServersPaginateTypeDef,
-    _OptionalListResourceServersRequestListResourceServersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListResourceServersRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceServersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListResourceServersRequestRequestTypeDef = TypedDict(
@@ -1574,22 +1434,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListUserImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserImportJobsRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "MaxResults": int,
     },
 )
@@ -1605,36 +1457,14 @@
 class ListUserImportJobsRequestRequestTypeDef(
     _RequiredListUserImportJobsRequestRequestTypeDef,
     _OptionalListUserImportJobsRequestRequestTypeDef,
 ):
     pass
 
 
-_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
-    "_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
-    "_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef(
-    _RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
-    _OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUserPoolClientsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserPoolClientsRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListUserPoolClientsRequestRequestTypeDef = TypedDict(
@@ -1660,22 +1490,14 @@
         "ClientId": str,
         "UserPoolId": str,
         "ClientName": str,
     },
     total=False,
 )
 
-ListUserPoolsRequestListUserPoolsPaginateTypeDef = TypedDict(
-    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 _RequiredListUserPoolsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserPoolsRequestRequestTypeDef",
     {
         "MaxResults": int,
     },
 )
 _OptionalListUserPoolsRequestRequestTypeDef = TypedDict(
@@ -1689,37 +1511,14 @@
 
 class ListUserPoolsRequestRequestTypeDef(
     _RequiredListUserPoolsRequestRequestTypeDef, _OptionalListUserPoolsRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
-    "_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
-    {
-        "UserPoolId": str,
-        "GroupName": str,
-    },
-)
-_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
-    "_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUsersInGroupRequestListUsersInGroupPaginateTypeDef(
-    _RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
-    _OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUsersInGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersInGroupRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "GroupName": str,
     },
 )
@@ -1735,38 +1534,14 @@
 
 class ListUsersInGroupRequestRequestTypeDef(
     _RequiredListUsersInGroupRequestRequestTypeDef, _OptionalListUsersInGroupRequestRequestTypeDef
 ):
     pass
 
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "AttributesToGet": Sequence[str],
-        "Filter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -1812,48 +1587,27 @@
     {
         "MinValue": str,
         "MaxValue": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PasswordPolicyTypeTypeDef = TypedDict(
     "PasswordPolicyTypeTypeDef",
     {
         "MinimumLength": int,
         "RequireUppercase": bool,
         "RequireLowercase": bool,
         "RequireNumbers": bool,
         "RequireSymbols": bool,
         "TemporaryPasswordValidityDays": int,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredRevokeTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRevokeTokenRequestRequestTypeDef",
     {
         "Token": str,
         "ClientId": str,
     },
 )
@@ -2025,22 +1779,14 @@
 class UpdateIdentityProviderRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
 
-UpdateUserPoolDomainResponseTypeDef = TypedDict(
-    "UpdateUserPoolDomainResponseTypeDef",
-    {
-        "CloudFrontDomain": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredVerifySoftwareTokenRequestRequestTypeDef = TypedDict(
     "_RequiredVerifySoftwareTokenRequestRequestTypeDef",
     {
         "UserCode": str,
     },
 )
 _OptionalVerifySoftwareTokenRequestRequestTypeDef = TypedDict(
@@ -2057,23 +1803,14 @@
 class VerifySoftwareTokenRequestRequestTypeDef(
     _RequiredVerifySoftwareTokenRequestRequestTypeDef,
     _OptionalVerifySoftwareTokenRequestRequestTypeDef,
 ):
     pass
 
 
-VerifySoftwareTokenResponseTypeDef = TypedDict(
-    "VerifySoftwareTokenResponseTypeDef",
-    {
-        "Status": VerifySoftwareTokenResponseTypeType,
-        "Session": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VerifyUserAttributeRequestRequestTypeDef = TypedDict(
     "VerifyUserAttributeRequestRequestTypeDef",
     {
         "AccessToken": str,
         "AttributeName": str,
         "Code": str,
     },
@@ -2190,14 +1927,88 @@
 class UpdateUserAttributesRequestRequestTypeDef(
     _RequiredUpdateUserAttributesRequestRequestTypeDef,
     _OptionalUpdateUserAttributesRequestRequestTypeDef,
 ):
     pass
 
 
+AssociateSoftwareTokenResponseTypeDef = TypedDict(
+    "AssociateSoftwareTokenResponseTypeDef",
+    {
+        "SecretCode": str,
+        "Session": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmDeviceResponseTypeDef = TypedDict(
+    "ConfirmDeviceResponseTypeDef",
+    {
+        "UserConfirmationNecessary": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserPoolDomainResponseTypeDef = TypedDict(
+    "CreateUserPoolDomainResponseTypeDef",
+    {
+        "CloudFrontDomain": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCSVHeaderResponseTypeDef = TypedDict(
+    "GetCSVHeaderResponseTypeDef",
+    {
+        "UserPoolId": str,
+        "CSVHeader": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSigningCertificateResponseTypeDef = TypedDict(
+    "GetSigningCertificateResponseTypeDef",
+    {
+        "Certificate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateUserPoolDomainResponseTypeDef = TypedDict(
+    "UpdateUserPoolDomainResponseTypeDef",
+    {
+        "CloudFrontDomain": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifySoftwareTokenResponseTypeDef = TypedDict(
+    "VerifySoftwareTokenResponseTypeDef",
+    {
+        "Status": VerifySoftwareTokenResponseTypeType,
+        "Session": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AdminDisableProviderForUserRequestRequestTypeDef = TypedDict(
     "AdminDisableProviderForUserRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "User": ProviderUserIdentifierTypeTypeDef,
     },
 )
@@ -2219,15 +2030,15 @@
         "UserCreateDate": datetime,
         "UserLastModifiedDate": datetime,
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
         "MFAOptions": List[MFAOptionTypeTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminSetUserSettingsRequestRequestTypeDef = TypedDict(
     "AdminSetUserSettingsRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -2240,15 +2051,15 @@
     "GetUserResponseTypeDef",
     {
         "Username": str,
         "UserAttributes": List[AttributeTypeTypeDef],
         "MFAOptions": List[MFAOptionTypeTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetUserSettingsRequestRequestTypeDef = TypedDict(
     "SetUserSettingsRequestRequestTypeDef",
     {
         "AccessToken": str,
@@ -2266,53 +2077,242 @@
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
         "MFAOptions": List[MFAOptionTypeTypeDef],
     },
     total=False,
 )
 
+_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
+    "_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    {
+        "Username": str,
+        "UserPoolId": str,
+    },
+)
+_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
+    "_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef(
+    _RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    _OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+):
+    pass
+
+
+_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
+    "_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+        "Username": str,
+    },
+)
+_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
+    "_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef(
+    _RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+    _OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListGroupsRequestListGroupsPaginateTypeDef(
+    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
+    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef(
+    _RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    _OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
+    "_RequiredListResourceServersRequestListResourceServersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
+    "_OptionalListResourceServersRequestListResourceServersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListResourceServersRequestListResourceServersPaginateTypeDef(
+    _RequiredListResourceServersRequestListResourceServersPaginateTypeDef,
+    _OptionalListResourceServersRequestListResourceServersPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
+    "_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
+    "_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef(
+    _RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+    _OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+):
+    pass
+
+
+ListUserPoolsRequestListUserPoolsPaginateTypeDef = TypedDict(
+    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
+    "_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
+    {
+        "UserPoolId": str,
+        "GroupName": str,
+    },
+)
+_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
+    "_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUsersInGroupRequestListUsersInGroupPaginateTypeDef(
+    _RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+    _OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+):
+    pass
+
+
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "AttributesToGet": Sequence[str],
+        "Filter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
+
 AdminListGroupsForUserResponseTypeDef = TypedDict(
     "AdminListGroupsForUserResponseTypeDef",
     {
         "Groups": List[GroupTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupResponseTypeDef = TypedDict(
     "GetGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGroupResponseTypeDef = TypedDict(
     "UpdateGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef = TypedDict(
     "_RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef",
     {
         "Username": str,
@@ -2387,49 +2387,49 @@
     total=False,
 )
 
 ForgotPasswordResponseTypeDef = TypedDict(
     "ForgotPasswordResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserAttributeVerificationCodeResponseTypeDef = TypedDict(
     "GetUserAttributeVerificationCodeResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResendConfirmationCodeResponseTypeDef = TypedDict(
     "ResendConfirmationCodeResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SignUpResponseTypeDef = TypedDict(
     "SignUpResponseTypeDef",
     {
         "UserConfirmed": bool,
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
         "UserSub": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserAttributesResponseTypeDef = TypedDict(
     "UpdateUserAttributesResponseTypeDef",
     {
         "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
     "_RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
         "Actions": CompromisedCredentialsActionsTypeTypeDef,
@@ -2682,39 +2682,39 @@
     pass
 
 
 CreateIdentityProviderResponseTypeDef = TypedDict(
     "CreateIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeIdentityProviderResponseTypeDef = TypedDict(
     "DescribeIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentityProviderByIdentifierResponseTypeDef = TypedDict(
     "GetIdentityProviderByIdentifierResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIdentityProviderResponseTypeDef = TypedDict(
     "UpdateIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateResourceServerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceServerRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -2773,48 +2773,48 @@
     pass
 
 
 CreateUserImportJobResponseTypeDef = TypedDict(
     "CreateUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserImportJobResponseTypeDef = TypedDict(
     "DescribeUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserImportJobsResponseTypeDef = TypedDict(
     "ListUserImportJobsResponseTypeDef",
     {
         "UserImportJobs": List[UserImportJobTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartUserImportJobResponseTypeDef = TypedDict(
     "StartUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopUserImportJobResponseTypeDef = TypedDict(
     "StopUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUserPoolClientRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserPoolClientRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -3006,41 +3006,41 @@
     total=False,
 )
 
 GetUICustomizationResponseTypeDef = TypedDict(
     "GetUICustomizationResponseTypeDef",
     {
         "UICustomization": UICustomizationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetUICustomizationResponseTypeDef = TypedDict(
     "SetUICustomizationResponseTypeDef",
     {
         "UICustomization": UICustomizationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "Providers": List[ProviderDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserPoolClientsResponseTypeDef = TypedDict(
     "ListUserPoolClientsResponseTypeDef",
     {
         "UserPoolClients": List[UserPoolClientDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredNotifyConfigurationTypeTypeDef = TypedDict(
     "_RequiredNotifyConfigurationTypeTypeDef",
     {
         "SourceArn": str,
@@ -3087,120 +3087,120 @@
     total=False,
 )
 
 AdminGetDeviceResponseTypeDef = TypedDict(
     "AdminGetDeviceResponseTypeDef",
     {
         "Device": DeviceTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminListDevicesResponseTypeDef = TypedDict(
     "AdminListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeviceResponseTypeDef = TypedDict(
     "GetDeviceResponseTypeDef",
     {
         "Device": DeviceTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminCreateUserResponseTypeDef = TypedDict(
     "AdminCreateUserResponseTypeDef",
     {
         "User": UserTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersInGroupResponseTypeDef = TypedDict(
     "ListUsersInGroupResponseTypeDef",
     {
         "Users": List[UserTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminListUserAuthEventsResponseTypeDef = TypedDict(
     "AdminListUserAuthEventsResponseTypeDef",
     {
         "AuthEvents": List[AuthEventTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminInitiateAuthResponseTypeDef = TypedDict(
     "AdminInitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminRespondToAuthChallengeResponseTypeDef = TypedDict(
     "AdminRespondToAuthChallengeResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InitiateAuthResponseTypeDef = TypedDict(
     "InitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RespondToAuthChallengeResponseTypeDef = TypedDict(
     "RespondToAuthChallengeResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAdminInitiateAuthRequestRequestTypeDef = TypedDict(
     "_RequiredAdminInitiateAuthRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -3254,82 +3254,82 @@
     pass
 
 
 CreateResourceServerResponseTypeDef = TypedDict(
     "CreateResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeResourceServerResponseTypeDef = TypedDict(
     "DescribeResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceServersResponseTypeDef = TypedDict(
     "ListResourceServersResponseTypeDef",
     {
         "ResourceServers": List[ResourceServerTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResourceServerResponseTypeDef = TypedDict(
     "UpdateResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateUserPoolClientResponseTypeDef = TypedDict(
     "CreateUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserPoolClientResponseTypeDef = TypedDict(
     "DescribeUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserPoolClientResponseTypeDef = TypedDict(
     "UpdateUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserPoolDomainResponseTypeDef = TypedDict(
     "DescribeUserPoolDomainResponseTypeDef",
     {
         "DomainDescription": DomainDescriptionTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserPoolMfaConfigResponseTypeDef = TypedDict(
     "GetUserPoolMfaConfigResponseTypeDef",
     {
         "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSetUserPoolMfaConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSetUserPoolMfaConfigRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -3355,15 +3355,15 @@
 
 SetUserPoolMfaConfigResponseTypeDef = TypedDict(
     "SetUserPoolMfaConfigResponseTypeDef",
     {
         "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserPoolDescriptionTypeTypeDef = TypedDict(
     "UserPoolDescriptionTypeTypeDef",
     {
         "Id": str,
@@ -3527,15 +3527,15 @@
 )
 
 ListUserPoolsResponseTypeDef = TypedDict(
     "ListUserPoolsResponseTypeDef",
     {
         "UserPools": List[UserPoolDescriptionTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RiskConfigurationTypeTypeDef = TypedDict(
     "RiskConfigurationTypeTypeDef",
     {
         "UserPoolId": str,
@@ -3577,34 +3577,34 @@
     pass
 
 
 CreateUserPoolResponseTypeDef = TypedDict(
     "CreateUserPoolResponseTypeDef",
     {
         "UserPool": UserPoolTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserPoolResponseTypeDef = TypedDict(
     "DescribeUserPoolResponseTypeDef",
     {
         "UserPool": UserPoolTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRiskConfigurationResponseTypeDef = TypedDict(
     "DescribeRiskConfigurationResponseTypeDef",
     {
         "RiskConfiguration": RiskConfigurationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetRiskConfigurationResponseTypeDef = TypedDict(
     "SetRiskConfigurationResponseTypeDef",
     {
         "RiskConfiguration": RiskConfigurationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp/type_defs.pyi` & `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -67,62 +67,59 @@
 __all__ = (
     "RecoveryOptionTypeTypeDef",
     "AccountTakeoverActionTypeTypeDef",
     "AdminAddUserToGroupRequestRequestTypeDef",
     "AdminConfirmSignUpRequestRequestTypeDef",
     "MessageTemplateTypeTypeDef",
     "AttributeTypeTypeDef",
+    "ResponseMetadataTypeDef",
     "AdminDeleteUserAttributesRequestRequestTypeDef",
     "AdminDeleteUserRequestRequestTypeDef",
     "ProviderUserIdentifierTypeTypeDef",
     "AdminDisableUserRequestRequestTypeDef",
     "AdminEnableUserRequestRequestTypeDef",
     "AdminForgetDeviceRequestRequestTypeDef",
     "AdminGetDeviceRequestRequestTypeDef",
     "AdminGetUserRequestRequestTypeDef",
     "MFAOptionTypeTypeDef",
     "AnalyticsMetadataTypeTypeDef",
     "AdminListDevicesRequestRequestTypeDef",
-    "AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    "PaginatorConfigTypeDef",
     "AdminListGroupsForUserRequestRequestTypeDef",
     "GroupTypeTypeDef",
-    "AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
     "AdminListUserAuthEventsRequestRequestTypeDef",
     "AdminRemoveUserFromGroupRequestRequestTypeDef",
     "AdminResetUserPasswordRequestRequestTypeDef",
     "SMSMfaSettingsTypeTypeDef",
     "SoftwareTokenMfaSettingsTypeTypeDef",
     "AdminSetUserPasswordRequestRequestTypeDef",
     "AdminUpdateAuthEventFeedbackRequestRequestTypeDef",
     "AdminUpdateDeviceStatusRequestRequestTypeDef",
     "AdminUserGlobalSignOutRequestRequestTypeDef",
     "AnalyticsConfigurationTypeTypeDef",
     "AssociateSoftwareTokenRequestRequestTypeDef",
-    "AssociateSoftwareTokenResponseTypeDef",
     "ChallengeResponseTypeTypeDef",
     "EventContextDataTypeTypeDef",
     "EventFeedbackTypeTypeDef",
     "EventRiskTypeTypeDef",
     "NewDeviceMetadataTypeTypeDef",
     "ChangePasswordRequestRequestTypeDef",
     "CodeDeliveryDetailsTypeTypeDef",
     "CompromisedCredentialsActionsTypeTypeDef",
     "DeviceSecretVerifierConfigTypeTypeDef",
-    "ConfirmDeviceResponseTypeDef",
     "UserContextDataTypeTypeDef",
     "HttpHeaderTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "CreateIdentityProviderRequestRequestTypeDef",
     "IdentityProviderTypeTypeDef",
     "ResourceServerScopeTypeTypeDef",
     "CreateUserImportJobRequestRequestTypeDef",
     "UserImportJobTypeTypeDef",
     "TokenValidityUnitsTypeTypeDef",
     "CustomDomainConfigTypeTypeDef",
-    "CreateUserPoolDomainResponseTypeDef",
     "DeviceConfigurationTypeTypeDef",
     "EmailConfigurationTypeTypeDef",
     "SmsConfigurationTypeTypeDef",
     "UserAttributeUpdateSettingsTypeTypeDef",
     "UserPoolAddOnsTypeTypeDef",
     "UsernameConfigurationTypeTypeDef",
     "VerificationMessageTemplateTypeTypeDef",
@@ -139,85 +136,88 @@
     "DescribeIdentityProviderRequestRequestTypeDef",
     "DescribeResourceServerRequestRequestTypeDef",
     "DescribeRiskConfigurationRequestRequestTypeDef",
     "DescribeUserImportJobRequestRequestTypeDef",
     "DescribeUserPoolClientRequestRequestTypeDef",
     "DescribeUserPoolDomainRequestRequestTypeDef",
     "DescribeUserPoolRequestRequestTypeDef",
-    "EmptyResponseMetadataTypeDef",
     "ForgetDeviceRequestRequestTypeDef",
     "GetCSVHeaderRequestRequestTypeDef",
-    "GetCSVHeaderResponseTypeDef",
     "GetDeviceRequestRequestTypeDef",
     "GetGroupRequestRequestTypeDef",
     "GetIdentityProviderByIdentifierRequestRequestTypeDef",
     "GetSigningCertificateRequestRequestTypeDef",
-    "GetSigningCertificateResponseTypeDef",
     "GetUICustomizationRequestRequestTypeDef",
     "UICustomizationTypeTypeDef",
     "GetUserAttributeVerificationCodeRequestRequestTypeDef",
     "GetUserPoolMfaConfigRequestRequestTypeDef",
     "SoftwareTokenMfaConfigTypeTypeDef",
     "GetUserRequestRequestTypeDef",
     "GlobalSignOutRequestRequestTypeDef",
     "ListDevicesRequestRequestTypeDef",
-    "ListGroupsRequestListGroupsPaginateTypeDef",
     "ListGroupsRequestRequestTypeDef",
-    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
     "ListIdentityProvidersRequestRequestTypeDef",
     "ProviderDescriptionTypeDef",
-    "ListResourceServersRequestListResourceServersPaginateTypeDef",
     "ListResourceServersRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
-    "ListTagsForResourceResponseTypeDef",
     "ListUserImportJobsRequestRequestTypeDef",
-    "ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
     "ListUserPoolClientsRequestRequestTypeDef",
     "UserPoolClientDescriptionTypeDef",
-    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
     "ListUserPoolsRequestRequestTypeDef",
-    "ListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
     "ListUsersInGroupRequestRequestTypeDef",
-    "ListUsersRequestListUsersPaginateTypeDef",
     "ListUsersRequestRequestTypeDef",
     "NotifyEmailTypeTypeDef",
     "NumberAttributeConstraintsTypeTypeDef",
-    "PaginatorConfigTypeDef",
     "PasswordPolicyTypeTypeDef",
-    "ResponseMetadataTypeDef",
     "RevokeTokenRequestRequestTypeDef",
     "RiskExceptionConfigurationTypeTypeDef",
     "StringAttributeConstraintsTypeTypeDef",
     "SetUICustomizationRequestRequestTypeDef",
     "StartUserImportJobRequestRequestTypeDef",
     "StopUserImportJobRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAuthEventFeedbackRequestRequestTypeDef",
     "UpdateDeviceStatusRequestRequestTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateIdentityProviderRequestRequestTypeDef",
-    "UpdateUserPoolDomainResponseTypeDef",
     "VerifySoftwareTokenRequestRequestTypeDef",
-    "VerifySoftwareTokenResponseTypeDef",
     "VerifyUserAttributeRequestRequestTypeDef",
     "AccountRecoverySettingTypeTypeDef",
     "AccountTakeoverActionsTypeTypeDef",
     "AdminCreateUserConfigTypeTypeDef",
     "AdminCreateUserRequestRequestTypeDef",
     "AdminUpdateUserAttributesRequestRequestTypeDef",
     "DeviceTypeTypeDef",
     "UpdateUserAttributesRequestRequestTypeDef",
+    "AssociateSoftwareTokenResponseTypeDef",
+    "ConfirmDeviceResponseTypeDef",
+    "CreateUserPoolDomainResponseTypeDef",
+    "EmptyResponseMetadataTypeDef",
+    "GetCSVHeaderResponseTypeDef",
+    "GetSigningCertificateResponseTypeDef",
+    "ListTagsForResourceResponseTypeDef",
+    "UpdateUserPoolDomainResponseTypeDef",
+    "VerifySoftwareTokenResponseTypeDef",
     "AdminDisableProviderForUserRequestRequestTypeDef",
     "AdminLinkProviderForUserRequestRequestTypeDef",
     "AdminGetUserResponseTypeDef",
     "AdminSetUserSettingsRequestRequestTypeDef",
     "GetUserResponseTypeDef",
     "SetUserSettingsRequestRequestTypeDef",
     "UserTypeTypeDef",
+    "AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    "AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
+    "ListGroupsRequestListGroupsPaginateTypeDef",
+    "ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    "ListResourceServersRequestListResourceServersPaginateTypeDef",
+    "ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
+    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
+    "ListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
+    "ListUsersRequestListUsersPaginateTypeDef",
     "AdminListGroupsForUserResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "GetGroupResponseTypeDef",
     "ListGroupsResponseTypeDef",
     "UpdateGroupResponseTypeDef",
     "AdminSetUserMFAPreferenceRequestRequestTypeDef",
     "SetUserMFAPreferenceRequestRequestTypeDef",
@@ -374,14 +374,25 @@
     },
     total=False,
 )
 
 class AttributeTypeTypeDef(_RequiredAttributeTypeTypeDef, _OptionalAttributeTypeTypeDef):
     pass
 
+ResponseMetadataTypeDef = TypedDict(
+    "ResponseMetadataTypeDef",
+    {
+        "RequestId": str,
+        "HostId": str,
+        "HTTPStatusCode": int,
+        "HTTPHeaders": Dict[str, str],
+        "RetryAttempts": int,
+    },
+)
+
 AdminDeleteUserAttributesRequestRequestTypeDef = TypedDict(
     "AdminDeleteUserAttributesRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
         "UserAttributeNames": Sequence[str],
     },
@@ -481,35 +492,24 @@
 )
 
 class AdminListDevicesRequestRequestTypeDef(
     _RequiredAdminListDevicesRequestRequestTypeDef, _OptionalAdminListDevicesRequestRequestTypeDef
 ):
     pass
 
-_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
-    "_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
-    {
-        "Username": str,
-        "UserPoolId": str,
-    },
-)
-_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
-    "_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+PaginatorConfigTypeDef = TypedDict(
+    "PaginatorConfigTypeDef",
     {
-        "PaginationConfig": "PaginatorConfigTypeDef",
+        "MaxItems": int,
+        "PageSize": int,
+        "StartingToken": str,
     },
     total=False,
 )
 
-class AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef(
-    _RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
-    _OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
-):
-    pass
-
 _RequiredAdminListGroupsForUserRequestRequestTypeDef = TypedDict(
     "_RequiredAdminListGroupsForUserRequestRequestTypeDef",
     {
         "Username": str,
         "UserPoolId": str,
     },
 )
@@ -538,35 +538,14 @@
         "Precedence": int,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
     total=False,
 )
 
-_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
-    "_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-        "Username": str,
-    },
-)
-_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
-    "_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef(
-    _RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
-    _OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
-):
-    pass
-
 _RequiredAdminListUserAuthEventsRequestRequestTypeDef = TypedDict(
     "_RequiredAdminListUserAuthEventsRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "Username": str,
     },
 )
@@ -712,23 +691,14 @@
     {
         "AccessToken": str,
         "Session": str,
     },
     total=False,
 )
 
-AssociateSoftwareTokenResponseTypeDef = TypedDict(
-    "AssociateSoftwareTokenResponseTypeDef",
-    {
-        "SecretCode": str,
-        "Session": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 ChallengeResponseTypeTypeDef = TypedDict(
     "ChallengeResponseTypeTypeDef",
     {
         "ChallengeName": ChallengeNameType,
         "ChallengeResponse": ChallengeResponseType,
     },
     total=False,
@@ -816,22 +786,14 @@
     {
         "PasswordVerifier": str,
         "Salt": str,
     },
     total=False,
 )
 
-ConfirmDeviceResponseTypeDef = TypedDict(
-    "ConfirmDeviceResponseTypeDef",
-    {
-        "UserConfirmationNecessary": bool,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 UserContextDataTypeTypeDef = TypedDict(
     "UserContextDataTypeTypeDef",
     {
         "IpAddress": str,
         "EncodedData": str,
     },
     total=False,
@@ -957,22 +919,14 @@
 CustomDomainConfigTypeTypeDef = TypedDict(
     "CustomDomainConfigTypeTypeDef",
     {
         "CertificateArn": str,
     },
 )
 
-CreateUserPoolDomainResponseTypeDef = TypedDict(
-    "CreateUserPoolDomainResponseTypeDef",
-    {
-        "CloudFrontDomain": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 DeviceConfigurationTypeTypeDef = TypedDict(
     "DeviceConfigurationTypeTypeDef",
     {
         "ChallengeRequiredOnNewDevice": bool,
         "DeviceOnlyRememberedOnUserPrompt": bool,
     },
     total=False,
@@ -1185,21 +1139,14 @@
 DescribeUserPoolRequestRequestTypeDef = TypedDict(
     "DescribeUserPoolRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
-EmptyResponseMetadataTypeDef = TypedDict(
-    "EmptyResponseMetadataTypeDef",
-    {
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredForgetDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredForgetDeviceRequestRequestTypeDef",
     {
         "DeviceKey": str,
     },
 )
 _OptionalForgetDeviceRequestRequestTypeDef = TypedDict(
@@ -1218,23 +1165,14 @@
 GetCSVHeaderRequestRequestTypeDef = TypedDict(
     "GetCSVHeaderRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
-GetCSVHeaderResponseTypeDef = TypedDict(
-    "GetCSVHeaderResponseTypeDef",
-    {
-        "UserPoolId": str,
-        "CSVHeader": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetDeviceRequestRequestTypeDef = TypedDict(
     "_RequiredGetDeviceRequestRequestTypeDef",
     {
         "DeviceKey": str,
     },
 )
 _OptionalGetDeviceRequestRequestTypeDef = TypedDict(
@@ -1269,22 +1207,14 @@
 GetSigningCertificateRequestRequestTypeDef = TypedDict(
     "GetSigningCertificateRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 
-GetSigningCertificateResponseTypeDef = TypedDict(
-    "GetSigningCertificateResponseTypeDef",
-    {
-        "Certificate": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredGetUICustomizationRequestRequestTypeDef = TypedDict(
     "_RequiredGetUICustomizationRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalGetUICustomizationRequestRequestTypeDef = TypedDict(
@@ -1381,34 +1311,14 @@
 )
 
 class ListDevicesRequestRequestTypeDef(
     _RequiredListDevicesRequestRequestTypeDef, _OptionalListDevicesRequestRequestTypeDef
 ):
     pass
 
-_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
-    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListGroupsRequestListGroupsPaginateTypeDef(
-    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
-    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
-):
-    pass
-
 _RequiredListGroupsRequestRequestTypeDef = TypedDict(
     "_RequiredListGroupsRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListGroupsRequestRequestTypeDef = TypedDict(
@@ -1421,34 +1331,14 @@
 )
 
 class ListGroupsRequestRequestTypeDef(
     _RequiredListGroupsRequestRequestTypeDef, _OptionalListGroupsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
-    "_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef(
-    _RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-    _OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
-):
-    pass
-
 _RequiredListIdentityProvidersRequestRequestTypeDef = TypedDict(
     "_RequiredListIdentityProvidersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListIdentityProvidersRequestRequestTypeDef = TypedDict(
@@ -1473,34 +1363,14 @@
         "ProviderType": IdentityProviderTypeTypeType,
         "LastModifiedDate": datetime,
         "CreationDate": datetime,
     },
     total=False,
 )
 
-_RequiredListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
-    "_RequiredListResourceServersRequestListResourceServersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
-    "_OptionalListResourceServersRequestListResourceServersPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListResourceServersRequestListResourceServersPaginateTypeDef(
-    _RequiredListResourceServersRequestListResourceServersPaginateTypeDef,
-    _OptionalListResourceServersRequestListResourceServersPaginateTypeDef,
-):
-    pass
-
 _RequiredListResourceServersRequestRequestTypeDef = TypedDict(
     "_RequiredListResourceServersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListResourceServersRequestRequestTypeDef = TypedDict(
@@ -1521,22 +1391,14 @@
 ListTagsForResourceRequestRequestTypeDef = TypedDict(
     "ListTagsForResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
     },
 )
 
-ListTagsForResourceResponseTypeDef = TypedDict(
-    "ListTagsForResourceResponseTypeDef",
-    {
-        "Tags": Dict[str, str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredListUserImportJobsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserImportJobsRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "MaxResults": int,
     },
 )
@@ -1550,34 +1412,14 @@
 
 class ListUserImportJobsRequestRequestTypeDef(
     _RequiredListUserImportJobsRequestRequestTypeDef,
     _OptionalListUserImportJobsRequestRequestTypeDef,
 ):
     pass
 
-_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
-    "_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
-    "_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef(
-    _RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
-    _OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
-):
-    pass
-
 _RequiredListUserPoolClientsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserPoolClientsRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListUserPoolClientsRequestRequestTypeDef = TypedDict(
@@ -1601,22 +1443,14 @@
         "ClientId": str,
         "UserPoolId": str,
         "ClientName": str,
     },
     total=False,
 )
 
-ListUserPoolsRequestListUserPoolsPaginateTypeDef = TypedDict(
-    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
 _RequiredListUserPoolsRequestRequestTypeDef = TypedDict(
     "_RequiredListUserPoolsRequestRequestTypeDef",
     {
         "MaxResults": int,
     },
 )
 _OptionalListUserPoolsRequestRequestTypeDef = TypedDict(
@@ -1628,35 +1462,14 @@
 )
 
 class ListUserPoolsRequestRequestTypeDef(
     _RequiredListUserPoolsRequestRequestTypeDef, _OptionalListUserPoolsRequestRequestTypeDef
 ):
     pass
 
-_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
-    "_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
-    {
-        "UserPoolId": str,
-        "GroupName": str,
-    },
-)
-_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
-    "_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
-    {
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUsersInGroupRequestListUsersInGroupPaginateTypeDef(
-    _RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
-    _OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
-):
-    pass
-
 _RequiredListUsersInGroupRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersInGroupRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "GroupName": str,
     },
 )
@@ -1670,36 +1483,14 @@
 )
 
 class ListUsersInGroupRequestRequestTypeDef(
     _RequiredListUsersInGroupRequestRequestTypeDef, _OptionalListUsersInGroupRequestRequestTypeDef
 ):
     pass
 
-_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_RequiredListUsersRequestListUsersPaginateTypeDef",
-    {
-        "UserPoolId": str,
-    },
-)
-_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
-    "_OptionalListUsersRequestListUsersPaginateTypeDef",
-    {
-        "AttributesToGet": Sequence[str],
-        "Filter": str,
-        "PaginationConfig": "PaginatorConfigTypeDef",
-    },
-    total=False,
-)
-
-class ListUsersRequestListUsersPaginateTypeDef(
-    _RequiredListUsersRequestListUsersPaginateTypeDef,
-    _OptionalListUsersRequestListUsersPaginateTypeDef,
-):
-    pass
-
 _RequiredListUsersRequestRequestTypeDef = TypedDict(
     "_RequiredListUsersRequestRequestTypeDef",
     {
         "UserPoolId": str,
     },
 )
 _OptionalListUsersRequestRequestTypeDef = TypedDict(
@@ -1741,48 +1532,27 @@
     {
         "MinValue": str,
         "MaxValue": str,
     },
     total=False,
 )
 
-PaginatorConfigTypeDef = TypedDict(
-    "PaginatorConfigTypeDef",
-    {
-        "MaxItems": int,
-        "PageSize": int,
-        "StartingToken": str,
-    },
-    total=False,
-)
-
 PasswordPolicyTypeTypeDef = TypedDict(
     "PasswordPolicyTypeTypeDef",
     {
         "MinimumLength": int,
         "RequireUppercase": bool,
         "RequireLowercase": bool,
         "RequireNumbers": bool,
         "RequireSymbols": bool,
         "TemporaryPasswordValidityDays": int,
     },
     total=False,
 )
 
-ResponseMetadataTypeDef = TypedDict(
-    "ResponseMetadataTypeDef",
-    {
-        "RequestId": str,
-        "HostId": str,
-        "HTTPStatusCode": int,
-        "HTTPHeaders": Dict[str, str],
-        "RetryAttempts": int,
-    },
-)
-
 _RequiredRevokeTokenRequestRequestTypeDef = TypedDict(
     "_RequiredRevokeTokenRequestRequestTypeDef",
     {
         "Token": str,
         "ClientId": str,
     },
 )
@@ -1944,22 +1714,14 @@
 
 class UpdateIdentityProviderRequestRequestTypeDef(
     _RequiredUpdateIdentityProviderRequestRequestTypeDef,
     _OptionalUpdateIdentityProviderRequestRequestTypeDef,
 ):
     pass
 
-UpdateUserPoolDomainResponseTypeDef = TypedDict(
-    "UpdateUserPoolDomainResponseTypeDef",
-    {
-        "CloudFrontDomain": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 _RequiredVerifySoftwareTokenRequestRequestTypeDef = TypedDict(
     "_RequiredVerifySoftwareTokenRequestRequestTypeDef",
     {
         "UserCode": str,
     },
 )
 _OptionalVerifySoftwareTokenRequestRequestTypeDef = TypedDict(
@@ -1974,23 +1736,14 @@
 
 class VerifySoftwareTokenRequestRequestTypeDef(
     _RequiredVerifySoftwareTokenRequestRequestTypeDef,
     _OptionalVerifySoftwareTokenRequestRequestTypeDef,
 ):
     pass
 
-VerifySoftwareTokenResponseTypeDef = TypedDict(
-    "VerifySoftwareTokenResponseTypeDef",
-    {
-        "Status": VerifySoftwareTokenResponseTypeType,
-        "Session": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
-    },
-)
-
 VerifyUserAttributeRequestRequestTypeDef = TypedDict(
     "VerifyUserAttributeRequestRequestTypeDef",
     {
         "AccessToken": str,
         "AttributeName": str,
         "Code": str,
     },
@@ -2101,14 +1854,88 @@
 
 class UpdateUserAttributesRequestRequestTypeDef(
     _RequiredUpdateUserAttributesRequestRequestTypeDef,
     _OptionalUpdateUserAttributesRequestRequestTypeDef,
 ):
     pass
 
+AssociateSoftwareTokenResponseTypeDef = TypedDict(
+    "AssociateSoftwareTokenResponseTypeDef",
+    {
+        "SecretCode": str,
+        "Session": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ConfirmDeviceResponseTypeDef = TypedDict(
+    "ConfirmDeviceResponseTypeDef",
+    {
+        "UserConfirmationNecessary": bool,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+CreateUserPoolDomainResponseTypeDef = TypedDict(
+    "CreateUserPoolDomainResponseTypeDef",
+    {
+        "CloudFrontDomain": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+EmptyResponseMetadataTypeDef = TypedDict(
+    "EmptyResponseMetadataTypeDef",
+    {
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetCSVHeaderResponseTypeDef = TypedDict(
+    "GetCSVHeaderResponseTypeDef",
+    {
+        "UserPoolId": str,
+        "CSVHeader": List[str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+GetSigningCertificateResponseTypeDef = TypedDict(
+    "GetSigningCertificateResponseTypeDef",
+    {
+        "Certificate": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+ListTagsForResourceResponseTypeDef = TypedDict(
+    "ListTagsForResourceResponseTypeDef",
+    {
+        "Tags": Dict[str, str],
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+UpdateUserPoolDomainResponseTypeDef = TypedDict(
+    "UpdateUserPoolDomainResponseTypeDef",
+    {
+        "CloudFrontDomain": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
+VerifySoftwareTokenResponseTypeDef = TypedDict(
+    "VerifySoftwareTokenResponseTypeDef",
+    {
+        "Status": VerifySoftwareTokenResponseTypeType,
+        "Session": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 AdminDisableProviderForUserRequestRequestTypeDef = TypedDict(
     "AdminDisableProviderForUserRequestRequestTypeDef",
     {
         "UserPoolId": str,
         "User": ProviderUserIdentifierTypeTypeDef,
     },
 )
@@ -2130,15 +1957,15 @@
         "UserCreateDate": datetime,
         "UserLastModifiedDate": datetime,
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
         "MFAOptions": List[MFAOptionTypeTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminSetUserSettingsRequestRequestTypeDef = TypedDict(
     "AdminSetUserSettingsRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -2151,15 +1978,15 @@
     "GetUserResponseTypeDef",
     {
         "Username": str,
         "UserAttributes": List[AttributeTypeTypeDef],
         "MFAOptions": List[MFAOptionTypeTypeDef],
         "PreferredMfaSetting": str,
         "UserMFASettingList": List[str],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetUserSettingsRequestRequestTypeDef = TypedDict(
     "SetUserSettingsRequestRequestTypeDef",
     {
         "AccessToken": str,
@@ -2177,53 +2004,226 @@
         "Enabled": bool,
         "UserStatus": UserStatusTypeType,
         "MFAOptions": List[MFAOptionTypeTypeDef],
     },
     total=False,
 )
 
+_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
+    "_RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    {
+        "Username": str,
+        "UserPoolId": str,
+    },
+)
+_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef = TypedDict(
+    "_OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef(
+    _RequiredAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    _OptionalAdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+):
+    pass
+
+_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
+    "_RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+        "Username": str,
+    },
+)
+_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef = TypedDict(
+    "_OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef(
+    _RequiredAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+    _OptionalAdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+):
+    pass
+
+_RequiredListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_RequiredListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListGroupsRequestListGroupsPaginateTypeDef = TypedDict(
+    "_OptionalListGroupsRequestListGroupsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListGroupsRequestListGroupsPaginateTypeDef(
+    _RequiredListGroupsRequestListGroupsPaginateTypeDef,
+    _OptionalListGroupsRequestListGroupsPaginateTypeDef,
+):
+    pass
+
+_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "_RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef = TypedDict(
+    "_OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef(
+    _RequiredListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    _OptionalListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+):
+    pass
+
+_RequiredListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
+    "_RequiredListResourceServersRequestListResourceServersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListResourceServersRequestListResourceServersPaginateTypeDef = TypedDict(
+    "_OptionalListResourceServersRequestListResourceServersPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListResourceServersRequestListResourceServersPaginateTypeDef(
+    _RequiredListResourceServersRequestListResourceServersPaginateTypeDef,
+    _OptionalListResourceServersRequestListResourceServersPaginateTypeDef,
+):
+    pass
+
+_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
+    "_RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef = TypedDict(
+    "_OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef(
+    _RequiredListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+    _OptionalListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+):
+    pass
+
+ListUserPoolsRequestListUserPoolsPaginateTypeDef = TypedDict(
+    "ListUserPoolsRequestListUserPoolsPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
+    "_RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
+    {
+        "UserPoolId": str,
+        "GroupName": str,
+    },
+)
+_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef = TypedDict(
+    "_OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef",
+    {
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUsersInGroupRequestListUsersInGroupPaginateTypeDef(
+    _RequiredListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+    _OptionalListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+):
+    pass
+
+_RequiredListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_RequiredListUsersRequestListUsersPaginateTypeDef",
+    {
+        "UserPoolId": str,
+    },
+)
+_OptionalListUsersRequestListUsersPaginateTypeDef = TypedDict(
+    "_OptionalListUsersRequestListUsersPaginateTypeDef",
+    {
+        "AttributesToGet": Sequence[str],
+        "Filter": str,
+        "PaginationConfig": PaginatorConfigTypeDef,
+    },
+    total=False,
+)
+
+class ListUsersRequestListUsersPaginateTypeDef(
+    _RequiredListUsersRequestListUsersPaginateTypeDef,
+    _OptionalListUsersRequestListUsersPaginateTypeDef,
+):
+    pass
+
 AdminListGroupsForUserResponseTypeDef = TypedDict(
     "AdminListGroupsForUserResponseTypeDef",
     {
         "Groups": List[GroupTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetGroupResponseTypeDef = TypedDict(
     "GetGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "Groups": List[GroupTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateGroupResponseTypeDef = TypedDict(
     "UpdateGroupResponseTypeDef",
     {
         "Group": GroupTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef = TypedDict(
     "_RequiredAdminSetUserMFAPreferenceRequestRequestTypeDef",
     {
         "Username": str,
@@ -2294,49 +2294,49 @@
     total=False,
 )
 
 ForgotPasswordResponseTypeDef = TypedDict(
     "ForgotPasswordResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserAttributeVerificationCodeResponseTypeDef = TypedDict(
     "GetUserAttributeVerificationCodeResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ResendConfirmationCodeResponseTypeDef = TypedDict(
     "ResendConfirmationCodeResponseTypeDef",
     {
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SignUpResponseTypeDef = TypedDict(
     "SignUpResponseTypeDef",
     {
         "UserConfirmed": bool,
         "CodeDeliveryDetails": CodeDeliveryDetailsTypeTypeDef,
         "UserSub": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserAttributesResponseTypeDef = TypedDict(
     "UpdateUserAttributesResponseTypeDef",
     {
         "CodeDeliveryDetailsList": List[CodeDeliveryDetailsTypeTypeDef],
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef = TypedDict(
     "_RequiredCompromisedCredentialsRiskConfigurationTypeTypeDef",
     {
         "Actions": CompromisedCredentialsActionsTypeTypeDef,
@@ -2569,39 +2569,39 @@
 class ContextDataTypeTypeDef(_RequiredContextDataTypeTypeDef, _OptionalContextDataTypeTypeDef):
     pass
 
 CreateIdentityProviderResponseTypeDef = TypedDict(
     "CreateIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeIdentityProviderResponseTypeDef = TypedDict(
     "DescribeIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetIdentityProviderByIdentifierResponseTypeDef = TypedDict(
     "GetIdentityProviderByIdentifierResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateIdentityProviderResponseTypeDef = TypedDict(
     "UpdateIdentityProviderResponseTypeDef",
     {
         "IdentityProvider": IdentityProviderTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateResourceServerRequestRequestTypeDef = TypedDict(
     "_RequiredCreateResourceServerRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -2656,48 +2656,48 @@
 ):
     pass
 
 CreateUserImportJobResponseTypeDef = TypedDict(
     "CreateUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserImportJobResponseTypeDef = TypedDict(
     "DescribeUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserImportJobsResponseTypeDef = TypedDict(
     "ListUserImportJobsResponseTypeDef",
     {
         "UserImportJobs": List[UserImportJobTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StartUserImportJobResponseTypeDef = TypedDict(
     "StartUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 StopUserImportJobResponseTypeDef = TypedDict(
     "StopUserImportJobResponseTypeDef",
     {
         "UserImportJob": UserImportJobTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredCreateUserPoolClientRequestRequestTypeDef = TypedDict(
     "_RequiredCreateUserPoolClientRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -2883,41 +2883,41 @@
     total=False,
 )
 
 GetUICustomizationResponseTypeDef = TypedDict(
     "GetUICustomizationResponseTypeDef",
     {
         "UICustomization": UICustomizationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetUICustomizationResponseTypeDef = TypedDict(
     "SetUICustomizationResponseTypeDef",
     {
         "UICustomization": UICustomizationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListIdentityProvidersResponseTypeDef = TypedDict(
     "ListIdentityProvidersResponseTypeDef",
     {
         "Providers": List[ProviderDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUserPoolClientsResponseTypeDef = TypedDict(
     "ListUserPoolClientsResponseTypeDef",
     {
         "UserPoolClients": List[UserPoolClientDescriptionTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredNotifyConfigurationTypeTypeDef = TypedDict(
     "_RequiredNotifyConfigurationTypeTypeDef",
     {
         "SourceArn": str,
@@ -2962,120 +2962,120 @@
     total=False,
 )
 
 AdminGetDeviceResponseTypeDef = TypedDict(
     "AdminGetDeviceResponseTypeDef",
     {
         "Device": DeviceTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminListDevicesResponseTypeDef = TypedDict(
     "AdminListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetDeviceResponseTypeDef = TypedDict(
     "GetDeviceResponseTypeDef",
     {
         "Device": DeviceTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListDevicesResponseTypeDef = TypedDict(
     "ListDevicesResponseTypeDef",
     {
         "Devices": List[DeviceTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminCreateUserResponseTypeDef = TypedDict(
     "AdminCreateUserResponseTypeDef",
     {
         "User": UserTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersInGroupResponseTypeDef = TypedDict(
     "ListUsersInGroupResponseTypeDef",
     {
         "Users": List[UserTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "Users": List[UserTypeTypeDef],
         "PaginationToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminListUserAuthEventsResponseTypeDef = TypedDict(
     "AdminListUserAuthEventsResponseTypeDef",
     {
         "AuthEvents": List[AuthEventTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminInitiateAuthResponseTypeDef = TypedDict(
     "AdminInitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 AdminRespondToAuthChallengeResponseTypeDef = TypedDict(
     "AdminRespondToAuthChallengeResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 InitiateAuthResponseTypeDef = TypedDict(
     "InitiateAuthResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RespondToAuthChallengeResponseTypeDef = TypedDict(
     "RespondToAuthChallengeResponseTypeDef",
     {
         "ChallengeName": ChallengeNameTypeType,
         "Session": str,
         "ChallengeParameters": Dict[str, str],
         "AuthenticationResult": AuthenticationResultTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredAdminInitiateAuthRequestRequestTypeDef = TypedDict(
     "_RequiredAdminInitiateAuthRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -3125,82 +3125,82 @@
 ):
     pass
 
 CreateResourceServerResponseTypeDef = TypedDict(
     "CreateResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeResourceServerResponseTypeDef = TypedDict(
     "DescribeResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 ListResourceServersResponseTypeDef = TypedDict(
     "ListResourceServersResponseTypeDef",
     {
         "ResourceServers": List[ResourceServerTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateResourceServerResponseTypeDef = TypedDict(
     "UpdateResourceServerResponseTypeDef",
     {
         "ResourceServer": ResourceServerTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 CreateUserPoolClientResponseTypeDef = TypedDict(
     "CreateUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserPoolClientResponseTypeDef = TypedDict(
     "DescribeUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UpdateUserPoolClientResponseTypeDef = TypedDict(
     "UpdateUserPoolClientResponseTypeDef",
     {
         "UserPoolClient": UserPoolClientTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserPoolDomainResponseTypeDef = TypedDict(
     "DescribeUserPoolDomainResponseTypeDef",
     {
         "DomainDescription": DomainDescriptionTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 GetUserPoolMfaConfigResponseTypeDef = TypedDict(
     "GetUserPoolMfaConfigResponseTypeDef",
     {
         "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 _RequiredSetUserPoolMfaConfigRequestRequestTypeDef = TypedDict(
     "_RequiredSetUserPoolMfaConfigRequestRequestTypeDef",
     {
         "UserPoolId": str,
@@ -3224,15 +3224,15 @@
 
 SetUserPoolMfaConfigResponseTypeDef = TypedDict(
     "SetUserPoolMfaConfigResponseTypeDef",
     {
         "SmsMfaConfiguration": SmsMfaConfigTypeTypeDef,
         "SoftwareTokenMfaConfiguration": SoftwareTokenMfaConfigTypeTypeDef,
         "MfaConfiguration": UserPoolMfaTypeType,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 UserPoolDescriptionTypeTypeDef = TypedDict(
     "UserPoolDescriptionTypeTypeDef",
     {
         "Id": str,
@@ -3390,15 +3390,15 @@
 )
 
 ListUserPoolsResponseTypeDef = TypedDict(
     "ListUserPoolsResponseTypeDef",
     {
         "UserPools": List[UserPoolDescriptionTypeTypeDef],
         "NextToken": str,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 RiskConfigurationTypeTypeDef = TypedDict(
     "RiskConfigurationTypeTypeDef",
     {
         "UserPoolId": str,
@@ -3438,34 +3438,34 @@
 ):
     pass
 
 CreateUserPoolResponseTypeDef = TypedDict(
     "CreateUserPoolResponseTypeDef",
     {
         "UserPool": UserPoolTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeUserPoolResponseTypeDef = TypedDict(
     "DescribeUserPoolResponseTypeDef",
     {
         "UserPool": UserPoolTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 DescribeRiskConfigurationResponseTypeDef = TypedDict(
     "DescribeRiskConfigurationResponseTypeDef",
     {
         "RiskConfiguration": RiskConfigurationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
 SetRiskConfigurationResponseTypeDef = TypedDict(
     "SetRiskConfigurationResponseTypeDef",
     {
         "RiskConfiguration": RiskConfigurationTypeTypeDef,
-        "ResponseMetadata": "ResponseMetadataTypeDef",
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp.egg-info/PKG-INFO` & `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-cognito-idp
-Version: 1.28.0
-Summary: Type annotations for boto3.CognitoIdentityProvider 1.28.0 service generated with mypy-boto3-builder 7.14.5
+Version: 1.28.2
+Summary: Type annotations for boto3.CognitoIdentityProvider 1.28.2 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -38,15 +38,15 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-cognito-idp.svg?color=blue)](https://pypi.org/project/mypy-boto3-cognito-idp)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_cognito_idp/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-cognito-idp?color=blue)](https://pypistats.org/packages/mypy-boto3-cognito-idp)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.CognitoIdentityProvider 1.28.0](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
+[boto3.CognitoIdentityProvider 1.28.2](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp.html#CognitoIdentityProvider)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
@@ -400,62 +400,59 @@
 from mypy_boto3_cognito_idp.type_defs import (
     RecoveryOptionTypeTypeDef,
     AccountTakeoverActionTypeTypeDef,
     AdminAddUserToGroupRequestRequestTypeDef,
     AdminConfirmSignUpRequestRequestTypeDef,
     MessageTemplateTypeTypeDef,
     AttributeTypeTypeDef,
+    ResponseMetadataTypeDef,
     AdminDeleteUserAttributesRequestRequestTypeDef,
     AdminDeleteUserRequestRequestTypeDef,
     ProviderUserIdentifierTypeTypeDef,
     AdminDisableUserRequestRequestTypeDef,
     AdminEnableUserRequestRequestTypeDef,
     AdminForgetDeviceRequestRequestTypeDef,
     AdminGetDeviceRequestRequestTypeDef,
     AdminGetUserRequestRequestTypeDef,
     MFAOptionTypeTypeDef,
     AnalyticsMetadataTypeTypeDef,
     AdminListDevicesRequestRequestTypeDef,
-    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    PaginatorConfigTypeDef,
     AdminListGroupsForUserRequestRequestTypeDef,
     GroupTypeTypeDef,
-    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
     AdminListUserAuthEventsRequestRequestTypeDef,
     AdminRemoveUserFromGroupRequestRequestTypeDef,
     AdminResetUserPasswordRequestRequestTypeDef,
     SMSMfaSettingsTypeTypeDef,
     SoftwareTokenMfaSettingsTypeTypeDef,
     AdminSetUserPasswordRequestRequestTypeDef,
     AdminUpdateAuthEventFeedbackRequestRequestTypeDef,
     AdminUpdateDeviceStatusRequestRequestTypeDef,
     AdminUserGlobalSignOutRequestRequestTypeDef,
     AnalyticsConfigurationTypeTypeDef,
     AssociateSoftwareTokenRequestRequestTypeDef,
-    AssociateSoftwareTokenResponseTypeDef,
     ChallengeResponseTypeTypeDef,
     EventContextDataTypeTypeDef,
     EventFeedbackTypeTypeDef,
     EventRiskTypeTypeDef,
     NewDeviceMetadataTypeTypeDef,
     ChangePasswordRequestRequestTypeDef,
     CodeDeliveryDetailsTypeTypeDef,
     CompromisedCredentialsActionsTypeTypeDef,
     DeviceSecretVerifierConfigTypeTypeDef,
-    ConfirmDeviceResponseTypeDef,
     UserContextDataTypeTypeDef,
     HttpHeaderTypeDef,
     CreateGroupRequestRequestTypeDef,
     CreateIdentityProviderRequestRequestTypeDef,
     IdentityProviderTypeTypeDef,
     ResourceServerScopeTypeTypeDef,
     CreateUserImportJobRequestRequestTypeDef,
     UserImportJobTypeTypeDef,
     TokenValidityUnitsTypeTypeDef,
     CustomDomainConfigTypeTypeDef,
-    CreateUserPoolDomainResponseTypeDef,
     DeviceConfigurationTypeTypeDef,
     EmailConfigurationTypeTypeDef,
     SmsConfigurationTypeTypeDef,
     UserAttributeUpdateSettingsTypeTypeDef,
     UserPoolAddOnsTypeTypeDef,
     UsernameConfigurationTypeTypeDef,
     VerificationMessageTemplateTypeTypeDef,
@@ -472,85 +469,88 @@
     DescribeIdentityProviderRequestRequestTypeDef,
     DescribeResourceServerRequestRequestTypeDef,
     DescribeRiskConfigurationRequestRequestTypeDef,
     DescribeUserImportJobRequestRequestTypeDef,
     DescribeUserPoolClientRequestRequestTypeDef,
     DescribeUserPoolDomainRequestRequestTypeDef,
     DescribeUserPoolRequestRequestTypeDef,
-    EmptyResponseMetadataTypeDef,
     ForgetDeviceRequestRequestTypeDef,
     GetCSVHeaderRequestRequestTypeDef,
-    GetCSVHeaderResponseTypeDef,
     GetDeviceRequestRequestTypeDef,
     GetGroupRequestRequestTypeDef,
     GetIdentityProviderByIdentifierRequestRequestTypeDef,
     GetSigningCertificateRequestRequestTypeDef,
-    GetSigningCertificateResponseTypeDef,
     GetUICustomizationRequestRequestTypeDef,
     UICustomizationTypeTypeDef,
     GetUserAttributeVerificationCodeRequestRequestTypeDef,
     GetUserPoolMfaConfigRequestRequestTypeDef,
     SoftwareTokenMfaConfigTypeTypeDef,
     GetUserRequestRequestTypeDef,
     GlobalSignOutRequestRequestTypeDef,
     ListDevicesRequestRequestTypeDef,
-    ListGroupsRequestListGroupsPaginateTypeDef,
     ListGroupsRequestRequestTypeDef,
-    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
     ListIdentityProvidersRequestRequestTypeDef,
     ProviderDescriptionTypeDef,
-    ListResourceServersRequestListResourceServersPaginateTypeDef,
     ListResourceServersRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
-    ListTagsForResourceResponseTypeDef,
     ListUserImportJobsRequestRequestTypeDef,
-    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
     ListUserPoolClientsRequestRequestTypeDef,
     UserPoolClientDescriptionTypeDef,
-    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
     ListUserPoolsRequestRequestTypeDef,
-    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
     ListUsersInGroupRequestRequestTypeDef,
-    ListUsersRequestListUsersPaginateTypeDef,
     ListUsersRequestRequestTypeDef,
     NotifyEmailTypeTypeDef,
     NumberAttributeConstraintsTypeTypeDef,
-    PaginatorConfigTypeDef,
     PasswordPolicyTypeTypeDef,
-    ResponseMetadataTypeDef,
     RevokeTokenRequestRequestTypeDef,
     RiskExceptionConfigurationTypeTypeDef,
     StringAttributeConstraintsTypeTypeDef,
     SetUICustomizationRequestRequestTypeDef,
     StartUserImportJobRequestRequestTypeDef,
     StopUserImportJobRequestRequestTypeDef,
     TagResourceRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateAuthEventFeedbackRequestRequestTypeDef,
     UpdateDeviceStatusRequestRequestTypeDef,
     UpdateGroupRequestRequestTypeDef,
     UpdateIdentityProviderRequestRequestTypeDef,
-    UpdateUserPoolDomainResponseTypeDef,
     VerifySoftwareTokenRequestRequestTypeDef,
-    VerifySoftwareTokenResponseTypeDef,
     VerifyUserAttributeRequestRequestTypeDef,
     AccountRecoverySettingTypeTypeDef,
     AccountTakeoverActionsTypeTypeDef,
     AdminCreateUserConfigTypeTypeDef,
     AdminCreateUserRequestRequestTypeDef,
     AdminUpdateUserAttributesRequestRequestTypeDef,
     DeviceTypeTypeDef,
     UpdateUserAttributesRequestRequestTypeDef,
+    AssociateSoftwareTokenResponseTypeDef,
+    ConfirmDeviceResponseTypeDef,
+    CreateUserPoolDomainResponseTypeDef,
+    EmptyResponseMetadataTypeDef,
+    GetCSVHeaderResponseTypeDef,
+    GetSigningCertificateResponseTypeDef,
+    ListTagsForResourceResponseTypeDef,
+    UpdateUserPoolDomainResponseTypeDef,
+    VerifySoftwareTokenResponseTypeDef,
     AdminDisableProviderForUserRequestRequestTypeDef,
     AdminLinkProviderForUserRequestRequestTypeDef,
     AdminGetUserResponseTypeDef,
     AdminSetUserSettingsRequestRequestTypeDef,
     GetUserResponseTypeDef,
     SetUserSettingsRequestRequestTypeDef,
     UserTypeTypeDef,
+    AdminListGroupsForUserRequestAdminListGroupsForUserPaginateTypeDef,
+    AdminListUserAuthEventsRequestAdminListUserAuthEventsPaginateTypeDef,
+    ListGroupsRequestListGroupsPaginateTypeDef,
+    ListIdentityProvidersRequestListIdentityProvidersPaginateTypeDef,
+    ListResourceServersRequestListResourceServersPaginateTypeDef,
+    ListUserPoolClientsRequestListUserPoolClientsPaginateTypeDef,
+    ListUserPoolsRequestListUserPoolsPaginateTypeDef,
+    ListUsersInGroupRequestListUsersInGroupPaginateTypeDef,
+    ListUsersRequestListUsersPaginateTypeDef,
     AdminListGroupsForUserResponseTypeDef,
     CreateGroupResponseTypeDef,
     GetGroupResponseTypeDef,
     ListGroupsResponseTypeDef,
     UpdateGroupResponseTypeDef,
     AdminSetUserMFAPreferenceRequestRequestTypeDef,
     SetUserMFAPreferenceRequestRequestTypeDef,
```

### Comparing `mypy-boto3-cognito-idp-1.28.0/mypy_boto3_cognito_idp.egg-info/SOURCES.txt` & `mypy-boto3-cognito-idp-1.28.2/mypy_boto3_cognito_idp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-cognito-idp-1.28.0/setup.py` & `mypy-boto3-cognito-idp-1.28.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-cognito-idp",
-    version="1.28.0",
+    version="1.28.2",
     packages=["mypy_boto3_cognito_idp"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.CognitoIdentityProvider 1.28.0 service generated with"
+        "Type annotations for boto3.CognitoIdentityProvider 1.28.2 service generated with"
         " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
```

