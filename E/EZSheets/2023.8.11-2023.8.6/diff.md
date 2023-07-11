# Comparing `tmp/EZSheets-2023.8.11.tar.gz` & `tmp/EZSheets-2023.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\EZSheets-2023.8.11.tar", last modified: Tue Jul 11 17:19:52 2023, max compression
+gzip compressed data, was "dist\EZSheets-2023.8.6.tar", last modified: Thu Jul  6 21:45:15 2023, max compression
```

## Comparing `EZSheets-2023.8.11.tar` & `EZSheets-2023.8.6.tar`

### file list

```diff
@@ -1,22 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-07-11 17:19:52.000000 EZSheets-2023.8.11/
--rw-rw-rw-   0        0        0      164 2020-08-04 06:42:17.000000 EZSheets-2023.8.11/AUTHORS.txt
--rw-rw-rw-   0        0        0    35821 2019-02-08 06:36:15.000000 EZSheets-2023.8.11/LICENSE.txt
--rw-rw-rw-   0        0        0       19 2019-02-08 06:36:15.000000 EZSheets-2023.8.11/MANIFEST.in
--rw-rw-rw-   0        0        0    12476 2023-07-11 17:19:52.000000 EZSheets-2023.8.11/PKG-INFO
--rw-rw-rw-   0        0        0    11509 2023-07-07 15:11:55.000000 EZSheets-2023.8.11/README.md
--rw-rw-rw-   0        0        0       34 2023-04-25 17:29:09.000000 EZSheets-2023.8.11/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-11 17:19:52.000000 EZSheets-2023.8.11/setup.cfg
--rw-rw-rw-   0        0        0     1664 2023-07-07 20:30:00.000000 EZSheets-2023.8.11/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:19:52.000000 EZSheets-2023.8.11/src/
-drwxrwxrwx   0        0        0        0 2023-07-11 17:19:52.000000 EZSheets-2023.8.11/src/EZSheets.egg-info/
--rw-rw-rw-   0        0        0    12476 2023-07-11 17:19:52.000000 EZSheets-2023.8.11/src/EZSheets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-07-11 17:19:52.000000 EZSheets-2023.8.11/src/EZSheets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-11 17:19:52.000000 EZSheets-2023.8.11/src/EZSheets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-07-11 17:19:52.000000 EZSheets-2023.8.11/src/EZSheets.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-11 17:19:52.000000 EZSheets-2023.8.11/src/EZSheets.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-11 17:19:52.000000 EZSheets-2023.8.11/src/ezsheets/
--rw-rw-rw-   0        0        0    82511 2023-07-11 17:19:37.000000 EZSheets-2023.8.11/src/ezsheets/__init__.py
--rw-rw-rw-   0        0        0     6293 2023-04-25 17:21:45.000000 EZSheets-2023.8.11/src/ezsheets/colorvalues.py
-drwxrwxrwx   0        0        0        0 2023-07-11 17:19:52.000000 EZSheets-2023.8.11/tests/
--rw-rw-rw-   0        0        0    19970 2023-07-09 16:54:39.000000 EZSheets-2023.8.11/tests/test_automate2nded.py
--rw-rw-rw-   0        0        0    32826 2023-07-11 16:48:20.000000 EZSheets-2023.8.11/tests/test_ezsheets.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/
+-rw-rw-rw-   0        0        0      164 2020-08-04 06:42:17.000000 EZSheets-2023.8.6/AUTHORS.txt
+-rw-rw-rw-   0        0        0    35821 2019-02-08 06:36:15.000000 EZSheets-2023.8.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       19 2019-02-08 06:36:15.000000 EZSheets-2023.8.6/MANIFEST.in
+-rw-rw-rw-   0        0        0    12278 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11312 2023-07-06 21:41:59.000000 EZSheets-2023.8.6/README.md
+-rw-rw-rw-   0        0        0       34 2023-04-25 17:29:09.000000 EZSheets-2023.8.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/setup.cfg
+-rw-rw-rw-   0        0        0     1632 2022-10-10 19:12:14.000000 EZSheets-2023.8.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/src/
+drwxrwxrwx   0        0        0        0 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/src/EZSheets.egg-info/
+-rw-rw-rw-   0        0        0    12278 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/src/EZSheets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      324 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/src/EZSheets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/src/EZSheets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/src/EZSheets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/src/EZSheets.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/src/ezsheets/
+-rw-rw-rw-   0        0        0    79498 2023-07-06 21:41:31.000000 EZSheets-2023.8.6/src/ezsheets/__init__.py
+-rw-rw-rw-   0        0        0     6293 2023-04-25 17:21:45.000000 EZSheets-2023.8.6/src/ezsheets/colorvalues.py
+drwxrwxrwx   0        0        0        0 2023-07-06 21:45:15.000000 EZSheets-2023.8.6/tests/
+-rw-rw-rw-   0        0        0    31821 2023-07-06 20:09:52.000000 EZSheets-2023.8.6/tests/test_ezsheets.py
```

### Comparing `EZSheets-2023.8.11/LICENSE.txt` & `EZSheets-2023.8.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EZSheets-2023.8.11/PKG-INFO` & `EZSheets-2023.8.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EZSheets
-Version: 2023.8.11
+Version: 2023.8.6
 Summary: A Pythonic interface to the Google Sheets API that actually works as of July 2023.
 Home-page: https://github.com/asweigart/ezsheets
 Author: Al Sweigart
 Author-email: al@inventwithpython.com
 License: GPLv3+
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
@@ -28,35 +28,27 @@
 
 ## Installation and Setup
 
 To install with pip, run:
 
     pip install ezsheets
 
-For your Python script to use EZSheets to access and edit your Google Sheets spreadsheets, you need a credentials JSON file and a token JSON file. If you have a Google/Gmail account, you can do this and it is free. I strongly recommend creating a new Google account instead of using your existing one, to prevent a bug in your Python script from affecting the spreadsheets in your personal Google account. There are five parts to creating credentials:
-
-1. Create a new Google Cloud project.
-2. Enable the Google Sheets API and Google Drive API for your project.
-3. Configure the OAuth Consent Screen for your project.
-4. Create credentials for your project.
-5. Log in with the credentials file.
-
-This may seem like a lot of work, but you only have to perform this setup once.
+For your Python script to use ezsheets to access and edit your Google Sheets spreadsheets, you need a credentials JSON file and a token JSON file. This requires a one-time set up on Google Cloud services using your Google account. If you have a Google/Gmail account, you can do this and it is free (unless you are making large use of the Google Sheets API by sending out thousands of emails every day.) There's several steps to this, detailed in the following sections. These instructions were last updated September 2022.
 
 ### Create a new Google Cloud Project
 
