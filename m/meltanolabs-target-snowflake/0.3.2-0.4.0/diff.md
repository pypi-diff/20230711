# Comparing `tmp/meltanolabs_target_snowflake-0.3.2.tar.gz` & `tmp/meltanolabs_target_snowflake-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meltanolabs_target_snowflake-0.3.2.tar", max compression
+gzip compressed data, was "meltanolabs_target_snowflake-0.4.0.tar", max compression
```

## Comparing `meltanolabs_target_snowflake-0.3.2.tar` & `meltanolabs_target_snowflake-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     3860 2023-07-07 21:27:05.276414 meltanolabs_target_snowflake-0.3.2/LICENSE
--rw-r--r--   0        0        0     3924 2023-07-07 21:27:05.276414 meltanolabs_target_snowflake-0.3.2/README.md
--rw-r--r--   0        0        0     1307 2023-07-07 21:27:28.452564 meltanolabs_target_snowflake-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       89 2023-07-07 21:27:28.452564 meltanolabs_target_snowflake-0.3.2/target_snowflake/__init__.py
--rw-r--r--   0        0        0    17854 2023-07-07 21:27:05.280414 meltanolabs_target_snowflake-0.3.2/target_snowflake/connector.py
--rw-r--r--   0        0        0     8248 2023-07-07 21:27:05.280414 meltanolabs_target_snowflake-0.3.2/target_snowflake/sinks.py
--rw-r--r--   0        0        0      724 2023-07-07 21:27:05.280414 meltanolabs_target_snowflake-0.3.2/target_snowflake/snowflake_types.py
--rw-r--r--   0        0        0     2188 2023-07-07 21:27:05.280414 meltanolabs_target_snowflake-0.3.2/target_snowflake/target.py
--rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     3860 2023-07-11 20:38:24.182498 meltanolabs_target_snowflake-0.4.0/LICENSE
+-rw-r--r--   0        0        0     5010 2023-07-11 20:38:24.182498 meltanolabs_target_snowflake-0.4.0/README.md
+-rw-r--r--   0        0        0     1307 2023-07-11 20:38:47.326425 meltanolabs_target_snowflake-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       89 2023-07-11 20:38:47.330425 meltanolabs_target_snowflake-0.4.0/target_snowflake/__init__.py
+-rw-r--r--   0        0        0    19306 2023-07-11 20:38:24.182498 meltanolabs_target_snowflake-0.4.0/target_snowflake/connector.py
+-rw-r--r--   0        0        0     2651 2023-07-11 20:38:24.182498 meltanolabs_target_snowflake-0.4.0/target_snowflake/initializer.py
+-rw-r--r--   0        0        0     8248 2023-07-11 20:38:24.182498 meltanolabs_target_snowflake-0.4.0/target_snowflake/sinks.py
+-rw-r--r--   0        0        0      724 2023-07-11 20:38:24.182498 meltanolabs_target_snowflake-0.4.0/target_snowflake/snowflake_types.py
+-rw-r--r--   0        0        0     3147 2023-07-11 20:38:24.182498 meltanolabs_target_snowflake-0.4.0/target_snowflake/target.py
+-rw-r--r--   0        0        0     5804 1970-01-01 00:00:00.000000 meltanolabs_target_snowflake-0.4.0/PKG-INFO
```

### Comparing `meltanolabs_target_snowflake-0.3.2/LICENSE` & `meltanolabs_target_snowflake-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.3.2/README.md` & `meltanolabs_target_snowflake-0.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -28,14 +28,45 @@
 | stream_maps          | False    | None    | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |
 | stream_map_config    | False    | None    | User-defined config values to be used within map expressions. |
 | flattening_enabled   | False    | None    | 'True' to enable schema flattening and automatically expand nested properties. |
 | flattening_max_depth | False    | None    | The max depth to flatten schemas. |
 
 A full list of supported settings and capabilities is available by running: `target-snowflake --about`
 
