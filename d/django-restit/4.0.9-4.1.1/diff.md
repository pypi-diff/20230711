# Comparing `tmp/django_restit-4.0.9.tar.gz` & `tmp/django_restit-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_restit-4.0.9.tar", max compression
+gzip compressed data, was "django_restit-4.1.1.tar", max compression
```

## Comparing `django_restit-4.0.9.tar` & `django_restit-4.1.1.tar`

### file list

```diff
@@ -1,452 +1,457 @@
--rw-r--r--   0        0        0     1068 2023-06-27 05:37:44.430230 django_restit-4.0.9/LICENSE.md
--rw-r--r--   0        0        0     6240 2023-06-30 17:03:51.486194 django_restit-4.0.9/README.md
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.430501 django_restit-4.0.9/account/__init__.py
--rw-r--r--   0        0        0     1839 2023-06-27 05:37:44.430617 django_restit-4.0.9/account/admin.py
--rw-r--r--   0        0        0      980 2023-06-27 05:37:44.430754 django_restit-4.0.9/account/fcm/__init__.py
--rw-r--r--   0        0        0    15894 2023-06-27 05:37:44.430954 django_restit-4.0.9/account/migrations/0001_initial.py
--rw-r--r--   0        0        0      738 2023-06-27 05:37:44.431054 django_restit-4.0.9/account/migrations/0003_member_phone_number.py
--rw-r--r--   0        0        0      551 2023-06-27 05:37:44.431131 django_restit-4.0.9/account/migrations/0004_group_modified_alter_group_created.py
--rw-r--r--   0        0        0      437 2023-06-27 05:37:44.431211 django_restit-4.0.9/account/migrations/0005_member_auth_code_expires.py
--rw-r--r--   0        0        0      450 2023-06-27 05:37:44.431293 django_restit-4.0.9/account/migrations/0006_member_security_token.py
--rw-r--r--   0        0        0     1654 2023-06-27 05:37:44.431375 django_restit-4.0.9/account/migrations/0007_authtoken_signature_authsession.py
--rw-r--r--   0        0        0     2379 2023-06-27 05:37:44.431464 django_restit-4.0.9/account/migrations/0008_memberdevice_memberdevicemetadata.py
--rw-r--r--   0        0        0      468 2023-06-27 05:37:44.431538 django_restit-4.0.9/account/migrations/0009_alter_member_phone_number.py
--rw-r--r--   0        0        0      305 2023-06-27 05:37:44.431613 django_restit-4.0.9/account/migrations/0010_delete_authtoken.py
--rw-r--r--   0        0        0     1062 2023-06-27 05:37:44.431685 django_restit-4.0.9/account/migrations/0011_authtoken.py
--rw-r--r--   0        0        0     2043 2023-06-27 05:37:44.431755 django_restit-4.0.9/account/migrations/0012_settings_settingsmetadata.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.431784 django_restit-4.0.9/account/migrations/__init__.py
--rw-r--r--   0        0        0      341 2023-06-27 05:37:44.431899 django_restit-4.0.9/account/models/__init__.py
--rw-r--r--   0        0        0     3070 2023-06-27 05:37:44.431980 django_restit-4.0.9/account/models/device.py
--rw-r--r--   0        0        0     1437 2023-06-27 05:37:44.432051 django_restit-4.0.9/account/models/feeds.py
--rw-r--r--   0        0        0    18165 2023-06-27 22:00:18.627797 django_restit-4.0.9/account/models/group.py
--rw-r--r--   0        0        0     2720 2023-06-27 05:37:44.432315 django_restit-4.0.9/account/models/legacy.py
--rw-r--r--   0        0        0    46749 2023-06-27 22:00:18.628155 django_restit-4.0.9/account/models/member.py
--rw-r--r--   0        0        0     6842 2023-06-27 05:37:44.432689 django_restit-4.0.9/account/models/membership.py
--rw-r--r--   0        0        0    10739 2023-06-27 05:37:44.432797 django_restit-4.0.9/account/models/notify.py
--rw-r--r--   0        0        0     3345 2023-06-27 05:37:44.432886 django_restit-4.0.9/account/models/session.py
--rw-r--r--   0        0        0     2137 2023-06-27 05:37:44.432966 django_restit-4.0.9/account/models/settings.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.433042 django_restit-4.0.9/account/oauth/__init__.py
--rw-r--r--   0        0        0     2078 2023-06-27 05:37:44.433131 django_restit-4.0.9/account/oauth/google.py
--rw-r--r--   0        0        0      578 2023-06-27 05:37:44.433195 django_restit-4.0.9/account/periodic.py
--rw-r--r--   0        0        0      152 2023-06-27 05:37:44.433297 django_restit-4.0.9/account/rpc/__init__.py
--rw-r--r--   0        0        0    12428 2023-06-27 05:37:44.433416 django_restit-4.0.9/account/rpc/auth.py
--rw-r--r--   0        0        0     2104 2023-06-27 05:37:44.433497 django_restit-4.0.9/account/rpc/device.py
--rw-r--r--   0        0        0     3078 2023-06-27 05:37:44.433585 django_restit-4.0.9/account/rpc/group.py
--rw-r--r--   0        0        0     1150 2023-06-27 05:37:44.433650 django_restit-4.0.9/account/rpc/member.py
--rw-r--r--   0        0        0     3344 2023-06-27 05:37:44.433726 django_restit-4.0.9/account/rpc/notify.py
--rw-r--r--   0        0        0     2610 2023-06-27 05:37:44.433805 django_restit-4.0.9/account/rpc/oauth.py
--rw-r--r--   0        0        0      271 2023-06-27 05:37:44.433874 django_restit-4.0.9/account/rpc/settings.py
--rw-r--r--   0        0        0       53 2023-06-27 05:37:44.433934 django_restit-4.0.9/account/settings.py
--rw-r--r--   0        0        0     9709 2023-06-27 05:37:44.434095 django_restit-4.0.9/account/templates/email/base.html
--rw-r--r--   0        0        0    10567 2023-06-27 05:37:44.434205 django_restit-4.0.9/account/templates/email/invite.html
--rw-r--r--   0        0        0    15185 2023-06-27 05:37:44.434344 django_restit-4.0.9/account/templates/email/plain/invite.html
--rw-r--r--   0        0        0    13954 2023-06-27 05:37:44.434450 django_restit-4.0.9/account/templates/email/plain/reset_code.html
--rw-r--r--   0        0        0    10261 2023-06-27 05:37:44.434528 django_restit-4.0.9/account/templates/email/reset_code.html
--rw-r--r--   0        0        0    15163 2023-06-27 05:37:44.434627 django_restit-4.0.9/account/templates/email/simple/invite.html
--rw-r--r--   0        0        0    13944 2023-06-27 05:37:44.434713 django_restit-4.0.9/account/templates/email/simple/reset_code.html
--rw-r--r--   0        0        0      520 2023-06-27 05:37:44.434828 django_restit-4.0.9/auditlog/README
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.434859 django_restit-4.0.9/auditlog/__init__.py
--rw-r--r--   0        0        0     1006 2023-06-27 05:37:44.434933 django_restit-4.0.9/auditlog/admin.py
--rw-r--r--   0        0        0     6553 2023-06-27 05:37:44.435019 django_restit-4.0.9/auditlog/decorators.py
--rw-r--r--   0        0        0     1329 2023-06-27 05:37:44.435081 django_restit-4.0.9/auditlog/middleware.py
--rw-r--r--   0        0        0     3309 2023-06-27 05:37:44.435191 django_restit-4.0.9/auditlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.435224 django_restit-4.0.9/auditlog/migrations/__init__.py
--rw-r--r--   0        0        0    16051 2023-06-27 16:49:06.686531 django_restit-4.0.9/auditlog/models.py
--rw-r--r--   0        0        0      264 2023-06-27 05:37:44.435414 django_restit-4.0.9/auditlog/periodic.py
--rw-r--r--   0        0        0     3591 2023-06-27 05:37:44.435492 django_restit-4.0.9/auditlog/rpc.py
--rw-r--r--   0        0        0     2019 2023-06-27 05:37:44.435560 django_restit-4.0.9/auditlog/tq.py
--rw-r--r--   0        0        0      163 2023-06-27 05:37:44.435623 django_restit-4.0.9/auditlog/urls.py
--rw-r--r--   0        0        0     2169 2023-06-27 05:37:44.435745 django_restit-4.0.9/inbox/README.md
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.435775 django_restit-4.0.9/inbox/__init__.py
--rw-r--r--   0        0        0      243 2023-06-27 05:37:44.435850 django_restit-4.0.9/inbox/admin.py
--rw-r--r--   0        0        0     5621 2023-06-27 05:37:44.435936 django_restit-4.0.9/inbox/handlers.py
--rw-r--r--   0        0        0     6429 2023-06-27 05:37:44.436034 django_restit-4.0.9/inbox/migrations/0001_initial.py
--rw-r--r--   0        0        0      380 2023-06-27 05:37:44.436102 django_restit-4.0.9/inbox/migrations/0002_alter_message_cc.py
--rw-r--r--   0        0        0      416 2023-06-27 05:37:44.436177 django_restit-4.0.9/inbox/migrations/0003_attachment_content_type.py
--rw-r--r--   0        0        0     1140 2023-06-27 05:37:44.436249 django_restit-4.0.9/inbox/migrations/0004_mailtemplate.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.436274 django_restit-4.0.9/inbox/migrations/__init__.py
--rw-r--r--   0        0        0      174 2023-06-27 05:37:44.436383 django_restit-4.0.9/inbox/models/__init__.py
--rw-r--r--   0        0        0     2832 2023-06-27 05:37:44.436463 django_restit-4.0.9/inbox/models/bounce.py
--rw-r--r--   0        0        0     2468 2023-06-27 05:37:44.436568 django_restit-4.0.9/inbox/models/complaint.py
--rw-r--r--   0        0        0     2879 2023-06-27 05:37:44.436797 django_restit-4.0.9/inbox/models/message.py
--rw-r--r--   0        0        0     1013 2023-06-27 05:37:44.436870 django_restit-4.0.9/inbox/models/template.py
--rw-r--r--   0        0        0     1534 2023-06-27 05:37:44.436956 django_restit-4.0.9/inbox/rpc.py
--rw-r--r--   0        0        0       89 2023-06-27 05:37:44.437057 django_restit-4.0.9/inbox/utils/__init__.py
--rw-r--r--   0        0        0     4366 2023-06-27 05:37:44.437161 django_restit-4.0.9/inbox/utils/parsing.py
--rw-r--r--   0        0        0     4098 2023-06-27 05:37:44.437260 django_restit-4.0.9/inbox/utils/render.py
--rw-r--r--   0        0        0     2109 2023-06-27 05:37:44.437361 django_restit-4.0.9/inbox/utils/sending.py
--rw-r--r--   0        0        0     1114 2023-06-27 05:37:44.437469 django_restit-4.0.9/incident/README.md
--rw-r--r--   0        0        0     1468 2023-06-27 22:00:18.628468 django_restit-4.0.9/incident/__init__.py
--rw-r--r--   0        0        0     9720 2023-06-27 05:37:44.437670 django_restit-4.0.9/incident/migrations/0001_initial.py
--rw-r--r--   0        0        0      595 2023-06-27 05:37:44.437757 django_restit-4.0.9/incident/migrations/0002_event_component_event_component_id.py
--rw-r--r--   0        0        0      425 2023-06-27 05:37:44.437826 django_restit-4.0.9/incident/migrations/0003_rule_action.py
--rw-r--r--   0        0        0      662 2023-06-27 05:37:44.437890 django_restit-4.0.9/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py
--rw-r--r--   0        0        0      698 2023-06-27 05:37:44.437964 django_restit-4.0.9/incident/migrations/0005_incident_component_alter_incident_state.py
--rw-r--r--   0        0        0      324 2023-06-27 05:37:44.438034 django_restit-4.0.9/incident/migrations/0006_delete_eventmetadata.py
--rw-r--r--   0        0        0      414 2023-06-27 05:37:44.438100 django_restit-4.0.9/incident/migrations/0007_event_metadata.py
--rw-r--r--   0        0        0      903 2023-06-27 05:37:44.438184 django_restit-4.0.9/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.438214 django_restit-4.0.9/incident/migrations/__init__.py
--rw-r--r--   0        0        0      167 2023-06-27 05:37:44.438331 django_restit-4.0.9/incident/models/__init__.py
--rw-r--r--   0        0        0     5068 2023-06-27 22:00:18.628641 django_restit-4.0.9/incident/models/event.py
--rw-r--r--   0        0        0    10022 2023-06-27 05:37:44.438560 django_restit-4.0.9/incident/models/incident.py
--rw-r--r--   0        0        0     2187 2023-06-27 05:37:44.438718 django_restit-4.0.9/incident/models/ossec.py
--rw-r--r--   0        0        0     5300 2023-06-27 05:37:44.438826 django_restit-4.0.9/incident/models/rules.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.438911 django_restit-4.0.9/incident/parsers/__init__.py
--rw-r--r--   0        0        0     5289 2023-06-27 05:37:44.439057 django_restit-4.0.9/incident/parsers/ossec.py
--rw-r--r--   0        0        0      723 2023-06-27 05:37:44.439158 django_restit-4.0.9/incident/periodic.py
--rw-r--r--   0        0        0     2831 2023-06-27 05:37:44.439252 django_restit-4.0.9/incident/rpc.py
--rw-r--r--   0        0        0    12732 2023-06-27 05:37:44.439416 django_restit-4.0.9/incident/templates/email/incident_change.html
--rw-r--r--   0        0        0    15173 2023-06-27 05:37:44.439515 django_restit-4.0.9/incident/templates/email/incident_new.html
--rw-r--r--   0        0        0    13208 2023-06-27 05:37:44.439626 django_restit-4.0.9/incident/templates/email/incident_plain.html
--rw-r--r--   0        0        0      796 2023-06-27 05:37:44.439700 django_restit-4.0.9/incident/tq.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.439791 django_restit-4.0.9/location/__init__.py
--rw-r--r--   0        0        0      297 2023-06-27 05:37:44.439885 django_restit-4.0.9/location/admin.py
--rw-r--r--   0        0        0     1694 2023-06-27 05:37:44.440042 django_restit-4.0.9/location/geolocate.py
--rw-r--r--   0        0        0     7000 2023-06-27 05:37:44.440236 django_restit-4.0.9/location/migrations/0001_initial.py
--rw-r--r--   0        0        0      576 2023-06-27 05:37:44.440313 django_restit-4.0.9/location/migrations/0002_geoip_subnet_alter_geoip_ip.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.440339 django_restit-4.0.9/location/migrations/__init__.py
--rw-r--r--   0        0        0      230 2023-06-27 05:37:44.440480 django_restit-4.0.9/location/models/__init__.py
--rw-r--r--   0        0        0     2028 2023-06-27 05:37:44.440559 django_restit-4.0.9/location/models/address.py
--rw-r--r--   0        0        0     3500 2023-06-27 05:37:44.440656 django_restit-4.0.9/location/models/ip.py
--rw-r--r--   0        0        0     1994 2023-06-27 05:37:44.440722 django_restit-4.0.9/location/models/legacy.py
--rw-r--r--   0        0        0     2316 2023-06-27 05:37:44.440785 django_restit-4.0.9/location/models/location.py
--rw-r--r--   0        0        0     1474 2023-06-27 05:37:44.440843 django_restit-4.0.9/location/models/track.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.440920 django_restit-4.0.9/location/providers/__init__.py
--rw-r--r--   0        0        0      730 2023-06-27 05:37:44.441046 django_restit-4.0.9/location/providers/iplookup/__init__.py
--rw-r--r--   0        0        0     2419 2023-06-27 05:37:44.441128 django_restit-4.0.9/location/providers/iplookup/abstractapi.py
--rw-r--r--   0        0        0     1345 2023-06-27 05:37:44.441192 django_restit-4.0.9/location/providers/iplookup/extremeip.py
--rw-r--r--   0        0        0     2121 2023-06-27 05:37:44.441260 django_restit-4.0.9/location/providers/iplookup/geoplugin.py
--rw-r--r--   0        0        0     1797 2023-06-27 05:37:44.441325 django_restit-4.0.9/location/providers/iplookup/ipapi.py
--rw-r--r--   0        0        0     1265 2023-06-27 05:37:44.441395 django_restit-4.0.9/location/providers/iplookup/ipinfo.py
--rw-r--r--   0        0        0      937 2023-06-27 05:37:44.441463 django_restit-4.0.9/location/providers/iplookup/restit.py
--rw-r--r--   0        0        0       42 2023-06-27 05:37:44.441569 django_restit-4.0.9/location/providers/location/__init__.py
--rw-r--r--   0        0        0     2860 2023-06-27 05:37:44.441653 django_restit-4.0.9/location/providers/location/google.py
--rw-r--r--   0        0        0       46 2023-06-27 05:37:44.441777 django_restit-4.0.9/location/providers/timezones/__init__.py
--rw-r--r--   0        0        0      619 2023-06-27 05:37:44.441855 django_restit-4.0.9/location/providers/timezones/google.py
--rw-r--r--   0        0        0     1935 2023-06-27 05:37:44.441924 django_restit-4.0.9/location/providers/zillow.py
--rw-r--r--   0        0        0      123 2023-06-27 05:37:44.442046 django_restit-4.0.9/location/rpc/__init__.py
--rw-r--r--   0        0        0      875 2023-07-03 18:37:00.843398 django_restit-4.0.9/location/rpc/ip.py
--rw-r--r--   0        0        0      779 2023-06-27 05:37:44.442183 django_restit-4.0.9/location/rpc/location.py
--rw-r--r--   0        0        0     3735 2023-06-27 05:37:44.442254 django_restit-4.0.9/location/rpc/track.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.442312 django_restit-4.0.9/medialib/__init__.py
--rw-r--r--   0        0        0     2261 2023-06-27 05:37:44.442393 django_restit-4.0.9/medialib/admin.py
--rw-r--r--   0        0        0       27 2023-06-27 05:37:44.442482 django_restit-4.0.9/medialib/cvutil/__init__.py
--rw-r--r--   0        0        0     4269 2023-06-27 05:37:44.442556 django_restit-4.0.9/medialib/cvutil/contours.py
--rw-r--r--   0        0        0    12649 2023-06-27 05:37:44.442653 django_restit-4.0.9/medialib/cvutil/images.py
--rw-r--r--   0        0        0     9586 2023-06-27 05:37:44.442744 django_restit-4.0.9/medialib/cvutil/misc.py
--rw-r--r--   0        0        0     5824 2023-06-27 05:37:44.442838 django_restit-4.0.9/medialib/cvutil/text.py
--rw-r--r--   0        0        0    48442 2023-06-27 05:37:44.443047 django_restit-4.0.9/medialib/fixtures/initial_data.json
--rw-r--r--   0        0        0    31978 2023-06-27 05:37:44.443182 django_restit-4.0.9/medialib/fixtures/medialib.json
--rw-r--r--   0        0        0    16989 2023-06-27 05:37:44.443279 django_restit-4.0.9/medialib/fixtures/medialib_test_fixture.json
--rw-r--r--   0        0        0     5442 2023-06-27 05:37:44.443362 django_restit-4.0.9/medialib/forms.py
--rw-r--r--   0        0        0    20518 2023-06-27 05:37:44.443459 django_restit-4.0.9/medialib/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.443499 django_restit-4.0.9/medialib/migrations/__init__.py
--rw-r--r--   0        0        0    52121 2023-06-27 05:37:44.443702 django_restit-4.0.9/medialib/models.py
--rw-r--r--   0        0        0     1189 2023-06-27 05:37:44.443785 django_restit-4.0.9/medialib/ocr.py
--rw-r--r--   0        0        0     1275 2023-06-27 05:37:44.443858 django_restit-4.0.9/medialib/pdf.py
--rw-r--r--   0        0        0      545 2023-06-27 05:37:44.443925 django_restit-4.0.9/medialib/qrcode.py
--rw-r--r--   0        0        0    10312 2023-06-27 05:37:44.444059 django_restit-4.0.9/medialib/render/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.444125 django_restit-4.0.9/medialib/render/engines/__init__.py
--rw-r--r--   0        0        0     3531 2023-06-27 05:37:44.444213 django_restit-4.0.9/medialib/render/engines/anigif.py
--rw-r--r--   0        0        0     6881 2023-06-27 05:37:44.444291 django_restit-4.0.9/medialib/render/engines/ffmpeg.py
--rw-r--r--   0        0        0      792 2023-06-27 05:37:44.444369 django_restit-4.0.9/medialib/render/engines/gifsicle.py
--rw-r--r--   0        0        0     3436 2023-06-27 05:37:44.444438 django_restit-4.0.9/medialib/render/engines/hls.py
--rw-r--r--   0        0        0      983 2023-06-27 05:37:44.444498 django_restit-4.0.9/medialib/render/engines/mp4box.py
--rw-r--r--   0        0        0      397 2023-06-27 05:37:44.444604 django_restit-4.0.9/medialib/render/engines/rtmp/Makefile
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.444636 django_restit-4.0.9/medialib/render/engines/rtmp/__init__.py
--rw-r--r--   0        0        0     4026 2023-06-27 05:37:44.444726 django_restit-4.0.9/medialib/render/engines/rtmp/rtmp.i
--rw-r--r--   0        0        0      699 2023-06-27 05:37:44.444798 django_restit-4.0.9/medialib/render/engines/rtmpdump.py
--rw-r--r--   0        0        0     1017 2023-06-27 05:37:44.444865 django_restit-4.0.9/medialib/render/engines/rtmpsink.py
--rw-r--r--   0        0        0     3466 2023-06-27 05:37:44.444941 django_restit-4.0.9/medialib/render/engines/video_getinfo.py
--rw-r--r--   0        0        0      809 2023-06-27 05:37:44.445017 django_restit-4.0.9/medialib/render/engines/websnap.py
--rw-r--r--   0        0        0     2193 2023-06-27 05:37:44.445078 django_restit-4.0.9/medialib/render/exceptions.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.445133 django_restit-4.0.9/medialib/render/presets/__init__.py
--rw-r--r--   0        0        0     4179 2023-06-27 05:37:44.445227 django_restit-4.0.9/medialib/render/presets/akamai.py
--rw-r--r--   0        0        0     3284 2023-06-27 05:37:44.445306 django_restit-4.0.9/medialib/render/presets/animated_thumbnail.py
--rw-r--r--   0        0        0     4004 2023-06-27 05:37:44.445394 django_restit-4.0.9/medialib/render/presets/ffmpeg.py
--rw-r--r--   0        0        0     2087 2023-06-27 05:37:44.445469 django_restit-4.0.9/medialib/render/presets/flv.py
--rw-r--r--   0        0        0     6567 2023-06-27 05:37:44.445567 django_restit-4.0.9/medialib/render/presets/hls.py
--rw-r--r--   0        0        0     6955 2023-06-27 05:37:44.445668 django_restit-4.0.9/medialib/render/presets/image_transcode.py
--rw-r--r--   0        0        0     1094 2023-06-27 05:37:44.445750 django_restit-4.0.9/medialib/render/presets/image_validate.py
--rw-r--r--   0        0        0     2423 2023-06-27 05:37:44.445825 django_restit-4.0.9/medialib/render/presets/mp4.py
--rw-r--r--   0        0        0     4997 2023-06-27 05:37:44.445908 django_restit-4.0.9/medialib/render/presets/video_still.py
--rw-r--r--   0        0        0     3228 2023-06-27 05:37:44.445986 django_restit-4.0.9/medialib/render/presets/video_validate.py
--rw-r--r--   0        0        0      863 2023-06-27 05:37:44.446101 django_restit-4.0.9/medialib/render/presets/websnap.py
--rw-r--r--   0        0        0     2282 2023-06-27 05:37:44.446183 django_restit-4.0.9/medialib/render/presets/youtube.py
--rw-r--r--   0        0        0    16451 2023-06-27 05:37:44.446294 django_restit-4.0.9/medialib/render/render_utils.py
--rw-r--r--   0        0        0      370 2023-06-27 05:37:44.446381 django_restit-4.0.9/medialib/render/schedule.py
--rw-r--r--   0        0        0       82 2023-06-27 05:37:44.446525 django_restit-4.0.9/medialib/rpc/__init__.py
--rw-r--r--   0        0        0    37925 2023-06-27 05:37:44.446687 django_restit-4.0.9/medialib/rpc/legacy.py
--rw-r--r--   0        0        0      617 2023-06-27 05:37:44.446776 django_restit-4.0.9/medialib/rpc/media.py
--rw-r--r--   0        0        0      956 2023-06-27 05:37:44.446852 django_restit-4.0.9/medialib/rpc/tools.py
--rwxr-xr-x   0        0        0     7875 2023-06-27 05:37:44.446994 django_restit-4.0.9/medialib/scripts/init_config
--rw-r--r--   0        0        0     4499 2023-06-27 05:37:44.447158 django_restit-4.0.9/medialib/static/css/base_medialibui.css
--rw-r--r--   0        0        0     3128 2023-06-27 05:37:44.447238 django_restit-4.0.9/medialib/static/css/base_widgets.css
--rw-r--r--   0        0        0     3263 2023-06-27 05:37:44.447311 django_restit-4.0.9/medialib/static/css/jquery.jcrop.css
--rw-r--r--   0        0        0      193 2023-06-27 05:37:44.447412 django_restit-4.0.9/medialib/static/img/arrow-down-white.png
--rw-r--r--   0        0        0     4589 2023-06-27 05:37:44.447507 django_restit-4.0.9/medialib/static/img/bg-body.gif
--rw-r--r--   0        0        0      441 2023-06-27 05:37:44.447579 django_restit-4.0.9/medialib/static/img/cancel.gif
--rw-r--r--   0        0        0      341 2023-06-27 05:37:44.447648 django_restit-4.0.9/medialib/static/img/icon-generic.gif
--rw-r--r--   0        0        0      355 2023-06-27 05:37:44.447712 django_restit-4.0.9/medialib/static/img/icon-image.gif
--rw-r--r--   0        0        0      359 2023-06-27 05:37:44.447775 django_restit-4.0.9/medialib/static/img/icon-media.gif
--rw-r--r--   0        0        0      355 2023-06-27 05:37:44.447850 django_restit-4.0.9/medialib/static/img/icon-zip.gif
--rw-r--r--   0        0        0     3208 2023-06-27 05:37:44.447934 django_restit-4.0.9/medialib/static/img/loading.gif
--rw-r--r--   0        0        0     2537 2023-06-27 05:37:44.448000 django_restit-4.0.9/medialib/static/img/noimage.gif
--rw-r--r--   0        0        0     1057 2023-06-27 05:37:44.448065 django_restit-4.0.9/medialib/static/img/render_err.gif
--rw-r--r--   0        0        0     6716 2023-06-27 05:37:44.448158 django_restit-4.0.9/medialib/static/img/rendering.gif
--rw-r--r--   0        0        0      292 2023-06-27 05:37:44.448225 django_restit-4.0.9/medialib/static/img/star_off.png
--rw-r--r--   0        0        0      297 2023-06-27 05:37:44.448287 django_restit-4.0.9/medialib/static/img/star_on.png
--rw-r--r--   0        0        0     1130 2023-06-27 05:37:44.448351 django_restit-4.0.9/medialib/static/img/unknown.gif
--rwxr-xr-x   0        0        0    74054 2023-06-27 05:37:44.448677 django_restit-4.0.9/medialib/static/lib/caman.full.js
--rw-r--r--   0        0        0    17360 2023-06-27 05:37:44.448823 django_restit-4.0.9/medialib/static/lib/hammer.min.js
--rwxr-xr-x   0        0        0    42434 2023-06-27 05:37:44.449017 django_restit-4.0.9/medialib/static/lib/jquery.Jcrop.js
--rw-r--r--   0        0        0      743 2023-06-27 05:37:44.449098 django_restit-4.0.9/medialib/static/lib/jquery.hammer.js
--rw-r--r--   0        0        0    16587 2023-06-27 05:37:44.449224 django_restit-4.0.9/medialib/static/lib/load-image.min.js
--rwxr-xr-x   0        0        0   111779 2023-06-27 05:37:44.449542 django_restit-4.0.9/medialib/static/lib/swiper.js
--rw-r--r--   0        0        0     1163 2023-06-27 05:37:44.449771 django_restit-4.0.9/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js
--rw-r--r--   0        0        0     1163 2023-06-27 05:37:44.449850 django_restit-4.0.9/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js
--rw-r--r--   0        0        0     5708 2023-06-27 05:37:44.449979 django_restit-4.0.9/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js
--rw-r--r--   0        0        0     3502 2023-06-27 05:37:44.450059 django_restit-4.0.9/medialib/static/lib/tinymce/plugins/medialib/medialib.html
--rw-r--r--   0        0        0     5876 2023-06-27 05:37:44.450187 django_restit-4.0.9/medialib/stores/__init__.py
--rw-r--r--   0        0        0      601 2023-06-27 05:37:44.450314 django_restit-4.0.9/medialib/stores/apiclient/__init__.py
--rw-r--r--   0        0        0     9852 2023-06-27 05:37:44.450415 django_restit-4.0.9/medialib/stores/apiclient/channel.py
--rw-r--r--   0        0        0    35929 2023-06-27 05:37:44.450591 django_restit-4.0.9/medialib/stores/apiclient/discovery.py
--rw-r--r--   0        0        0     3516 2023-06-27 05:37:44.450684 django_restit-4.0.9/medialib/stores/apiclient/errors.py
--rw-r--r--   0        0        0    52911 2023-06-27 05:37:44.450906 django_restit-4.0.9/medialib/stores/apiclient/http.py
--rw-r--r--   0        0        0     6505 2023-06-27 05:37:44.451002 django_restit-4.0.9/medialib/stores/apiclient/mimeparse.py
--rw-r--r--   0        0        0    11761 2023-06-27 05:37:44.451111 django_restit-4.0.9/medialib/stores/apiclient/model.py
--rw-r--r--   0        0        0     3528 2023-06-27 05:37:44.451205 django_restit-4.0.9/medialib/stores/apiclient/sample_tools.py
--rw-r--r--   0        0        0     9293 2023-06-27 05:37:44.451302 django_restit-4.0.9/medialib/stores/apiclient/schema.py
--rw-r--r--   0        0        0     1592 2023-06-27 05:37:44.451390 django_restit-4.0.9/medialib/stores/filestore.py
--rw-r--r--   0        0        0    69575 2023-06-27 05:37:44.451712 django_restit-4.0.9/medialib/stores/httplib2/__init__.py
--rw-r--r--   0        0        0    39670 2023-06-27 05:37:44.451937 django_restit-4.0.9/medialib/stores/httplib2/cacerts.txt
--rw-r--r--   0        0        0     3821 2023-06-27 05:37:44.452031 django_restit-4.0.9/medialib/stores/httplib2/iri2uri.py
--rw-r--r--   0        0        0    18452 2023-06-27 05:37:44.452160 django_restit-4.0.9/medialib/stores/httplib2/socks.py
--rw-r--r--   0        0        0      706 2023-06-27 05:37:44.452238 django_restit-4.0.9/medialib/stores/httpstore.py
--rw-r--r--   0        0        0      304 2023-06-27 05:37:44.452325 django_restit-4.0.9/medialib/stores/nullstore.py
--rw-r--r--   0        0        0      213 2023-06-27 05:37:44.452492 django_restit-4.0.9/medialib/stores/oauth2client/__init__.py
--rw-r--r--   0        0        0     1044 2023-06-27 05:37:44.452598 django_restit-4.0.9/medialib/stores/oauth2client/anyjson.py
--rw-r--r--   0        0        0    32534 2023-06-27 05:37:44.452767 django_restit-4.0.9/medialib/stores/oauth2client/appengine.py
--rw-r--r--   0        0        0    44346 2023-06-27 05:37:44.452995 django_restit-4.0.9/medialib/stores/oauth2client/client.py
--rw-r--r--   0        0        0     4425 2023-06-27 05:37:44.453091 django_restit-4.0.9/medialib/stores/oauth2client/clientsecrets.py
--rw-r--r--   0        0        0    10239 2023-06-27 05:37:44.453196 django_restit-4.0.9/medialib/stores/oauth2client/crypt.py
--rw-r--r--   0        0        0     3755 2023-06-27 05:37:44.453276 django_restit-4.0.9/medialib/stores/oauth2client/django_orm.py
--rw-r--r--   0        0        0     3164 2023-06-27 05:37:44.453391 django_restit-4.0.9/medialib/stores/oauth2client/file.py
--rw-r--r--   0        0        0     3036 2023-06-27 05:37:44.453451 django_restit-4.0.9/medialib/stores/oauth2client/gce.py
--rw-r--r--   0        0        0     3229 2023-06-27 05:37:44.453541 django_restit-4.0.9/medialib/stores/oauth2client/keyring_storage.py
--rw-r--r--   0        0        0    11393 2023-06-27 05:37:44.453634 django_restit-4.0.9/medialib/stores/oauth2client/locked_file.py
--rw-r--r--   0        0        0    13950 2023-06-27 05:37:44.453698 django_restit-4.0.9/medialib/stores/oauth2client/multistore_file.py
--rw-r--r--   0        0        0     5588 2023-06-27 05:37:44.453764 django_restit-4.0.9/medialib/stores/oauth2client/old_run.py
--rw-r--r--   0        0        0     8379 2023-06-27 05:37:44.453855 django_restit-4.0.9/medialib/stores/oauth2client/tools.py
--rw-r--r--   0        0        0     5706 2023-06-27 05:37:44.453938 django_restit-4.0.9/medialib/stores/oauth2client/util.py
--rw-r--r--   0        0        0     3367 2023-06-27 05:37:44.454013 django_restit-4.0.9/medialib/stores/oauth2client/xsrfutil.py
--rw-r--r--   0        0        0      500 2023-06-27 05:37:44.454077 django_restit-4.0.9/medialib/stores/rtmpstore.py
--rw-r--r--   0        0        0     4583 2023-06-27 05:37:44.454163 django_restit-4.0.9/medialib/stores/s3store.py
--rw-r--r--   0        0        0     4996 2023-06-27 05:37:44.454272 django_restit-4.0.9/medialib/stores/uritemplate/__init__.py
--rw-r--r--   0        0        0      406 2023-06-27 05:37:44.454334 django_restit-4.0.9/medialib/stores/youtubestore.py
--rw-r--r--   0        0        0     3691 2023-06-27 05:37:44.454500 django_restit-4.0.9/medialib/templates/medialib/base.html
--rw-r--r--   0        0        0     1277 2023-06-27 05:37:44.454591 django_restit-4.0.9/medialib/templates/medialib/instances.html
--rw-r--r--   0        0        0     1170 2023-06-27 05:37:44.454657 django_restit-4.0.9/medialib/templates/medialib/items.html
--rw-r--r--   0        0        0     8194 2023-06-27 05:37:44.454746 django_restit-4.0.9/medialib/templates/medialib/library.html
--rw-r--r--   0        0        0       65 2023-06-27 05:37:44.454810 django_restit-4.0.9/medialib/templates/medialib/notify_error.subject
--rw-r--r--   0        0        0       49 2023-06-27 05:37:44.454869 django_restit-4.0.9/medialib/templates/medialib/notify_error.to
--rw-r--r--   0        0        0      272 2023-06-27 05:37:44.454932 django_restit-4.0.9/medialib/templates/medialib/notify_error.txt
--rw-r--r--   0        0        0       71 2023-06-27 05:37:44.454996 django_restit-4.0.9/medialib/templates/medialib/notify_ready.subject
--rw-r--r--   0        0        0       49 2023-06-27 05:37:44.455056 django_restit-4.0.9/medialib/templates/medialib/notify_ready.to
--rw-r--r--   0        0        0      298 2023-06-27 05:37:44.455113 django_restit-4.0.9/medialib/templates/medialib/notify_ready.txt
--rw-r--r--   0        0        0       64 2023-06-27 05:37:44.455175 django_restit-4.0.9/medialib/templates/medialib/notify_render_error.subject
--rw-r--r--   0        0        0       48 2023-06-27 05:37:44.455232 django_restit-4.0.9/medialib/templates/medialib/notify_render_error.to
--rw-r--r--   0        0        0      271 2023-06-27 05:37:44.455301 django_restit-4.0.9/medialib/templates/medialib/notify_render_error.txt
--rw-r--r--   0        0        0       68 2023-06-27 05:37:44.455380 django_restit-4.0.9/medialib/templates/medialib/notify_validate_error.subject
--rw-r--r--   0        0        0       48 2023-06-27 05:37:44.455452 django_restit-4.0.9/medialib/templates/medialib/notify_validate_error.to
--rw-r--r--   0        0        0      275 2023-06-27 05:37:44.455521 django_restit-4.0.9/medialib/templates/medialib/notify_validate_error.txt
--rw-r--r--   0        0        0      206 2023-06-27 05:37:44.455593 django_restit-4.0.9/medialib/templates/medialib/smil
--rw-r--r--   0        0        0     1177 2023-06-27 05:37:44.455665 django_restit-4.0.9/medialib/templates/medialib/test.html
--rw-r--r--   0        0        0     1549 2023-06-27 05:37:44.455737 django_restit-4.0.9/medialib/templates/medialib/testpicker.html
--rw-r--r--   0        0        0     6045 2023-06-27 05:37:44.455814 django_restit-4.0.9/medialib/tests.py
--rw-r--r--   0        0        0      544 2023-06-27 05:37:44.455873 django_restit-4.0.9/medialib/tq.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.455894 django_restit-4.0.9/medialib/urls.py
--rw-r--r--   0        0        0     3756 2023-06-27 05:37:44.455970 django_restit-4.0.9/medialib/utils.py
--rw-r--r--   0        0        0     4321 2023-06-27 05:37:44.456050 django_restit-4.0.9/medialib/views.py
--rw-r--r--   0        0        0     4303 2023-06-27 05:37:44.456166 django_restit-4.0.9/medialib/youtube/__init__.py
--rw-r--r--   0        0        0      601 2023-06-27 05:37:44.456272 django_restit-4.0.9/medialib/youtube/apiclient/__init__.py
--rw-r--r--   0        0        0     9886 2023-06-27 05:37:44.456332 django_restit-4.0.9/medialib/youtube/apiclient/channel.py
--rw-r--r--   0        0        0    35907 2023-06-27 05:37:44.456516 django_restit-4.0.9/medialib/youtube/apiclient/discovery.py
--rw-r--r--   0        0        0     3550 2023-06-27 05:37:44.456592 django_restit-4.0.9/medialib/youtube/apiclient/errors.py
--rw-r--r--   0        0        0    52945 2023-06-27 05:37:44.456694 django_restit-4.0.9/medialib/youtube/apiclient/http.py
--rw-r--r--   0        0        0     6505 2023-06-27 05:37:44.456785 django_restit-4.0.9/medialib/youtube/apiclient/mimeparse.py
--rw-r--r--   0        0        0    11795 2023-06-27 05:37:44.456835 django_restit-4.0.9/medialib/youtube/apiclient/model.py
--rw-r--r--   0        0        0     3596 2023-06-27 05:37:44.456895 django_restit-4.0.9/medialib/youtube/apiclient/sample_tools.py
--rw-r--r--   0        0        0     9327 2023-06-27 05:37:44.456959 django_restit-4.0.9/medialib/youtube/apiclient/schema.py
--rw-r--r--   0        0        0    69581 2023-06-27 05:37:44.457093 django_restit-4.0.9/medialib/youtube/httplib2/__init__.py
--rw-r--r--   0        0        0    39670 2023-06-27 05:37:44.457310 django_restit-4.0.9/medialib/youtube/httplib2/cacerts.txt
--rw-r--r--   0        0        0     3821 2023-06-27 05:37:44.457412 django_restit-4.0.9/medialib/youtube/httplib2/iri2uri.py
--rw-r--r--   0        0        0    18452 2023-06-27 05:37:44.457533 django_restit-4.0.9/medialib/youtube/httplib2/socks.py
--rw-r--r--   0        0        0      213 2023-06-27 05:37:44.457629 django_restit-4.0.9/medialib/youtube/oauth2client/__init__.py
--rw-r--r--   0        0        0     1044 2023-06-27 05:37:44.457687 django_restit-4.0.9/medialib/youtube/oauth2client/anyjson.py
--rw-r--r--   0        0        0    32534 2023-06-27 05:37:44.457830 django_restit-4.0.9/medialib/youtube/oauth2client/appengine.py
--rw-r--r--   0        0        0    44431 2023-06-27 05:37:44.457905 django_restit-4.0.9/medialib/youtube/oauth2client/client.py
--rw-r--r--   0        0        0     4425 2023-06-27 05:37:44.457990 django_restit-4.0.9/medialib/youtube/oauth2client/clientsecrets.py
--rw-r--r--   0        0        0    10239 2023-06-27 05:37:44.458075 django_restit-4.0.9/medialib/youtube/oauth2client/crypt.py
--rw-r--r--   0        0        0     3753 2023-06-27 05:37:44.458140 django_restit-4.0.9/medialib/youtube/oauth2client/django_orm.py
--rw-r--r--   0        0        0     3164 2023-06-27 05:37:44.458204 django_restit-4.0.9/medialib/youtube/oauth2client/file.py
--rw-r--r--   0        0        0     3036 2023-06-27 05:37:44.458255 django_restit-4.0.9/medialib/youtube/oauth2client/gce.py
--rw-r--r--   0        0        0     3229 2023-06-27 05:37:44.458323 django_restit-4.0.9/medialib/youtube/oauth2client/keyring_storage.py
--rw-r--r--   0        0        0    11393 2023-06-27 05:37:44.458399 django_restit-4.0.9/medialib/youtube/oauth2client/locked_file.py
--rw-r--r--   0        0        0    13950 2023-06-27 05:37:44.458454 django_restit-4.0.9/medialib/youtube/oauth2client/multistore_file.py
--rw-r--r--   0        0        0     5588 2023-06-27 05:37:44.458510 django_restit-4.0.9/medialib/youtube/oauth2client/old_run.py
--rw-r--r--   0        0        0     8379 2023-06-27 05:37:44.458604 django_restit-4.0.9/medialib/youtube/oauth2client/tools.py
--rw-r--r--   0        0        0     5706 2023-06-27 05:37:44.458680 django_restit-4.0.9/medialib/youtube/oauth2client/util.py
--rw-r--r--   0        0        0     3367 2023-06-27 05:37:44.458745 django_restit-4.0.9/medialib/youtube/oauth2client/xsrfutil.py
--rw-r--r--   0        0        0     2849 2023-06-27 05:37:44.458806 django_restit-4.0.9/medialib/youtube/upload.py
--rw-r--r--   0        0        0     4996 2023-06-27 05:37:44.458902 django_restit-4.0.9/medialib/youtube/uritemplate/__init__.py
--rw-r--r--   0        0        0     2307 2023-06-27 05:37:44.459001 django_restit-4.0.9/metrics/README.md
--rw-r--r--   0        0        0       90 2023-06-27 05:37:44.459061 django_restit-4.0.9/metrics/__init__.py
--rw-r--r--   0        0        0    23460 2023-06-27 05:37:44.459219 django_restit-4.0.9/metrics/client.py
--rw-r--r--   0        0        0     9182 2023-06-27 05:37:44.459333 django_restit-4.0.9/metrics/eod.py
--rw-r--r--   0        0        0     1664 2023-06-27 05:37:44.459430 django_restit-4.0.9/metrics/examples/eod_example.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.459493 django_restit-4.0.9/metrics/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.459564 django_restit-4.0.9/metrics/management/commands/__init__.py
--rw-r--r--   0        0        0      429 2023-06-27 05:37:44.459636 django_restit-4.0.9/metrics/management/commands/delete_gauge.py
--rw-r--r--   0        0        0      464 2023-06-27 05:37:44.459697 django_restit-4.0.9/metrics/management/commands/delete_metric.py
--rw-r--r--   0        0        0     2801 2023-06-27 05:37:44.459766 django_restit-4.0.9/metrics/management/commands/fix_redis_metrics_keys.py
--rw-r--r--   0        0        0     1928 2023-06-27 05:37:44.459829 django_restit-4.0.9/metrics/management/commands/generate_test_metrics.py
--rw-r--r--   0        0        0     1742 2023-06-27 05:37:44.459896 django_restit-4.0.9/metrics/management/commands/redis_metrics_send_mail.py
--rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.459957 django_restit-4.0.9/metrics/management/commands/reset_weekly_metrics.py
--rw-r--r--   0        0        0     4343 2023-06-27 05:37:44.460023 django_restit-4.0.9/metrics/management/commands/system_metric.py
--rw-r--r--   0        0        0     2399 2023-06-27 05:37:44.460109 django_restit-4.0.9/metrics/migrations/0001_initial.py
--rw-r--r--   0        0        0     1510 2023-06-27 05:37:44.460172 django_restit-4.0.9/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py
--rw-r--r--   0        0        0      453 2023-06-27 05:37:44.460231 django_restit-4.0.9/metrics/migrations/0003_metrics_expires.py
--rw-r--r--   0        0        0     3271 2023-06-27 05:37:44.460284 django_restit-4.0.9/metrics/migrations/0004_eodmetrics.py
--rw-r--r--   0        0        0     2358 2023-06-27 05:37:44.460347 django_restit-4.0.9/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460367 django_restit-4.0.9/metrics/migrations/__init__.py
--rw-r--r--   0        0        0    10599 2023-06-27 05:37:44.460461 django_restit-4.0.9/metrics/models.py
--rw-r--r--   0        0        0      480 2023-06-27 05:37:44.460528 django_restit-4.0.9/metrics/periodic.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460587 django_restit-4.0.9/metrics/providers/__init__.py
--rw-r--r--   0        0        0     7335 2023-06-27 05:37:44.460691 django_restit-4.0.9/metrics/providers/aws.py
--rw-r--r--   0        0        0    14826 2023-06-27 05:37:44.460783 django_restit-4.0.9/metrics/rpc.py
--rw-r--r--   0        0        0      132 2023-06-27 05:37:44.460832 django_restit-4.0.9/metrics/settings.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460855 django_restit-4.0.9/metrics/tq.py
--rw-r--r--   0        0        0    10490 2023-06-27 05:37:44.460959 django_restit-4.0.9/metrics/utils.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461016 django_restit-4.0.9/pushit/__init__.py
--rw-r--r--   0        0        0      451 2023-06-27 05:37:44.461079 django_restit-4.0.9/pushit/admin.py
--rw-r--r--   0        0        0     4555 2023-06-27 05:37:44.461167 django_restit-4.0.9/pushit/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461190 django_restit-4.0.9/pushit/migrations/__init__.py
--rw-r--r--   0        0        0     5076 2023-06-27 05:37:44.461264 django_restit-4.0.9/pushit/models.py
--rw-r--r--   0        0        0       88 2023-06-27 05:37:44.461351 django_restit-4.0.9/pushit/rpc/__init__.py
--rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.461414 django_restit-4.0.9/pushit/rpc/githooks.py
--rw-r--r--   0        0        0     5028 2023-06-27 05:37:44.461473 django_restit-4.0.9/pushit/rpc/legacy.py
--rw-r--r--   0        0        0      378 2023-06-27 05:37:44.461520 django_restit-4.0.9/pushit/rpc/products.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461605 django_restit-4.0.9/pushit/static/js/models_pushit.js
--rw-r--r--   0        0        0      131 2023-06-27 05:37:44.461676 django_restit-4.0.9/pushit/tq.py
--rw-r--r--   0        0        0     1966 2023-06-27 05:37:44.461734 django_restit-4.0.9/pushit/utils.py
--rw-r--r--   0        0        0     1401 2023-07-05 22:47:38.289177 django_restit-4.0.9/pyproject.toml
--rw-r--r--   0        0        0      118 2023-06-27 05:37:44.461884 django_restit-4.0.9/rest/.gitignore
--rw-r--r--   0        0        0     5460 2023-06-27 05:37:44.461959 django_restit-4.0.9/rest/README.md
--rw-r--r--   0        0        0       72 2023-06-27 05:37:44.462010 django_restit-4.0.9/rest/RemoteEvents.py
--rw-r--r--   0        0        0      120 2023-06-27 22:00:34.176061 django_restit-4.0.9/rest/__init__.py
--rw-r--r--   0        0        0     1967 2023-06-27 05:37:44.462114 django_restit-4.0.9/rest/arc4.py
--rw-r--r--   0        0        0       83 2023-06-27 05:37:44.462161 django_restit-4.0.9/rest/cache.py
--rw-r--r--   0        0        0       72 2023-06-27 05:37:44.462295 django_restit-4.0.9/rest/crypto/__init__.py
--rw-r--r--   0        0        0     3605 2023-06-27 05:37:44.462374 django_restit-4.0.9/rest/crypto/aes.py
--rw-r--r--   0        0        0     4082 2023-06-27 05:37:44.462442 django_restit-4.0.9/rest/crypto/privpub.py
--rw-r--r--   0        0        0     3955 2023-06-27 05:37:44.462509 django_restit-4.0.9/rest/crypto/util.py
--rw-r--r--   0        0        0     7784 2023-06-27 05:37:44.462604 django_restit-4.0.9/rest/datem.py
--rw-r--r--   0        0        0    15603 2023-06-27 22:00:18.629029 django_restit-4.0.9/rest/decorators.py
--rw-r--r--   0        0        0      788 2023-06-27 05:37:44.462816 django_restit-4.0.9/rest/encryption.py
--rw-r--r--   0        0        0       54 2023-06-27 05:37:44.462913 django_restit-4.0.9/rest/extra/__init__.py
--rw-r--r--   0        0        0     1078 2023-06-27 05:37:44.462982 django_restit-4.0.9/rest/extra/json_metadata.py
--rw-r--r--   0        0        0     9719 2023-06-27 05:37:44.463072 django_restit-4.0.9/rest/fields.py
--rw-r--r--   0        0        0     6316 2023-06-27 05:37:44.463145 django_restit-4.0.9/rest/forms.py
--rw-r--r--   0        0        0    23837 2023-06-27 05:37:44.463266 django_restit-4.0.9/rest/helpers.py
--rw-r--r--   0        0        0      260 2023-06-27 05:37:44.463338 django_restit-4.0.9/rest/joke.py
--rw-r--r--   0        0        0     2298 2023-06-27 05:37:44.463411 django_restit-4.0.9/rest/jwtoken.py
--rw-r--r--   0        0        0    20930 2023-06-27 15:33:50.289063 django_restit-4.0.9/rest/log.py
--rw-r--r--   0        0        0     7754 2023-06-27 05:37:44.463623 django_restit-4.0.9/rest/mail.py
--rw-r--r--   0        0        0     9174 2023-06-27 05:37:44.463711 django_restit-4.0.9/rest/mailman.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.463776 django_restit-4.0.9/rest/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.463861 django_restit-4.0.9/rest/management/commands/__init__.py
--rw-r--r--   0        0        0      389 2023-06-27 05:37:44.463942 django_restit-4.0.9/rest/management/commands/rpc.py
--rw-r--r--   0        0        0       33 2023-06-27 05:37:44.464028 django_restit-4.0.9/rest/middleware/__init__.py
--rw-r--r--   0        0        0     3513 2023-06-27 05:37:44.464096 django_restit-4.0.9/rest/middleware/cors.py
--rw-r--r--   0        0        0     2345 2023-06-27 05:37:44.464159 django_restit-4.0.9/rest/middleware/db_router.py
--rw-r--r--   0        0        0     5395 2023-06-27 05:37:44.464226 django_restit-4.0.9/rest/middleware/jwt.py
--rw-r--r--   0        0        0     4127 2023-06-27 05:37:44.464313 django_restit-4.0.9/rest/middleware/request.py
--rw-r--r--   0        0        0     9015 2023-06-27 05:37:44.464386 django_restit-4.0.9/rest/middleware/session.py
--rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.464450 django_restit-4.0.9/rest/middleware/session_store.py
--rw-r--r--   0        0        0    76369 2023-07-03 04:39:31.567264 django_restit-4.0.9/rest/models.py
--rw-r--r--   0        0        0   149463 2023-06-27 05:37:44.465139 django_restit-4.0.9/rest/regexes.yaml
--rw-r--r--   0        0        0    14894 2023-06-27 05:37:44.465209 django_restit-4.0.9/rest/requestex.py
--rw-r--r--   0        0        0     3713 2023-06-27 15:25:34.225162 django_restit-4.0.9/rest/rpc.py
--rw-r--r--   0        0        0     7645 2023-06-27 05:37:44.465350 django_restit-4.0.9/rest/search.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.465410 django_restit-4.0.9/rest/serializers/__init__.py
--rw-r--r--   0        0        0     1644 2023-06-27 05:37:44.465494 django_restit-4.0.9/rest/serializers/collection.py
--rw-r--r--   0        0        0     2975 2023-06-27 05:37:44.465556 django_restit-4.0.9/rest/serializers/csv.py
--rw-r--r--   0        0        0     1077 2023-06-27 05:37:44.465616 django_restit-4.0.9/rest/serializers/excel.py
--rw-r--r--   0        0        0     1736 2023-06-27 05:37:44.465675 django_restit-4.0.9/rest/serializers/json.py
--rw-r--r--   0        0        0    61738 2023-06-27 05:37:44.465903 django_restit-4.0.9/rest/serializers/legacy.py
--rw-r--r--   0        0        0     4943 2023-06-27 05:37:44.465981 django_restit-4.0.9/rest/serializers/model.py
--rw-r--r--   0        0        0     6403 2023-06-28 15:14:43.267808 django_restit-4.0.9/rest/serializers/response.py
--rw-r--r--   0        0        0     2734 2023-06-27 05:37:44.466139 django_restit-4.0.9/rest/serializers/util.py
--rw-r--r--   0        0        0     1532 2023-06-27 05:37:44.466216 django_restit-4.0.9/rest/settings_helper.py
--rw-r--r--   0        0        0    95786 2023-06-27 05:37:44.466685 django_restit-4.0.9/rest/static/lib/jquery.js
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466742 django_restit-4.0.9/rest/static/rest/app.css
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466776 django_restit-4.0.9/rest/static/rest/app.js
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466808 django_restit-4.0.9/rest/static/rest/rest.js
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466846 django_restit-4.0.9/rest/static/rest/rest.scss
--rw-r--r--   0        0        0      529 2023-06-27 05:37:44.466992 django_restit-4.0.9/rest/templates/email/error.html
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.467020 django_restit-4.0.9/rest/templates/email/error.subject
--rw-r--r--   0        0        0     7148 2023-06-27 05:37:44.467101 django_restit-4.0.9/rest/templates/rest_docs.html
--rw-r--r--   0        0        0    10880 2023-06-27 05:37:44.467182 django_restit-4.0.9/rest/templates/rest_html.html
--rw-r--r--   0        0        0   185122 2023-06-27 05:37:44.467607 django_restit-4.0.9/rest/ua.py
--rw-r--r--   0        0        0    17064 2023-06-27 05:37:44.467734 django_restit-4.0.9/rest/uberdict.py
--rw-r--r--   0        0        0    11881 2023-06-27 05:37:44.467820 django_restit-4.0.9/rest/url_docs.py
--rw-r--r--   0        0        0     1787 2023-06-27 05:37:44.467877 django_restit-4.0.9/rest/urls.py
--rw-r--r--   0        0        0     1056 2023-06-27 05:37:44.467929 django_restit-4.0.9/rest/views.py
--rw-r--r--   0        0        0      118 2023-06-27 05:37:44.468007 django_restit-4.0.9/sessionlog/.gitignore
--rw-r--r--   0        0        0       62 2023-06-27 05:37:44.468062 django_restit-4.0.9/sessionlog/README.md
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468086 django_restit-4.0.9/sessionlog/__init__.py
--rw-r--r--   0        0        0      245 2023-06-27 05:37:44.468153 django_restit-4.0.9/sessionlog/admin.py
--rw-r--r--   0        0        0     1694 2023-06-27 05:37:44.468231 django_restit-4.0.9/sessionlog/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468261 django_restit-4.0.9/sessionlog/migrations/__init__.py
--rw-r--r--   0        0        0     3978 2023-07-05 22:43:30.431976 django_restit-4.0.9/sessionlog/models.py
--rw-r--r--   0        0        0      383 2023-06-27 05:37:44.468400 django_restit-4.0.9/sessionlog/tests.py
--rw-r--r--   0        0        0       26 2023-06-27 05:37:44.468451 django_restit-4.0.9/sessionlog/views.py
--rw-r--r--   0        0        0     2196 2023-06-27 05:37:44.468543 django_restit-4.0.9/taskqueue/README.md
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468569 django_restit-4.0.9/taskqueue/__init__.py
--rw-r--r--   0        0        0      208 2023-06-27 05:37:44.468635 django_restit-4.0.9/taskqueue/admin.py
--rw-r--r--   0        0        0     4738 2023-06-27 05:37:44.468730 django_restit-4.0.9/taskqueue/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468758 django_restit-4.0.9/taskqueue/migrations/__init__.py
--rw-r--r--   0        0        0    16531 2023-06-27 05:37:44.468876 django_restit-4.0.9/taskqueue/models.py
--rw-r--r--   0        0        0     3072 2023-06-27 05:37:44.468952 django_restit-4.0.9/taskqueue/periodic.py
--rw-r--r--   0        0        0     5326 2023-06-27 05:37:44.469019 django_restit-4.0.9/taskqueue/rpc.py
--rw-r--r--   0        0        0      942 2023-06-27 05:37:44.469073 django_restit-4.0.9/taskqueue/tq.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469126 django_restit-4.0.9/taskqueue/transports/__init__.py
--rw-r--r--   0        0        0      623 2023-06-27 05:37:44.469185 django_restit-4.0.9/taskqueue/transports/email.py
--rw-r--r--   0        0        0     2409 2023-06-27 05:37:44.469240 django_restit-4.0.9/taskqueue/transports/http.py
--rw-r--r--   0        0        0     1099 2023-06-27 05:37:44.469291 django_restit-4.0.9/taskqueue/transports/s3.py
--rw-r--r--   0        0        0     1891 2023-06-27 05:37:44.469341 django_restit-4.0.9/taskqueue/transports/sftp.py
--rw-r--r--   0        0        0      142 2023-06-27 05:37:44.469388 django_restit-4.0.9/taskqueue/transports/sms.py
--rw-r--r--   0        0        0    13660 2023-06-27 05:37:44.469465 django_restit-4.0.9/taskqueue/worker.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469517 django_restit-4.0.9/telephony/__init__.py
--rw-r--r--   0        0        0      243 2023-06-27 05:37:44.469571 django_restit-4.0.9/telephony/admin.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469591 django_restit-4.0.9/telephony/decorators.py
--rw-r--r--   0        0        0     3030 2023-06-27 05:37:44.469692 django_restit-4.0.9/telephony/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469714 django_restit-4.0.9/telephony/migrations/__init__.py
--rw-r--r--   0        0        0     7753 2023-06-27 05:37:44.469796 django_restit-4.0.9/telephony/models.py
--rw-r--r--   0        0        0     2126 2023-06-27 05:37:44.469861 django_restit-4.0.9/telephony/phone_util.py
--rw-r--r--   0        0        0     2659 2023-06-27 05:37:44.469923 django_restit-4.0.9/telephony/rpc.py
--rw-r--r--   0        0        0     3624 2023-06-27 05:37:44.470008 django_restit-4.0.9/ws4redis/README.md
--rwxr-xr-x   0        0        0       46 2023-06-27 05:37:44.470065 django_restit-4.0.9/ws4redis/__init__.py
--rw-r--r--   0        0        0     4942 2023-06-27 05:37:44.470133 django_restit-4.0.9/ws4redis/client.py
--rw-r--r--   0        0        0    13026 2023-06-27 05:37:44.470238 django_restit-4.0.9/ws4redis/connection.py
--rwxr-xr-x   0        0        0      636 2023-06-27 05:37:44.470295 django_restit-4.0.9/ws4redis/exceptions.py
--rw-r--r--   0        0        0     5548 2023-06-27 05:37:44.470365 django_restit-4.0.9/ws4redis/redis.py
--rw-r--r--   0        0        0        0 2023-06-27 05:37:44.470422 django_restit-4.0.9/ws4redis/servers/__init__.py
--rw-r--r--   0        0        0     3747 2023-06-27 05:37:44.470507 django_restit-4.0.9/ws4redis/servers/base.py
--rw-r--r--   0        0        0     4329 2023-06-27 05:37:44.470582 django_restit-4.0.9/ws4redis/servers/django.py
--rw-r--r--   0        0        0     1723 2023-06-27 05:37:44.470638 django_restit-4.0.9/ws4redis/servers/uwsgi.py
--rwxr-xr-x   0        0        0     1411 2023-06-27 05:37:44.470697 django_restit-4.0.9/ws4redis/settings.py
--rwxr-xr-x   0        0        0     5122 2023-06-27 05:37:44.470772 django_restit-4.0.9/ws4redis/utf8validator.py
--rwxr-xr-x   0        0        0    14848 2023-06-27 05:37:44.470868 django_restit-4.0.9/ws4redis/websocket.py
--rw-r--r--   0        0        0     7531 1970-01-01 00:00:00.000000 django_restit-4.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-06-27 05:37:44.430230 django_restit-4.1.1/LICENSE.md
+-rw-r--r--   0        0        0     6240 2023-06-30 17:03:51.486194 django_restit-4.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.430501 django_restit-4.1.1/account/__init__.py
+-rw-r--r--   0        0        0     1839 2023-06-27 05:37:44.430617 django_restit-4.1.1/account/admin.py
+-rw-r--r--   0        0        0      980 2023-06-27 05:37:44.430754 django_restit-4.1.1/account/fcm/__init__.py
+-rw-r--r--   0        0        0    15894 2023-06-27 05:37:44.430954 django_restit-4.1.1/account/migrations/0001_initial.py
+-rw-r--r--   0        0        0      738 2023-06-27 05:37:44.431054 django_restit-4.1.1/account/migrations/0003_member_phone_number.py
+-rw-r--r--   0        0        0      551 2023-06-27 05:37:44.431131 django_restit-4.1.1/account/migrations/0004_group_modified_alter_group_created.py
+-rw-r--r--   0        0        0      437 2023-06-27 05:37:44.431211 django_restit-4.1.1/account/migrations/0005_member_auth_code_expires.py
+-rw-r--r--   0        0        0      450 2023-06-27 05:37:44.431293 django_restit-4.1.1/account/migrations/0006_member_security_token.py
+-rw-r--r--   0        0        0     1654 2023-06-27 05:37:44.431375 django_restit-4.1.1/account/migrations/0007_authtoken_signature_authsession.py
+-rw-r--r--   0        0        0     2379 2023-06-27 05:37:44.431464 django_restit-4.1.1/account/migrations/0008_memberdevice_memberdevicemetadata.py
+-rw-r--r--   0        0        0      468 2023-06-27 05:37:44.431538 django_restit-4.1.1/account/migrations/0009_alter_member_phone_number.py
+-rw-r--r--   0        0        0      305 2023-06-27 05:37:44.431613 django_restit-4.1.1/account/migrations/0010_delete_authtoken.py
+-rw-r--r--   0        0        0     1062 2023-06-27 05:37:44.431685 django_restit-4.1.1/account/migrations/0011_authtoken.py
+-rw-r--r--   0        0        0     2043 2023-06-27 05:37:44.431755 django_restit-4.1.1/account/migrations/0012_settings_settingsmetadata.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.431784 django_restit-4.1.1/account/migrations/__init__.py
+-rw-r--r--   0        0        0      341 2023-06-27 05:37:44.431899 django_restit-4.1.1/account/models/__init__.py
+-rw-r--r--   0        0        0     3070 2023-06-27 05:37:44.431980 django_restit-4.1.1/account/models/device.py
+-rw-r--r--   0        0        0     1437 2023-06-27 05:37:44.432051 django_restit-4.1.1/account/models/feeds.py
+-rw-r--r--   0        0        0    18165 2023-06-27 22:00:18.627797 django_restit-4.1.1/account/models/group.py
+-rw-r--r--   0        0        0     2720 2023-06-27 05:37:44.432315 django_restit-4.1.1/account/models/legacy.py
+-rw-r--r--   0        0        0    46749 2023-06-27 22:00:18.628155 django_restit-4.1.1/account/models/member.py
+-rw-r--r--   0        0        0     6842 2023-06-27 05:37:44.432689 django_restit-4.1.1/account/models/membership.py
+-rw-r--r--   0        0        0    10739 2023-06-27 05:37:44.432797 django_restit-4.1.1/account/models/notify.py
+-rw-r--r--   0        0        0     3345 2023-06-27 05:37:44.432886 django_restit-4.1.1/account/models/session.py
+-rw-r--r--   0        0        0     2137 2023-06-27 05:37:44.432966 django_restit-4.1.1/account/models/settings.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.433042 django_restit-4.1.1/account/oauth/__init__.py
+-rw-r--r--   0        0        0     2078 2023-06-27 05:37:44.433131 django_restit-4.1.1/account/oauth/google.py
+-rw-r--r--   0        0        0      578 2023-06-27 05:37:44.433195 django_restit-4.1.1/account/periodic.py
+-rw-r--r--   0        0        0      152 2023-06-27 05:37:44.433297 django_restit-4.1.1/account/rpc/__init__.py
+-rw-r--r--   0        0        0    12428 2023-06-27 05:37:44.433416 django_restit-4.1.1/account/rpc/auth.py
+-rw-r--r--   0        0        0     2104 2023-06-27 05:37:44.433497 django_restit-4.1.1/account/rpc/device.py
+-rw-r--r--   0        0        0     3078 2023-06-27 05:37:44.433585 django_restit-4.1.1/account/rpc/group.py
+-rw-r--r--   0        0        0     1150 2023-06-27 05:37:44.433650 django_restit-4.1.1/account/rpc/member.py
+-rw-r--r--   0        0        0     3344 2023-06-27 05:37:44.433726 django_restit-4.1.1/account/rpc/notify.py
+-rw-r--r--   0        0        0     2610 2023-06-27 05:37:44.433805 django_restit-4.1.1/account/rpc/oauth.py
+-rw-r--r--   0        0        0      271 2023-06-27 05:37:44.433874 django_restit-4.1.1/account/rpc/settings.py
+-rw-r--r--   0        0        0       53 2023-06-27 05:37:44.433934 django_restit-4.1.1/account/settings.py
+-rw-r--r--   0        0        0     9709 2023-06-27 05:37:44.434095 django_restit-4.1.1/account/templates/email/base.html
+-rw-r--r--   0        0        0    10567 2023-06-27 05:37:44.434205 django_restit-4.1.1/account/templates/email/invite.html
+-rw-r--r--   0        0        0    15185 2023-06-27 05:37:44.434344 django_restit-4.1.1/account/templates/email/plain/invite.html
+-rw-r--r--   0        0        0    13954 2023-06-27 05:37:44.434450 django_restit-4.1.1/account/templates/email/plain/reset_code.html
+-rw-r--r--   0        0        0    10261 2023-06-27 05:37:44.434528 django_restit-4.1.1/account/templates/email/reset_code.html
+-rw-r--r--   0        0        0    15163 2023-06-27 05:37:44.434627 django_restit-4.1.1/account/templates/email/simple/invite.html
+-rw-r--r--   0        0        0    13944 2023-06-27 05:37:44.434713 django_restit-4.1.1/account/templates/email/simple/reset_code.html
+-rw-r--r--   0        0        0      520 2023-06-27 05:37:44.434828 django_restit-4.1.1/auditlog/README
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.434859 django_restit-4.1.1/auditlog/__init__.py
+-rw-r--r--   0        0        0     1006 2023-06-27 05:37:44.434933 django_restit-4.1.1/auditlog/admin.py
+-rw-r--r--   0        0        0     6553 2023-06-27 05:37:44.435019 django_restit-4.1.1/auditlog/decorators.py
+-rw-r--r--   0        0        0     1329 2023-06-27 05:37:44.435081 django_restit-4.1.1/auditlog/middleware.py
+-rw-r--r--   0        0        0     3309 2023-06-27 05:37:44.435191 django_restit-4.1.1/auditlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.435224 django_restit-4.1.1/auditlog/migrations/__init__.py
+-rw-r--r--   0        0        0    16051 2023-06-27 16:49:06.686531 django_restit-4.1.1/auditlog/models.py
+-rw-r--r--   0        0        0      264 2023-06-27 05:37:44.435414 django_restit-4.1.1/auditlog/periodic.py
+-rw-r--r--   0        0        0     3591 2023-06-27 05:37:44.435492 django_restit-4.1.1/auditlog/rpc.py
+-rw-r--r--   0        0        0     2019 2023-06-27 05:37:44.435560 django_restit-4.1.1/auditlog/tq.py
+-rw-r--r--   0        0        0      163 2023-06-27 05:37:44.435623 django_restit-4.1.1/auditlog/urls.py
+-rw-r--r--   0        0        0     2169 2023-06-27 05:37:44.435745 django_restit-4.1.1/inbox/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.435775 django_restit-4.1.1/inbox/__init__.py
+-rw-r--r--   0        0        0      243 2023-06-27 05:37:44.435850 django_restit-4.1.1/inbox/admin.py
+-rw-r--r--   0        0        0     5621 2023-06-27 05:37:44.435936 django_restit-4.1.1/inbox/handlers.py
+-rw-r--r--   0        0        0     6429 2023-06-27 05:37:44.436034 django_restit-4.1.1/inbox/migrations/0001_initial.py
+-rw-r--r--   0        0        0      380 2023-06-27 05:37:44.436102 django_restit-4.1.1/inbox/migrations/0002_alter_message_cc.py
+-rw-r--r--   0        0        0      416 2023-06-27 05:37:44.436177 django_restit-4.1.1/inbox/migrations/0003_attachment_content_type.py
+-rw-r--r--   0        0        0     1140 2023-06-27 05:37:44.436249 django_restit-4.1.1/inbox/migrations/0004_mailtemplate.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.436274 django_restit-4.1.1/inbox/migrations/__init__.py
+-rw-r--r--   0        0        0      174 2023-06-27 05:37:44.436383 django_restit-4.1.1/inbox/models/__init__.py
+-rw-r--r--   0        0        0     2832 2023-06-27 05:37:44.436463 django_restit-4.1.1/inbox/models/bounce.py
+-rw-r--r--   0        0        0     2468 2023-06-27 05:37:44.436568 django_restit-4.1.1/inbox/models/complaint.py
+-rw-r--r--   0        0        0     2879 2023-06-27 05:37:44.436797 django_restit-4.1.1/inbox/models/message.py
+-rw-r--r--   0        0        0     1013 2023-06-27 05:37:44.436870 django_restit-4.1.1/inbox/models/template.py
+-rw-r--r--   0        0        0     1534 2023-06-27 05:37:44.436956 django_restit-4.1.1/inbox/rpc.py
+-rw-r--r--   0        0        0       89 2023-06-27 05:37:44.437057 django_restit-4.1.1/inbox/utils/__init__.py
+-rw-r--r--   0        0        0     4366 2023-06-27 05:37:44.437161 django_restit-4.1.1/inbox/utils/parsing.py
+-rw-r--r--   0        0        0     4098 2023-06-27 05:37:44.437260 django_restit-4.1.1/inbox/utils/render.py
+-rw-r--r--   0        0        0     2109 2023-06-27 05:37:44.437361 django_restit-4.1.1/inbox/utils/sending.py
+-rw-r--r--   0        0        0     1114 2023-06-27 05:37:44.437469 django_restit-4.1.1/incident/README.md
+-rw-r--r--   0        0        0     1468 2023-06-27 22:00:18.628468 django_restit-4.1.1/incident/__init__.py
+-rw-r--r--   0        0        0     9720 2023-06-27 05:37:44.437670 django_restit-4.1.1/incident/migrations/0001_initial.py
+-rw-r--r--   0        0        0      595 2023-06-27 05:37:44.437757 django_restit-4.1.1/incident/migrations/0002_event_component_event_component_id.py
+-rw-r--r--   0        0        0      425 2023-06-27 05:37:44.437826 django_restit-4.1.1/incident/migrations/0003_rule_action.py
+-rw-r--r--   0        0        0      662 2023-06-27 05:37:44.437890 django_restit-4.1.1/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py
+-rw-r--r--   0        0        0      698 2023-06-27 05:37:44.437964 django_restit-4.1.1/incident/migrations/0005_incident_component_alter_incident_state.py
+-rw-r--r--   0        0        0      324 2023-06-27 05:37:44.438034 django_restit-4.1.1/incident/migrations/0006_delete_eventmetadata.py
+-rw-r--r--   0        0        0      414 2023-06-27 05:37:44.438100 django_restit-4.1.1/incident/migrations/0007_event_metadata.py
+-rw-r--r--   0        0        0      903 2023-06-27 05:37:44.438184 django_restit-4.1.1/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.438214 django_restit-4.1.1/incident/migrations/__init__.py
+-rw-r--r--   0        0        0      167 2023-06-27 05:37:44.438331 django_restit-4.1.1/incident/models/__init__.py
+-rw-r--r--   0        0        0     5068 2023-06-27 22:00:18.628641 django_restit-4.1.1/incident/models/event.py
+-rw-r--r--   0        0        0    10022 2023-06-27 05:37:44.438560 django_restit-4.1.1/incident/models/incident.py
+-rw-r--r--   0        0        0     2187 2023-06-27 05:37:44.438718 django_restit-4.1.1/incident/models/ossec.py
+-rw-r--r--   0        0        0     5300 2023-06-27 05:37:44.438826 django_restit-4.1.1/incident/models/rules.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.438911 django_restit-4.1.1/incident/parsers/__init__.py
+-rw-r--r--   0        0        0     5289 2023-06-27 05:37:44.439057 django_restit-4.1.1/incident/parsers/ossec.py
+-rw-r--r--   0        0        0      723 2023-06-27 05:37:44.439158 django_restit-4.1.1/incident/periodic.py
+-rw-r--r--   0        0        0     2831 2023-06-27 05:37:44.439252 django_restit-4.1.1/incident/rpc.py
+-rw-r--r--   0        0        0    12732 2023-06-27 05:37:44.439416 django_restit-4.1.1/incident/templates/email/incident_change.html
+-rw-r--r--   0        0        0    15173 2023-06-27 05:37:44.439515 django_restit-4.1.1/incident/templates/email/incident_new.html
+-rw-r--r--   0        0        0    13208 2023-06-27 05:37:44.439626 django_restit-4.1.1/incident/templates/email/incident_plain.html
+-rw-r--r--   0        0        0      796 2023-06-27 05:37:44.439700 django_restit-4.1.1/incident/tq.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.439791 django_restit-4.1.1/location/__init__.py
+-rw-r--r--   0        0        0      297 2023-06-27 05:37:44.439885 django_restit-4.1.1/location/admin.py
+-rw-r--r--   0        0        0     1694 2023-06-27 05:37:44.440042 django_restit-4.1.1/location/geolocate.py
+-rw-r--r--   0        0        0     7000 2023-06-27 05:37:44.440236 django_restit-4.1.1/location/migrations/0001_initial.py
+-rw-r--r--   0        0        0      576 2023-06-27 05:37:44.440313 django_restit-4.1.1/location/migrations/0002_geoip_subnet_alter_geoip_ip.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.440339 django_restit-4.1.1/location/migrations/__init__.py
+-rw-r--r--   0        0        0      230 2023-06-27 05:37:44.440480 django_restit-4.1.1/location/models/__init__.py
+-rw-r--r--   0        0        0     2028 2023-06-27 05:37:44.440559 django_restit-4.1.1/location/models/address.py
+-rw-r--r--   0        0        0     3500 2023-06-27 05:37:44.440656 django_restit-4.1.1/location/models/ip.py
+-rw-r--r--   0        0        0     1994 2023-06-27 05:37:44.440722 django_restit-4.1.1/location/models/legacy.py
+-rw-r--r--   0        0        0     2316 2023-06-27 05:37:44.440785 django_restit-4.1.1/location/models/location.py
+-rw-r--r--   0        0        0     1474 2023-06-27 05:37:44.440843 django_restit-4.1.1/location/models/track.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.440920 django_restit-4.1.1/location/providers/__init__.py
+-rw-r--r--   0        0        0      730 2023-06-27 05:37:44.441046 django_restit-4.1.1/location/providers/iplookup/__init__.py
+-rw-r--r--   0        0        0     2419 2023-06-27 05:37:44.441128 django_restit-4.1.1/location/providers/iplookup/abstractapi.py
+-rw-r--r--   0        0        0     1345 2023-06-27 05:37:44.441192 django_restit-4.1.1/location/providers/iplookup/extremeip.py
+-rw-r--r--   0        0        0     2121 2023-06-27 05:37:44.441260 django_restit-4.1.1/location/providers/iplookup/geoplugin.py
+-rw-r--r--   0        0        0     1797 2023-06-27 05:37:44.441325 django_restit-4.1.1/location/providers/iplookup/ipapi.py
+-rw-r--r--   0        0        0     1265 2023-06-27 05:37:44.441395 django_restit-4.1.1/location/providers/iplookup/ipinfo.py
+-rw-r--r--   0        0        0      937 2023-06-27 05:37:44.441463 django_restit-4.1.1/location/providers/iplookup/restit.py
+-rw-r--r--   0        0        0       42 2023-06-27 05:37:44.441569 django_restit-4.1.1/location/providers/location/__init__.py
+-rw-r--r--   0        0        0     2860 2023-06-27 05:37:44.441653 django_restit-4.1.1/location/providers/location/google.py
+-rw-r--r--   0        0        0       46 2023-06-27 05:37:44.441777 django_restit-4.1.1/location/providers/timezones/__init__.py
+-rw-r--r--   0        0        0      619 2023-06-27 05:37:44.441855 django_restit-4.1.1/location/providers/timezones/google.py
+-rw-r--r--   0        0        0     1935 2023-06-27 05:37:44.441924 django_restit-4.1.1/location/providers/zillow.py
+-rw-r--r--   0        0        0      123 2023-06-27 05:37:44.442046 django_restit-4.1.1/location/rpc/__init__.py
+-rw-r--r--   0        0        0      875 2023-07-03 18:37:00.843398 django_restit-4.1.1/location/rpc/ip.py
+-rw-r--r--   0        0        0      779 2023-06-27 05:37:44.442183 django_restit-4.1.1/location/rpc/location.py
+-rw-r--r--   0        0        0     3735 2023-06-27 05:37:44.442254 django_restit-4.1.1/location/rpc/track.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.442312 django_restit-4.1.1/medialib/__init__.py
+-rw-r--r--   0        0        0     2261 2023-06-27 05:37:44.442393 django_restit-4.1.1/medialib/admin.py
+-rw-r--r--   0        0        0       27 2023-06-27 05:37:44.442482 django_restit-4.1.1/medialib/cvutil/__init__.py
+-rw-r--r--   0        0        0     4269 2023-06-27 05:37:44.442556 django_restit-4.1.1/medialib/cvutil/contours.py
+-rw-r--r--   0        0        0    12649 2023-06-27 05:37:44.442653 django_restit-4.1.1/medialib/cvutil/images.py
+-rw-r--r--   0        0        0     9586 2023-06-27 05:37:44.442744 django_restit-4.1.1/medialib/cvutil/misc.py
+-rw-r--r--   0        0        0     5824 2023-06-27 05:37:44.442838 django_restit-4.1.1/medialib/cvutil/text.py
+-rw-r--r--   0        0        0    48442 2023-06-27 05:37:44.443047 django_restit-4.1.1/medialib/fixtures/initial_data.json
+-rw-r--r--   0        0        0    31978 2023-06-27 05:37:44.443182 django_restit-4.1.1/medialib/fixtures/medialib.json
+-rw-r--r--   0        0        0    16989 2023-06-27 05:37:44.443279 django_restit-4.1.1/medialib/fixtures/medialib_test_fixture.json
+-rw-r--r--   0        0        0     5442 2023-06-27 05:37:44.443362 django_restit-4.1.1/medialib/forms.py
+-rw-r--r--   0        0        0    20518 2023-06-27 05:37:44.443459 django_restit-4.1.1/medialib/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.443499 django_restit-4.1.1/medialib/migrations/__init__.py
+-rw-r--r--   0        0        0    52121 2023-06-27 05:37:44.443702 django_restit-4.1.1/medialib/models.py
+-rw-r--r--   0        0        0     1189 2023-06-27 05:37:44.443785 django_restit-4.1.1/medialib/ocr.py
+-rw-r--r--   0        0        0     1275 2023-06-27 05:37:44.443858 django_restit-4.1.1/medialib/pdf.py
+-rw-r--r--   0        0        0      545 2023-06-27 05:37:44.443925 django_restit-4.1.1/medialib/qrcode.py
+-rw-r--r--   0        0        0    10312 2023-06-27 05:37:44.444059 django_restit-4.1.1/medialib/render/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.444125 django_restit-4.1.1/medialib/render/engines/__init__.py
+-rw-r--r--   0        0        0     3531 2023-06-27 05:37:44.444213 django_restit-4.1.1/medialib/render/engines/anigif.py
+-rw-r--r--   0        0        0     6881 2023-06-27 05:37:44.444291 django_restit-4.1.1/medialib/render/engines/ffmpeg.py
+-rw-r--r--   0        0        0      792 2023-06-27 05:37:44.444369 django_restit-4.1.1/medialib/render/engines/gifsicle.py
+-rw-r--r--   0        0        0     3436 2023-06-27 05:37:44.444438 django_restit-4.1.1/medialib/render/engines/hls.py
+-rw-r--r--   0        0        0      983 2023-06-27 05:37:44.444498 django_restit-4.1.1/medialib/render/engines/mp4box.py
+-rw-r--r--   0        0        0      397 2023-06-27 05:37:44.444604 django_restit-4.1.1/medialib/render/engines/rtmp/Makefile
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.444636 django_restit-4.1.1/medialib/render/engines/rtmp/__init__.py
+-rw-r--r--   0        0        0     4026 2023-06-27 05:37:44.444726 django_restit-4.1.1/medialib/render/engines/rtmp/rtmp.i
+-rw-r--r--   0        0        0      699 2023-06-27 05:37:44.444798 django_restit-4.1.1/medialib/render/engines/rtmpdump.py
+-rw-r--r--   0        0        0     1017 2023-06-27 05:37:44.444865 django_restit-4.1.1/medialib/render/engines/rtmpsink.py
+-rw-r--r--   0        0        0     3466 2023-06-27 05:37:44.444941 django_restit-4.1.1/medialib/render/engines/video_getinfo.py
+-rw-r--r--   0        0        0      809 2023-06-27 05:37:44.445017 django_restit-4.1.1/medialib/render/engines/websnap.py
+-rw-r--r--   0        0        0     2193 2023-06-27 05:37:44.445078 django_restit-4.1.1/medialib/render/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.445133 django_restit-4.1.1/medialib/render/presets/__init__.py
+-rw-r--r--   0        0        0     4179 2023-06-27 05:37:44.445227 django_restit-4.1.1/medialib/render/presets/akamai.py
+-rw-r--r--   0        0        0     3284 2023-06-27 05:37:44.445306 django_restit-4.1.1/medialib/render/presets/animated_thumbnail.py
+-rw-r--r--   0        0        0     4004 2023-06-27 05:37:44.445394 django_restit-4.1.1/medialib/render/presets/ffmpeg.py
+-rw-r--r--   0        0        0     2087 2023-06-27 05:37:44.445469 django_restit-4.1.1/medialib/render/presets/flv.py
+-rw-r--r--   0        0        0     6567 2023-06-27 05:37:44.445567 django_restit-4.1.1/medialib/render/presets/hls.py
+-rw-r--r--   0        0        0     6955 2023-06-27 05:37:44.445668 django_restit-4.1.1/medialib/render/presets/image_transcode.py
+-rw-r--r--   0        0        0     1094 2023-06-27 05:37:44.445750 django_restit-4.1.1/medialib/render/presets/image_validate.py
+-rw-r--r--   0        0        0     2423 2023-06-27 05:37:44.445825 django_restit-4.1.1/medialib/render/presets/mp4.py
+-rw-r--r--   0        0        0     4997 2023-06-27 05:37:44.445908 django_restit-4.1.1/medialib/render/presets/video_still.py
+-rw-r--r--   0        0        0     3228 2023-06-27 05:37:44.445986 django_restit-4.1.1/medialib/render/presets/video_validate.py
+-rw-r--r--   0        0        0      863 2023-06-27 05:37:44.446101 django_restit-4.1.1/medialib/render/presets/websnap.py
+-rw-r--r--   0        0        0     2282 2023-06-27 05:37:44.446183 django_restit-4.1.1/medialib/render/presets/youtube.py
+-rw-r--r--   0        0        0    16451 2023-06-27 05:37:44.446294 django_restit-4.1.1/medialib/render/render_utils.py
+-rw-r--r--   0        0        0      370 2023-06-27 05:37:44.446381 django_restit-4.1.1/medialib/render/schedule.py
+-rw-r--r--   0        0        0       82 2023-06-27 05:37:44.446525 django_restit-4.1.1/medialib/rpc/__init__.py
+-rw-r--r--   0        0        0    37925 2023-06-27 05:37:44.446687 django_restit-4.1.1/medialib/rpc/legacy.py
+-rw-r--r--   0        0        0      617 2023-06-27 05:37:44.446776 django_restit-4.1.1/medialib/rpc/media.py
+-rw-r--r--   0        0        0      956 2023-06-27 05:37:44.446852 django_restit-4.1.1/medialib/rpc/tools.py
+-rwxr-xr-x   0        0        0     7875 2023-06-27 05:37:44.446994 django_restit-4.1.1/medialib/scripts/init_config
+-rw-r--r--   0        0        0     4499 2023-06-27 05:37:44.447158 django_restit-4.1.1/medialib/static/css/base_medialibui.css
+-rw-r--r--   0        0        0     3128 2023-06-27 05:37:44.447238 django_restit-4.1.1/medialib/static/css/base_widgets.css
+-rw-r--r--   0        0        0     3263 2023-06-27 05:37:44.447311 django_restit-4.1.1/medialib/static/css/jquery.jcrop.css
+-rw-r--r--   0        0        0      193 2023-06-27 05:37:44.447412 django_restit-4.1.1/medialib/static/img/arrow-down-white.png
+-rw-r--r--   0        0        0     4589 2023-06-27 05:37:44.447507 django_restit-4.1.1/medialib/static/img/bg-body.gif
+-rw-r--r--   0        0        0      441 2023-06-27 05:37:44.447579 django_restit-4.1.1/medialib/static/img/cancel.gif
+-rw-r--r--   0        0        0      341 2023-06-27 05:37:44.447648 django_restit-4.1.1/medialib/static/img/icon-generic.gif
+-rw-r--r--   0        0        0      355 2023-06-27 05:37:44.447712 django_restit-4.1.1/medialib/static/img/icon-image.gif
+-rw-r--r--   0        0        0      359 2023-06-27 05:37:44.447775 django_restit-4.1.1/medialib/static/img/icon-media.gif
+-rw-r--r--   0        0        0      355 2023-06-27 05:37:44.447850 django_restit-4.1.1/medialib/static/img/icon-zip.gif
+-rw-r--r--   0        0        0     3208 2023-06-27 05:37:44.447934 django_restit-4.1.1/medialib/static/img/loading.gif
+-rw-r--r--   0        0        0     2537 2023-06-27 05:37:44.448000 django_restit-4.1.1/medialib/static/img/noimage.gif
+-rw-r--r--   0        0        0     1057 2023-06-27 05:37:44.448065 django_restit-4.1.1/medialib/static/img/render_err.gif
+-rw-r--r--   0        0        0     6716 2023-06-27 05:37:44.448158 django_restit-4.1.1/medialib/static/img/rendering.gif
+-rw-r--r--   0        0        0      292 2023-06-27 05:37:44.448225 django_restit-4.1.1/medialib/static/img/star_off.png
+-rw-r--r--   0        0        0      297 2023-06-27 05:37:44.448287 django_restit-4.1.1/medialib/static/img/star_on.png
+-rw-r--r--   0        0        0     1130 2023-06-27 05:37:44.448351 django_restit-4.1.1/medialib/static/img/unknown.gif
+-rwxr-xr-x   0        0        0    74054 2023-06-27 05:37:44.448677 django_restit-4.1.1/medialib/static/lib/caman.full.js
+-rw-r--r--   0        0        0    17360 2023-06-27 05:37:44.448823 django_restit-4.1.1/medialib/static/lib/hammer.min.js
+-rwxr-xr-x   0        0        0    42434 2023-06-27 05:37:44.449017 django_restit-4.1.1/medialib/static/lib/jquery.Jcrop.js
+-rw-r--r--   0        0        0      743 2023-06-27 05:37:44.449098 django_restit-4.1.1/medialib/static/lib/jquery.hammer.js
+-rw-r--r--   0        0        0    16587 2023-06-27 05:37:44.449224 django_restit-4.1.1/medialib/static/lib/load-image.min.js
+-rwxr-xr-x   0        0        0   111779 2023-06-27 05:37:44.449542 django_restit-4.1.1/medialib/static/lib/swiper.js
+-rw-r--r--   0        0        0     1163 2023-06-27 05:37:44.449771 django_restit-4.1.1/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js
+-rw-r--r--   0        0        0     1163 2023-06-27 05:37:44.449850 django_restit-4.1.1/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js
+-rw-r--r--   0        0        0     5708 2023-06-27 05:37:44.449979 django_restit-4.1.1/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js
+-rw-r--r--   0        0        0     3502 2023-06-27 05:37:44.450059 django_restit-4.1.1/medialib/static/lib/tinymce/plugins/medialib/medialib.html
+-rw-r--r--   0        0        0     5876 2023-06-27 05:37:44.450187 django_restit-4.1.1/medialib/stores/__init__.py
+-rw-r--r--   0        0        0      601 2023-06-27 05:37:44.450314 django_restit-4.1.1/medialib/stores/apiclient/__init__.py
+-rw-r--r--   0        0        0     9852 2023-06-27 05:37:44.450415 django_restit-4.1.1/medialib/stores/apiclient/channel.py
+-rw-r--r--   0        0        0    35929 2023-06-27 05:37:44.450591 django_restit-4.1.1/medialib/stores/apiclient/discovery.py
+-rw-r--r--   0        0        0     3516 2023-06-27 05:37:44.450684 django_restit-4.1.1/medialib/stores/apiclient/errors.py
+-rw-r--r--   0        0        0    52911 2023-06-27 05:37:44.450906 django_restit-4.1.1/medialib/stores/apiclient/http.py
+-rw-r--r--   0        0        0     6505 2023-06-27 05:37:44.451002 django_restit-4.1.1/medialib/stores/apiclient/mimeparse.py
+-rw-r--r--   0        0        0    11761 2023-06-27 05:37:44.451111 django_restit-4.1.1/medialib/stores/apiclient/model.py
+-rw-r--r--   0        0        0     3528 2023-06-27 05:37:44.451205 django_restit-4.1.1/medialib/stores/apiclient/sample_tools.py
+-rw-r--r--   0        0        0     9293 2023-06-27 05:37:44.451302 django_restit-4.1.1/medialib/stores/apiclient/schema.py
+-rw-r--r--   0        0        0     1592 2023-06-27 05:37:44.451390 django_restit-4.1.1/medialib/stores/filestore.py
+-rw-r--r--   0        0        0    69575 2023-06-27 05:37:44.451712 django_restit-4.1.1/medialib/stores/httplib2/__init__.py
+-rw-r--r--   0        0        0    39670 2023-06-27 05:37:44.451937 django_restit-4.1.1/medialib/stores/httplib2/cacerts.txt
+-rw-r--r--   0        0        0     3821 2023-06-27 05:37:44.452031 django_restit-4.1.1/medialib/stores/httplib2/iri2uri.py
+-rw-r--r--   0        0        0    18452 2023-06-27 05:37:44.452160 django_restit-4.1.1/medialib/stores/httplib2/socks.py
+-rw-r--r--   0        0        0      706 2023-06-27 05:37:44.452238 django_restit-4.1.1/medialib/stores/httpstore.py
+-rw-r--r--   0        0        0      304 2023-06-27 05:37:44.452325 django_restit-4.1.1/medialib/stores/nullstore.py
+-rw-r--r--   0        0        0      213 2023-06-27 05:37:44.452492 django_restit-4.1.1/medialib/stores/oauth2client/__init__.py
+-rw-r--r--   0        0        0     1044 2023-06-27 05:37:44.452598 django_restit-4.1.1/medialib/stores/oauth2client/anyjson.py
+-rw-r--r--   0        0        0    32534 2023-06-27 05:37:44.452767 django_restit-4.1.1/medialib/stores/oauth2client/appengine.py
+-rw-r--r--   0        0        0    44346 2023-06-27 05:37:44.452995 django_restit-4.1.1/medialib/stores/oauth2client/client.py
+-rw-r--r--   0        0        0     4425 2023-06-27 05:37:44.453091 django_restit-4.1.1/medialib/stores/oauth2client/clientsecrets.py
+-rw-r--r--   0        0        0    10239 2023-06-27 05:37:44.453196 django_restit-4.1.1/medialib/stores/oauth2client/crypt.py
+-rw-r--r--   0        0        0     3755 2023-06-27 05:37:44.453276 django_restit-4.1.1/medialib/stores/oauth2client/django_orm.py
+-rw-r--r--   0        0        0     3164 2023-06-27 05:37:44.453391 django_restit-4.1.1/medialib/stores/oauth2client/file.py
+-rw-r--r--   0        0        0     3036 2023-06-27 05:37:44.453451 django_restit-4.1.1/medialib/stores/oauth2client/gce.py
+-rw-r--r--   0        0        0     3229 2023-06-27 05:37:44.453541 django_restit-4.1.1/medialib/stores/oauth2client/keyring_storage.py
+-rw-r--r--   0        0        0    11393 2023-06-27 05:37:44.453634 django_restit-4.1.1/medialib/stores/oauth2client/locked_file.py
+-rw-r--r--   0        0        0    13950 2023-06-27 05:37:44.453698 django_restit-4.1.1/medialib/stores/oauth2client/multistore_file.py
+-rw-r--r--   0        0        0     5588 2023-06-27 05:37:44.453764 django_restit-4.1.1/medialib/stores/oauth2client/old_run.py
+-rw-r--r--   0        0        0     8379 2023-06-27 05:37:44.453855 django_restit-4.1.1/medialib/stores/oauth2client/tools.py
+-rw-r--r--   0        0        0     5706 2023-06-27 05:37:44.453938 django_restit-4.1.1/medialib/stores/oauth2client/util.py
+-rw-r--r--   0        0        0     3367 2023-06-27 05:37:44.454013 django_restit-4.1.1/medialib/stores/oauth2client/xsrfutil.py
+-rw-r--r--   0        0        0      500 2023-06-27 05:37:44.454077 django_restit-4.1.1/medialib/stores/rtmpstore.py
+-rw-r--r--   0        0        0     4583 2023-06-27 05:37:44.454163 django_restit-4.1.1/medialib/stores/s3store.py
+-rw-r--r--   0        0        0     4996 2023-06-27 05:37:44.454272 django_restit-4.1.1/medialib/stores/uritemplate/__init__.py
+-rw-r--r--   0        0        0      406 2023-06-27 05:37:44.454334 django_restit-4.1.1/medialib/stores/youtubestore.py
+-rw-r--r--   0        0        0     3691 2023-06-27 05:37:44.454500 django_restit-4.1.1/medialib/templates/medialib/base.html
+-rw-r--r--   0        0        0     1277 2023-06-27 05:37:44.454591 django_restit-4.1.1/medialib/templates/medialib/instances.html
+-rw-r--r--   0        0        0     1170 2023-06-27 05:37:44.454657 django_restit-4.1.1/medialib/templates/medialib/items.html
+-rw-r--r--   0        0        0     8194 2023-06-27 05:37:44.454746 django_restit-4.1.1/medialib/templates/medialib/library.html
+-rw-r--r--   0        0        0       65 2023-06-27 05:37:44.454810 django_restit-4.1.1/medialib/templates/medialib/notify_error.subject
+-rw-r--r--   0        0        0       49 2023-06-27 05:37:44.454869 django_restit-4.1.1/medialib/templates/medialib/notify_error.to
+-rw-r--r--   0        0        0      272 2023-06-27 05:37:44.454932 django_restit-4.1.1/medialib/templates/medialib/notify_error.txt
+-rw-r--r--   0        0        0       71 2023-06-27 05:37:44.454996 django_restit-4.1.1/medialib/templates/medialib/notify_ready.subject
+-rw-r--r--   0        0        0       49 2023-06-27 05:37:44.455056 django_restit-4.1.1/medialib/templates/medialib/notify_ready.to
+-rw-r--r--   0        0        0      298 2023-06-27 05:37:44.455113 django_restit-4.1.1/medialib/templates/medialib/notify_ready.txt
+-rw-r--r--   0        0        0       64 2023-06-27 05:37:44.455175 django_restit-4.1.1/medialib/templates/medialib/notify_render_error.subject
+-rw-r--r--   0        0        0       48 2023-06-27 05:37:44.455232 django_restit-4.1.1/medialib/templates/medialib/notify_render_error.to
+-rw-r--r--   0        0        0      271 2023-06-27 05:37:44.455301 django_restit-4.1.1/medialib/templates/medialib/notify_render_error.txt
+-rw-r--r--   0        0        0       68 2023-06-27 05:37:44.455380 django_restit-4.1.1/medialib/templates/medialib/notify_validate_error.subject
+-rw-r--r--   0        0        0       48 2023-06-27 05:37:44.455452 django_restit-4.1.1/medialib/templates/medialib/notify_validate_error.to
+-rw-r--r--   0        0        0      275 2023-06-27 05:37:44.455521 django_restit-4.1.1/medialib/templates/medialib/notify_validate_error.txt
+-rw-r--r--   0        0        0      206 2023-06-27 05:37:44.455593 django_restit-4.1.1/medialib/templates/medialib/smil
+-rw-r--r--   0        0        0     1177 2023-06-27 05:37:44.455665 django_restit-4.1.1/medialib/templates/medialib/test.html
+-rw-r--r--   0        0        0     1549 2023-06-27 05:37:44.455737 django_restit-4.1.1/medialib/templates/medialib/testpicker.html
+-rw-r--r--   0        0        0     6045 2023-06-27 05:37:44.455814 django_restit-4.1.1/medialib/tests.py
+-rw-r--r--   0        0        0      544 2023-06-27 05:37:44.455873 django_restit-4.1.1/medialib/tq.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.455894 django_restit-4.1.1/medialib/urls.py
+-rw-r--r--   0        0        0     3756 2023-06-27 05:37:44.455970 django_restit-4.1.1/medialib/utils.py
+-rw-r--r--   0        0        0     4321 2023-06-27 05:37:44.456050 django_restit-4.1.1/medialib/views.py
+-rw-r--r--   0        0        0     4303 2023-06-27 05:37:44.456166 django_restit-4.1.1/medialib/youtube/__init__.py
+-rw-r--r--   0        0        0      601 2023-06-27 05:37:44.456272 django_restit-4.1.1/medialib/youtube/apiclient/__init__.py
+-rw-r--r--   0        0        0     9886 2023-06-27 05:37:44.456332 django_restit-4.1.1/medialib/youtube/apiclient/channel.py
+-rw-r--r--   0        0        0    35907 2023-06-27 05:37:44.456516 django_restit-4.1.1/medialib/youtube/apiclient/discovery.py
+-rw-r--r--   0        0        0     3550 2023-06-27 05:37:44.456592 django_restit-4.1.1/medialib/youtube/apiclient/errors.py
+-rw-r--r--   0        0        0    52945 2023-06-27 05:37:44.456694 django_restit-4.1.1/medialib/youtube/apiclient/http.py
+-rw-r--r--   0        0        0     6505 2023-06-27 05:37:44.456785 django_restit-4.1.1/medialib/youtube/apiclient/mimeparse.py
+-rw-r--r--   0        0        0    11795 2023-06-27 05:37:44.456835 django_restit-4.1.1/medialib/youtube/apiclient/model.py
+-rw-r--r--   0        0        0     3596 2023-06-27 05:37:44.456895 django_restit-4.1.1/medialib/youtube/apiclient/sample_tools.py
+-rw-r--r--   0        0        0     9327 2023-06-27 05:37:44.456959 django_restit-4.1.1/medialib/youtube/apiclient/schema.py
+-rw-r--r--   0        0        0    69581 2023-06-27 05:37:44.457093 django_restit-4.1.1/medialib/youtube/httplib2/__init__.py
+-rw-r--r--   0        0        0    39670 2023-06-27 05:37:44.457310 django_restit-4.1.1/medialib/youtube/httplib2/cacerts.txt
+-rw-r--r--   0        0        0     3821 2023-06-27 05:37:44.457412 django_restit-4.1.1/medialib/youtube/httplib2/iri2uri.py
+-rw-r--r--   0        0        0    18452 2023-06-27 05:37:44.457533 django_restit-4.1.1/medialib/youtube/httplib2/socks.py
+-rw-r--r--   0        0        0      213 2023-06-27 05:37:44.457629 django_restit-4.1.1/medialib/youtube/oauth2client/__init__.py
+-rw-r--r--   0        0        0     1044 2023-06-27 05:37:44.457687 django_restit-4.1.1/medialib/youtube/oauth2client/anyjson.py
+-rw-r--r--   0        0        0    32534 2023-06-27 05:37:44.457830 django_restit-4.1.1/medialib/youtube/oauth2client/appengine.py
+-rw-r--r--   0        0        0    44431 2023-06-27 05:37:44.457905 django_restit-4.1.1/medialib/youtube/oauth2client/client.py
+-rw-r--r--   0        0        0     4425 2023-06-27 05:37:44.457990 django_restit-4.1.1/medialib/youtube/oauth2client/clientsecrets.py
+-rw-r--r--   0        0        0    10239 2023-06-27 05:37:44.458075 django_restit-4.1.1/medialib/youtube/oauth2client/crypt.py
+-rw-r--r--   0        0        0     3753 2023-06-27 05:37:44.458140 django_restit-4.1.1/medialib/youtube/oauth2client/django_orm.py
+-rw-r--r--   0        0        0     3164 2023-06-27 05:37:44.458204 django_restit-4.1.1/medialib/youtube/oauth2client/file.py
+-rw-r--r--   0        0        0     3036 2023-06-27 05:37:44.458255 django_restit-4.1.1/medialib/youtube/oauth2client/gce.py
+-rw-r--r--   0        0        0     3229 2023-06-27 05:37:44.458323 django_restit-4.1.1/medialib/youtube/oauth2client/keyring_storage.py
+-rw-r--r--   0        0        0    11393 2023-06-27 05:37:44.458399 django_restit-4.1.1/medialib/youtube/oauth2client/locked_file.py
+-rw-r--r--   0        0        0    13950 2023-06-27 05:37:44.458454 django_restit-4.1.1/medialib/youtube/oauth2client/multistore_file.py
+-rw-r--r--   0        0        0     5588 2023-06-27 05:37:44.458510 django_restit-4.1.1/medialib/youtube/oauth2client/old_run.py
+-rw-r--r--   0        0        0     8379 2023-06-27 05:37:44.458604 django_restit-4.1.1/medialib/youtube/oauth2client/tools.py
+-rw-r--r--   0        0        0     5706 2023-06-27 05:37:44.458680 django_restit-4.1.1/medialib/youtube/oauth2client/util.py
+-rw-r--r--   0        0        0     3367 2023-06-27 05:37:44.458745 django_restit-4.1.1/medialib/youtube/oauth2client/xsrfutil.py
+-rw-r--r--   0        0        0     2849 2023-06-27 05:37:44.458806 django_restit-4.1.1/medialib/youtube/upload.py
+-rw-r--r--   0        0        0     4996 2023-06-27 05:37:44.458902 django_restit-4.1.1/medialib/youtube/uritemplate/__init__.py
+-rw-r--r--   0        0        0     2307 2023-06-27 05:37:44.459001 django_restit-4.1.1/metrics/README.md
+-rw-r--r--   0        0        0       90 2023-06-27 05:37:44.459061 django_restit-4.1.1/metrics/__init__.py
+-rw-r--r--   0        0        0    23460 2023-06-27 05:37:44.459219 django_restit-4.1.1/metrics/client.py
+-rw-r--r--   0        0        0     9182 2023-06-27 05:37:44.459333 django_restit-4.1.1/metrics/eod.py
+-rw-r--r--   0        0        0     1664 2023-06-27 05:37:44.459430 django_restit-4.1.1/metrics/examples/eod_example.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.459493 django_restit-4.1.1/metrics/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.459564 django_restit-4.1.1/metrics/management/commands/__init__.py
+-rw-r--r--   0        0        0      429 2023-06-27 05:37:44.459636 django_restit-4.1.1/metrics/management/commands/delete_gauge.py
+-rw-r--r--   0        0        0      464 2023-06-27 05:37:44.459697 django_restit-4.1.1/metrics/management/commands/delete_metric.py
+-rw-r--r--   0        0        0     2801 2023-06-27 05:37:44.459766 django_restit-4.1.1/metrics/management/commands/fix_redis_metrics_keys.py
+-rw-r--r--   0        0        0     1928 2023-06-27 05:37:44.459829 django_restit-4.1.1/metrics/management/commands/generate_test_metrics.py
+-rw-r--r--   0        0        0     1742 2023-06-27 05:37:44.459896 django_restit-4.1.1/metrics/management/commands/redis_metrics_send_mail.py
+-rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.459957 django_restit-4.1.1/metrics/management/commands/reset_weekly_metrics.py
+-rw-r--r--   0        0        0     4343 2023-06-27 05:37:44.460023 django_restit-4.1.1/metrics/management/commands/system_metric.py
+-rw-r--r--   0        0        0     2399 2023-06-27 05:37:44.460109 django_restit-4.1.1/metrics/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1510 2023-06-27 05:37:44.460172 django_restit-4.1.1/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py
+-rw-r--r--   0        0        0      453 2023-06-27 05:37:44.460231 django_restit-4.1.1/metrics/migrations/0003_metrics_expires.py
+-rw-r--r--   0        0        0     3271 2023-06-27 05:37:44.460284 django_restit-4.1.1/metrics/migrations/0004_eodmetrics.py
+-rw-r--r--   0        0        0     2358 2023-06-27 05:37:44.460347 django_restit-4.1.1/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460367 django_restit-4.1.1/metrics/migrations/__init__.py
+-rw-r--r--   0        0        0    10599 2023-06-27 05:37:44.460461 django_restit-4.1.1/metrics/models.py
+-rw-r--r--   0        0        0      480 2023-06-27 05:37:44.460528 django_restit-4.1.1/metrics/periodic.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460587 django_restit-4.1.1/metrics/providers/__init__.py
+-rw-r--r--   0        0        0     7335 2023-06-27 05:37:44.460691 django_restit-4.1.1/metrics/providers/aws.py
+-rw-r--r--   0        0        0    14827 2023-07-11 15:48:34.905677 django_restit-4.1.1/metrics/rpc.py
+-rw-r--r--   0        0        0      132 2023-06-27 05:37:44.460832 django_restit-4.1.1/metrics/settings.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.460855 django_restit-4.1.1/metrics/tq.py
+-rw-r--r--   0        0        0    10490 2023-06-27 05:37:44.460959 django_restit-4.1.1/metrics/utils.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461016 django_restit-4.1.1/pushit/__init__.py
+-rw-r--r--   0        0        0      451 2023-06-27 05:37:44.461079 django_restit-4.1.1/pushit/admin.py
+-rw-r--r--   0        0        0     4555 2023-06-27 05:37:44.461167 django_restit-4.1.1/pushit/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461190 django_restit-4.1.1/pushit/migrations/__init__.py
+-rw-r--r--   0        0        0     5066 2023-07-11 15:47:46.945937 django_restit-4.1.1/pushit/models.py
+-rw-r--r--   0        0        0       88 2023-06-27 05:37:44.461351 django_restit-4.1.1/pushit/rpc/__init__.py
+-rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.461414 django_restit-4.1.1/pushit/rpc/githooks.py
+-rw-r--r--   0        0        0     5028 2023-06-27 05:37:44.461473 django_restit-4.1.1/pushit/rpc/legacy.py
+-rw-r--r--   0        0        0      378 2023-06-27 05:37:44.461520 django_restit-4.1.1/pushit/rpc/products.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.461605 django_restit-4.1.1/pushit/static/js/models_pushit.js
+-rw-r--r--   0        0        0      131 2023-06-27 05:37:44.461676 django_restit-4.1.1/pushit/tq.py
+-rw-r--r--   0        0        0     1966 2023-06-27 05:37:44.461734 django_restit-4.1.1/pushit/utils.py
+-rw-r--r--   0        0        0     1167 2023-07-11 18:19:59.918769 django_restit-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0      118 2023-06-27 05:37:44.461884 django_restit-4.1.1/rest/.gitignore
+-rw-r--r--   0        0        0     5460 2023-06-27 05:37:44.461959 django_restit-4.1.1/rest/README.md
+-rw-r--r--   0        0        0       72 2023-06-27 05:37:44.462010 django_restit-4.1.1/rest/RemoteEvents.py
+-rw-r--r--   0        0        0      120 2023-07-11 18:19:59.951382 django_restit-4.1.1/rest/__init__.py
+-rw-r--r--   0        0        0     1967 2023-06-27 05:37:44.462114 django_restit-4.1.1/rest/arc4.py
+-rw-r--r--   0        0        0       83 2023-06-27 05:37:44.462161 django_restit-4.1.1/rest/cache.py
+-rw-r--r--   0        0        0       72 2023-06-27 05:37:44.462295 django_restit-4.1.1/rest/crypto/__init__.py
+-rw-r--r--   0        0        0     3605 2023-06-27 05:37:44.462374 django_restit-4.1.1/rest/crypto/aes.py
+-rw-r--r--   0        0        0     4082 2023-06-27 05:37:44.462442 django_restit-4.1.1/rest/crypto/privpub.py
+-rw-r--r--   0        0        0     4514 2023-07-11 15:29:38.508089 django_restit-4.1.1/rest/crypto/util.py
+-rw-r--r--   0        0        0     7784 2023-06-27 05:37:44.462604 django_restit-4.1.1/rest/datem.py
+-rw-r--r--   0        0        0    15573 2023-07-11 15:46:20.585526 django_restit-4.1.1/rest/decorators.py
+-rw-r--r--   0        0        0      788 2023-06-27 05:37:44.462816 django_restit-4.1.1/rest/encryption.py
+-rw-r--r--   0        0        0      501 2023-07-11 15:16:32.180675 django_restit-4.1.1/rest/errors.py
+-rw-r--r--   0        0        0       54 2023-06-27 05:37:44.462913 django_restit-4.1.1/rest/extra/__init__.py
+-rw-r--r--   0        0        0     1078 2023-06-27 05:37:44.462982 django_restit-4.1.1/rest/extra/json_metadata.py
+-rw-r--r--   0        0        0     9719 2023-06-27 05:37:44.463072 django_restit-4.1.1/rest/fields.py
+-rw-r--r--   0        0        0     6316 2023-06-27 05:37:44.463145 django_restit-4.1.1/rest/forms.py
+-rw-r--r--   0        0        0    24650 2023-07-11 15:25:55.654664 django_restit-4.1.1/rest/helpers.py
+-rw-r--r--   0        0        0      260 2023-06-27 05:37:44.463338 django_restit-4.1.1/rest/joke.py
+-rw-r--r--   0        0        0     2298 2023-06-27 05:37:44.463411 django_restit-4.1.1/rest/jwtoken.py
+-rw-r--r--   0        0        0    20930 2023-06-27 15:33:50.289063 django_restit-4.1.1/rest/log.py
+-rw-r--r--   0        0        0     7754 2023-06-27 05:37:44.463623 django_restit-4.1.1/rest/mail.py
+-rw-r--r--   0        0        0     9174 2023-06-27 05:37:44.463711 django_restit-4.1.1/rest/mailman.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.463776 django_restit-4.1.1/rest/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.463861 django_restit-4.1.1/rest/management/commands/__init__.py
+-rw-r--r--   0        0        0      389 2023-06-27 05:37:44.463942 django_restit-4.1.1/rest/management/commands/rpc.py
+-rw-r--r--   0        0        0       33 2023-06-27 05:37:44.464028 django_restit-4.1.1/rest/middleware/__init__.py
+-rw-r--r--   0        0        0     3513 2023-06-27 05:37:44.464096 django_restit-4.1.1/rest/middleware/cors.py
+-rw-r--r--   0        0        0     2345 2023-06-27 05:37:44.464159 django_restit-4.1.1/rest/middleware/db_router.py
+-rw-r--r--   0        0        0     5395 2023-06-27 05:37:44.464226 django_restit-4.1.1/rest/middleware/jwt.py
+-rw-r--r--   0        0        0     4127 2023-06-27 05:37:44.464313 django_restit-4.1.1/rest/middleware/request.py
+-rw-r--r--   0        0        0     9015 2023-06-27 05:37:44.464386 django_restit-4.1.1/rest/middleware/session.py
+-rw-r--r--   0        0        0     1874 2023-06-27 05:37:44.464450 django_restit-4.1.1/rest/middleware/session_store.py
+-rw-r--r--   0        0        0      130 2023-07-11 15:56:36.722347 django_restit-4.1.1/rest/models/__init__.py
+-rw-r--r--   0        0        0    62119 2023-07-11 15:52:56.358820 django_restit-4.1.1/rest/models/base.py
+-rw-r--r--   0        0        0      578 2023-07-11 16:03:40.953305 django_restit-4.1.1/rest/models/cacher.py
+-rw-r--r--   0        0        0    11606 2023-07-11 15:42:46.818779 django_restit-4.1.1/rest/models/metadata.py
+-rw-r--r--   0        0        0   149463 2023-06-27 05:37:44.465139 django_restit-4.1.1/rest/regexes.yaml
+-rw-r--r--   0        0        0    14894 2023-06-27 05:37:44.465209 django_restit-4.1.1/rest/requestex.py
+-rw-r--r--   0        0        0     3713 2023-06-27 15:25:34.225162 django_restit-4.1.1/rest/rpc.py
+-rw-r--r--   0        0        0     7645 2023-06-27 05:37:44.465350 django_restit-4.1.1/rest/search.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.465410 django_restit-4.1.1/rest/serializers/__init__.py
+-rw-r--r--   0        0        0     2008 2023-07-11 17:55:17.285164 django_restit-4.1.1/rest/serializers/collection.py
+-rw-r--r--   0        0        0     2975 2023-06-27 05:37:44.465556 django_restit-4.1.1/rest/serializers/csv.py
+-rw-r--r--   0        0        0     1077 2023-06-27 05:37:44.465616 django_restit-4.1.1/rest/serializers/excel.py
+-rw-r--r--   0        0        0     1736 2023-06-27 05:37:44.465675 django_restit-4.1.1/rest/serializers/json.py
+-rw-r--r--   0        0        0    61795 2023-07-11 16:27:26.664542 django_restit-4.1.1/rest/serializers/legacy.py
+-rw-r--r--   0        0        0     6624 2023-07-11 17:55:26.790313 django_restit-4.1.1/rest/serializers/model.py
+-rw-r--r--   0        0        0      997 2023-07-06 18:50:18.372944 django_restit-4.1.1/rest/serializers/profiler.py
+-rw-r--r--   0        0        0     6464 2023-07-06 19:20:17.703981 django_restit-4.1.1/rest/serializers/response.py
+-rw-r--r--   0        0        0     2734 2023-06-27 05:37:44.466139 django_restit-4.1.1/rest/serializers/util.py
+-rw-r--r--   0        0        0     1532 2023-06-27 05:37:44.466216 django_restit-4.1.1/rest/settings_helper.py
+-rw-r--r--   0        0        0    95786 2023-06-27 05:37:44.466685 django_restit-4.1.1/rest/static/lib/jquery.js
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466742 django_restit-4.1.1/rest/static/rest/app.css
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466776 django_restit-4.1.1/rest/static/rest/app.js
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466808 django_restit-4.1.1/rest/static/rest/rest.js
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.466846 django_restit-4.1.1/rest/static/rest/rest.scss
+-rw-r--r--   0        0        0      529 2023-06-27 05:37:44.466992 django_restit-4.1.1/rest/templates/email/error.html
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.467020 django_restit-4.1.1/rest/templates/email/error.subject
+-rw-r--r--   0        0        0     7148 2023-06-27 05:37:44.467101 django_restit-4.1.1/rest/templates/rest_docs.html
+-rw-r--r--   0        0        0    10880 2023-06-27 05:37:44.467182 django_restit-4.1.1/rest/templates/rest_html.html
+-rw-r--r--   0        0        0   185122 2023-06-27 05:37:44.467607 django_restit-4.1.1/rest/ua.py
+-rw-r--r--   0        0        0    17064 2023-06-27 05:37:44.467734 django_restit-4.1.1/rest/uberdict.py
+-rw-r--r--   0        0        0    11881 2023-06-27 05:37:44.467820 django_restit-4.1.1/rest/url_docs.py
+-rw-r--r--   0        0        0     1787 2023-06-27 05:37:44.467877 django_restit-4.1.1/rest/urls.py
+-rw-r--r--   0        0        0     1056 2023-06-27 05:37:44.467929 django_restit-4.1.1/rest/views.py
+-rw-r--r--   0        0        0      118 2023-06-27 05:37:44.468007 django_restit-4.1.1/sessionlog/.gitignore
+-rw-r--r--   0        0        0       62 2023-06-27 05:37:44.468062 django_restit-4.1.1/sessionlog/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468086 django_restit-4.1.1/sessionlog/__init__.py
+-rw-r--r--   0        0        0      245 2023-06-27 05:37:44.468153 django_restit-4.1.1/sessionlog/admin.py
+-rw-r--r--   0        0        0     1694 2023-06-27 05:37:44.468231 django_restit-4.1.1/sessionlog/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468261 django_restit-4.1.1/sessionlog/migrations/__init__.py
+-rw-r--r--   0        0        0     3978 2023-07-05 22:43:30.431976 django_restit-4.1.1/sessionlog/models.py
+-rw-r--r--   0        0        0      383 2023-06-27 05:37:44.468400 django_restit-4.1.1/sessionlog/tests.py
+-rw-r--r--   0        0        0       26 2023-06-27 05:37:44.468451 django_restit-4.1.1/sessionlog/views.py
+-rw-r--r--   0        0        0     2196 2023-06-27 05:37:44.468543 django_restit-4.1.1/taskqueue/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468569 django_restit-4.1.1/taskqueue/__init__.py
+-rw-r--r--   0        0        0      208 2023-06-27 05:37:44.468635 django_restit-4.1.1/taskqueue/admin.py
+-rw-r--r--   0        0        0     4738 2023-06-27 05:37:44.468730 django_restit-4.1.1/taskqueue/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.468758 django_restit-4.1.1/taskqueue/migrations/__init__.py
+-rw-r--r--   0        0        0    16531 2023-06-27 05:37:44.468876 django_restit-4.1.1/taskqueue/models.py
+-rw-r--r--   0        0        0     3072 2023-06-27 05:37:44.468952 django_restit-4.1.1/taskqueue/periodic.py
+-rw-r--r--   0        0        0     5326 2023-06-27 05:37:44.469019 django_restit-4.1.1/taskqueue/rpc.py
+-rw-r--r--   0        0        0      942 2023-06-27 05:37:44.469073 django_restit-4.1.1/taskqueue/tq.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469126 django_restit-4.1.1/taskqueue/transports/__init__.py
+-rw-r--r--   0        0        0      623 2023-06-27 05:37:44.469185 django_restit-4.1.1/taskqueue/transports/email.py
+-rw-r--r--   0        0        0     2409 2023-06-27 05:37:44.469240 django_restit-4.1.1/taskqueue/transports/http.py
+-rw-r--r--   0        0        0     1099 2023-06-27 05:37:44.469291 django_restit-4.1.1/taskqueue/transports/s3.py
+-rw-r--r--   0        0        0     1891 2023-06-27 05:37:44.469341 django_restit-4.1.1/taskqueue/transports/sftp.py
+-rw-r--r--   0        0        0      142 2023-06-27 05:37:44.469388 django_restit-4.1.1/taskqueue/transports/sms.py
+-rw-r--r--   0        0        0    13660 2023-06-27 05:37:44.469465 django_restit-4.1.1/taskqueue/worker.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469517 django_restit-4.1.1/telephony/__init__.py
+-rw-r--r--   0        0        0      243 2023-06-27 05:37:44.469571 django_restit-4.1.1/telephony/admin.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469591 django_restit-4.1.1/telephony/decorators.py
+-rw-r--r--   0        0        0     3030 2023-06-27 05:37:44.469692 django_restit-4.1.1/telephony/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.469714 django_restit-4.1.1/telephony/migrations/__init__.py
+-rw-r--r--   0        0        0     7753 2023-06-27 05:37:44.469796 django_restit-4.1.1/telephony/models.py
+-rw-r--r--   0        0        0     2126 2023-06-27 05:37:44.469861 django_restit-4.1.1/telephony/phone_util.py
+-rw-r--r--   0        0        0     2659 2023-06-27 05:37:44.469923 django_restit-4.1.1/telephony/rpc.py
+-rw-r--r--   0        0        0     3624 2023-06-27 05:37:44.470008 django_restit-4.1.1/ws4redis/README.md
+-rwxr-xr-x   0        0        0       46 2023-06-27 05:37:44.470065 django_restit-4.1.1/ws4redis/__init__.py
+-rw-r--r--   0        0        0     4942 2023-06-27 05:37:44.470133 django_restit-4.1.1/ws4redis/client.py
+-rw-r--r--   0        0        0    13110 2023-07-08 23:34:53.804529 django_restit-4.1.1/ws4redis/connection.py
+-rwxr-xr-x   0        0        0      636 2023-06-27 05:37:44.470295 django_restit-4.1.1/ws4redis/exceptions.py
+-rw-r--r--   0        0        0     5561 2023-07-08 23:30:25.146274 django_restit-4.1.1/ws4redis/redis.py
+-rw-r--r--   0        0        0        0 2023-06-27 05:37:44.470422 django_restit-4.1.1/ws4redis/servers/__init__.py
+-rw-r--r--   0        0        0     3747 2023-06-27 05:37:44.470507 django_restit-4.1.1/ws4redis/servers/base.py
+-rw-r--r--   0        0        0     4329 2023-06-27 05:37:44.470582 django_restit-4.1.1/ws4redis/servers/django.py
+-rw-r--r--   0        0        0     1723 2023-06-27 05:37:44.470638 django_restit-4.1.1/ws4redis/servers/uwsgi.py
+-rwxr-xr-x   0        0        0     1411 2023-06-27 05:37:44.470697 django_restit-4.1.1/ws4redis/settings.py
+-rwxr-xr-x   0        0        0     5122 2023-06-27 05:37:44.470772 django_restit-4.1.1/ws4redis/utf8validator.py
+-rwxr-xr-x   0        0        0    14848 2023-06-27 05:37:44.470868 django_restit-4.1.1/ws4redis/websocket.py
+-rw-r--r--   0        0        0     7531 1970-01-01 00:00:00.000000 django_restit-4.1.1/PKG-INFO
```

### Comparing `django_restit-4.0.9/LICENSE.md` & `django_restit-4.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/README.md` & `django_restit-4.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/admin.py` & `django_restit-4.1.1/account/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/fcm/__init__.py` & `django_restit-4.1.1/account/fcm/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/migrations/0001_initial.py` & `django_restit-4.1.1/account/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/migrations/0003_member_phone_number.py` & `django_restit-4.1.1/account/migrations/0003_member_phone_number.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/migrations/0004_group_modified_alter_group_created.py` & `django_restit-4.1.1/account/migrations/0004_group_modified_alter_group_created.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/migrations/0007_authtoken_signature_authsession.py` & `django_restit-4.1.1/account/migrations/0007_authtoken_signature_authsession.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/migrations/0008_memberdevice_memberdevicemetadata.py` & `django_restit-4.1.1/account/migrations/0008_memberdevice_memberdevicemetadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/migrations/0011_authtoken.py` & `django_restit-4.1.1/account/migrations/0011_authtoken.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/migrations/0012_settings_settingsmetadata.py` & `django_restit-4.1.1/account/migrations/0012_settings_settingsmetadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/models/device.py` & `django_restit-4.1.1/account/models/device.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/models/feeds.py` & `django_restit-4.1.1/account/models/feeds.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/models/group.py` & `django_restit-4.1.1/account/models/group.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/models/legacy.py` & `django_restit-4.1.1/account/models/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/models/member.py` & `django_restit-4.1.1/account/models/member.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/models/membership.py` & `django_restit-4.1.1/account/models/membership.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/models/notify.py` & `django_restit-4.1.1/account/models/notify.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/models/session.py` & `django_restit-4.1.1/account/models/session.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/models/settings.py` & `django_restit-4.1.1/account/models/settings.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/oauth/google.py` & `django_restit-4.1.1/account/oauth/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/periodic.py` & `django_restit-4.1.1/account/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/rpc/auth.py` & `django_restit-4.1.1/account/rpc/auth.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/rpc/device.py` & `django_restit-4.1.1/account/rpc/device.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/rpc/group.py` & `django_restit-4.1.1/account/rpc/group.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/rpc/member.py` & `django_restit-4.1.1/account/rpc/member.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/rpc/notify.py` & `django_restit-4.1.1/account/rpc/notify.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/rpc/oauth.py` & `django_restit-4.1.1/account/rpc/oauth.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/templates/email/base.html` & `django_restit-4.1.1/account/templates/email/base.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/templates/email/invite.html` & `django_restit-4.1.1/account/templates/email/invite.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/templates/email/plain/invite.html` & `django_restit-4.1.1/account/templates/email/plain/invite.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/templates/email/plain/reset_code.html` & `django_restit-4.1.1/account/templates/email/plain/reset_code.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/templates/email/reset_code.html` & `django_restit-4.1.1/account/templates/email/reset_code.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/templates/email/simple/invite.html` & `django_restit-4.1.1/account/templates/email/simple/invite.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/account/templates/email/simple/reset_code.html` & `django_restit-4.1.1/account/templates/email/simple/reset_code.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/auditlog/README` & `django_restit-4.1.1/auditlog/README`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/auditlog/admin.py` & `django_restit-4.1.1/auditlog/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/auditlog/decorators.py` & `django_restit-4.1.1/auditlog/decorators.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/auditlog/middleware.py` & `django_restit-4.1.1/auditlog/middleware.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/auditlog/migrations/0001_initial.py` & `django_restit-4.1.1/auditlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/auditlog/models.py` & `django_restit-4.1.1/auditlog/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/auditlog/rpc.py` & `django_restit-4.1.1/auditlog/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/auditlog/tq.py` & `django_restit-4.1.1/auditlog/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/inbox/README.md` & `django_restit-4.1.1/inbox/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/inbox/handlers.py` & `django_restit-4.1.1/inbox/handlers.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/inbox/migrations/0001_initial.py` & `django_restit-4.1.1/inbox/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/inbox/migrations/0004_mailtemplate.py` & `django_restit-4.1.1/inbox/migrations/0004_mailtemplate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/inbox/models/bounce.py` & `django_restit-4.1.1/inbox/models/bounce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/inbox/models/complaint.py` & `django_restit-4.1.1/inbox/models/complaint.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/inbox/models/message.py` & `django_restit-4.1.1/inbox/models/message.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/inbox/models/template.py` & `django_restit-4.1.1/inbox/models/template.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/inbox/rpc.py` & `django_restit-4.1.1/inbox/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/inbox/utils/parsing.py` & `django_restit-4.1.1/inbox/utils/parsing.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/inbox/utils/render.py` & `django_restit-4.1.1/inbox/utils/render.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/inbox/utils/sending.py` & `django_restit-4.1.1/inbox/utils/sending.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/README.md` & `django_restit-4.1.1/incident/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/__init__.py` & `django_restit-4.1.1/incident/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/migrations/0001_initial.py` & `django_restit-4.1.1/incident/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/migrations/0002_event_component_event_component_id.py` & `django_restit-4.1.1/incident/migrations/0002_event_component_event_component_id.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py` & `django_restit-4.1.1/incident/migrations/0004_serverossecalert_ssh_sig_alter_rulecheck_parent.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/migrations/0005_incident_component_alter_incident_state.py` & `django_restit-4.1.1/incident/migrations/0005_incident_component_alter_incident_state.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py` & `django_restit-4.1.1/incident/migrations/0008_incident_action_sent_incident_hostname_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/models/event.py` & `django_restit-4.1.1/incident/models/event.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/models/incident.py` & `django_restit-4.1.1/incident/models/incident.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/models/ossec.py` & `django_restit-4.1.1/incident/models/ossec.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/models/rules.py` & `django_restit-4.1.1/incident/models/rules.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/parsers/ossec.py` & `django_restit-4.1.1/incident/parsers/ossec.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/periodic.py` & `django_restit-4.1.1/incident/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/rpc.py` & `django_restit-4.1.1/incident/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/templates/email/incident_change.html` & `django_restit-4.1.1/incident/templates/email/incident_change.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/templates/email/incident_new.html` & `django_restit-4.1.1/incident/templates/email/incident_new.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/templates/email/incident_plain.html` & `django_restit-4.1.1/incident/templates/email/incident_plain.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/incident/tq.py` & `django_restit-4.1.1/incident/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/geolocate.py` & `django_restit-4.1.1/location/geolocate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/migrations/0001_initial.py` & `django_restit-4.1.1/location/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/migrations/0002_geoip_subnet_alter_geoip_ip.py` & `django_restit-4.1.1/location/migrations/0002_geoip_subnet_alter_geoip_ip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/models/address.py` & `django_restit-4.1.1/location/models/address.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/models/ip.py` & `django_restit-4.1.1/location/models/ip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/models/legacy.py` & `django_restit-4.1.1/location/models/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/models/location.py` & `django_restit-4.1.1/location/models/location.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/models/track.py` & `django_restit-4.1.1/location/models/track.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/providers/iplookup/__init__.py` & `django_restit-4.1.1/location/providers/iplookup/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/providers/iplookup/abstractapi.py` & `django_restit-4.1.1/location/providers/iplookup/abstractapi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/providers/iplookup/extremeip.py` & `django_restit-4.1.1/location/providers/iplookup/extremeip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/providers/iplookup/geoplugin.py` & `django_restit-4.1.1/location/providers/iplookup/geoplugin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/providers/iplookup/ipapi.py` & `django_restit-4.1.1/location/providers/iplookup/ipapi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/providers/iplookup/ipinfo.py` & `django_restit-4.1.1/location/providers/iplookup/ipinfo.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/providers/iplookup/restit.py` & `django_restit-4.1.1/location/providers/iplookup/restit.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/providers/location/google.py` & `django_restit-4.1.1/location/providers/location/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/providers/timezones/google.py` & `django_restit-4.1.1/location/providers/timezones/google.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/providers/zillow.py` & `django_restit-4.1.1/location/providers/zillow.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/rpc/ip.py` & `django_restit-4.1.1/location/rpc/ip.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/rpc/location.py` & `django_restit-4.1.1/location/rpc/location.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/location/rpc/track.py` & `django_restit-4.1.1/location/rpc/track.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/admin.py` & `django_restit-4.1.1/medialib/admin.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/cvutil/contours.py` & `django_restit-4.1.1/medialib/cvutil/contours.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/cvutil/images.py` & `django_restit-4.1.1/medialib/cvutil/images.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/cvutil/misc.py` & `django_restit-4.1.1/medialib/cvutil/misc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/cvutil/text.py` & `django_restit-4.1.1/medialib/cvutil/text.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/fixtures/initial_data.json` & `django_restit-4.1.1/medialib/fixtures/initial_data.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/fixtures/medialib.json` & `django_restit-4.1.1/medialib/fixtures/medialib.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/fixtures/medialib_test_fixture.json` & `django_restit-4.1.1/medialib/fixtures/medialib_test_fixture.json`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/forms.py` & `django_restit-4.1.1/medialib/forms.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/migrations/0001_initial.py` & `django_restit-4.1.1/medialib/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/models.py` & `django_restit-4.1.1/medialib/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/ocr.py` & `django_restit-4.1.1/medialib/ocr.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/pdf.py` & `django_restit-4.1.1/medialib/pdf.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/qrcode.py` & `django_restit-4.1.1/medialib/qrcode.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/__init__.py` & `django_restit-4.1.1/medialib/render/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/engines/anigif.py` & `django_restit-4.1.1/medialib/render/engines/anigif.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/engines/ffmpeg.py` & `django_restit-4.1.1/medialib/render/engines/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/engines/gifsicle.py` & `django_restit-4.1.1/medialib/render/engines/gifsicle.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/engines/hls.py` & `django_restit-4.1.1/medialib/render/engines/hls.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/engines/mp4box.py` & `django_restit-4.1.1/medialib/render/engines/mp4box.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/engines/rtmp/rtmp.i` & `django_restit-4.1.1/medialib/render/engines/rtmp/rtmp.i`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/engines/rtmpdump.py` & `django_restit-4.1.1/medialib/render/engines/rtmpdump.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/engines/rtmpsink.py` & `django_restit-4.1.1/medialib/render/engines/rtmpsink.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/engines/video_getinfo.py` & `django_restit-4.1.1/medialib/render/engines/video_getinfo.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/engines/websnap.py` & `django_restit-4.1.1/medialib/render/engines/websnap.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/exceptions.py` & `django_restit-4.1.1/medialib/render/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/presets/akamai.py` & `django_restit-4.1.1/medialib/render/presets/akamai.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/presets/animated_thumbnail.py` & `django_restit-4.1.1/medialib/render/presets/animated_thumbnail.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/presets/ffmpeg.py` & `django_restit-4.1.1/medialib/render/presets/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/presets/flv.py` & `django_restit-4.1.1/medialib/render/presets/flv.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/presets/hls.py` & `django_restit-4.1.1/medialib/render/presets/hls.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/presets/image_transcode.py` & `django_restit-4.1.1/medialib/render/presets/image_transcode.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/presets/image_validate.py` & `django_restit-4.1.1/medialib/render/presets/image_validate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/presets/mp4.py` & `django_restit-4.1.1/medialib/render/presets/mp4.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/presets/video_still.py` & `django_restit-4.1.1/medialib/render/presets/video_still.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/presets/video_validate.py` & `django_restit-4.1.1/medialib/render/presets/video_validate.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/presets/websnap.py` & `django_restit-4.1.1/medialib/render/presets/websnap.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/presets/youtube.py` & `django_restit-4.1.1/medialib/render/presets/youtube.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/render/render_utils.py` & `django_restit-4.1.1/medialib/render/render_utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/rpc/legacy.py` & `django_restit-4.1.1/medialib/rpc/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/rpc/media.py` & `django_restit-4.1.1/medialib/rpc/media.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/rpc/tools.py` & `django_restit-4.1.1/medialib/rpc/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/scripts/init_config` & `django_restit-4.1.1/medialib/scripts/init_config`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/css/base_medialibui.css` & `django_restit-4.1.1/medialib/static/css/base_medialibui.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/css/base_widgets.css` & `django_restit-4.1.1/medialib/static/css/base_widgets.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/css/jquery.jcrop.css` & `django_restit-4.1.1/medialib/static/css/jquery.jcrop.css`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/img/bg-body.gif` & `django_restit-4.1.1/medialib/static/img/bg-body.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/img/loading.gif` & `django_restit-4.1.1/medialib/static/img/loading.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/img/noimage.gif` & `django_restit-4.1.1/medialib/static/img/noimage.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/img/render_err.gif` & `django_restit-4.1.1/medialib/static/img/render_err.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/img/rendering.gif` & `django_restit-4.1.1/medialib/static/img/rendering.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/img/unknown.gif` & `django_restit-4.1.1/medialib/static/img/unknown.gif`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/lib/caman.full.js` & `django_restit-4.1.1/medialib/static/lib/caman.full.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/lib/hammer.min.js` & `django_restit-4.1.1/medialib/static/lib/hammer.min.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/lib/jquery.Jcrop.js` & `django_restit-4.1.1/medialib/static/lib/jquery.Jcrop.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/lib/jquery.hammer.js` & `django_restit-4.1.1/medialib/static/lib/jquery.hammer.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/lib/load-image.min.js` & `django_restit-4.1.1/medialib/static/lib/load-image.min.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/lib/swiper.js` & `django_restit-4.1.1/medialib/static/lib/swiper.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js` & `django_restit-4.1.1/medialib/static/lib/tinymce/plugins/medialib/editor_plugin.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js` & `django_restit-4.1.1/medialib/static/lib/tinymce/plugins/medialib/editor_plugin_src.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js` & `django_restit-4.1.1/medialib/static/lib/tinymce/plugins/medialib/js/dialog.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/static/lib/tinymce/plugins/medialib/medialib.html` & `django_restit-4.1.1/medialib/static/lib/tinymce/plugins/medialib/medialib.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/__init__.py` & `django_restit-4.1.1/medialib/stores/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/apiclient/__init__.py` & `django_restit-4.1.1/medialib/stores/apiclient/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/apiclient/channel.py` & `django_restit-4.1.1/medialib/stores/apiclient/channel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/apiclient/discovery.py` & `django_restit-4.1.1/medialib/stores/apiclient/discovery.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/apiclient/errors.py` & `django_restit-4.1.1/medialib/stores/apiclient/errors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/apiclient/http.py` & `django_restit-4.1.1/medialib/stores/apiclient/http.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/apiclient/mimeparse.py` & `django_restit-4.1.1/medialib/stores/apiclient/mimeparse.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/apiclient/model.py` & `django_restit-4.1.1/medialib/stores/apiclient/model.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/apiclient/sample_tools.py` & `django_restit-4.1.1/medialib/stores/apiclient/sample_tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/apiclient/schema.py` & `django_restit-4.1.1/medialib/stores/apiclient/schema.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/filestore.py` & `django_restit-4.1.1/medialib/stores/filestore.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/httplib2/__init__.py` & `django_restit-4.1.1/medialib/stores/httplib2/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/httplib2/cacerts.txt` & `django_restit-4.1.1/medialib/stores/httplib2/cacerts.txt`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/httplib2/iri2uri.py` & `django_restit-4.1.1/medialib/stores/httplib2/iri2uri.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/httplib2/socks.py` & `django_restit-4.1.1/medialib/stores/httplib2/socks.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/httpstore.py` & `django_restit-4.1.1/medialib/stores/httpstore.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/oauth2client/anyjson.py` & `django_restit-4.1.1/medialib/stores/oauth2client/anyjson.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/oauth2client/appengine.py` & `django_restit-4.1.1/medialib/stores/oauth2client/appengine.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/oauth2client/client.py` & `django_restit-4.1.1/medialib/stores/oauth2client/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/oauth2client/clientsecrets.py` & `django_restit-4.1.1/medialib/stores/oauth2client/clientsecrets.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/oauth2client/crypt.py` & `django_restit-4.1.1/medialib/stores/oauth2client/crypt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/oauth2client/django_orm.py` & `django_restit-4.1.1/medialib/stores/oauth2client/django_orm.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/oauth2client/file.py` & `django_restit-4.1.1/medialib/stores/oauth2client/file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/oauth2client/gce.py` & `django_restit-4.1.1/medialib/stores/oauth2client/gce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/oauth2client/keyring_storage.py` & `django_restit-4.1.1/medialib/stores/oauth2client/keyring_storage.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/oauth2client/locked_file.py` & `django_restit-4.1.1/medialib/stores/oauth2client/locked_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/oauth2client/multistore_file.py` & `django_restit-4.1.1/medialib/stores/oauth2client/multistore_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/oauth2client/old_run.py` & `django_restit-4.1.1/medialib/stores/oauth2client/old_run.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/oauth2client/tools.py` & `django_restit-4.1.1/medialib/stores/oauth2client/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/oauth2client/util.py` & `django_restit-4.1.1/medialib/stores/oauth2client/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/oauth2client/xsrfutil.py` & `django_restit-4.1.1/medialib/stores/oauth2client/xsrfutil.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/s3store.py` & `django_restit-4.1.1/medialib/stores/s3store.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/stores/uritemplate/__init__.py` & `django_restit-4.1.1/medialib/stores/uritemplate/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/templates/medialib/base.html` & `django_restit-4.1.1/medialib/templates/medialib/base.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/templates/medialib/instances.html` & `django_restit-4.1.1/medialib/templates/medialib/instances.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/templates/medialib/items.html` & `django_restit-4.1.1/medialib/templates/medialib/items.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/templates/medialib/library.html` & `django_restit-4.1.1/medialib/templates/medialib/library.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/templates/medialib/test.html` & `django_restit-4.1.1/medialib/templates/medialib/test.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/templates/medialib/testpicker.html` & `django_restit-4.1.1/medialib/templates/medialib/testpicker.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/tests.py` & `django_restit-4.1.1/medialib/tests.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/tq.py` & `django_restit-4.1.1/medialib/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/utils.py` & `django_restit-4.1.1/medialib/utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/views.py` & `django_restit-4.1.1/medialib/views.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/__init__.py` & `django_restit-4.1.1/medialib/youtube/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/apiclient/__init__.py` & `django_restit-4.1.1/medialib/youtube/apiclient/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/apiclient/channel.py` & `django_restit-4.1.1/medialib/youtube/apiclient/channel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/apiclient/discovery.py` & `django_restit-4.1.1/medialib/youtube/apiclient/discovery.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/apiclient/errors.py` & `django_restit-4.1.1/medialib/youtube/apiclient/errors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/apiclient/http.py` & `django_restit-4.1.1/medialib/youtube/apiclient/http.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/apiclient/mimeparse.py` & `django_restit-4.1.1/medialib/youtube/apiclient/mimeparse.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/apiclient/model.py` & `django_restit-4.1.1/medialib/youtube/apiclient/model.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/apiclient/sample_tools.py` & `django_restit-4.1.1/medialib/youtube/apiclient/sample_tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/apiclient/schema.py` & `django_restit-4.1.1/medialib/youtube/apiclient/schema.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/httplib2/__init__.py` & `django_restit-4.1.1/medialib/youtube/httplib2/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/httplib2/cacerts.txt` & `django_restit-4.1.1/medialib/youtube/httplib2/cacerts.txt`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/httplib2/iri2uri.py` & `django_restit-4.1.1/medialib/youtube/httplib2/iri2uri.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/httplib2/socks.py` & `django_restit-4.1.1/medialib/youtube/httplib2/socks.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/oauth2client/anyjson.py` & `django_restit-4.1.1/medialib/youtube/oauth2client/anyjson.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/oauth2client/appengine.py` & `django_restit-4.1.1/medialib/youtube/oauth2client/appengine.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/oauth2client/client.py` & `django_restit-4.1.1/medialib/youtube/oauth2client/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/oauth2client/clientsecrets.py` & `django_restit-4.1.1/medialib/youtube/oauth2client/clientsecrets.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/oauth2client/crypt.py` & `django_restit-4.1.1/medialib/youtube/oauth2client/crypt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/oauth2client/django_orm.py` & `django_restit-4.1.1/medialib/youtube/oauth2client/django_orm.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/oauth2client/file.py` & `django_restit-4.1.1/medialib/youtube/oauth2client/file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/oauth2client/gce.py` & `django_restit-4.1.1/medialib/youtube/oauth2client/gce.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/oauth2client/keyring_storage.py` & `django_restit-4.1.1/medialib/youtube/oauth2client/keyring_storage.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/oauth2client/locked_file.py` & `django_restit-4.1.1/medialib/youtube/oauth2client/locked_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/oauth2client/multistore_file.py` & `django_restit-4.1.1/medialib/youtube/oauth2client/multistore_file.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/oauth2client/old_run.py` & `django_restit-4.1.1/medialib/youtube/oauth2client/old_run.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/oauth2client/tools.py` & `django_restit-4.1.1/medialib/youtube/oauth2client/tools.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/oauth2client/util.py` & `django_restit-4.1.1/medialib/youtube/oauth2client/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/oauth2client/xsrfutil.py` & `django_restit-4.1.1/medialib/youtube/oauth2client/xsrfutil.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/upload.py` & `django_restit-4.1.1/medialib/youtube/upload.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/medialib/youtube/uritemplate/__init__.py` & `django_restit-4.1.1/medialib/youtube/uritemplate/__init__.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/metrics/README.md` & `django_restit-4.1.1/metrics/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/metrics/client.py` & `django_restit-4.1.1/metrics/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/metrics/eod.py` & `django_restit-4.1.1/metrics/eod.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/metrics/examples/eod_example.py` & `django_restit-4.1.1/metrics/examples/eod_example.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/metrics/management/commands/fix_redis_metrics_keys.py` & `django_restit-4.1.1/metrics/management/commands/fix_redis_metrics_keys.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/metrics/management/commands/generate_test_metrics.py` & `django_restit-4.1.1/metrics/management/commands/generate_test_metrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/metrics/management/commands/redis_metrics_send_mail.py` & `django_restit-4.1.1/metrics/management/commands/redis_metrics_send_mail.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/metrics/management/commands/reset_weekly_metrics.py` & `django_restit-4.1.1/metrics/management/commands/reset_weekly_metrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/metrics/management/commands/system_metric.py` & `django_restit-4.1.1/metrics/management/commands/system_metric.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/metrics/migrations/0001_initial.py` & `django_restit-4.1.1/metrics/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py` & `django_restit-4.1.1/metrics/migrations/0002_metrics_k11_metrics_k12_metrics_k13_metrics_k14_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/metrics/migrations/0004_eodmetrics.py` & `django_restit-4.1.1/metrics/migrations/0004_eodmetrics.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py` & `django_restit-4.1.1/metrics/migrations/0005_alter_metrics_v1_alter_metrics_v10_alter_metrics_v11_and_more.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/metrics/models.py` & `django_restit-4.1.1/metrics/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/metrics/providers/aws.py` & `django_restit-4.1.1/metrics/providers/aws.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/metrics/rpc.py` & `django_restit-4.1.1/metrics/rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from datetime import datetime
 from rest import decorators as rd
 from rest import views as rv
 from rest import settings