-First, you need to set up a Google Cloud project. In your browser, go to https://console.cloud.google.com and sign in to your Google account with your username and password. (Your app can connect to any Google account, but this Google account will manage the Google API access for EZSheets.) You will be taken to a Getting Started page. At the top of the page, click on "Select a project". In the pop-up window that appears, click "New Project".
+First, you need to set up a Google Cloud project. In your browser, go to https://console.cloud.google.com and sign in to you Google account with your username and password. (Your app can connect to any Google account, but this Google account will be one that manages the Google API access for EZSheets.) You will be taken to a Getting Started page. At the top of the page, click on "Select a project". In the pop-up window that appears, click "New Project".
 
 ![Navigate to new project](google-cloud-new-project.png)
 
-This takes you to a new project page. A Project Name like "My Project 23135" will be generated for you. There is also a Project ID like "macro-nuance-362516" randomly generated for you. These names won't be visible to users of your Python scripts and you can use whatever name you want. You can change the Project Name later but not the Project ID. I just use the default names that the website generates for me. You can leave the Location as "No organization". Free Google accounts can have up to 12 projects but you only need one project for all the Python scripts that you want to create. Click the blue "CREATE" button to create the project.
+This takes to a new project page. A Project Name like "My Project 23135" will be generated for you. There is also a Project ID like "macro-nuance-362516" randomly generated for you. These names won't be visible to users of your Python scripts and you can use whatever name you want. You can change the Project Name later but not the Project ID. I just use the default names that are generated for me. The Location can be left as "No organization". Note that at the free tier, you can only create 12 projects (as of September 2022) but you only need one for all the Python scripts that you want to create. Click the blue "CREATE" button to create the project.
 
 ![Create a new project](create-new-project.png)
 
-
+Free Google accounts can have up to 10 projects.
 
 Click on "Select a project" at the top of the page again, and select the project you just created. You will be taken to the dashboard page for this Google Cloud Project. Next, you need to enable the Google Sheets API and Google Drive API for your project.
 
 ### Enable the Google Sheets API and Google Drive API for Your Project
 
 On the https://console.cloud.google.com page, click on the Navigation button in the upper left (the icon is three horizontal stripes, often called the "hamburger" icon.) Navigate to "APIs & Services" and then "Library" to go to the API Library page. There are many Google APIs for Gmail, Google Maps, Google Cloud Storage, and other Google services. We need to allow our project to use the Google Sheets and Google Drive APIs.
 