+### Initializing a Snowflake Account
+
+This target has an interactive feature that will help you get a Snowflake account initialized with everything needed to get started loading data.
+
+- User
+- Role
+- Warehouse
+- Database
+- Proper grants
+
+The CLI will ask you to provide information about the new user/role/etc. you want to create but it will also need SYSADMIN credentials to execute the queries.
+You should prepare the following inputs:
+
+- Account
+- User that has SYSADMIN and SECURITYADMIN access. These comes default with the user that created the Snowflake account.
+- The password for your SYSADMIN user.
+
+Run the following command to get started with the interactive CLI.
+Note - the CLI will print the SQL queries it is planning to run and confirm with you before it makes any changes.
+
+```bash
+poetry run target-snowflake --initialize
+
+# Alternatively using Meltano CLI
+meltano invoke target-snowflake --initialize
+```
+
+The CLI also has a "dry run" mode that will print the queries without executing them.
+
+Check out the demo of this [on YouTube](https://youtu.be/9vEFxw-0nxI).
+
 ### Configure using environment variables
 
 This Singer target will automatically import any environment variables within the working directory's
 `.env` if the `--config=ENV` is provided, such that config values will be considered if a matching
 environment variable is set either in the terminal context or in the `.env` file.
 
 ## Usage
```

### Comparing `meltanolabs_target_snowflake-0.3.2/pyproject.toml` & `meltanolabs_target_snowflake-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "meltanolabs-target-snowflake"
-version = "0.3.2"
+version = "0.4.0"
 description = "`target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets."
 readme = "README.md"
 authors = ["Ken Payne"]
 keywords = [
     "ELT",
     "Snowflake",
 ]
```

### Comparing `meltanolabs_target_snowflake-0.3.2/target_snowflake/connector.py` & `meltanolabs_target_snowflake-0.4.0/target_snowflake/connector.py`

 * *Files 8% similar despite different names*

```diff
@@ -457,7 +457,56 @@
         """
         with self._connect() as conn:
             remove_statement, kwargs = self._get_stage_files_remove_statement(
                 sync_id=sync_id
             )
             self.logger.debug(f"Removing staged files with SQL: {remove_statement!s}")
             conn.execute(remove_statement, **kwargs)
+
+    @staticmethod
+    def get_initialize_script(role, user, password, warehouse, database):
+        # https://fivetran.com/docs/destinations/snowflake/setup-guide
+        return f"""
+            begin;
+
+            -- change role to securityadmin for user / role steps
+            use role securityadmin;
+
+            -- create role
+            create role if not exists {role};
+            grant role {role} to role SYSADMIN;
+
+            -- create a user
+            create user if not exists {user}
+            password = '{password}'
+            default_role = {role}
+            default_warehouse = {warehouse};
+
+            grant role {role} to user {user};
+
+            -- change role to sysadmin for warehouse / database steps
+            use role sysadmin;
+
+            -- create a warehouse
+            create warehouse if not exists {warehouse}
+            warehouse_size = xsmall
+            warehouse_type = standard
+            auto_suspend = 60
+            auto_resume = true
+            initially_suspended = true;
+
+            -- create database
+            create database if not exists {database};
+
+            -- grant role access to warehouse
+            grant USAGE
+            on warehouse {warehouse}
+            to role {role};
+
+            -- grant access to database
+            grant CREATE SCHEMA, MONITOR, USAGE
+            on database {database}
+            to role {role};
+            
+            commit;
+
+        """
```

### Comparing `meltanolabs_target_snowflake-0.3.2/target_snowflake/sinks.py` & `meltanolabs_target_snowflake-0.4.0/target_snowflake/sinks.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.3.2/target_snowflake/snowflake_types.py` & `meltanolabs_target_snowflake-0.4.0/target_snowflake/snowflake_types.py`

 * *Files identical despite different names*

### Comparing `meltanolabs_target_snowflake-0.3.2/PKG-INFO` & `meltanolabs_target_snowflake-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meltanolabs-target-snowflake
-Version: 0.3.2
+Version: 0.4.0
 Summary: `target-snowflake` is a Singer target for Snowflake, built with the Meltano SDK for Singer Targets.
 License: Apache 2.0
 Keywords: ELT,Snowflake
 Author: Ken Payne
 Requires-Python: >=3.7.1,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -48,14 +48,45 @@
 | stream_maps          | False    | None    | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |
 | stream_map_config    | False    | None    | User-defined config values to be used within map expressions. |
 | flattening_enabled   | False    | None    | 'True' to enable schema flattening and automatically expand nested properties. |
 | flattening_max_depth | False    | None    | The max depth to flatten schemas. |
 
 A full list of supported settings and capabilities is available by running: `target-snowflake --about`
 
+### Initializing a Snowflake Account
+
+This target has an interactive feature that will help you get a Snowflake account initialized with everything needed to get started loading data.
+
+- User
+- Role
+- Warehouse
+- Database
+- Proper grants
+
+The CLI will ask you to provide information about the new user/role/etc. you want to create but it will also need SYSADMIN credentials to execute the queries.
+You should prepare the following inputs:
+
+- Account
+- User that has SYSADMIN and SECURITYADMIN access. These comes default with the user that created the Snowflake account.
+- The password for your SYSADMIN user.
+
+Run the following command to get started with the interactive CLI.
+Note - the CLI will print the SQL queries it is planning to run and confirm with you before it makes any changes.
+
+```bash
+poetry run target-snowflake --initialize
+
+# Alternatively using Meltano CLI
+meltano invoke target-snowflake --initialize
+```
+
+The CLI also has a "dry run" mode that will print the queries without executing them.
+
+Check out the demo of this [on YouTube](https://youtu.be/9vEFxw-0nxI).
+
 ### Configure using environment variables
 
 This Singer target will automatically import any environment variables within the working directory's
 `.env` if the `--config=ENV` is provided, such that config values will be considered if a matching
 environment variable is set either in the terminal context or in the `.env` file.
 
 ## Usage
```

