# Comparing `tmp/activecampaign_python-1.0.8.tar.gz` & `tmp/activecampaign_python-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activecampaign_python-1.0.8.tar", max compression
+gzip compressed data, was "activecampaign_python-1.0.9.tar", max compression
```

## Comparing `activecampaign_python-1.0.8.tar` & `activecampaign_python-1.0.9.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0     1065 2023-03-27 20:59:00.982544 activecampaign_python-1.0.8/LICENSE
--rw-r--r--   0        0        0    15391 2023-06-23 13:30:45.288998 activecampaign_python-1.0.8/README.md
--rw-r--r--   0        0        0        0 2023-03-27 20:59:00.982882 activecampaign_python-1.0.8/activecampaign/__init__.py
--rw-r--r--   0        0        0      245 2023-03-27 20:59:00.983020 activecampaign_python-1.0.8/activecampaign/automations.py
--rw-r--r--   0        0        0      457 2023-07-07 13:57:13.984494 activecampaign_python-1.0.8/activecampaign/campaigns.py
--rw-r--r--   0        0        0     2281 2023-07-07 13:57:13.984688 activecampaign_python-1.0.8/activecampaign/client.py
--rw-r--r--   0        0        0     5856 2023-03-27 20:59:00.983212 activecampaign_python-1.0.8/activecampaign/contacts.py
--rw-r--r--   0        0        0     6205 2023-06-23 13:30:45.289308 activecampaign_python-1.0.8/activecampaign/customobjects.py
--rw-r--r--   0        0        0      255 2023-03-27 20:59:00.983313 activecampaign_python-1.0.8/activecampaign/dealActivities.py
--rw-r--r--   0        0        0     4374 2023-03-27 20:59:00.983429 activecampaign_python-1.0.8/activecampaign/deals.py
--rw-r--r--   0        0        0     3782 2023-03-27 20:59:00.983524 activecampaign_python-1.0.8/activecampaign/deepdataintegrations.py
--rw-r--r--   0        0        0      258 2023-03-27 20:59:00.983601 activecampaign_python-1.0.8/activecampaign/emailActivities.py
--rw-r--r--   0        0        0       86 2023-03-27 20:59:00.983691 activecampaign_python-1.0.8/activecampaign/exception.py
--rw-r--r--   0        0        0     1485 2023-03-27 20:59:00.983787 activecampaign_python-1.0.8/activecampaign/lists.py
--rw-r--r--   0        0        0      268 2023-03-27 20:59:00.983875 activecampaign_python-1.0.8/activecampaign/messages.py
--rw-r--r--   0        0        0     1165 2023-03-27 20:59:00.983965 activecampaign_python-1.0.8/activecampaign/notes.py
--rw-r--r--   0        0        0     1099 2023-03-27 20:59:00.984046 activecampaign_python-1.0.8/activecampaign/tags.py
--rw-r--r--   0        0        0     1157 2023-03-27 20:59:00.984140 activecampaign_python-1.0.8/activecampaign/tasks.py
--rw-r--r--   0        0        0     2148 2023-03-27 20:59:00.984242 activecampaign_python-1.0.8/activecampaign/users.py
--rw-r--r--   0        0        0     1380 2023-03-27 20:59:00.984331 activecampaign_python-1.0.8/activecampaign/webhooks.py
--rw-r--r--   0        0        0      415 2023-07-07 13:57:23.096302 activecampaign_python-1.0.8/pyproject.toml
--rw-r--r--   0        0        0    16052 1970-01-01 00:00:00.000000 activecampaign_python-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-03-27 20:59:00.982544 activecampaign_python-1.0.9/LICENSE
+-rw-r--r--   0        0        0    18856 2023-07-11 16:44:06.918299 activecampaign_python-1.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-03-27 20:59:00.982882 activecampaign_python-1.0.9/activecampaign/__init__.py
+-rw-r--r--   0        0        0      925 2023-07-11 16:44:06.918530 activecampaign_python-1.0.9/activecampaign/addresses.py
+-rw-r--r--   0        0        0      245 2023-03-27 20:59:00.983020 activecampaign_python-1.0.9/activecampaign/automations.py
+-rw-r--r--   0        0        0      430 2023-07-11 16:44:06.918665 activecampaign_python-1.0.9/activecampaign/brandings.py
+-rw-r--r--   0        0        0      457 2023-07-07 13:57:13.984494 activecampaign_python-1.0.9/activecampaign/campaigns.py
+-rw-r--r--   0        0        0     2429 2023-07-11 16:44:06.918872 activecampaign_python-1.0.9/activecampaign/client.py
+-rw-r--r--   0        0        0     7259 2023-07-11 16:44:06.919073 activecampaign_python-1.0.9/activecampaign/contacts.py
+-rw-r--r--   0        0        0     6205 2023-06-23 13:30:45.289308 activecampaign_python-1.0.9/activecampaign/customobjects.py
+-rw-r--r--   0        0        0      255 2023-03-27 20:59:00.983313 activecampaign_python-1.0.9/activecampaign/dealActivities.py
+-rw-r--r--   0        0        0     4374 2023-03-27 20:59:00.983429 activecampaign_python-1.0.9/activecampaign/deals.py
+-rw-r--r--   0        0        0     3782 2023-03-27 20:59:00.983524 activecampaign_python-1.0.9/activecampaign/deepdataintegrations.py
+-rw-r--r--   0        0        0      258 2023-03-27 20:59:00.983601 activecampaign_python-1.0.9/activecampaign/emailActivities.py
+-rw-r--r--   0        0        0       86 2023-03-27 20:59:00.983691 activecampaign_python-1.0.9/activecampaign/exception.py
+-rw-r--r--   0        0        0     1485 2023-03-27 20:59:00.983787 activecampaign_python-1.0.9/activecampaign/lists.py
+-rw-r--r--   0        0        0      268 2023-03-27 20:59:00.983875 activecampaign_python-1.0.9/activecampaign/messages.py
+-rw-r--r--   0        0        0     1165 2023-03-27 20:59:00.983965 activecampaign_python-1.0.9/activecampaign/notes.py
+-rw-r--r--   0        0        0     1099 2023-03-27 20:59:00.984046 activecampaign_python-1.0.9/activecampaign/tags.py
+-rw-r--r--   0        0        0     1157 2023-03-27 20:59:00.984140 activecampaign_python-1.0.9/activecampaign/tasks.py
+-rw-r--r--   0        0        0     2148 2023-03-27 20:59:00.984242 activecampaign_python-1.0.9/activecampaign/users.py
+-rw-r--r--   0        0        0     1380 2023-03-27 20:59:00.984331 activecampaign_python-1.0.9/activecampaign/webhooks.py
+-rw-r--r--   0        0        0      415 2023-07-11 16:44:06.919261 activecampaign_python-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0    19517 1970-01-01 00:00:00.000000 activecampaign_python-1.0.9/PKG-INFO
```

### Comparing `activecampaign_python-1.0.8/LICENSE` & `activecampaign_python-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.8/README.md` & `activecampaign_python-1.0.9/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -209,14 +209,79 @@
 ```
 
 #### Retrieve field options
 ```
 response = client.contacts.retrieve_field_options("field_id")
 ```
 
+#### Create a custom field value
+```
+response = activecampaign_client.contacts.create_a_custom_field_value(data)
+```
+
+#### Retrieve a custom field value
+```
+response = activecampaign_client.contacts.retrieve_a_custom_field_value(field_value_id="some-id")
+```
+
+#### Update a custom field value for contact
+```
+response = activecampaign_client.contacts.update_a_custom_field_value_for_contact(data, field_value_id="some-id")
+```
+
+#### Delete a custom field value
+```
+response = activecampaign_client.contacts.delete_a_custom_field_value(field_value_id="some-id")
+```
+
+#### List all custom field values
+```
+response = activecampaign_client.contacts.list_all_custom_field_values()
+```
+
+#### Retrieve a contact's field values
+```
+response = activecampaign_client.contacts.retrieve_a_contacts_field_values(contact_id="some-id")
+```
+
+#### Retrieve a contact's tracking logs
+```
+response = activecampaign_client.contacts.retrieve_a_contacts_tracking_logs(contact_id="some-id")
+```
+
+#### Retrieve a contact's data
+```
+response = activecampaign_client.contacts.retrieve_a_contacts_data(contact_id="some-id")
+```
+
+#### Retrieve a contact's bounce logs
+```
+response = activecampaign_client.contacts.retrieve_a_contacts_bounce_logs(contact_id="some-id")
+```
+
+#### Retrieve a contact's geo ips
+```
+response = activecampaign_client.contacts.retrieve_a_contacts_geo_ips(contact_id="some-id")
+```
+
+#### Retrieve a contact's organization
+```
+response = activecampaign_client.contacts.retrieve_a_contacts_organization(contact_id="some-id")
+```
+
+#### Retrieve a contact's account contacts
+```
+response = activecampaign_client.contacts.retrieve_a_contacts_account_contacts(contact_id="some-id")
+```
+
+#### Retrieve a contact's automation entry counts
+```
+response = activecampaign_client.contacts.retrieve_a_contacts_automation_entry_counts(contact_id="some-id")
+```
+
 #### Add a tag to a contact
 ```
 data = {
     "contactTag": {
         "contact": "1",
         "tag": "20"
     }
@@ -772,14 +837,82 @@
 #### List all records
 ```
 response = client.customobjects.list_all_records(
         schema_id="some-id", contact_id="some-contact-id", deal_id=None, account_id=None,
         limit=20, offset=0)
 ```
 
+### Addresses
+#### Create an address
+```
+response = activecampaign_client.addresses.create_an_address(data)
+```
+
+#### Retrieve an address
+```
+response = activecampaign_client.addresses.retrieve_address(address_id="some-id")
+```
+
+#### Update an address
+```
+response = activecampaign_client.addresses.update_address(data, address_id="some-id")
+```
+
+#### Delete an address
+```
+response = activecampaign_client.addresses.delete_address(address_id="some-id")
+```
+
+#### Delete an address associated with a user group
+```
+response = activecampaign_client.addresses.delete_address_associated_with_user_group(group_id="some-id")
+```
+
+#### Delete an address associated with a list
+```
+response = activecampaign_client.addresses.delete_address_associated_with_list(list_id="some-id")
+```
+
+#### Retrieve all addresses
+```
+response = activecampaign_client.addresses.retrieve_all_addresses()
+```
+
+### Campaigns
+#### List all campaigns
+```
+response = activecampaign_client.campaigns.list_all_campaigns()
+```
+
+#### Retrieve a link associated campaign
+```
+response = activecampaign_client.campaigns.retrieve_a_link_associated_campaign(campaign_id="some-id")
+```
+
+#### Retrieve a campaign
+```
+response = activecampaign_client.campaigns.retrieve_a_campaign(campaign_id="some-id")
+```
+
+### Brandings
+#### Retrieve a branding
+```
+response = activecampaign_client.brandings.retrieve_a_branding(branding_id="some-id")
+```
+
+#### Update a branding
+```
+response = activecampaign_client.brandings.update_a_branding(data, branding_id="some-id")
+```
+
+#### List all brandings
+```
+response = activecampaign_client.brandings.list_all_brandings()
+```
+
 ## About API v1
 
 You can clone and checkout our tag v0.1.1.
 
 ```
 $ git clone https://github.com/GearPlug/activecampaign-python.git
 $ git checkout tags/v0.1.1 -b <branch_name>
```

### Comparing `activecampaign_python-1.0.8/activecampaign/client.py` & `activecampaign_python-1.0.9/activecampaign/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from .webhooks import Webhooks
 from .messages import Messages
 from .tags import Tags
 from .emailActivities import EmailActivities
 from .dealActivities import DealActivities
 from .customobjects import CustomObjects
 from .campaigns import Campaigns
+from .addresses import Addresses
+from .brandings import Brandings
 
 class Client(object):
     BASE_URL = '{}/api/3'
 
     def __init__(self, url, api_key):
         self.BASE_URL = self.BASE_URL.format(url)
         self.api_key = api_key
@@ -34,14 +36,16 @@
         self.messages = Messages(self)
         self.deepdataintegrations = DeepDataIntegrations(self)
         self.tags = Tags(self)
         self.emailActivities = EmailActivities(self)
         self.dealActivities = DealActivities(self)
         self.customobjects = CustomObjects(self)
         self.campaigns = Campaigns(self)
+        self.addresses = Addresses(self)
+        self.brandings = Brandings(self)
 
     def _get(self, endpoint, **kwargs):
         return self._request('GET', endpoint, **kwargs)
 
     def _post(self, endpoint, **kwargs):
         return self._request('POST', endpoint, **kwargs)
```

### Comparing `activecampaign_python-1.0.8/activecampaign/contacts.py` & `activecampaign_python-1.0.9/activecampaign/contacts.py`

 * *Files 18% similar despite different names*

```diff
@@ -229,28 +229,52 @@
             data:
 
         Returns:
 
         """
         return self.client._post("/fieldOption/bulk", json=data)
 
-    def create_a_custom_field_value(self):
-        raise NotImplementedError
+    def create_a_custom_field_value(self, data):
+        return self.client._post("/fieldValues", json=data)
+    
+    def retrieve_a_custom_field_value(self, field_value_id):
+        return self.client._get("/fieldValues/{}".format(field_value_id))
 
-    def retrieve_a_custom_field_value(self):
-        raise NotImplementedError
+    def update_a_custom_field_value_for_contact(self, data, field_value_id):
+         return self.client._put("/fieldValues/{}".format(field_value_id), json=data)
 
-    def update_a_custom_field_value_for_contact(self):
-        raise NotImplementedError
-
-    def delete_a_custom_field_value(self):
-        raise NotImplementedError
+    def delete_a_custom_field_value(self, field_value_id):
+        return self.client._delete("/fieldValues/{}".format(field_value_id))
 
     def list_all_custom_field_values(self):
-        raise NotImplementedError
+        return self.client._get("/fieldValues")
+    
+    def retrieve_a_contacts_field_values(self, contact_id):
+        return self.client._get("/contacts/{}/fieldValues".format(contact_id))
+    
+    def retrieve_a_contacts_tracking_logs(self, contact_id):
+        return self.client._get("/contacts/{}/trackingLogs".format(contact_id))
+    
+    def retrieve_a_contacts_data(self, contact_id):
+        return self.client._get("/contacts/{}/contactData".format(contact_id))
+    
+    def retrieve_a_contacts_bounce_logs(self, contact_id):
+        return self.client._get("/contacts/{}/bounceLogs".format(contact_id))
+    
+    def retrieve_a_contacts_geo_ips(self, contact_id):
+        return self.client._get("/contacts/{}/geoIps".format(contact_id))
+    
+    def retrieve_a_contacts_organization(self, contact_id):
+        return self.client._get("/contacts/{}/organization".format(contact_id))
+    
+    def retrieve_a_contacts_account_contacts(self, contact_id):
+        return self.client._get("/contacts/{}/accountContacts".format(contact_id))
+    
+    def retrieve_a_contacts_automation_entry_counts(self, contact_id):
+        return self.client._get("/contacts/{}/automationEntryCounts".format(contact_id))
 
     def add_a_tag_to_contact(self, data):
         """
         Add a tag to a contact
 
         :param data:
         :return:
```

### Comparing `activecampaign_python-1.0.8/activecampaign/customobjects.py` & `activecampaign_python-1.0.9/activecampaign/customobjects.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.8/activecampaign/deals.py` & `activecampaign_python-1.0.9/activecampaign/deals.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.8/activecampaign/deepdataintegrations.py` & `activecampaign_python-1.0.9/activecampaign/deepdataintegrations.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.8/activecampaign/lists.py` & `activecampaign_python-1.0.9/activecampaign/lists.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.8/activecampaign/notes.py` & `activecampaign_python-1.0.9/activecampaign/notes.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.8/activecampaign/tags.py` & `activecampaign_python-1.0.9/activecampaign/tags.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.8/activecampaign/tasks.py` & `activecampaign_python-1.0.9/activecampaign/tasks.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.8/activecampaign/users.py` & `activecampaign_python-1.0.9/activecampaign/users.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.8/activecampaign/webhooks.py` & `activecampaign_python-1.0.9/activecampaign/webhooks.py`

 * *Files identical despite different names*

### Comparing `activecampaign_python-1.0.8/PKG-INFO` & `activecampaign_python-1.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: activecampaign-python
-Version: 1.0.8
+Version: 1.0.9
 Summary: API wrapper for ActiveCampaign written in Python
 License: MIT
 Author: Miguel Ferrer
 Author-email: ingferrermiguel@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -227,14 +227,79 @@
 ```
 
 #### Retrieve field options
 ```
 response = client.contacts.retrieve_field_options("field_id")
 ```
 
+#### Create a custom field value
+```
+response = activecampaign_client.contacts.create_a_custom_field_value(data)
+```
+
+#### Retrieve a custom field value
+```
+response = activecampaign_client.contacts.retrieve_a_custom_field_value(field_value_id="some-id")
+```
+
+#### Update a custom field value for contact
+```
+response = activecampaign_client.contacts.update_a_custom_field_value_for_contact(data, field_value_id="some-id")
+```
+
+#### Delete a custom field value
+```
+response = activecampaign_client.contacts.delete_a_custom_field_value(field_value_id="some-id")
+```
+
+#### List all custom field values
+```
+response = activecampaign_client.contacts.list_all_custom_field_values()
+```
+
+#### Retrieve a contact's field values
+```
+response = activecampaign_client.contacts.retrieve_a_contacts_field_values(contact_id="some-id")
+```
+
+#### Retrieve a contact's tracking logs
+```
+response = activecampaign_client.contacts.retrieve_a_contacts_tracking_logs(contact_id="some-id")
+```
+
+#### Retrieve a contact's data
+```
+response = activecampaign_client.contacts.retrieve_a_contacts_data(contact_id="some-id")
+```
+
+#### Retrieve a contact's bounce logs
+```
+response = activecampaign_client.contacts.retrieve_a_contacts_bounce_logs(contact_id="some-id")
+```
+
+#### Retrieve a contact's geo ips
+```
+response = activecampaign_client.contacts.retrieve_a_contacts_geo_ips(contact_id="some-id")
+```
+
+#### Retrieve a contact's organization
+```
+response = activecampaign_client.contacts.retrieve_a_contacts_organization(contact_id="some-id")
+```
+
+#### Retrieve a contact's account contacts
+```
+response = activecampaign_client.contacts.retrieve_a_contacts_account_contacts(contact_id="some-id")
+```
+
+#### Retrieve a contact's automation entry counts
+```
+response = activecampaign_client.contacts.retrieve_a_contacts_automation_entry_counts(contact_id="some-id")
+```
+
 #### Add a tag to a contact
 ```
 data = {
     "contactTag": {
         "contact": "1",
         "tag": "20"
     }
@@ -790,14 +855,82 @@
 #### List all records
 ```
 response = client.customobjects.list_all_records(
         schema_id="some-id", contact_id="some-contact-id", deal_id=None, account_id=None,
         limit=20, offset=0)
 ```
 
+### Addresses
+#### Create an address
+```
+response = activecampaign_client.addresses.create_an_address(data)
+```
+
+#### Retrieve an address
+```
+response = activecampaign_client.addresses.retrieve_address(address_id="some-id")
+```
+
+#### Update an address
+```
+response = activecampaign_client.addresses.update_address(data, address_id="some-id")
+```
+
+#### Delete an address
+```
+response = activecampaign_client.addresses.delete_address(address_id="some-id")
+```
+
+#### Delete an address associated with a user group
+```
+response = activecampaign_client.addresses.delete_address_associated_with_user_group(group_id="some-id")
+```
+
+#### Delete an address associated with a list
+```
+response = activecampaign_client.addresses.delete_address_associated_with_list(list_id="some-id")
+```
+
+#### Retrieve all addresses
+```
+response = activecampaign_client.addresses.retrieve_all_addresses()
+```
+
+### Campaigns
+#### List all campaigns
+```
+response = activecampaign_client.campaigns.list_all_campaigns()
+```
+
+#### Retrieve a link associated campaign
+```
+response = activecampaign_client.campaigns.retrieve_a_link_associated_campaign(campaign_id="some-id")
+```
+
+#### Retrieve a campaign
+```
+response = activecampaign_client.campaigns.retrieve_a_campaign(campaign_id="some-id")
+```
+
+### Brandings
+#### Retrieve a branding
+```
+response = activecampaign_client.brandings.retrieve_a_branding(branding_id="some-id")
+```
+
+#### Update a branding
+```
+response = activecampaign_client.brandings.update_a_branding(data, branding_id="some-id")
+```
+
+#### List all brandings
+```
+response = activecampaign_client.brandings.list_all_brandings()
+```
+
 ## About API v1
 
 You can clone and checkout our tag v0.1.1.
 
 ```
 $ git clone https://github.com/GearPlug/activecampaign-python.git
 $ git checkout tags/v0.1.1 -b <branch_name>
```