@@ -66,39 +58,39 @@
 
 Next, you need to configure your project's OAuth Consent Screen.
 
 ### Configure the OAuth Consent Screen for Your Project
 
 Click on the Navigation button in the upper left and then navigate to "APIs & Services" and then "OAuth Consent Screen." The consent screen will appear the first time when you or users of your Python script use EZSheets. With a free Google account that is not set up as a Google Workspace user, you'll have to select the External User Type option instead of Internal User Type. These are further explained on Google's [Setting up your OAuth consent screen help page](https://support.google.com/cloud/answer/10311615).
 
-On Step 1 "OAuth consent screen", select External and click the blue "CREATE" button. The next page shows what the OAuth consent screen looks like. This screen appears to the user when they first import the ezsheets module. Pick a name for App Name (I use something generic like Python Google API Script) and enter your email address for the User Support Email and Developer Contact Information. Then click the "SAVE AND CONTINUE" button.
+On Step 1 "OAuth consent screen", select External and click the blue "CREATE" button. You'll be taken to a page where you set up what the OAuth consent screen looks like. This screen appears to the user when they first import the ezsheets module. Pick a name for App Name (I use something generic like Python Google API Script) and enter your email address for the User Support Email and Developer Contact Information. Then click "SAVE AND CONTINUE."
 
-On Step 2 "Scopes", your projects' scopes are the permissions for what the project is allowed to access. Click the "ADD OR REMOVE SCOPES" button, and in the new panel that appears, go through the table and check the checkboxes for the scopes `.../auth/drive` (Google Drive API) and `.../auth/spreadsheets` (Google Sheets API) and click the blue "UPDATE" button. Then click "SAVE AND CONTINUE."
+Step 2 "Scopes" involves adding your projects' scopes, which is a term Google chose for "permissions." Click the "ADD OR REMOVE SCOPES" button, and in the new panel that appears, go through the table and check the checkboxes for the scopes `.../auth/drive` (Google Drive API) and `.../auth/spreadsheets` (Google Sheets API) and click the blue "UPDATE" button. Then click "SAVE AND CONTINUE."
 
-Step 3 "Test users" requires you to add the Gmail email addresses of the Google accounts that own the spreadsheets your Python script will interact with. Without going through Google's app approval process, your scripts are limited to interacting with the email addresses you provide in this step. Click the "+ ADD USERS" button and in the new panel that appears, enter the Gmail address of your Google account and click the blue "ADD" button. Then click "SAVE AND CONTINUE."
+Step 3 "Test users" requires you to add the Gmail email addresses of the Google accounts that own the spreadsheets your Python script will interact with. Without going through Google's app approval process, your scripts will be limited to interacting with the email addresses you provide in this step. Click the "+ ADD USERS" button and in the new panel that appears, enter the Gmail addresses and click the blue "ADD" button. Then click "SAVE AND CONTINUE."
 
 Step 4 "Summary" provides a summary of the previous steps. If all the information looks right, click the "BACK TO DASHBOARD" button. The next step is to create credentials for your project.
 
 ### Create Credentials for Your Project
 
 From the Navigation sidebar menu, click on "APIs & Services" and then "Credentials" to go to the Credentials page. Click the "+ CREATE CREDENTIALS" link at the top of the page. A submenu will open asking what kind of credentials you want to create: "API key", "OAuth client ID", or "Service account". Click on "OAuth client ID".
 
 ![Create credentials](create-credentials.png)
 
 On the new page that appears, select "Desktop app" for the "Application type" and leave "Name" as the default "Desktop client 1." (You can change this to a different name if you want, it doesn't appear to the users of your Python script.) Click the blue "CREATE" button.
 
-On the pop up that appears, click "DOWNLOAD JSON" to download the credentials file. This credentials JSON file will have a name like *client_secret_282792235794-p2o9gfcub4htibfg2u207gcomco9nqm7.apps.googleusercontent.com.json*. Place it in the same folder that your Python script will be in.
+The pop up that appears shows your , click "DOWNLOAD JSON" to download the credentials file. This file will have a name like *client_secret_282792235794-p2o9gfcub4htibfg2u207gcomco9nqm7.apps.googleusercontent.com.json*. Rename it to *credentials-sheets.json* and place it in the same folder that your Python script will be in.
 
 ### Log In with the Credentials File
 
-Run the Python interactive shell from the same folder that the credentials JSON file is in and run `import ezsheets`. Or, place a *.py* Python program in this folder and have it run `import ezsheets`. EZSheets will load and automatically check this folder for a credentials JSON file and, if found, launches your web browser to the OAuth consent screen. Sign in with the Google account you want to access from your Python script. This must be the same email address that you gave for the "test user" when configuring the Google Cloud project's OAuth consent screen.
+Run the Python interactive shell from the same folder that the *credentials-sheets.json* file is in and run `import ezsheets`. Or, place a *.py* Python program in this folder and have it run `import ezsheets`. EZSheets will load and automatically check this folder for a *credentials-sheets.json* file and, if found, launches your web browser to the OAuth consent screen. Sign in with the Google account you want to access from your Python script. This must be the same email address that you gave for the "test user" when configuring the Google Cloud project's OAuth consent screen.
 
 You will get a warning message that reads "Google hasn't verified this app," but that's fine because this is the app (or project) that you've just created yourself. Click the Continue link. You'll come to another page that says "Python Google API Script wants access to your Google Account" (or whatever name you gave in the OAuth consent screen setup.) Click Continue.
 
-You'll come to a plain web page that says, "The authentication flow has completed." You can now close the browser window. In the same folder as your credentials JSON file, you'll now see a *token-drive.pickle* and *token-sheets.pickle* file. Treat these files like passwords and do not share them: they can be used to log in and access your Google Sheets spreadsheets.
+You'll come to a plain web page that says, "The authentication flow has completed." You can now close the browser window. In the same folder as your *credentials-sheets.json* file, you'll now see a *token.json* file. Do not share these files: they can be used to log in and access your Google Sheets spreadsheets.
 
 ## Quickstart Guide
 
 After you've set up your credentials and token files, you can import EZSheets to access your Google Sheets. Create a `Spreadsheet` object by using the Spreadsheet's URL:
 
     >>> import ezsheets
     >>> s = ezsheets.Spreadsheet('https://docs.google.com/spreadsheets/d/16RWH9XBBwd8pRYZDSo9EontzdVPqxdGnwM5MnP6T48c/edit#gid=0')
```

### Comparing `EZSheets-2023.8.11/README.md` & `EZSheets-2023.8.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,35 +5,27 @@
 
 ## Installation and Setup
 
 To install with pip, run:
 
     pip install ezsheets
 
-For your Python script to use EZSheets to access and edit your Google Sheets spreadsheets, you need a credentials JSON file and a token JSON file. If you have a Google/Gmail account, you can do this and it is free. I strongly recommend creating a new Google account instead of using your existing one, to prevent a bug in your Python script from affecting the spreadsheets in your personal Google account. There are five parts to creating credentials:
-
-1. Create a new Google Cloud project.
-2. Enable the Google Sheets API and Google Drive API for your project.
-3. Configure the OAuth Consent Screen for your project.
-4. Create credentials for your project.
-5. Log in with the credentials file.
-
-This may seem like a lot of work, but you only have to perform this setup once.
+For your Python script to use ezsheets to access and edit your Google Sheets spreadsheets, you need a credentials JSON file and a token JSON file. This requires a one-time set up on Google Cloud services using your Google account. If you have a Google/Gmail account, you can do this and it is free (unless you are making large use of the Google Sheets API by sending out thousands of emails every day.) There's several steps to this, detailed in the following sections. These instructions were last updated September 2022.
 
 ### Create a new Google Cloud Project
 
-First, you need to set up a Google Cloud project. In your browser, go to https://console.cloud.google.com and sign in to your Google account with your username and password. (Your app can connect to any Google account, but this Google account will manage the Google API access for EZSheets.) You will be taken to a Getting Started page. At the top of the page, click on "Select a project". In the pop-up window that appears, click "New Project".
+First, you need to set up a Google Cloud project. In your browser, go to https://console.cloud.google.com and sign in to you Google account with your username and password. (Your app can connect to any Google account, but this Google account will be one that manages the Google API access for EZSheets.) You will be taken to a Getting Started page. At the top of the page, click on "Select a project". In the pop-up window that appears, click "New Project".
 
 ![Navigate to new project](google-cloud-new-project.png)
 
-This takes you to a new project page. A Project Name like "My Project 23135" will be generated for you. There is also a Project ID like "macro-nuance-362516" randomly generated for you. These names won't be visible to users of your Python scripts and you can use whatever name you want. You can change the Project Name later but not the Project ID. I just use the default names that the website generates for me. You can leave the Location as "No organization". Free Google accounts can have up to 12 projects but you only need one project for all the Python scripts that you want to create. Click the blue "CREATE" button to create the project.
+This takes to a new project page. A Project Name like "My Project 23135" will be generated for you. There is also a Project ID like "macro-nuance-362516" randomly generated for you. These names won't be visible to users of your Python scripts and you can use whatever name you want. You can change the Project Name later but not the Project ID. I just use the default names that are generated for me. The Location can be left as "No organization". Note that at the free tier, you can only create 12 projects (as of September 2022) but you only need one for all the Python scripts that you want to create. Click the blue "CREATE" button to create the project.
 
 ![Create a new project](create-new-project.png)
 
-
+Free Google accounts can have up to 10 projects.
 
 Click on "Select a project" at the top of the page again, and select the project you just created. You will be taken to the dashboard page for this Google Cloud Project. Next, you need to enable the Google Sheets API and Google Drive API for your project.
 
 ### Enable the Google Sheets API and Google Drive API for Your Project
 
 On the https://console.cloud.google.com page, click on the Navigation button in the upper left (the icon is three horizontal stripes, often called the "hamburger" icon.) Navigate to "APIs & Services" and then "Library" to go to the API Library page. There are many Google APIs for Gmail, Google Maps, Google Cloud Storage, and other Google services. We need to allow our project to use the Google Sheets and Google Drive APIs.
 
@@ -43,39 +35,39 @@
 
 Next, you need to configure your project's OAuth Consent Screen.
 
 ### Configure the OAuth Consent Screen for Your Project
 
 Click on the Navigation button in the upper left and then navigate to "APIs & Services" and then "OAuth Consent Screen." The consent screen will appear the first time when you or users of your Python script use EZSheets. With a free Google account that is not set up as a Google Workspace user, you'll have to select the External User Type option instead of Internal User Type. These are further explained on Google's [Setting up your OAuth consent screen help page](https://support.google.com/cloud/answer/10311615).
 
-On Step 1 "OAuth consent screen", select External and click the blue "CREATE" button. The next page shows what the OAuth consent screen looks like. This screen appears to the user when they first import the ezsheets module. Pick a name for App Name (I use something generic like Python Google API Script) and enter your email address for the User Support Email and Developer Contact Information. Then click the "SAVE AND CONTINUE" button.
+On Step 1 "OAuth consent screen", select External and click the blue "CREATE" button. You'll be taken to a page where you set up what the OAuth consent screen looks like. This screen appears to the user when they first import the ezsheets module. Pick a name for App Name (I use something generic like Python Google API Script) and enter your email address for the User Support Email and Developer Contact Information. Then click "SAVE AND CONTINUE."
 
-On Step 2 "Scopes", your projects' scopes are the permissions for what the project is allowed to access. Click the "ADD OR REMOVE SCOPES" button, and in the new panel that appears, go through the table and check the checkboxes for the scopes `.../auth/drive` (Google Drive API) and `.../auth/spreadsheets` (Google Sheets API) and click the blue "UPDATE" button. Then click "SAVE AND CONTINUE."
+Step 2 "Scopes" involves adding your projects' scopes, which is a term Google chose for "permissions." Click the "ADD OR REMOVE SCOPES" button, and in the new panel that appears, go through the table and check the checkboxes for the scopes `.../auth/drive` (Google Drive API) and `.../auth/spreadsheets` (Google Sheets API) and click the blue "UPDATE" button. Then click "SAVE AND CONTINUE."
 
-Step 3 "Test users" requires you to add the Gmail email addresses of the Google accounts that own the spreadsheets your Python script will interact with. Without going through Google's app approval process, your scripts are limited to interacting with the email addresses you provide in this step. Click the "+ ADD USERS" button and in the new panel that appears, enter the Gmail address of your Google account and click the blue "ADD" button. Then click "SAVE AND CONTINUE."
+Step 3 "Test users" requires you to add the Gmail email addresses of the Google accounts that own the spreadsheets your Python script will interact with. Without going through Google's app approval process, your scripts will be limited to interacting with the email addresses you provide in this step. Click the "+ ADD USERS" button and in the new panel that appears, enter the Gmail addresses and click the blue "ADD" button. Then click "SAVE AND CONTINUE."
 
 Step 4 "Summary" provides a summary of the previous steps. If all the information looks right, click the "BACK TO DASHBOARD" button. The next step is to create credentials for your project.
 
 ### Create Credentials for Your Project
 
 From the Navigation sidebar menu, click on "APIs & Services" and then "Credentials" to go to the Credentials page. Click the "+ CREATE CREDENTIALS" link at the top of the page. A submenu will open asking what kind of credentials you want to create: "API key", "OAuth client ID", or "Service account". Click on "OAuth client ID".
 
 ![Create credentials](create-credentials.png)
 
 On the new page that appears, select "Desktop app" for the "Application type" and leave "Name" as the default "Desktop client 1." (You can change this to a different name if you want, it doesn't appear to the users of your Python script.) Click the blue "CREATE" button.
 
-On the pop up that appears, click "DOWNLOAD JSON" to download the credentials file. This credentials JSON file will have a name like *client_secret_282792235794-p2o9gfcub4htibfg2u207gcomco9nqm7.apps.googleusercontent.com.json*. Place it in the same folder that your Python script will be in.
+The pop up that appears shows your , click "DOWNLOAD JSON" to download the credentials file. This file will have a name like *client_secret_282792235794-p2o9gfcub4htibfg2u207gcomco9nqm7.apps.googleusercontent.com.json*. Rename it to *credentials-sheets.json* and place it in the same folder that your Python script will be in.
 
 ### Log In with the Credentials File
 
-Run the Python interactive shell from the same folder that the credentials JSON file is in and run `import ezsheets`. Or, place a *.py* Python program in this folder and have it run `import ezsheets`. EZSheets will load and automatically check this folder for a credentials JSON file and, if found, launches your web browser to the OAuth consent screen. Sign in with the Google account you want to access from your Python script. This must be the same email address that you gave for the "test user" when configuring the Google Cloud project's OAuth consent screen.
+Run the Python interactive shell from the same folder that the *credentials-sheets.json* file is in and run `import ezsheets`. Or, place a *.py* Python program in this folder and have it run `import ezsheets`. EZSheets will load and automatically check this folder for a *credentials-sheets.json* file and, if found, launches your web browser to the OAuth consent screen. Sign in with the Google account you want to access from your Python script. This must be the same email address that you gave for the "test user" when configuring the Google Cloud project's OAuth consent screen.
 
 You will get a warning message that reads "Google hasn't verified this app," but that's fine because this is the app (or project) that you've just created yourself. Click the Continue link. You'll come to another page that says "Python Google API Script wants access to your Google Account" (or whatever name you gave in the OAuth consent screen setup.) Click Continue.
 
-You'll come to a plain web page that says, "The authentication flow has completed." You can now close the browser window. In the same folder as your credentials JSON file, you'll now see a *token-drive.pickle* and *token-sheets.pickle* file. Treat these files like passwords and do not share them: they can be used to log in and access your Google Sheets spreadsheets.
+You'll come to a plain web page that says, "The authentication flow has completed." You can now close the browser window. In the same folder as your *credentials-sheets.json* file, you'll now see a *token.json* file. Do not share these files: they can be used to log in and access your Google Sheets spreadsheets.
 
 ## Quickstart Guide
 
 After you've set up your credentials and token files, you can import EZSheets to access your Google Sheets. Create a `Spreadsheet` object by using the Spreadsheet's URL:
 
     >>> import ezsheets
     >>> s = ezsheets.Spreadsheet('https://docs.google.com/spreadsheets/d/16RWH9XBBwd8pRYZDSo9EontzdVPqxdGnwM5MnP6T48c/edit#gid=0')
```

### Comparing `EZSheets-2023.8.11/setup.py` & `EZSheets-2023.8.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     description=description,
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='GPLv3+',
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     test_suite='tests',
-    install_requires=['google-api-python-client', 'google-auth-httplib2', 'google-auth-oauthlib'],
+    install_requires=['google-api-python-client', 'oauth2client'],
     keywords='',
     classifiers=[
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.4',
         'Programming Language :: Python :: 3.5',
```

### Comparing `EZSheets-2023.8.11/src/EZSheets.egg-info/PKG-INFO` & `EZSheets-2023.8.6/src/EZSheets.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EZSheets
-Version: 2023.8.11
+Version: 2023.8.6
 Summary: A Pythonic interface to the Google Sheets API that actually works as of July 2023.
 Home-page: https://github.com/asweigart/ezsheets
 Author: Al Sweigart
 Author-email: al@inventwithpython.com
 License: GPLv3+
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python
@@ -28,35 +28,27 @@
 
 ## Installation and Setup
 
 To install with pip, run:
 
     pip install ezsheets
 
-For your Python script to use EZSheets to access and edit your Google Sheets spreadsheets, you need a credentials JSON file and a token JSON file. If you have a Google/Gmail account, you can do this and it is free. I strongly recommend creating a new Google account instead of using your existing one, to prevent a bug in your Python script from affecting the spreadsheets in your personal Google account. There are five parts to creating credentials:
-
-1. Create a new Google Cloud project.
-2. Enable the Google Sheets API and Google Drive API for your project.
-3. Configure the OAuth Consent Screen for your project.
-4. Create credentials for your project.
-5. Log in with the credentials file.
-
-This may seem like a lot of work, but you only have to perform this setup once.
+For your Python script to use ezsheets to access and edit your Google Sheets spreadsheets, you need a credentials JSON file and a token JSON file. This requires a one-time set up on Google Cloud services using your Google account. If you have a Google/Gmail account, you can do this and it is free (unless you are making large use of the Google Sheets API by sending out thousands of emails every day.) There's several steps to this, detailed in the following sections. These instructions were last updated September 2022.
 
 ### Create a new Google Cloud Project
 
-First, you need to set up a Google Cloud project. In your browser, go to https://console.cloud.google.com and sign in to your Google account with your username and password. (Your app can connect to any Google account, but this Google account will manage the Google API access for EZSheets.) You will be taken to a Getting Started page. At the top of the page, click on "Select a project". In the pop-up window that appears, click "New Project".
+First, you need to set up a Google Cloud project. In your browser, go to https://console.cloud.google.com and sign in to you Google account with your username and password. (Your app can connect to any Google account, but this Google account will be one that manages the Google API access for EZSheets.) You will be taken to a Getting Started page. At the top of the page, click on "Select a project". In the pop-up window that appears, click "New Project".
 
 ![Navigate to new project](google-cloud-new-project.png)
 
-This takes you to a new project page. A Project Name like "My Project 23135" will be generated for you. There is also a Project ID like "macro-nuance-362516" randomly generated for you. These names won't be visible to users of your Python scripts and you can use whatever name you want. You can change the Project Name later but not the Project ID. I just use the default names that the website generates for me. You can leave the Location as "No organization". Free Google accounts can have up to 12 projects but you only need one project for all the Python scripts that you want to create. Click the blue "CREATE" button to create the project.
+This takes to a new project page. A Project Name like "My Project 23135" will be generated for you. There is also a Project ID like "macro-nuance-362516" randomly generated for you. These names won't be visible to users of your Python scripts and you can use whatever name you want. You can change the Project Name later but not the Project ID. I just use the default names that are generated for me. The Location can be left as "No organization". Note that at the free tier, you can only create 12 projects (as of September 2022) but you only need one for all the Python scripts that you want to create. Click the blue "CREATE" button to create the project.
 
 ![Create a new project](create-new-project.png)
 
-
+Free Google accounts can have up to 10 projects.
 
 Click on "Select a project" at the top of the page again, and select the project you just created. You will be taken to the dashboard page for this Google Cloud Project. Next, you need to enable the Google Sheets API and Google Drive API for your project.
 
 ### Enable the Google Sheets API and Google Drive API for Your Project
 
 On the https://console.cloud.google.com page, click on the Navigation button in the upper left (the icon is three horizontal stripes, often called the "hamburger" icon.) Navigate to "APIs & Services" and then "Library" to go to the API Library page. There are many Google APIs for Gmail, Google Maps, Google Cloud Storage, and other Google services. We need to allow our project to use the Google Sheets and Google Drive APIs.
 
@@ -66,39 +58,39 @@
 
 Next, you need to configure your project's OAuth Consent Screen.
 
 ### Configure the OAuth Consent Screen for Your Project
 
 Click on the Navigation button in the upper left and then navigate to "APIs & Services" and then "OAuth Consent Screen." The consent screen will appear the first time when you or users of your Python script use EZSheets. With a free Google account that is not set up as a Google Workspace user, you'll have to select the External User Type option instead of Internal User Type. These are further explained on Google's [Setting up your OAuth consent screen help page](https://support.google.com/cloud/answer/10311615).
 
-On Step 1 "OAuth consent screen", select External and click the blue "CREATE" button. The next page shows what the OAuth consent screen looks like. This screen appears to the user when they first import the ezsheets module. Pick a name for App Name (I use something generic like Python Google API Script) and enter your email address for the User Support Email and Developer Contact Information. Then click the "SAVE AND CONTINUE" button.
+On Step 1 "OAuth consent screen", select External and click the blue "CREATE" button. You'll be taken to a page where you set up what the OAuth consent screen looks like. This screen appears to the user when they first import the ezsheets module. Pick a name for App Name (I use something generic like Python Google API Script) and enter your email address for the User Support Email and Developer Contact Information. Then click "SAVE AND CONTINUE."
 
-On Step 2 "Scopes", your projects' scopes are the permissions for what the project is allowed to access. Click the "ADD OR REMOVE SCOPES" button, and in the new panel that appears, go through the table and check the checkboxes for the scopes `.../auth/drive` (Google Drive API) and `.../auth/spreadsheets` (Google Sheets API) and click the blue "UPDATE" button. Then click "SAVE AND CONTINUE."
+Step 2 "Scopes" involves adding your projects' scopes, which is a term Google chose for "permissions." Click the "ADD OR REMOVE SCOPES" button, and in the new panel that appears, go through the table and check the checkboxes for the scopes `.../auth/drive` (Google Drive API) and `.../auth/spreadsheets` (Google Sheets API) and click the blue "UPDATE" button. Then click "SAVE AND CONTINUE."
 
-Step 3 "Test users" requires you to add the Gmail email addresses of the Google accounts that own the spreadsheets your Python script will interact with. Without going through Google's app approval process, your scripts are limited to interacting with the email addresses you provide in this step. Click the "+ ADD USERS" button and in the new panel that appears, enter the Gmail address of your Google account and click the blue "ADD" button. Then click "SAVE AND CONTINUE."
+Step 3 "Test users" requires you to add the Gmail email addresses of the Google accounts that own the spreadsheets your Python script will interact with. Without going through Google's app approval process, your scripts will be limited to interacting with the email addresses you provide in this step. Click the "+ ADD USERS" button and in the new panel that appears, enter the Gmail addresses and click the blue "ADD" button. Then click "SAVE AND CONTINUE."
 
 Step 4 "Summary" provides a summary of the previous steps. If all the information looks right, click the "BACK TO DASHBOARD" button. The next step is to create credentials for your project.
 
 ### Create Credentials for Your Project
 
 From the Navigation sidebar menu, click on "APIs & Services" and then "Credentials" to go to the Credentials page. Click the "+ CREATE CREDENTIALS" link at the top of the page. A submenu will open asking what kind of credentials you want to create: "API key", "OAuth client ID", or "Service account". Click on "OAuth client ID".
 
 ![Create credentials](create-credentials.png)
 
 On the new page that appears, select "Desktop app" for the "Application type" and leave "Name" as the default "Desktop client 1." (You can change this to a different name if you want, it doesn't appear to the users of your Python script.) Click the blue "CREATE" button.
 
-On the pop up that appears, click "DOWNLOAD JSON" to download the credentials file. This credentials JSON file will have a name like *client_secret_282792235794-p2o9gfcub4htibfg2u207gcomco9nqm7.apps.googleusercontent.com.json*. Place it in the same folder that your Python script will be in.
+The pop up that appears shows your , click "DOWNLOAD JSON" to download the credentials file. This file will have a name like *client_secret_282792235794-p2o9gfcub4htibfg2u207gcomco9nqm7.apps.googleusercontent.com.json*. Rename it to *credentials-sheets.json* and place it in the same folder that your Python script will be in.
 
 ### Log In with the Credentials File
 
-Run the Python interactive shell from the same folder that the credentials JSON file is in and run `import ezsheets`. Or, place a *.py* Python program in this folder and have it run `import ezsheets`. EZSheets will load and automatically check this folder for a credentials JSON file and, if found, launches your web browser to the OAuth consent screen. Sign in with the Google account you want to access from your Python script. This must be the same email address that you gave for the "test user" when configuring the Google Cloud project's OAuth consent screen.
+Run the Python interactive shell from the same folder that the *credentials-sheets.json* file is in and run `import ezsheets`. Or, place a *.py* Python program in this folder and have it run `import ezsheets`. EZSheets will load and automatically check this folder for a *credentials-sheets.json* file and, if found, launches your web browser to the OAuth consent screen. Sign in with the Google account you want to access from your Python script. This must be the same email address that you gave for the "test user" when configuring the Google Cloud project's OAuth consent screen.
 
 You will get a warning message that reads "Google hasn't verified this app," but that's fine because this is the app (or project) that you've just created yourself. Click the Continue link. You'll come to another page that says "Python Google API Script wants access to your Google Account" (or whatever name you gave in the OAuth consent screen setup.) Click Continue.
 
-You'll come to a plain web page that says, "The authentication flow has completed." You can now close the browser window. In the same folder as your credentials JSON file, you'll now see a *token-drive.pickle* and *token-sheets.pickle* file. Treat these files like passwords and do not share them: they can be used to log in and access your Google Sheets spreadsheets.
+You'll come to a plain web page that says, "The authentication flow has completed." You can now close the browser window. In the same folder as your *credentials-sheets.json* file, you'll now see a *token.json* file. Do not share these files: they can be used to log in and access your Google Sheets spreadsheets.
 
 ## Quickstart Guide
 
 After you've set up your credentials and token files, you can import EZSheets to access your Google Sheets. Create a `Spreadsheet` object by using the Spreadsheet's URL:
 
     >>> import ezsheets
     >>> s = ezsheets.Spreadsheet('https://docs.google.com/spreadsheets/d/16RWH9XBBwd8pRYZDSo9EontzdVPqxdGnwM5MnP6T48c/edit#gid=0')
```

### Comparing `EZSheets-2023.8.11/src/ezsheets/__init__.py` & `EZSheets-2023.8.6/src/ezsheets/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,26 +10,22 @@
 import collections
 import json
 import os.path
 import pickle
 import re
 import time
 import webbrowser
-import http.client
-from urllib.parse import urlparse
 
 from apiclient.http import MediaFileUpload, MediaIoBaseDownload
 from google.auth.transport.requests import Request
 from google_auth_oauthlib.flow import InstalledAppFlow
 from googleapiclient.discovery import build
 from googleapiclient.errors import HttpError
 
-from ezsheets.colorvalues import COLORS
-
-__version__ = "2023.8.11"
+__version__ = "2023.8.6"
 
 # SCOPES_SHEETS = ['https://www.googleapis.com/auth/spreadsheets.readonly']
 SCOPES_SHEETS = ["https://www.googleapis.com/auth/spreadsheets"]
 SHEETS_SERVICE = None
 IS_INITIALIZED = False
 
 # SCOPES_DRIVE = ['https://www.googleapis.com/auth/drive.readonly']
@@ -42,14 +38,16 @@
 DEFAULT_NEW_COLUMN_COUNT = 26  # This is the Google Sheets default for a new Sheet.
 DEFAULT_FROZEN_ROW_COUNT = 0
 DEFAULT_FROZEN_COLUMN_COUNT = 0
 DEFAULT_HIDE_GRID_LINES = False
 DEFAULT_ROW_GROUP_CONTROL_AFTER = False
 DEFAULT_COLUMN_GROUP_CONTROL_AFTER = False
 
+from ezsheets.colorvalues import COLORS
+
 # Quota throttling:
 _READ_REQUESTS = collections.deque()
 _WRITE_REQUESTS = collections.deque()
 READ_QUOTA = 90  # 50 reads per 100 seconds
 WRITE_QUOTA = 90  # 50 writes per 100 seconds
 IGNORE_QUOTA = False
 """ TODO - create a context manager to wrap calls, so that we can do both
@@ -185,35 +183,14 @@
 
         :param spreadsheetId: The ID or URL of the spreadsheet on Google Sheets. E.g. `'https://docs.google.com/spreadsheets/d/10tRbpHZYkfRecHyRHRjBLdQYoq5QWNBqZmH9tt4Tjng/edit#gid=0'` or `'10tRbpHZYkfRecHyRHRjBLdQYoq5QWNBqZmH9tt4Tjng'`
         """
         if not IS_INITIALIZED:
             init()  # Initialize this module if not done so already.
 
         try:
-            # Figure out if this URL redirects to the Google Sheets URL.
-            # NOTE: Restricted spreadsheets will redirect a docs.google.com url to their https://accounts.google.com/v3/signin/... URL, which
-            # we don't want, so if it begins with docs.google.com just use it and don't check for redirects. (This doesn't apply to shared spreadsheets.)
-            while spreadsheetId.lower().startswith('http') and not spreadsheetId.lower().startswith('https://docs.google.com'):
-
-                redirects = [spreadsheetId]
-                while True:
-                    parsed_url = urlparse(spreadsheetId)
-                    http_conn = http.client.HTTPConnection(parsed_url.netloc)
-                    http_conn.request("GET", parsed_url.path)
-                    response = http_conn.getresponse()
-                    redirects.append(spreadsheetId)
-
-                    spreadsheetId = response.getheader('Location')
-                    if spreadsheetId == redirects[-1] or response.status not in (301, 302):
-                        """There's some weird behavior where the google doc url keeps redirecting to itself forever,
-                        hence why I added the spreadsheetId == redirects[-1] check. I'm not sure what causes this.
-                        Requests doesn't have this problem, nor does `wget https://bit.ly/3D34nDh 2>&1 | grep Location:`
-                        so I can't quite fix it. But this works well enough for now."""
-                        break
-
             try:
                 spreadsheetId = getIdFromUrl(spreadsheetId)
             except ValueError:
                 pass  # No problem if it's not a valid ID or URL; it could be a title.
 
             # request = SHEETS_SERVICE.spreadsheets().get(spreadsheetId=spreadsheetId)
             # _logReadRequest(); request.execute()
@@ -351,27 +328,18 @@
         Return an iterable of the Sheet objects in this Spreadsheet.
         """
         return iter(self.sheets)
 
     @property
     def spreadsheetId(self):
         """
-        The unique, read-only id for this Spreadsheet on Google Sheets. (This is the old, deprecated name. Use id instead.)
-        """
-        return self._spreadsheetId
-
-
-    @property
-    def id(self):
-        """
-        The unique, read-only id for this Spreadsheet on Google Sheets.
+        The unique id for this Spreadsheet on Google Sheets.
         """
         return self._spreadsheetId
 
-
     @property
     def url(self):
         """
         The URL for this Spreadsheet on Google Sheets.
         """
         return "https://docs.google.com/spreadsheets/d/" + self._spreadsheetId + "/"
 
@@ -389,15 +357,14 @@
         return '<%s title="%s", %d sheets>' % (type(self).__name__, self.title, len(self.sheets))
 
     def __repr__(self):
         """
         A string representation of code that can recreate this Spreadsheet object.
         """
         return "%s(spreadsheetId=%r)" % (type(self).__name__, self.spreadsheetId)
-        # NOTE that the __str__ function will still use "spreadsheetId" instead of "id" to maintain backwards compatibility.
 
     @property
     def title(self):
         """
         The string title for this Spreadsheet on Google Sheets. Both Spreadsheets and Sheets have titles.
         """
         return self._title
@@ -496,23 +463,14 @@
             #                             body={'trashed': True}).execute()
             _makeRequest("drive.update", **{"fileId": self._spreadsheetId, "body": {"trashed": True}})
 
     def open(self):
         webbrowser.open(self.url)
 
 
-    def __eq__(self, other):
-        """
-        A Spreadsheet object is only considered equal to Spreadsheet objects with the same ID.
-        """
-        if not isinstance(other, Spreadsheet):
-            return False
-        return self.spreadsheetId == other.spreadsheetId
-
-
 def _makeFilenameSafe(filename):
     for replaceChar in ' \\/:*?"<>|':
         filename = filename.replace(replaceChar, "_")
     return filename
 
 
 class Sheet:
@@ -676,28 +634,19 @@
         if not isinstance(other, Sheet):
             return False
         return self._sheetId == other._sheetId
 
     @property
     def sheetId(self):
         """
-        The unique, read-only ID string of this Sheet object in its Spreadsheet. (This is the old, deprecated name. Use id instead.)
+        The unique ID string of this Sheet object in its Spreadsheet.
         """
         return self._sheetId
 
     @property
-    def id(self):
-        """
-        The unique, read-only ID string of this Sheet object in its Spreadsheet. (This is the old, deprecated name. Use id instead.)
-        """
-        # NOTE that the __str__ function will still use "sheetId" instead of "id" to maintain backwards compatibility.
-        return self._sheetId
-
-
-    @property
     def rowCount(self):
         """
         The number of rows in this Sheet object.
         """
         return self._rowCount
 
     @rowCount.setter
@@ -843,28 +792,26 @@
         return "<%s title=%r, sheetId=%r, rowCount=%r, columnCount=%r>" % (
             type(self).__name__,
             self._title,
             self._sheetId,
             self._rowCount,
             self._columnCount,
         )
-        # NOTE that the __str__ function will still use "sheetId" instead of "id" to maintain backwards compatibility.
 
     def __repr__(self):
         """
         TODO
         """
         return "<%s sheetId=%r, title=%r, rowCount=%r, columnCount=%r>" % (
             type(self).__name__,
             self._sheetId,
             self._title,
             self._rowCount,
             self._columnCount,
         )
-        # NOTE that the __str__ function will still use "sheetId" instead of "id" to maintain backwards compatibility.
 
     def get(self, *args):
         """
         Retrieve the value in a cell. The arguments to `get()` can either be two
         integers (column and row) or a single string such as 'A1'.
         """
         # TODO!!!! Add a switch or a mode or something so that all the ezsheets functions call refresh() before running.
@@ -1725,15 +1672,14 @@
     # But this isn't the name it has when you download it from Google
     # Cloud Console, so we'll just use the client_secret_*.json filename
     # format it already has, and fall back on credentials-sheets.json.
     # If credentialsFile is a folder name, use that folder to search for the credentials file.
 
     # credentialsFile is a bit misleading of a name because it can be a file or a folder (that contains the credentials file)
     if os.path.isdir(os.path.abspath(credentialsFile)):
-        # If credentialsFile is a folder, search that folder for credentials-sheets.json or client_secret_*.json files:
         possibleCredentialsFiles = []
         for filename in os.listdir(os.path.abspath(credentialsFile)):
             if (filename.startswith('client_secret_') and filename.endswith('.json')) or filename == 'credentials-sheets.json':
                 possibleCredentialsFiles.append(filename)
         if len(possibleCredentialsFiles) == 0:
             credentialsFile = 'credentials-sheets.json'  # Setting it to this nonexistant file will trigger the later EZSheetsException.
         elif len(possibleCredentialsFiles) > 1:
@@ -1744,15 +1690,15 @@
     try:
         if not os.path.exists(credentialsFile):
             raise EZSheetsException(
                 'Can\'t find credentials file at %s. You can download this file from https://developers.google.com/sheets/api/quickstart/python  and clicking "Enable the Google Sheets API". Rename the downloaded file to credentials-sheets.json.'
                 % (os.path.abspath(credentialsFile))
             )
 
-        # Find the token files, assume they are in the same folder as the credentials file:
+        # Assume that the token files are in the same folder as the credentials file:
         if not os.path.isabs(sheetsTokenFile):
             sheetsTokenFile = os.path.join(os.path.dirname(os.path.abspath(credentialsFile)), sheetsTokenFile)
         if not os.path.isabs(driveTokenFile):
             driveTokenFile = os.path.join(os.path.dirname(os.path.abspath(credentialsFile)), driveTokenFile)
 
         # Log in to Google Sheets API to generate token-sheets.pickle.
         creds = None
```

### Comparing `EZSheets-2023.8.11/src/ezsheets/colorvalues.py` & `EZSheets-2023.8.6/src/ezsheets/colorvalues.py`

 * *Files identical despite different names*

### Comparing `EZSheets-2023.8.11/tests/test_ezsheets.py` & `EZSheets-2023.8.6/tests/test_ezsheets.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,20 +39,18 @@
 
 
 def test_basic():
     pass # TODO - add unit tests
 
 
 def test_getIdFromUrl():
-    # Fake url and id
     assert ezsheets.getIdFromUrl("https://docs.google.com/spreadsheets/d/10tRbpHZYkfRecHyRHRjBLdQYoq5QWNBqZmH9tt4Tjng/edit#gid=0") == "10tRbpHZYkfRecHyRHRjBLdQYoq5QWNBqZmH9tt4Tjng"
 
     with pytest.raises(ValueError):
-        # Fake url and id
-        ezsheets.getIdFromUrl(r"https://docs.google.com/spread           sheets/d/10tRbpHZYkfRecHyRHRjBLdQYoq5QWNBqZmH9tt4Tjng/edit#gid=0")
+        ezsheets.getIdFromUrl(r"https://docs.google.com/spread sheets/d/10tRbpHZYkfRecHyRHRjBLdQYoq5QWNBqZmH9tt4Tjng/edit#gid=0")
 
 
 def test_getColumnLetterOf():
     assert ezsheets.getColumnLetterOf(1) == 'A'
     assert ezsheets.getColumnLetterOf(26) == 'Z'
     assert ezsheets.getColumnLetterOf(27) == 'AA'
     assert ezsheets.getColumnLetterOf(702) == 'ZZ'
@@ -147,16 +145,14 @@
 
 def test_Spreadsheet_attr(init, checkPreAndPostCondition):
     assert TEST_SS.title == 'Delete Me'
     assert TEST_SS.spreadsheetId != ''
     assert TEST_SS.sheetTitles == ('Sheet1',)
     assert len(TEST_SS) == 1
 
-    assert TEST_SS.spreadsheetId == TEST_SS.id
-
 
 def test_createSheet_deleteSheet(init, checkPreAndPostCondition):
     newSheet1 = TEST_SS.createSheet(title='New Sheet 1')
 
     assert 'New Sheet 1' in TEST_SS.sheetTitles
     assert newSheet1 == TEST_SS.sheets[1]
     assert newSheet1.title == 'New Sheet 1'
@@ -834,30 +830,7 @@
 
 
 
 def test_getitem(init, checkPreAndPostCondition):
     pass # TODO LEFT OFF
 
 
-def test_restricted_and_link_viewable():
-    # Restricted spreadsheet:
-    ezsheets.Spreadsheet('https://docs.google.com/spreadsheets/d/16O3PLFhA8EUH7CdmSeNtxie03kitBfLoi_aOex93WIA/edit#gid=0')
-
-    # Viewable by anyone with the link:
-    ezsheets.Spreadsheet('https://docs.google.com/spreadsheets/d/1WCKpKAgUjVJv2RM23dc4LHj9mOonK8VsvSXi_U4eqLk/edit#gid=0')
-
-
-def test_eq():
-    ss1 = ezsheets.Spreadsheet('https://autbor.com/examplegs')
-    ss2 = ezsheets.Spreadsheet('https://docs.google.com/spreadsheets/d/1TzOJxhNKr15tzdZxTqtQ3EmDP6em_elnbtmZIcyu8vI/')
-    ss3 = ezsheets.Spreadsheet('1TzOJxhNKr15tzdZxTqtQ3EmDP6em_elnbtmZIcyu8vI')
-
-    other_ss = ezsheets.Spreadsheet('https://docs.google.com/spreadsheets/d/1WCKpKAgUjVJv2RM23dc4LHj9mOonK8VsvSXi_U4eqLk/edit#gid=0')
-
-    assert ss1 == ss2 == ss3
-    assert ss1 != other_ss
-
-    assert ss1[0].id == ss1[0].sheetId
-
-
-
-
```