-from rest.models import requestHasPerms
+from rest.helpers import requestHasPerms
 from location.models import GeoIP
 from . import client as metrics
 from . import models as mm
 from . import models as em
 from .providers import aws
 from objict import objict
 import time
```

### Comparing `django_restit-4.0.9/metrics/utils.py` & `django_restit-4.1.1/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/pushit/migrations/0001_initial.py` & `django_restit-4.1.1/pushit/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/pushit/models.py` & `django_restit-4.1.1/pushit/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from account.models import User, Member, Group, MemberFeed
 from medialib.models import MediaItem, MediaLibrary
 from location.models import GeoIP, Address
 
 from rest import helpers as rest_helpers
 from rest.middleware import get_request
 from rest import RemoteEvents
-from rest.models import RestModel, MetaDataModel, MetaDataBase, UberDict
+from rest.models import RestModel, MetaDataModel, MetaDataBase
 
 class Product(models.Model, RestModel, MetaDataModel):
     class RestMeta:
         GRAPHS = {
             "base": {
                 "graphs": {
                     "current":"default",
```

### Comparing `django_restit-4.0.9/pushit/rpc/githooks.py` & `django_restit-4.1.1/pushit/rpc/githooks.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/pushit/rpc/legacy.py` & `django_restit-4.1.1/pushit/rpc/legacy.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/pushit/utils.py` & `django_restit-4.1.1/pushit/utils.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/pyproject.toml` & `django_restit-4.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-restit"
-version = "4.0.9"
+version = "4.1.1"
 description = "A Rest Framework for DJANGO"
 authors = ["Ian Starnes <ians@311labs.com>"]
 license = "MIT"
 readme = "README.md"
 
 packages = [
     {include = "account"},
@@ -46,26 +46,14 @@
 boto3 = "^1.26.160"
 pyotp = "^2.8.0"
 pyqrcode = "^1.2.1"
 redis = "^3.0.1"
 django-redis-cache = "^3.0.1"
 django-redis-sessions = "^0.6.2"
 
-
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
 
-[tool.bumpver]
-current_version = "4.0.3"
-version_pattern = "MAJOR.MINOR.PATCH"
-commit_message = "bump version {old_version} -> {new_version}"
-commit = false
-tag = true
-push = true
-
-[tool.poetry_bumpversion.file."rest/__init__.py"]
-
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `django_restit-4.0.9/rest/README.md` & `django_restit-4.1.1/rest/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/arc4.py` & `django_restit-4.1.1/rest/arc4.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/crypto/aes.py` & `django_restit-4.1.1/rest/crypto/aes.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/crypto/privpub.py` & `django_restit-4.1.1/rest/crypto/privpub.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/crypto/util.py` & `django_restit-4.1.1/rest/crypto/util.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,14 +9,34 @@
 
 
 def generateKey(bit_size=128, allow_punctuation=False):
     byte_size = int(bit_size / 8)
     return randomString(byte_size, allow_punctuation)
 
 
+def generateUUID(*args, **kwargs):
+    upper = kwargs.get("upper", True)
+    max_length = kwargs.get("max_length", None)
+    uuid = ""
+    for key in args:
+        if isinstance(key, float):
+            key = str(float)
+        if isinstance(key, int):
+            uuid += Hashids().encrypt(key)
+        if isinstance(key, str):
+            uuid += toString(md5(toBytes(key)).hexdigest())
+    if len(uuid) > 125:
+        uuid = uuid[:125]
+    if max_length != None:
+        uuid = uuid[:max_length]
+    if upper:
+        return uuid.upper()
+    return uuid
+
+
 def get_random_bits(bit_size=128):
     return crypt_random.getrandbits(bit_size)
 
 
 def randomString(str_size=128, allow_punctuation=False, char_list=None):
     if char_list is None:
         char_list = string.ascii_letters + string.digits
```

### Comparing `django_restit-4.0.9/rest/datem.py` & `django_restit-4.1.1/rest/datem.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/decorators.py` & `django_restit-4.1.1/rest/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from django.urls import re_path, path
 from django.shortcuts import Http404
 from django.http import HttpResponseRedirect
 from django.utils.cache import patch_cache_control, add_never_cache_headers, patch_vary_headers
 
 from rest import settings
 from rest.views import restStatus, restPermissionDenied
-from rest.models import RestError, requestHasPerms, PermissionDeniedException
-from rest import helpers
+from rest.errors import RestError, PermissionDeniedException
+from rest import helpers as rh
 import metrics
 import incident
 
 from datetime import datetime
 from auditlog.models import PersistentLog
 
 import importlib
@@ -57,24 +57,24 @@
         if REST_METRICS:
             metrics.metric("rest_calls")
             if REST_METRICS_BY_ENDPOINT:
                 slug_path = request.path.replace("/", "__")
                 metrics.metric(f"rest_call_{slug_path}", category="rest_calls")
         return func(request, *args, **kwargs)
     except PermissionDeniedException as err:
-        helpers.log_error("permission denied: '{}' for {} {}:{}".format(err, request.user, request.method, request.path))
+        rh.log_error("permission denied: '{}' for {} {}:{}".format(err, request.user, request.method, request.path))
         return restStatus(request, False, error=err.reason, error_code=err.code)
     except RestError as err:
-        helpers.log_exception(err.reason)
+        rh.log_exception(err.reason)
         if settings.get("REST_ERROR_METRICS", True):
             metrics.metric("rest_errors")
         return restStatus(request, False, error=err.reason, error_code=err.code)
     except Exception as err:
         # TODO email errors to admins
-        helpers.log_exception(request.path)
+        rh.log_exception(request.path)
         if settings.get("REST_ERROR_METRICS", True):
             metrics.metric("rest_errors")
         stack = str(traceback.format_exc())
         host = request.get_host()
         server = settings.get("HOSTNAME", "unknown")
         try:
             body = request.body.decode('utf-8')
@@ -190,15 +190,15 @@
                     if 'kwargs' not in kwargs:
                         kwargs['kwargs'] = {}
                     kwargs['kwargs']['__MODULE'] = rpc_root_module
                     kwargs['kwargs']['__PATTERN'] = pattern
                 else:
                     func = f
                 if not isinstance(pattern, str):
-                    helpers.log_print("NOT A STRING", pattern)
+                    rh.log_print("NOT A STRING", pattern)
                 if pattern.startswith("^") or pattern.endswith("$"):
                     rpc_root_module.urlpatterns += [re_path(pattern, func, *args, **kwargs)]
                 else:
                     rpc_root_module.urlpatterns += [path(pattern, func, *args, **kwargs)]
                     if not pattern.endswith("/") and not pattern.endswith(">"):
                         rpc_root_module.urlpatterns += [path(pattern + "/", func, *args, **kwargs)]
             f.__url__ = (lmethod, pattern)
@@ -365,29 +365,29 @@
 
 class perm_required(object):
     def __init__(self, perms):
         self.perms = perms
 
     def __call__(self, func):
         def inner_func(request=None, *args, **kwargs):
-            status, error, code = requestHasPerms(request, self.perms)
+            status, error, code = rh.requestHasPerms(request, self.perms)
             if not status:
                 return restStatus(request, False, error=error, error_code=code)
             return func(request, *args, **kwargs)
         return inner_func
 
 
 class post_perm_required(object):
     def __init__(self, perms):
         self.perms = perms
 
     def __call__(self, func):
         def inner_func(request=None, *args, **kwargs):
             if request.method == "post":
-                status, error, code = requestHasPerms(request, self.perms)
+                status, error, code = rh.requestHasPerms(request, self.perms)
                 if not status:
                     return restStatus(request, False, error=error, error_code=code)
             elif not request.user.is_authenticated:
                 return restStatus(request, False, error="permission denied", error_code=401)
             return func(request, *args, **kwargs)
         return inner_func
 
@@ -435,15 +435,15 @@
         @wraps(func)
         def inner_func(force=False, verbose=False, now=None):
             if now is None:
                 now = datetime.now()
             if force:
                 return func(force, verbose, now)
             if tz:
-                now = helpers.convertToLocalTime(tz, now)
+                now = rh.convertToLocalTime(tz, now)
             # lets create our when
             if minute is not None and not periodicCheckListHas(minute, now.minute):
                 return -22
             if hour is not None and not periodicCheckListHas(hour, now.hour):
                 return -22
             if day is not None and not periodicCheckListHas(day, now.day):
                 return -22
```

### Comparing `django_restit-4.0.9/rest/encryption.py` & `django_restit-4.1.1/rest/encryption.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/extra/json_metadata.py` & `django_restit-4.1.1/rest/extra/json_metadata.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/fields.py` & `django_restit-4.1.1/rest/fields.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/forms.py` & `django_restit-4.1.1/rest/forms.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/helpers.py` & `django_restit-4.1.1/rest/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,38 @@
 def getActiveRequest():
     if not HELPER_CACHE.get_request:
         mw = importlib.import_module("rest.middleware")
         HELPER_CACHE.get_request = mw.get_request
     return HELPER_CACHE.get_request()
 
 
+def requestHasPerms(request, perms, group=None):
+    # third party auth models
+    if request.auth_model is not None:
+        if request.auth_model.hasPerm(perms):
+            return True, None, None
+
+    if not request.user.is_authenticated:
+        return False, "auth required", 401
+
+    if request.member.hasPerm(perms):
+        return True, None, None
+    if group is None and hasattr(request, "group"):
+        group = request.group
+    ms_perms = None
+    if group:
+        ms = request.member.getMembershipFor(group)
+        if ms and ms.hasPerm(perms):
+            return True, None, None
+        if ms:
+            ms_perms = ms.getPermissions()
+
+    # rest_helpers.log_error(F"PERMISSION DENIED for {request.member.username}, {perms}", str(group), ms_perms)
+    return False, "permission denied", 402
+
 def importModule(name):
     return importlib.import_module(name)
 
 
 def log_print(*args):
     getLoggerByRequest(getActiveRequest()).info(*args)
```

### Comparing `django_restit-4.0.9/rest/jwtoken.py` & `django_restit-4.1.1/rest/jwtoken.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/log.py` & `django_restit-4.1.1/rest/log.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/mail.py` & `django_restit-4.1.1/rest/mail.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/mailman.py` & `django_restit-4.1.1/rest/mailman.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/middleware/cors.py` & `django_restit-4.1.1/rest/middleware/cors.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/middleware/db_router.py` & `django_restit-4.1.1/rest/middleware/db_router.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/middleware/jwt.py` & `django_restit-4.1.1/rest/middleware/jwt.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/middleware/request.py` & `django_restit-4.1.1/rest/middleware/request.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/middleware/session.py` & `django_restit-4.1.1/rest/middleware/session.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/middleware/session_store.py` & `django_restit-4.1.1/rest/middleware/session_store.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/models.py` & `django_restit-4.1.1/rest/models/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,416 +1,47 @@
-import os
-from django.conf import settings
-from django.core.exceptions import FieldDoesNotExist
-from hashids import Hashids
-import hashlib
-import string
-from io import StringIO
-
 from datetime import datetime, date, timedelta
 from decimal import Decimal
-TWOPLACES = Decimal(10) ** -2
+from objict import objict
+import importlib
 
-from django.db import models
-from django.apps import apps
+from django.db import models as dm
 from django.db.transaction import atomic
-get_model = apps.get_model
-
-from django.http import Http404
-from django.core.exceptions import ValidationError
-
-import threading
+from django.apps import apps
 
-from rest import helpers as rest_helpers
-from rest.uberdict import UberDict
-from rest import search
+from rest import helpers as rh
+from rest import errors as re
 from rest.encryption import ENCRYPTER, DECRYPTER
+from rest import crypto
+from rest import settings
+from rest import search
+from .metadata import MetaDataBase, MetaDataModel
 
-import importlib
+DB_ROUTING_MAPS = settings.get("DB_ROUTING_MAPS", {})
+TWO_DECIMAL_PLACES = Decimal(10) ** -2
 
-GRAPH_HELPERS = UberDict()
+GRAPH_HELPERS = objict()
 GRAPH_HELPERS.restGet = None
 GRAPH_HELPERS.get_request = None
 GRAPH_HELPERS.views = None
 
-NOTFOUND = "311!@#$%^&*"
-
-DB_ROUTING_MAPS = getattr(settings, "DB_ROUTING_MAPS", {})
-
-
-class RestError(Exception):
-    def __init__(self, reason, code=None):
-        self.reason = reason
-        self.code = code
-
-    def __repr__(self):
-        return self.reason
-
-
-class PermissionDeniedException(RestError):
-    def __init__(self, reason="permission denied", code=401):
-        self.reason = reason
-        self.code = code
-
-
-class RestValidationError(RestError):
-    def __init__(self, reason="rest data is not valid", code=123):
-        self.reason = reason
-        self.code = code
-
-
-def requestHasPerms(request, perms, group=None):
-    # third party auth models
-    if request.auth_model is not None:
-        if request.auth_model.hasPerm(perms):
-            return True, None, None
-
-    if not request.user.is_authenticated:
-        return False, "auth required", 401
-
-    if request.member.hasPerm(perms):
-        return True, None, None
-    if group is None and hasattr(request, "group"):
-        group = request.group
-    ms_perms = None
-    if group:
-        ms = request.member.getMembershipFor(group)
-        if ms and ms.hasPerm(perms):
-            return True, None, None
-        if ms:
-            ms_perms = ms.getPermissions()
-
-    # rest_helpers.log_error(F"PERMISSION DENIED for {request.member.username}, {perms}", str(group), ms_perms)
-    return False, "permission denied", 402
-
-
-class MetaDataBase(models.Model):
-    class Meta:
-        abstract = True
-
-    category = models.CharField(db_index=True, max_length=32, default=None, null=True, blank=True)
-
-    key = models.CharField(db_index=True, max_length=80)
-
-    value_format = models.CharField(max_length=16)
-    value = models.TextField()
-
-    int_value = models.IntegerField(default=None, null=True, blank=True)
-    float_value = models.IntegerField(default=None, null=True, blank=True)
-
-    def setValue(self, value):
-        self.value = "{}".format(value)
-        if type(value) is int or self.value in ["0", "1"]:
-            if type(value) is int and value > 2147483647:
-                self.value_format = "S"
-                return
-            self.value_format = "I"
-            self.int_value = value
-        elif type(value) is float:
-            self.value_format = "F"
-            self.float_value = value
-        elif isinstance(value, list):
-            self.value_format = "L"
-            # self.value = ",".join(value)
-        elif isinstance(value, dict):
-            self.value_format = "O"
-        elif type(value) in [str, str] and len(value) < 9 and value.isdigit():
-            self.value_format = "I"
-            self.int_value = value
-        elif value in ["True", "true", "False", "false"]:
-            self.value_format = "I"
-            if value in ["True", "true"]:
-                self.int_value = 1
-            else:
-                self.int_value = 0
-        elif isinstance(value, bool):
-            self.value_format = "I"
-            if value:
-                self.int_value = 1
-            else:
-                self.int_value = 0
-        else:
-            self.value_format = "S"
-
-    def getStrictType(self, field_type):
-        if type(self.value) is field_type:
-            return self.value
-        if field_type in [int, str, float, str]:
-            return field_type(self.value)
-        elif field_type is bool:
-            if self.value_format == 'I':
-                return self.int_value != 0
-            return self.value in [True, 1, '1', 'y', 'Y', 'Yes', 'true', 'True']
-        elif field_type in [date, datetime]:
-            return rest_helpers.parseDate(self.value)
-        return self.value
-
-    def getValue(self, field_type=None):
-        if field_type:
-            return self.getStrictType(field_type)
-        elif self.value_format == 'I':
-            return self.int_value
-        elif self.value_format == 'F':
-            return self.float_value
-        elif self.value_format in ["L", "O"] and self.value:
-            try:
-                return eval(self.value)
-            except Exception:
-                pass
-        return self.value
-
-    def __unicode__(self):
-        if self.category:
-            return "{}.{}={}".format(self.category, self.key, self.value)
-        return "{}={}".format(self.key, self.value)
-
-    def __str__(self):
-        if self.category:
-            return "{}.{}={}".format(self.category, self.key, self.value)
-        return "{}={}".format(self.key, self.value)
-
-
-class MetaDataModel(object):
-    def set_metadata(self, request, values=None):
-        # this may get called before the model is saved
-        if not self.id:
-            self.save()
-
-        if values is None:
-            values = request
-            request = None
-
-        if not isinstance(values, dict):
-            raise Exception("invalid metadata: {}".format(values))
-
-        for key, value in list(values.items()):
-            cat = None
-            if "." in key:
-                cat, key = key.split('.')
-            self.setProperty(key, value, cat, request=request)
-
-    def metadata(self):
-        return self.getProperties()
-
-    def removeProperties(self, category=None):
-        # this will remove all properties
-        # if category is not it will remove all properties
-        self.properties.filter(category=category).delete()
-
-    def getProperties(self, category=None):
-        ret = {}
-        for p in self.properties.all():
-            if p.category:
-                props = self.getFieldProps(p.category)
-                if props.hidden:
-                    continue
-                if p.category not in ret or not isinstance(ret.get(p.category, None), dict):
-                    ret[p.category] = {}
-                props = self.getFieldProps("{}.{}".format(p.category, p.key))
-                if props.hidden:
-                    continue
-                ret[p.category][p.key] = p.getValue()
-            else:
-                props = self.getFieldProps(p.key)
-                if props.hidden:
-                    continue
-                ret[p.key] = p.getValue()
-        if category is not None:
-            if category in ret:
-                return ret[category]
-            return {}
-        return ret
-
-    def __initFieldProps(self):
-        if not hasattr(self, "__field_props"):
-            if hasattr(self.RestMeta, "METADATA_FIELD_PROPERTIES"):
-                # this provides extra protection for metadata fields
-                self.__field_props = self.RestMeta.METADATA_FIELD_PROPERTIES
-            else:
-                self.__field_props = None
-
-    def getFieldProps(self, key):
-        self.__initFieldProps()
-        full_key = key
-        category = None
-        if "." in key:
-            category, key = key.split('.')
-        props = UberDict()
-        if self.__field_props:
-            if category and self.__field_props.get(category, None):
-                cat_props = self.__field_props.get(category, None)
-                if cat_props:
-                    props.notify = cat_props.get("notify", None)
-                    props.requires = cat_props.get("requires", None)
-                    props.on_change_name = cat_props.get("on_change", None)
-                    props.hidden = cat_props.get("hidden", False)
-                    if props.on_change_name:
-                        props.on_change = getattr(self, props.on_change_name, None)
-            field_props = self.__field_props.get(full_key, None)
-            if field_props:
-                props.notify = field_props.get("notify", props.notify)
-                props.requires = field_props.get("requires", None)
-                props.hidden = field_props.get("hidden", False)
-                on_change_name = field_props.get("on_change", None)
-                if on_change_name:
-                    on_change = getattr(self, on_change_name, None)
-                    if on_change:
-                        props.on_change = on_change
-        return props
-
-    def checkFieldPerms(self, full_key, props, request=None):
-        if not props.requires:
-            return True
-        if not request or not request.member:
-            return False
-        if request.member.hasPermission(props.requires) or request.user.is_superuser:
-            return True
-
-        # this a unauthorized attempt to change field, log and throw exception
-        if props.notify and request.member:
-            subject = "permission denied changing protected '{}' field".format(full_key)
-            msg = "permission denied changing protected field '{}'\nby user: {}\nfor: {}".format(
-                    full_key,
-                    request.user.username,
-                    self
-                )
-            request.member.notifyWithPermission(props.notify, subject, msg, email_only=True)
-        raise PermissionDeniedException(subject)
-
-    def setProperties(self, data, category=None, request=None, using=None):
-        for k, v in data.items():
-            self.setProperty(k, v, category, request=request, using=using)
-
-    def setProperty(self, key, value, category=None, request=None, using=None, ascii_only=False, encrypted=False):
-        # rest_helpers.log_print("{}:{} ({})".format(key, value, type(value)))
-        if ascii_only and isinstance(value, str):
-            value = "".join([x for x in value if x in string.printable])
-        if encrypted:
-            value = ENCRYPTER.encrypt(value)
-        on_change = None
-        if not using:
-            using = getattr(self.RestMeta, "DATABASE", using)
-        if not request:
-            request = RestModel.getActiveRequest()
-        self.__initFieldProps()
-
-        if isinstance(value, dict):
-            return self.setProperties(value, key)
-        username = "root"
-        if request and request.member:
-            username = request.member.username
-        prop = None
-
-        if "." in key:
-            category, key = key.split('.')
-        if category:
-            # delete any keys with this category name
-            full_key = "{}.{}".format(category, key)
-            # this deletes anything with the key that matches the category
-            # this works because the category is stored not in key but category field
-            # rest_helpers.log_print("deleting key={}".format(category))
-            self.properties.filter(key=category).delete()
-        else:
-            full_key = key
-
-        field_props = self.getFieldProps(full_key)
-        if not self.checkFieldPerms(full_key, field_props, request):
-            return False
-
-        check_value = "{}".format(value)
-        has_changed = False
-        prop = self.properties.filter(category=category, key=key).last()
-        old_value = None
-        if prop:
-            # existing property we need to make sure we delete
-            old_value = prop.getValue()
-            if value is None or value == "":
-                prop.delete()
-                has_changed = True
-            else:
-                has_changed = check_value != prop.value
-                if not has_changed:
-                    return
-                prop.setValue(value)
-                prop.save(using=using)
-            if field_props.on_change:
-                field_props.on_change(key, value, old_value, category)
-        elif value is None or value == "":
-            # do not create none or empty property
-            return False
-        else:
-            has_changed = True
-            PropClass = self.get_fk_model("properties")
-            prop = PropClass(parent=self, key=key, category=category)
-            prop.setValue(value)
-            # rest_helpers.log_print(u"saving {}.{}".format(category, key))
-            # rest_helpers.log_print(u"saving {} : {}".format(full_key, value))
-            prop.save(using=using)
-
-        if hasattr(self, "_recordRestChange"):
-            self._recordRestChange("metadata.{}".format(full_key), old_value)
-
-        if field_props.notify and request and request.member:
-            notify = field_props.get("notify")
-            if value:
-                value = str(value)
-                if len(value) > 5:
-                    value = "***"
-            msg = "protected field '{}' changed to '{}'\nby user: {}\nfor: {}".format(
-                full_key,
-                value,
-                username,
-                self
-            )
-            request.member.notifyWithPermission(notify, "protected '{}' field changed".format(full_key), msg, email_only=True)
-        return has_changed
-
-    def getProperty(self, key, default=None, category=None, field_type=None, decrypted=False):
-        try:
-            if "." in key:
-                category, key = key.split('.')
-            value = self.properties.get(category=category, key=key).getValue(field_type)
-            if decrypted and value is not None:
-                return DECRYPTER.decrypt(value)
-            return value
-        except Exception:
-            pass
-        return default
-
 
 class RestModel(object):
     class __RestMeta__:
         NO_SAVE_FIELDS = ["id", "pk", "created", "modified"]
         NO_SHOW_FIELDS = ["password"]
         WHITELISTED = ["merchant", "group", "user", "member"]
 
     class RestMeta:
         NO_SAVE_FIELDS = []
         SAVE_FIELDS = []
         GRAPHS = {}
 
     @staticmethod
     def generateUUID(*args, **kwargs):
-        upper = kwargs.get("upper", True)
-        max_length = kwargs.get("max_length", None)
-        uuid = ""
-        for key in args:
-            if isinstance(key, float):
-                key = str(float)
-            if isinstance(key, int):
-                uuid += Hashids().encrypt(key)
-            if isinstance(key, str):
-                uuid += rest_helpers.toString(hashlib.md5(rest_helpers.toBytes(key)).hexdigest())
-        if len(uuid) > 125:
-            uuid = uuid[:125]
-        if max_length != None:
-            uuid = uuid[:max_length]
-        if upper:
-            return uuid.upper()
-        return uuid
+        return crypto.generateUUID(*args, **kwargs)
 
     @classmethod
     def buildGraph(cls, name):
         # we need to build it
         if hasattr(cls.RestMeta, "GRAPHS"):
             graphs = cls.RestMeta.GRAPHS
             if name not in graphs and name != "basic":
@@ -453,16 +84,14 @@
 
                 if field.startswith("generic__"):
                     if field not in graph["recurse_into"]:
                         graph["recurse_into"].append((field, gname))
                         continue
 
                 if isinstance(gname, dict):
-                    size = gname.get("size")
-                    sort = gname.get("sort")
                     fm_name = gname.get("model")
                     gname = gname.get("graph")
                     if not gname:
                         gname = "default"
                     if fm_name:
                         a_name, m_name = fm_name.split(".")
                         ForeignModel = RestModel.getModel(a_name, m_name)
@@ -478,15 +107,15 @@
                                 if f not in graph[part]:
                                     graph[part].append(f)
                     continue
 
                 if not ForeignModel:
                     ForeignModel = cls.get_fk_model(field)
                 if not ForeignModel:
-                    rest_helpers.log_print("no foreignkey: {0}".format(field))
+                    rh.log_print("no foreignkey: {0}".format(field))
                     continue
 
                 if field not in graph["recurse_into"]:
                     graph["recurse_into"].append(field)
 
                 if not hasattr(ForeignModel, "getGraph"):
                     # print "NO getGraph"
@@ -587,29 +216,26 @@
             obj = getattr(obj, f, None)
             if obj is None:
                 return obj
         return obj
 
     @classmethod
     def getActiveLogger(cls):
-        return rest_helpers.getLogger(cls.getActiveRequest())
+        return rh.getLogger(cls.getActiveRequest())
 
     @classmethod
     def getActiveMember(cls):
         request = cls.getActiveRequest()
         if request:
             return request.member
         return None
 
     @classmethod
     def getActiveRequest(cls):
-        if not GRAPH_HELPERS.get_request:
-            mw = importlib.import_module("rest.middleware")
-            GRAPH_HELPERS.get_request = mw.get_request
-        return GRAPH_HELPERS.get_request()
+        return rh.getActiveRequest()
 
     @classmethod
     def getFromRequest(cls, request):
         key = cls.get_class_name().lower()
         key_p = "{0}_id".format(key)
         lookup_fields = [key, key_p]
         using = getattr(cls.RestMeta, "DATABASE", None)
@@ -657,24 +283,24 @@
     def getModel(app_name, model_name):
         return apps.get_model(app_name, model_name)
 
     def restGetGenericModel(self, field):
         # called by the rest module to magically parse
         # a component that is marked genericr elation in a graph
         if not hasattr(self, field):
-            rest_helpers.log_print("model has no field: {0}".format(field))
+            rh.log_print("model has no field: {0}".format(field))
             return None
 
         name = getattr(self, field)
         if not name or "." not in name:
             return None
         a_name, m_name = name.split(".")
         model = RestModel.getModel(a_name, m_name)
         if not model:
-            rest_helpers.log_print("GENERIC MODEL DOES NOT EXIST: {0}".format(name))
+            rh.log_print("GENERIC MODEL DOES NOT EXIST: {0}".format(name))
         return model
 
     def restGetGenericRelation(self, field):
         # called by the rest module to magically parse
         # a component that is marked genericrelation in a graph
         GenericModel = self.restGetGenericModel(field)
         if not GenericModel:
@@ -700,61 +326,61 @@
             return len(self._changed__) > 0
         return False
 
     def saveFields(self, allow_null=True, **kwargs):
         """
         Helper method to save a list of fields
         """
-        self._changed__ = UberDict()
+        self._changed__ = objict()
         for key, value in list(kwargs.items()):
             if value is None and not allow_null:
                 continue
             self.restSaveField(key, value)
         if len(self._changed__):
             self.save()
 
     def restSaveField(self, fieldname, value, has_fields=False, has_no_fields=False, using=None):
         if not hasattr(self, "_changed__"):
-            self._changed__ = UberDict()
+            self._changed__ = objict()
 
         if fieldname.startswith("_"):
             return
         if not hasattr(self, "_field_names__"):
             self._field_names__ = [f.name for f in self._meta.get_fields()]
         # print "saving field: {0} = {1}".format(fieldname, value)
         if fieldname in RestModel.__RestMeta__.NO_SAVE_FIELDS:
             return
         if has_no_fields and fieldname in self.RestMeta.NO_SAVE_FIELDS:
             return
         if has_fields and fieldname not in self.RestMeta.SAVE_FIELDS:
             return
         if fieldname.endswith("_id") and not self.get_field_type(fieldname):
-            # django will have ForeignKeys with _id, we don't want that, on_delete=models.CASCADE
+            # django will have ForeignKeys with _id, we don't want that, on_delete=dm.CASCADE
             fieldname = fieldname[:-3]
         setter = F"set_{fieldname}"
         if hasattr(self, setter):
             getattr(self, setter)(value)
             return
 
         if fieldname in self._field_names__:
             # TODO check if it is a function
-            if isinstance(value, models.Model):
+            if isinstance(value, dm.Model):
                 setattr(self, fieldname, value)
                 self._changed__[fieldname] = True
                 return
             ForeignModel = self.get_fk_model(fieldname)
             if ForeignModel and isinstance(value, dict):
                 obj = getattr(self, fieldname, None)
                 if obj is None:
                     obj = ForeignModel()
                 if using is None:
                     using = self.restGetModelDB()
                 obj.saveFromDict(None, value, using=using)
-                # rest_helpers.log_print("{} vs {}".format(self._state.db, obj._state.db))
-                # rest_helpers.log_print("saving FK to {} ({}.{}) - {}".format(fieldname, using, obj.pk, type(obj)), value)
+                # rh.log_print("{} vs {}".format(self._state.db, obj._state.db))
+                # rh.log_print("saving FK to {} ({}.{}) - {}".format(fieldname, using, obj.pk, type(obj)), value)
                 setattr(self, fieldname, obj)
                 self._changed__[fieldname] = True
                 return
             elif ForeignModel and value and (type(value) is int or value.isdigit()):
                 # print("\tforeign model({2}) field: {0} = {1}".format(fieldname, value, ForeignModel.__class__.__name__))
                 value = int(value)
                 using = None
@@ -776,24 +402,24 @@
                 # field_model, model, direct, mm = self._meta.get_field_by_name(fieldname)
                 field_model = self._meta.get_field(fieldname)
                 # hack to handle save datetime fields correctly from floats
                 try:
                     if field_model and value != None:
                         field_model_name = field_model.__class__.__name__
                         if field_model_name == "DateTimeField":
-                            value = rest_helpers.parseDateTime(value)
+                            value = rh.parseDateTime(value)
                             # value = datetime.fromtimestamp(float(value))
                         elif field_model_name == "DateField":
-                            value = rest_helpers.parseDate(value, as_date=True)
+                            value = rh.parseDate(value, as_date=True)
                         elif field_model_name == "IntegerField":
                             value = int(value)
                         elif field_model_name == "FloatField":
                             value = float(value)
                         elif field_model_name == "CurrencyField":
-                            value = Decimal(value).quantize(TWOPLACES)
+                            value = Decimal(value).quantize(TWO_DECIMAL_PLACES)
                         elif field_model_name == "BooleanField":
                             if value in [True, 1, 'True', 'true', '1', 't', 'y', 'yes']:
                                 value = True
                             else:
                                 value = False
                 except Exception:
                     return
@@ -806,58 +432,58 @@
     def saveFromRequest(self, request, **kwargs):
         if "files" not in kwargs:
             kwargs["files"] = request.FILES
         return self.saveFromDict(request, request.DATA, **kwargs)
 
     def _recordRestChange(self, fieldname, old_value):
         if not hasattr(self, "_changed__"):
-            self._changed__ = UberDict()
+            self._changed__ = objict()
         if "." in fieldname:
             fields = fieldname.split('.')
             root = self._changed__
             for f in fields[:-1]:
                 if f not in root:
-                    root[f] = UberDict()
+                    root[f] = objict()
                 root = root[f]
             root[fields[-1]] = old_value
         else:
             self._changed__[fieldname] = old_value
 
     def saveFromDict(self, request, data, files=None, **kwargs):
         can_save = getattr(self.RestMeta, "CAN_SAVE", True)
         if not can_save:
             return self.restStatus(request, False, error="saving not allowed via rest for this model.")
         save_media_files = getattr(self.RestMeta, "SAVE_MEDIA_FILES", False) or getattr(self.RestMeta, "SAVE_MEDIA_FILES_BY_NAME", False)
         # check check for save permissions
         if request is None:
             request = RestModel.getActiveRequest()
             if request is None:
-                request = UberDict(member=None, FILES=[], DATA=UberDict(), is_authenticated=False, is_local=True)
+                request = objict(member=None, FILES=[], DATA=objict(), is_authenticated=False, is_local=True)
         self.onRestCanSave(request)
         is_new = self.id is None
         has_fields = hasattr(self.RestMeta, "SAVE_FIELDS") and len(self.RestMeta.SAVE_FIELDS)
         has_no_fields = hasattr(self.RestMeta, "NO_SAVE_FIELDS") and len(self.RestMeta.NO_SAVE_FIELDS)
         self._field_names__ = [f.name for f in self._meta.get_fields()]
         # fix for multidatabase support and using readonly db for get
         self._state.db = kwargs.get("using", self.restGetModelDB("default"))
         auto_save_fields = getattr(self.RestMeta, "AUTO_SAVE", None)
         if auto_save_fields:
-            # rest_helpers.log_print(auto_save_fields)
+            # rh.log_print(auto_save_fields)
             for field in auto_save_fields:
-                # rest_helpers.log_print(field)
+                # rh.log_print(field)
                 if isinstance(field, tuple):
                     m_field, req_field = field
                 else:
                     m_field = field
                     req_field = field
                 req_value = getattr(request, req_field, None)
                 if request and req_value:
                     data[m_field] = req_value
-            # rest_helpers.log_print(data)
-        self._changed__ = UberDict()
+            # rh.log_print(data)
+        self._changed__ = objict()
         if hasattr(self.RestMeta, "POST_SAVE_FIELDS"):
             post_save_fields = self.RestMeta.POST_SAVE_FIELDS
         else:
             post_save_fields = []
         using = kwargs.get("using", self.restGetModelDB())
         deferred = {}
         group_fields = {}
@@ -916,32 +542,32 @@
         for name in files:
             key = f"upload__{name}"
             if hasattr(self, key):
                 getattr(self, key)(files[name], name)
             else:
                 ForeignModel = self.get_fk_model(name)
                 if ForeignModel and ForeignModel.__name__ == "MediaItem":
-                    # rest_helpers.log_print("saving media file: {}".format(name))
+                    # rh.log_print("saving media file: {}".format(name))
                     self.saveMediaFile(files[name], name)
                 else:
                     remaining_files[name] = files[name]
         return remaining_files
 
     def restSaveMediaFiles(self, files=None):
         MediaItemRef = RestModel.getModel("medialib", "MediaItemRef")
         component = self.get_class_name(True)
-        # rest_helpers.log_print("saving media files refs: {}".format(component))
+        # rh.log_print("saving media files refs: {}".format(component))
         for name in files:
             mi = self.saveMediaFile(files[name], name, is_local=False)
             mr = None
             if getattr(self.RestMeta, "SAVE_MEDIA_FILES_BY_NAME", False):
                 # use existing reference
                 mr = MediaItemRef.objects.filter(component=component, component_id=self.id, media__name=name).last()
                 if mr:
-                    rest_helpers.log_print(F"existing media files refs: {name}.{component}.{self.id}")
+                    rh.log_print(F"existing media files refs: {name}.{component}.{self.id}")
                     mr.media = mi
                     mr.save()
             if mr is None:
                 mr = MediaItemRef(media=mi, component=component, component_id=self.id)
                 mr.save()
 
     def getMediaFiles(self):
@@ -975,21 +601,21 @@
             # hack to handle save datetime fields correctly from floats
             try:
                 if field_model and value != None:
                     field_model_name = field_model.__class__.__name__
                     if field_model_name == "DateTimeField":
                         value = datetime.fromtimestamp(float(value))
                     elif field_model_name == "DateField":
-                        value = rest_helpers.parseDate(value)
+                        value = rh.parseDate(value)
                     elif field_model_name == "IntegerField":
                         value = int(value)
                     elif field_model_name == "FloatField":
                         value = float(value)
                     elif field_model_name == "CurrencyField":
-                        value = Decimal(value).quantize(TWOPLACES)
+                        value = Decimal(value).quantize(TWO_DECIMAL_PLACES)
                 if hasattr(self, key) and getattr(self, key) != value:
                     deltas.append(key)
             except:
                 pass
         return deltas
 
     def copyFieldsFrom(self, obj, fields):
@@ -1013,25 +639,25 @@
             else:
                 file = StringIO(file)
                 file.size = len(file)
                 file.name = file_name
                 mi = MediaItem(name=file_name, group=group, newfile=file)
         else:
             mi = MediaItem(name=file_name, newfile=file, group=group)
-        # rest_helpers.log_print(F"saving media file: {name}")
+        # rh.log_print(F"saving media file: {name}")
         mi.save()
         if is_local:
             setattr(self, name, mi)
         return mi
 
     def updateLogModel(self, request, model):
         if not request:
             request = self.getActiveRequest()
         if not request or not hasattr(request, "setLogModel"):
-            rest_helpers.log_print("request does not support setLogModel")
+            rh.log_print("request does not support setLogModel")
             return
         if not self.id:
             self.save()
         request.setLogModel(model, self.id)
 
     def checkIsOwner(self, member):
         owner_field = getattr(self.RestMeta, "OWNER_FIELD", None)
@@ -1045,17 +671,17 @@
     def on_rest_can_get(self, request):
         perms = getattr(self.RestMeta, "VIEW_PERMS", None)
         if perms:
             if "owner" in perms and self.checkIsOwner(request.member):
                 return True
             # we need to check if this user has permission
             group_field = getattr(self.RestMeta, "GROUP_FIELD", "group")
-            status, error, code = requestHasPerms(request, perms, getattr(self, group_field, None))
+            status, error, code = rh.requestHasPerms(request, perms, getattr(self, group_field, None))
             if not status:
-                raise PermissionDeniedException(error, code)
+                raise re.PermissionDeniedException(error, code)
         return True
 
     def on_rest_get(self, request):
         # check view permissions
         if not self.on_rest_can_get(request):
             return self.restStatus(request, False, error="permission denied", error_code=402)
         self.on_rest_pre_get(request)
@@ -1075,34 +701,34 @@
         if self.pk is None:
             perms = getattr(self.RestMeta, "CREATE_PERMS", perms)
         if perms:
             if "owner" in perms and self.checkIsOwner(request.member):
                 return True
             # we need to check if this user has permission
             group_field = getattr(self.RestMeta, "GROUP_FIELD", "group")
-            # rest_helpers.log_error(F"group field={group_field}")
+            # rh.log_error(F"group field={group_field}")
             if self.pk is None:
                 group = request.DATA.get(group_field)
             elif "__" in group_field and hasattr(self, "group"):
                 group = self.group
             elif "__" in group_field:
                 fields = group_field.split("__")
                 group = self
                 for field in fields:
                     group = getattr(group, field, None)
                     if group is None:
                         break
             else:
                 group = getattr(self, group_field, None)
-            status, error, code = requestHasPerms(request, perms, group)
+            status, error, code = rh.requestHasPerms(request, perms, group)
             if not status:
                 if self.pk is None and code == 402:
                     code = 435
-                rest_helpers.log_error(F"onRestCheckSavePerms: {request.member} {group} permission denied: status={status}, error={error}, code={code}", perms)
-                raise PermissionDeniedException(error, code)
+                rh.log_error(F"onRestCheckSavePerms: {request.member} {group} permission denied: status={status}, error={error}, code={code}", perms)
+                raise re.PermissionDeniedException(error, code)
 
     def on_rest_post(self, request):
         self.saveFromRequest(request)
         status_only = request.DATA.get("status_only", False, field_type=bool)
         if status_only:
             return self.restStatus(request, True)
         graph = request.DATA.get("graph", "default")
@@ -1194,15 +820,15 @@
         return cls.on_rest_list_perms(request, qset)
 
     @classmethod
     def on_rest_filter_member_field(cls, request, qset):
         member_field = getattr(cls.RestMeta, "VIEW_PERMS_MEMBER_FIELD", None)
         if member_field is None:
             return cls.objects.none()
-        # rest_helpers.log_error(dict(**{member_field: request.member}))
+        # rh.log_error(dict(**{member_field: request.member}))
         return qset.filter(**{member_field: request.member})
 
     @classmethod
     def on_rest_list_has_perms(cls, request, perms, qset=None):
         if request.auth_model is not None:
             if request.auth_model.hasPerm(perms):
                 return True
@@ -1227,15 +853,15 @@
             qset = cls.on_rest_filter_children(request, qset)
         if not has_perms:
             return cls.on_rest_filter_member_field(request, qset)
         return qset
 
     @classmethod
     def on_rest_filter_children(cls, request, qset=None):
-        # rest_helpers.log_error("filter by group?")
+        # rh.log_error("filter by group?")
         group_field = getattr(cls.RestMeta, "GROUP_FIELD", "group")
         if group_field is None or ("__" not in group_field and not cls.has_model_field_name(group_field)):
             return qset
         parent_kinds = getattr(cls.RestMeta, "LIST_PARENT_KINDS", ["org"])
         if request.DATA.get("child_groups") or request.group.kind in parent_kinds:
             ids = request.group.getAllChildrenIds()
             ids.append(request.group.id)
@@ -1247,22 +873,22 @@
             q = {}
             q["{}_id__in".format(group_field)] = ids
             return qset.filter(**q)
         elif "__" in group_field:
             q = {}
             q[group_field] = request.group.id
             qset = qset.filter(**q)
-            # rest_helpers.log_error(q, qset.count())
+            # rh.log_error(q, qset.count())
         return qset
 
     @classmethod
     def on_rest_list_ready(cls, request, qset=None):
         # override on do any post filters
-        # rest_helpers.log_error("RAW SQL")
-        # rest_helpers.log_error(qset.query)
+        # rh.log_error("RAW SQL")
+        # rh.log_error(qset.query)
         return qset
 
     @classmethod
     def on_rest_date_filter(cls, request, qset=None):
         dr_start = request.DATA.get("dr_start", field_type=datetime)
         dr_end = request.DATA.get("dr_end", field_type=datetime)
         if dr_start is not None:
@@ -1272,28 +898,28 @@
                 # dr_end = dr_end + timedelta(hours=24)
             elif dr_end == dr_start:
                 dr_end = dr_start + timedelta(days=1)
             dr_tz = request.DATA.get("dr_timezone")
             if dr_tz is not None:
                 dr_eod = request.DATA.get("dr_eod", 0, field_type=int)
                 dr_granularity = request.DATA.get("granularity", "day")
-                dr_start, dr_end = rest_helpers.getDateRangeZ(dr_start, dr_end, dr_granularity, dr_tz, hour=dr_eod)
+                dr_start, dr_end = rh.getDateRangeZ(dr_start, dr_end, dr_granularity, dr_tz, hour=dr_eod)
             else:
                 dr_offset = request.DATA.get("dr_offset", 0, field_type=int)
                 if dr_offset > 0:
                     dr_start = dr_start + timedelta(minutes=dr_offset)
                     dr_end = dr_end + timedelta(minutes=dr_offset)
             dr_field = request.DATA.get("dr_field", getattr(cls.RestMeta, "DATE_RANGE_FIELD", "created"))
             q = dict()
             q["{}__gte".format(dr_field)] = dr_start
             q["{}__lte".format(dr_field)] = dr_end
             qset = qset.filter(**q)
             request.response_extra = dict(
-                dr_start=rest_helpers.convertToEpoch(dr_start),
-                dr_end=rest_helpers.convertToEpoch(dr_end))
+                dr_start=rh.convertToEpoch(dr_start),
+                dr_end=rh.convertToEpoch(dr_end))
         return qset
 
     @classmethod
     def on_rest_list(cls, request, qset=None):
         qset = cls.on_rest_list_query(request, qset)
         graph = request.DATA.get("graph", "list")
         format = request.DATA.get("format")
@@ -1339,15 +965,15 @@
         return sort_args
 
     @classmethod
     def on_rest_list_format(cls, request, format, qset):
         if format in ["summary", "summary_only"]:
             return cls.on_rest_list_summary(request, qset)
         if hasattr(cls.RestMeta, "FORMATS"):
-            fields =  cls.RestMeta.FORMATS.get(format)
+            fields = cls.RestMeta.FORMATS.get(format)
         else:
             no_show_fields = RestModel.__RestMeta__.NO_SHOW_FIELDS
             if hasattr(cls.RestMeta, "NO_SHOW_FIELDS"):
                 no_show_fields = cls.RestMeta.NO_SHOW_FIELDS
 
             fields = []
             for f in cls._meta.fields:
@@ -1377,29 +1003,29 @@
             elif format == "flat":
                 return GRAPH_HELPERS.views.restFlat(request, qset, fields, name, format_size)
     
     @classmethod
     def on_rest_list_summary(cls, request, qset):
         cls._boundRest()
         summary_info = getattr(cls.RestMeta, "SUMMARY_FIELDS", {})
-        output = UberDict()
+        output = objict()
         output.count = qset.count()
         for key, value in summary_info.items():
             if key == "sum":
-                res = rest_helpers.getSum(qset, *value)
+                res = rh.getSum(qset, *value)
                 if isinstance(res, dict):
                     output.update(res)
                 else:
                     output[value[0]] = res
             elif key == "avg":
                 for f in value:
-                    output["avg_{}".format(f)] = rest_helpers.getAverage(qset, f)
+                    output["avg_{}".format(f)] = rh.getAverage(qset, f)
             elif key == "max":
                 for f in value:
-                    output["max_{}".format(f)] = rest_helpers.getMax(qset, f)
+                    output["max_{}".format(f)] = rh.getMax(qset, f)
             elif isinstance(value, dict):
                 if "|" in key:
                     fields = key.split("|")
                     if len(fields) > 1:
                         lbl = fields[0]
                         action = fields[1]
                         field = None
@@ -1409,19 +1035,19 @@
                     action = "count"
                     lbl = key
                     field = None
                 act_qset = qset.filter(**value)
                 if action == "count":
                     output[lbl] = act_qset.count()
                 elif action == "sum":
-                    output[lbl] = rest_helpers.getSum(act_qset, field)
+                    output[lbl] = rh.getSum(act_qset, field)
                 elif action == "avg":
-                    output[lbl] = rest_helpers.getAverage(act_qset, field)
+                    output[lbl] = rh.getAverage(act_qset, field)
                 elif action == "max":
-                    output[lbl] = rest_helpers.getMax(act_qset, field)
+                    output[lbl] = rh.getMax(act_qset, field)
         return GRAPH_HELPERS.restGet(request, output)
 
     @classmethod
     def on_rest_batch(cls, request, action):
         # this method is called when rest_batch='somme action'
         cls._boundRest()
         batch_ids = request.DATA.getlist("batch_ids", [])
@@ -1446,22 +1072,21 @@
             if not isinstance(update_fields, dict):
                 return GRAPH_HELPERS.restStatus(request, False, error="batch_update should be key/values")
             count = qset.update(**update_fields)
             return GRAPH_HELPERS.restStatus(request, True, error="updated {} items".format(count))
         elif action == "create":
             batch_data = request.DATA.getlist("batch_data", [])
             items = []
-            exist = []
             for item in batch_data:
                 try:
                     obj = cls.ro_objects().filter(**item).last()
                     if not obj:
                         obj.saveFromDict(request, item)
                     items.append(obj)
-                except:
+                except Exception:
                     pass
             return GRAPH_HELPERS.restList(request, items)
         return GRAPH_HELPERS.restStatus(request, False, error="not implemented")
 
     @classmethod
     def on_rest_create(cls, request, pk=None):
         # permissions are checked in the save routine
@@ -1470,15 +1095,15 @@
             return GRAPH_HELPERS.restStatus(request, False, error="creation not allowed via rest for this model.")
 
         if hasattr(cls.RestMeta, "KEY_TO_FIELD_MAP"):
             kv = {}
             for k, v in list(cls.RestMeta.KEY_TO_FIELD_MAP.items()):
                 if hasattr(request, k):
                     value = getattr(request, k)
-                    if value != None:
+                    if value is not None:
                         kv[v] = value
             obj = cls.createFromRequest(request, **kv)
         else:
             obj = cls.createFromRequest(request)
         graph = request.DATA.get("graph", "default")
         return obj.restGet(request, graph)
 
@@ -1497,15 +1122,15 @@
             GRAPH_HELPERS.restGet = views.restGet
         if not GRAPH_HELPERS.get_request:
             mw = importlib.import_module("rest.middleware")
             GRAPH_HELPERS.get_request = mw.get_request
 
     @classmethod
     def get_rest_help(cls):
-        output = UberDict()
+        output = objict()
         if cls.__doc__:
             output.doc = cls.__doc__.rstrip()
         else:
             output.doc = ""
         output.model_name = cls.get_class_name()
         output.fields = cls.rest_getQueryFields(True)
         output.graphs = {}
@@ -1622,21 +1247,21 @@
     @classmethod
     def on_rest_set_query_defaults(cls, request):
         if not hasattr(request, "default_rest_filters"):
             request.default_rest_filters = None
             default_filters = getattr(cls.RestMeta, "LIST_DEFAULT_FILTERS", None)
             if default_filters:
                 # make a copy so we can remove filters until the end
-                request.default_rest_filters = UberDict.fromdict(default_filters)
+                request.default_rest_filters = objict.fromdict(default_filters)
 
     @classmethod
     def filterFromRequest(cls, request, qset):
         '''returns None if not foreignkey, otherswise the relevant model'''
         filter = request.DATA.pop("filter")
-        # rest_helpers.debug("filterFromRequest")
+        # rh.debug("filterFromRequest")
         cls.on_rest_set_query_defaults(request)
         if not filter:
             return qset
 
         field_names = cls.rest_getQueryFields()
         q = {}
 
@@ -1694,22 +1319,22 @@
                     value = value.split(',')
                 elif value in ["true", "True", "1"]:
                     value = 1
                 elif value in ["false", "False", "0"]:
                     value = 0
                 if isinstance(value, str) and "(" in value and ")" in value:
                     # this is a special function call
-                    # rest_helpers.log_print(value)
+                    # rh.log_print(value)
                     if value.startswith("days("):
                         spos = value.find("(")+1
                         epos = value.find(")")
-                        # rest_helpers.log_print(int(value[spos:epos]))
+                        # rh.log_print(int(value[spos:epos]))
                         value = now + timedelta(days=int(value[spos:epos]))
-                        # rest_helpers.log_print(now)
-                        # rest_helpers.log_print(value)
+                        # rh.log_print(now)
+                        # rh.log_print(value)
                     elif value.startswith("hours("):
                         spos = value.find("(")+1
                         epos = value.find(")")
                         value = now + timedelta(hours=int(value[spos:epos]))
                     elif value.startswith("minutes("):
                         spos = value.find("(")+1
                         epos = value.find(")")
@@ -1719,17 +1344,17 @@
                         epos = value.find(")")
                         value = now + timedelta(seconds=int(value[spos:epos]))
                     else:
                         continue
                 if key.count('__') <= 4:
                     q[key] = value
             else:
-                rest_helpers.log_print("filterFromRequest: invalid field: {} or {}".format(name, key))
+                rh.log_print("filterFromRequest: invalid field: {} or {}".format(name, key))
         if q:
-            # rest_helpers.debug("filtering...", q)
+            # rh.debug("filtering...", q)
             qset = qset.filter(**q)
         return qset
 
     @classmethod
     def on_rest_handle_filter(cls, qset, filters, request=None):
         return qset
 
@@ -1778,15 +1403,15 @@
             <field_name>=<operator>:value
         """
         q = {}
         field_names = cls.rest_getQueryFields()
         query_keys = request.DATA.keys()
         special_keys = getattr(cls.RestMeta, "QUERY_FIELDS_SPECIAL", {})
         cls.on_rest_set_query_defaults(request)
-        # rest_helpers.debug("queryFromRequest.key", query_keys, special_keys, field_names)
+        # rh.debug("queryFromRequest.key", query_keys, special_keys, field_names)
         for key in query_keys:
             # remove the key from defaults
             if request.default_rest_filters:
                 j = request.default_rest_filters.pop(key, None)
                 for drk in request.default_rest_filters:
                     if drk.startswith(f"{key}__"):
                         j = request.default_rest_filters.pop(drk, None)
@@ -1850,18 +1475,18 @@
                 if isinstance(value, str) and ',' in value:
                     value = [a.strip() for a in value.split(',')]
             elif oper is None and value in ["null", "None"]:
                 key = "{}__isnull".format(key)
                 value = True
             ft = cls.get_field_type(fn)
             if ft == "DateTimeField":
-                value = rest_helpers.parseDateTime(value)
+                value = rh.parseDateTime(value)
             q[key] = value
         if bool(q):
-            rest_helpers.debug("queryFromRequest", q, request.default_rest_filters)
+            # rh.debug("queryFromRequest", q, request.default_rest_filters)
             qset = qset.filter(**q)
         return qset
 
     @classmethod
     def createFromRequest(cls, request, **kwargs):
         obj = cls()
         return obj.saveFromRequest(request, files=request.FILES, __is_new=True, **kwargs)
@@ -1918,9 +1543,9 @@
 
     @classmethod
     def get_fk_model(cls, fieldname):
         '''returns None if not foreignkey, otherswise the relevant model'''
         try:
             field = cls._meta.get_field(fieldname)
             return field.related_model
-        except:
+        except Exception:
             return None
```

### Comparing `django_restit-4.0.9/rest/regexes.yaml` & `django_restit-4.1.1/rest/regexes.yaml`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/requestex.py` & `django_restit-4.1.1/rest/requestex.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/rpc.py` & `django_restit-4.1.1/rest/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/search.py` & `django_restit-4.1.1/rest/search.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/serializers/collection.py` & `django_restit-4.1.1/rest/serializers/collection.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from . import model as ms
 from django.db.models.query import QuerySet
+from rest import settings
+# from . import profiler
 
 
 def serialize(qset, graph, sort=None, size=25, start=0):
     if isinstance(graph, str):
         model = getattr(qset, "model", None)
         if model:
             graph = model.getGraph(graph)
@@ -14,31 +16,38 @@
     fields = graph.get("fields", [])
     extra = graph.get("extra", [])
     exclude = graph.get("exclude", [])
     recurse_into = graph.get("recurse_into", [])
     return to_list(qset, sort, size, fields=fields, extra=extra, exclude=exclude, recurse_into=recurse_into)
 
 
-def to_list(qset, sort=None, size=25, start=0, fields=[], extra=[], exclude=[], recurse_into=[]):
+def to_list(qset, sort=None, size=25, start=0, fields=[], extra=[], exclude=[], recurse_into=[], cache=None):
+    if cache is None:
+        cache = dict()
     output = {"size": size, "start": start}
     if sort and isinstance(qset, QuerySet):
         sort_args = get_sort_args(qset, sort)
         try:
             qset = qset.order_by(*sort_args)
             output["sort"] = sort_args
         except Exception:
             pass
 
     qset = qset[start:start+size+1]
     if not fields:
         fields = ms.get_fields(qset)
+    if settings.REST_SELECT_RELATED:
+        # this should improve speed greatly for lookups
+        foreign_fields = ms.get_foreign_fields(qset.model, fields)
+        if foreign_fields:
+            qset = qset.select_related(*foreign_fields)
     data = []
     output["data"] = data
     for obj in qset:
-        data.append(ms.to_dict(obj, fields, extra, exclude, recurse_into))
+        data.append(ms.to_dict(obj, fields, extra, exclude, recurse_into, cache=cache))
     return output
 
 
 def get_sort_args(qset, sort):
     if not isinstance(sort, str) or "metadata" in sort:
         return None
     if sort.endswith("_display"):
```

### Comparing `django_restit-4.0.9/rest/serializers/csv.py` & `django_restit-4.1.1/rest/serializers/csv.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/serializers/excel.py` & `django_restit-4.1.1/rest/serializers/excel.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/serializers/json.py` & `django_restit-4.1.1/rest/serializers/json.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/serializers/legacy.py` & `django_restit-4.1.1/rest/serializers/legacy.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import time
 import pprint
 import re
 import inspect
 import base64
 import copy
 import json
-
+from . import profiler
 
 CHUNKDIR = os.path.join(os.environ.get('TMPDIR', '/tmp'), 'chunked_uploads')
 
 
 def toJSON(data, **kwargs):
     return json.dumps(data, cls=JSONEncoderExt)
     # return json.dumps(data, **kwargs)
@@ -490,14 +490,16 @@
                     raise ValueError('Invalid feature action: %s' % p)
 
     if got_features:
         return func(request, qset, features=features, **kwargs)
     else:
         return None
 
+
+@profiler.timeit
 def restGet(request, qset, model=None, fields=None, extra=[], exclude=[], fkey_depth=0, recurse_into=[], filter={}, orig_request=None, orig_objs={}, ignore_noattr=False, require_perms=[], accept_list=None, featuresets={}, features=[], return_httpresponse=True):
     """
     request: HttpRequest object
     qset: QuerySet or data object to return
     model: (optional) model of the queryset
     fields: (optional) fields to return, default to all fields.  string, or tuple(db_field, output_field)
     extra: (optional) extra fields to return
@@ -817,14 +819,15 @@
     ret["size"] = size
     ret["count"] = count
     ret["start"] = start
     ret["data"] = data_list
     return restResult(request, ret, accept_list)
 
 
+@profiler.timeit
 def restList(request, qset, model=None, size=25, start=0, sort=None, fields=None, extra=[], exclude=[], fkey_depth=0, recurse_into=[], filter={}, get_count=True, orig_request=None, orig_objs={}, page=None, ignore_noattr=False, todata=lambda x: x, require_perms=[], accept_list=None, featuresets={}, features=[], return_httpresponse=True, totals=None):
     """
     request: HttpRequest object
     qset: QuerySet or data object to return
     model: (optional) model of the queryset
     size: (optional) return set size, default 25, can override via GET[size].  0=return all.
     start: (optional) return set offset, default 0, can override via GET[start]
```

### Comparing `django_restit-4.0.9/rest/serializers/model.py` & `django_restit-4.1.1/rest/serializers/model.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import math
 from decimal import Decimal
 from django.db import models
 from itertools import chain
 from rest import helpers
 from objict import objict
 __MY_CACHE__ = objict()
+# from . import profiler
 
 
 def serialize(instance, graph):
     if isinstance(graph, str):
         graph = instance.getGraph(graph)
     return to_dict_from_graph(instance, graph)
 
@@ -19,18 +20,41 @@
     fields = graph.get("fields", [])
     extra = graph.get("extra", [])
     exclude = graph.get("exclude", [])
     recurse_into = graph.get("recurse_into", [])
     return to_dict(instance, fields=fields, extra=extra, exclude=exclude, recurse_into=recurse_into)
 
 
-def to_dict(instance, fields=None, extra=[], exclude=[], recurse_into=[]):
+def get_from_cache(cache, instance):
+    if cache is not None and isinstance(instance, models.Model) and hasattr(instance, "get_class_name"):
+        cn = instance.get_class_name()
+        key = f"{cn}.{instance.pk}"
+        if key in cache:
+            return cache[key]
+    return None
+
+
+def add_to_cache(cache, instance, data):
+    if cache is not None and isinstance(instance, models.Model) and hasattr(instance, "get_class_name"):
+        cn = instance.get_class_name()
+        key = f"{cn}.{instance.pk}"
+        if key not in cache:
+            cache[key] = data
+
+# @profiler.timeit
+def to_dict(instance, fields=None, extra=[], exclude=[], recurse_into=[], cache=None):
     data = {}
     fields = get_fields(instance) if not fields else fields
     recursed = []
+
+    cached_item = get_from_cache(cache, instance)
+    if cached_item:
+        # profiler.logger.info("cache hit")
+        return cached_item
+
     for f in chain(fields, extra, recurse_into):
         fin, fout = (f[0], f[1]) if isinstance(f, (list, tuple)) else (f, f)
         if fin in exclude:
             continue
         if "." in fin:
             top = fin.split('.')[0]
             if top in recursed:
@@ -48,52 +72,57 @@
             continue
         value = get_field_value(instance, fin)
         if isinstance(value, models.Model):
             if fin not in recursed:
                 recursed.append(fin)
             sfields = get_model_fields(fin, chain(fields, extra, recurse_into))
             if sfields:
-                data[fout] = to_dict(value, sfields)
+                data[fout] = to_dict(value, sfields, cache=cache)
             elif hasattr(value, "pk"):
                 data[fout] = value.pk
                 # FIXME we should use _id when not showing full model
                 # data[f"{fout}_id"] = value.pk
             continue
         if isinstance(value, models.Manager):
             if fin not in recursed:
                 recursed.append(fin)
             sfields = get_model_fields(fin, chain(fields, extra, recurse_into))
             if __MY_CACHE__.cs is None:
                 __MY_CACHE__.cs = helpers.importModule("rest.serializers.collection")
             data[fout] = __MY_CACHE__.cs.to_list(value.all(), fields=sfields)["data"]
             continue
         try:
-            data[fout] = serialize_value(value if not callable(value) else value())
+            if callable(value):
+                data[fout] = serialize_value(value())
+            else:
+                data[fout] = serialize_value(value)
         except Exception as err:
             data[fout] = str(err)
             helpers.log_exception(fout)
+    if cache is not None:
+        add_to_cache(cache, instance, data)
     return data
 
 
 def serialize_value(value):
     if isinstance(value, (str, int, float)):
         return value
     if isinstance(value, (tuple, list)):
-        return [serialize_value(v) for v in value]
+        value = [serialize_value(v) for v in value]
     elif isinstance(value, dict):
-        return {key: serialize_value(val) for key, val in value.items()}
+        value = {key: serialize_value(val) for key, val in value.items()}
     elif isinstance(value, datetime.datetime):
         # return int(time.mktime(value.timetuple()))
-        return time.mktime(value.timetuple())
+        value = value.timestamp()
     elif isinstance(value, datetime.date):
-        return value.strftime("%Y/%m/%d")
+        value = value.strftime("%Y/%m/%d")
     elif isinstance(value, float) and math.isnan(value):
-        return 0.0
+        value = 0.0
     elif isinstance(value, Decimal):
-        return float(value) if not value.is_nan() else 0.0
+        value = float(value) if not value.is_nan() else 0.0
     return value
 
 
 def get_generic_value(instance, key, graph="generic"):
     obj = None
     try:
         obj = instance.restGetGenericRelation(key)
@@ -136,7 +165,30 @@
     elif hasattr(qset, 'model'):
         fields = qset.model._meta.fields
     elif hasattr(qset, 'keys'):
         return list(qset.keys())
     elif model and hasattr(model, '_meta'):
         fields = model._meta.fields
     return [f.name for f in fields] if fields else None
+
+
+def get_foreign_fields(model, fields):
+    fkeys = objict()
+    ignore_keys = []
+    for key in fields:
+        if "." in key:
+            fields = key.split('.')
+            skey = fields.pop(0)
+            if skey not in fkeys and skey not in ignore_keys:
+                fm = model.get_fk_model(skey)
+                if not fm:
+                    ignore_keys.append(skey)
+                    continue
+                fkeys[skey] = objict(fields=[".".join(fields)], model=fm)
+            else:
+                fkeys[skey].fields.append(".".join(fields))
+
+    output = list(fkeys.keys())
+    for fkey, info in fkeys.items():
+        for sub_key in get_foreign_fields(info.model, info.fields):
+            output.append(f"{fkey}__{sub_key}")
+    return output
```

### Comparing `django_restit-4.0.9/rest/serializers/response.py` & `django_restit-4.1.1/rest/serializers/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,38 +7,39 @@
 import time
 from auditlog.models import PersistentLog
 from . import model as ms
 from . import collection as cs
 from . import json as js
 from . import csv
 from . import excel
-
+# from . import profiler
 
 def restStatus(request, status, data={}, **kwargs):
     if isinstance(data, str):
         if status:
             data = dict(message=data)
         else:
             data = dict(error=data)
     data = data.copy()
     data.update(kwargs)
     data["status"] = status
     return restResult(request, data)
 
 
+# @profiler.timeit
 def restGet(request, obj, fields=None, extra=[], exclude=[], recurse_into=[], **kwargs):
     data = ms.to_dict(obj, fields, extra, exclude, recurse_into)
     if not kwargs.get("return_httpresponse", True):
         return data
     data = dict(data=data, status=kwargs.get("status", True))
     data["datetime"] = int(time.time())
     data["elapsed"] = get_request_elapsed(request)
     return restResult(request, data)
 
-
+# @profiler.timeit
 def restList(request, qset, size=25, start=0, sort=None, fields=None, extra=[], exclude=[], recurse_into=[], **kwargs):
     count = 0
     if isinstance(qset, QuerySet):
         count = qset.count()
     elif isinstance(qset, list):
         count = len(qset)
     start = request.DATA.get("start", start, field_type=int)
```

### Comparing `django_restit-4.0.9/rest/serializers/util.py` & `django_restit-4.1.1/rest/serializers/util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/settings_helper.py` & `django_restit-4.1.1/rest/settings_helper.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/static/lib/jquery.js` & `django_restit-4.1.1/rest/static/lib/jquery.js`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/templates/email/error.html` & `django_restit-4.1.1/rest/templates/email/error.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/templates/rest_docs.html` & `django_restit-4.1.1/rest/templates/rest_docs.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/templates/rest_html.html` & `django_restit-4.1.1/rest/templates/rest_html.html`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/ua.py` & `django_restit-4.1.1/rest/ua.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/uberdict.py` & `django_restit-4.1.1/rest/uberdict.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/url_docs.py` & `django_restit-4.1.1/rest/url_docs.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/urls.py` & `django_restit-4.1.1/rest/urls.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/rest/views.py` & `django_restit-4.1.1/rest/views.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/sessionlog/migrations/0001_initial.py` & `django_restit-4.1.1/sessionlog/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/sessionlog/models.py` & `django_restit-4.1.1/sessionlog/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/taskqueue/README.md` & `django_restit-4.1.1/taskqueue/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/taskqueue/migrations/0001_initial.py` & `django_restit-4.1.1/taskqueue/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/taskqueue/models.py` & `django_restit-4.1.1/taskqueue/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/taskqueue/periodic.py` & `django_restit-4.1.1/taskqueue/periodic.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/taskqueue/rpc.py` & `django_restit-4.1.1/taskqueue/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/taskqueue/tq.py` & `django_restit-4.1.1/taskqueue/tq.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/taskqueue/transports/email.py` & `django_restit-4.1.1/taskqueue/transports/email.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/taskqueue/transports/http.py` & `django_restit-4.1.1/taskqueue/transports/http.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/taskqueue/transports/s3.py` & `django_restit-4.1.1/taskqueue/transports/s3.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/taskqueue/transports/sftp.py` & `django_restit-4.1.1/taskqueue/transports/sftp.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/taskqueue/worker.py` & `django_restit-4.1.1/taskqueue/worker.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/telephony/migrations/0001_initial.py` & `django_restit-4.1.1/telephony/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/telephony/models.py` & `django_restit-4.1.1/telephony/models.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/telephony/phone_util.py` & `django_restit-4.1.1/telephony/phone_util.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/telephony/rpc.py` & `django_restit-4.1.1/telephony/rpc.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/ws4redis/README.md` & `django_restit-4.1.1/ws4redis/README.md`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/ws4redis/client.py` & `django_restit-4.1.1/ws4redis/client.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/ws4redis/connection.py` & `django_restit-4.1.1/ws4redis/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,14 +199,16 @@
 
     def on_channel_msg(self, msg):
         if not self.canPublishTo(msg):
             logger.warning("on_channel_msg permission denied", msg)
             self.sendToWS(msg.channel, dict(error="cannot publish to channel"))
             return None
         ch_model = private_settings.WS4REDIS_CHANNELS.get(msg.channel, None)
+        if ch_model is None:
+            return None
         Model = self.getAppModel(ch_model)
         if not hasattr(Model, "onWS4RedisMessage"):
             logger.warning(f"{msg.channel} does not support onWS4RedisMessage")
             self.sendToWS(msg.channel, dict(error="channel does not support onWS4RedisMessage"))
             return None
         Model.onWS4RedisMessage(self.credentials, msg)
 
@@ -271,14 +273,15 @@
 
     def on_ws_pending(self):
         try:
             self.last_msg = self.websocket.receive()
             if bool(self.last_msg):
                 self.on_ws_msg(self.last_msg)
         except Exception:
+            logger.exception()
             logger.error("unable to recv on ws... flushing")
             self.websocket.flush()
 
     def checkHeartbeat(self):
         beat_delta = time.time() - self.last_beat
         if beat_delta > 30.0:
             self.last_beat = time.time()
```

### Comparing `django_restit-4.0.9/ws4redis/exceptions.py` & `django_restit-4.1.1/ws4redis/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/ws4redis/redis.py` & `django_restit-4.1.1/ws4redis/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             count = 0
             for spk in pk:
                 count += self.publish(message, channel, facility, pk=spk, expire=expire, prefix=prefix)
             return count
 
         channel_key = self.channelToKey(channel, facility, pk, prefix)
         if settings.WS4REDIS_LOG_DEBUG:
-            logger.info("publishing to: {0}".format(channel_key))
+            logger.info("publishing msg to: {0}".format(channel_key), message)
         count = self.connection.publish(channel_key, message)
         return count
 
     def getSubMessage(self):
         # get a message pending from subscription
         if self.pubsub:
             return self.pubsub.parse_response()
```

### Comparing `django_restit-4.0.9/ws4redis/servers/base.py` & `django_restit-4.1.1/ws4redis/servers/base.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/ws4redis/servers/django.py` & `django_restit-4.1.1/ws4redis/servers/django.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/ws4redis/servers/uwsgi.py` & `django_restit-4.1.1/ws4redis/servers/uwsgi.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/ws4redis/settings.py` & `django_restit-4.1.1/ws4redis/settings.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/ws4redis/utf8validator.py` & `django_restit-4.1.1/ws4redis/utf8validator.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/ws4redis/websocket.py` & `django_restit-4.1.1/ws4redis/websocket.py`

 * *Files identical despite different names*

### Comparing `django_restit-4.0.9/PKG-INFO` & `django_restit-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-restit
-Version: 4.0.9
+Version: 4.1.1
 Summary: A Rest Framework for DJANGO
 License: MIT
 Author: Ian Starnes
 Author-email: ians@311labs.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

