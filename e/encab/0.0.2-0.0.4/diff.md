# Comparing `tmp/encab-0.0.2.tar.gz` & `tmp/encab-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encab-0.0.2.tar", last modified: Tue Jul 11 13:33:11 2023, max compression
+gzip compressed data, was "encab-0.0.4.tar", last modified: Tue Jul 11 15:05:38 2023, max compression
```

## Comparing `encab-0.0.2.tar` & `encab-0.0.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-11 13:33:11.255822 encab-0.0.2/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1074 2023-04-18 07:01:45.000000 encab-0.0.2/LICENSE
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5545 2023-07-11 13:33:11.255822 encab-0.0.2/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4980 2023-07-11 13:20:21.000000 encab-0.0.2/README.md
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      967 2023-07-11 13:07:20.000000 encab-0.0.2/pyproject.toml
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2023-07-11 13:33:11.255822 encab-0.0.2/setup.cfg
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-11 13:33:11.247822 encab-0.0.2/src/
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-11 13:33:11.251822 encab-0.0.2/src/encab/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2022-11-29 14:01:58.000000 encab-0.0.2/src/encab/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       34 2022-12-05 16:39:25.000000 encab-0.0.2/src/encab/__main__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11043 2023-03-12 15:50:33.000000 encab-0.0.2/src/encab/config.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8042 2023-03-02 07:42:58.000000 encab-0.0.2/src/encab/encab.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-11 13:33:11.255822 encab-0.0.2/src/encab/ext/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2023-01-18 08:48:31.000000 encab-0.0.2/src/encab/ext/__init__.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     6020 2023-07-11 09:18:42.000000 encab-0.0.2/src/encab/ext/log_sanitizer.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12061 2023-07-11 09:18:42.000000 encab-0.0.2/src/encab/ext/startup_script.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14101 2023-07-11 09:18:42.000000 encab-0.0.2/src/encab/ext/validation.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5348 2023-03-02 07:56:10.000000 encab-0.0.2/src/encab/extensions.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     7517 2023-07-06 14:12:14.000000 encab-0.0.2/src/encab/program.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10017 2023-03-02 07:37:32.000000 encab-0.0.2/src/encab/program_state.py
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3160 2023-01-25 12:22:05.000000 encab-0.0.2/src/encab/programs.py
-drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-11 13:33:11.251822 encab-0.0.2/src/encab.egg-info/
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5545 2023-07-11 13:33:11.000000 encab-0.0.2/src/encab.egg-info/PKG-INFO
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      526 2023-07-11 13:33:11.000000 encab-0.0.2/src/encab.egg-info/SOURCES.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-07-11 13:33:11.000000 encab-0.0.2/src/encab.egg-info/dependency_links.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       44 2023-07-11 13:33:11.000000 encab-0.0.2/src/encab.egg-info/entry_points.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      178 2023-07-11 13:33:11.000000 encab-0.0.2/src/encab.egg-info/requires.txt
--rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        6 2023-07-11 13:33:11.000000 encab-0.0.2/src/encab.egg-info/top_level.txt
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-11 15:05:38.523630 encab-0.0.4/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     1074 2023-04-18 07:01:45.000000 encab-0.0.4/LICENSE
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4865 2023-07-11 15:05:38.523630 encab-0.0.4/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4299 2023-07-11 14:32:39.000000 encab-0.0.4/README.md
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      968 2023-07-11 14:42:58.000000 encab-0.0.4/pyproject.toml
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       38 2023-07-11 15:05:38.523630 encab-0.0.4/setup.cfg
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-11 15:05:38.515629 encab-0.0.4/src/
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-11 15:05:38.519629 encab-0.0.4/src/encab/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2022-11-29 14:01:58.000000 encab-0.0.4/src/encab/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       34 2022-12-05 16:39:25.000000 encab-0.0.4/src/encab/__main__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    11043 2023-03-12 15:50:33.000000 encab-0.0.4/src/encab/config.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     8042 2023-07-11 14:44:10.000000 encab-0.0.4/src/encab/encab.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-11 15:05:38.523630 encab-0.0.4/src/encab/ext/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        0 2023-01-18 08:48:31.000000 encab-0.0.4/src/encab/ext/__init__.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     6020 2023-07-11 09:18:42.000000 encab-0.0.4/src/encab/ext/log_sanitizer.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    12061 2023-07-11 09:18:42.000000 encab-0.0.4/src/encab/ext/startup_script.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    14101 2023-07-11 09:18:42.000000 encab-0.0.4/src/encab/ext/validation.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     5348 2023-03-02 07:56:10.000000 encab-0.0.4/src/encab/extensions.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     7603 2023-07-11 13:57:15.000000 encab-0.0.4/src/encab/program.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)    10017 2023-03-02 07:37:32.000000 encab-0.0.4/src/encab/program_state.py
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     3160 2023-01-25 12:22:05.000000 encab-0.0.4/src/encab/programs.py
+drwxrwxr-x   0 sebastian  (1000) sebastian  (1000)        0 2023-07-11 15:05:38.523630 encab-0.0.4/src/encab.egg-info/
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)     4865 2023-07-11 15:05:38.000000 encab-0.0.4/src/encab.egg-info/PKG-INFO
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      526 2023-07-11 15:05:38.000000 encab-0.0.4/src/encab.egg-info/SOURCES.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        1 2023-07-11 15:05:38.000000 encab-0.0.4/src/encab.egg-info/dependency_links.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)       44 2023-07-11 15:05:38.000000 encab-0.0.4/src/encab.egg-info/entry_points.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)      178 2023-07-11 15:05:38.000000 encab-0.0.4/src/encab.egg-info/requires.txt
+-rw-rw-r--   0 sebastian  (1000) sebastian  (1000)        6 2023-07-11 15:05:38.000000 encab-0.0.4/src/encab.egg-info/top_level.txt
```

### Comparing `encab-0.0.2/LICENSE` & `encab-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `encab-0.0.2/PKG-INFO` & `encab-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: encab
-Version: 0.0.2
-Summary: Docker entypoint tool
+Version: 0.0.4
+Summary: Docker entrypoint tool
 Author-email: Sebastian Kuebeck <sebastian.kuebeck@encab.io>
 Project-URL: Homepage, https://github.com/sebastian-kuebeck/encab
 Project-URL: Documentation, https://encab.readthedocs.io
 Project-URL: Bug Tracker, https://github.com/sebastian-kuebeck/encab
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,40 +14,40 @@
 License-File: LICENSE
 
 # Encab: A Docker Entrypoint Tool
 
 **Encab** is essentially a replacement for complex, hand-written Docker Container Entrypoint scripts,
 especially when dockerizing complex legacy applications.
 
-Add it as your [Dockerfile Entrypoint][1],
+1. Add it as your [Dockerfile Entrypoint][1],
 together with the encab configuration file `encab.yml`,
 
 ```dockerfile
    ...
    ADD encab.yml .
    ENTRYPOINT ["encab"]
 ```
 
 [1]: https://docs.docker.com/engine/reference/builder/#entrypoint
 
-define what you want to run in your container in `encab.yml`,
+2. Define what you want to run in your container in `encab.yml`,
 
 ```yaml
    programs:
       cron:
          command: cron -f
       main:
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.0.1
+   INFO  encab: encab 0.0.3
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -69,127 +69,119 @@
 
 ## Documentation
 
 [Encab Documentation](https://encab.readthedocs.io)
 
 ## Installation
 
-### From Source
-
-Encab is not yet at pypi so installation from source is the only option right now.
+### Install locally
 
 #### Prerequisites
 
-- [Docker](https://www.docker.com/) from your Linux distribution or Docker Desktop.
-- [git](https://git-scm.com/) distributed version control system
 - [Python](https://www.python.org/) Version >= 3.7
 - activated Python virtual environment such as [miniconda][2] or [virtualenv][3]
 
-[2]: https://docs.conda.io/en/latest/miniconda.html
-[3]: https://virtualenv.pypa.io/en/latest/
-
-#### Download
-
-```sh
-   git clone https://github.com/skuebeck/encab.git
-   cd encab
-   pip install -r requirements.txt
-```
-
-#### Build Wheel
-
 ```sh
-   make dist
+   pip install -U encab
 ```
 
-If all goes well, the encab [wheel file](https://packaging.python.org/en/latest/tutorials/installing-packages/#source-distributions-vs-wheels) will be in the `dist` directory.
+#### Run locally
 
-It's named `encab-<version>-py3-none-any.whl`
+1. Create sample encab file `encab.yml`
 
-#### Testing (optional)
-
-run unit tests:
-
-```sh
-   make test
+```yml
+   encab:
+      dry_run: false
+   programs:
+      main:
+         sh:
+            - echo "Hello Encab!"
 ```
 
-run localy:
+2. Run locally:
 
 ```sh
-   python -m encab
+   encab
 ```
 
-It'll use the sample `encab.yml` file.
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.0.1
+INFO  encab: encab 0.0.3
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
-INFO  encab: Dry run. No program will be started.
-INFO  encab: settings are valid.
-INFO  encab: settings are valid.
-INFO  encab: settings are valid.
-INFO  encab: Dry run succeeded. Exiting.
-```
-
-## Deployment
-
-1. Copy the generated wheel file into your Docker project directory.
-2. Create a configuration file `encab.yml`(see Configuration section for details).
-
-   ```yaml
-      programs:
-         main:
-            sh: echo 'Hello World'
+INFO  main: Hello Encab!
+INFO  main: Exited with rc: 0
    ```
 
-3. Add Encab to your [Docker file][4].
+### Install in Container
+
+#### Prerequisites
+
+- [Docker](https://www.docker.com/) from your Linux distribution or Docker Desktop.
+
+#### Run in Container
+
+1. Create sample encab file `encab.yml`
+
+```yml
+   encab:
+      dry_run: false
+   programs:
+      main:
+         sh:
+            - echo "Hello Encab!"
+```
+
+2. Add Encab to your [Docker file][4].
 
    ```dockerfile
-   FROM python:3.10.8-slim-bullseye
 
+   FROM python:3.10.8-slim-bullseye
+   # --------------------------------------------
+   # Install Venv 
+   #
+   ENV VIRTUAL_ENV=/opt/encabenv
+   ENV PATH="$VIRTUAL_ENV/bin:$PATH"
+   RUN python3 -m venv $VIRTUAL_ENV && \
+      pip install --upgrade pip
    # --------------------------------------------
    # Install Encab 
    #
-   ARG ENCAB_WHEEL=encab-0.0.1-py3-none-any.whl
 
-   ENV PATH=$PATH:/root/.local/bin
-   RUN python3 -m pip install --user pipx
-   ADD ${ENCAB_WHEEL} .
-   RUN python3 -m pipx install ./${ENCAB_WHEEL}
+   RUN pip install encab
 
    # -------------------------------------------
    # add configuration file
    #
    ADD encab.yml .
 
    # -------------------------------------------
    # set encab as entrypoint
    ENTRYPOINT ["encab"]
+
    ```
 
    [4]: https://docs.docker.com/engine/reference/builder/
 
-4. Build container
+2. Build container
 
    ```sh
-   docker build --build-arg ENCAB_WHEEL=`ls encab-*.whl` -t encab_minimum .
+   docker build -t encab_minimum .
    ```
 
-5. Run container
+3. Run container
 
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.0.1
+   INFO  encab: encab 0.0.3
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.0.2/README.md` & `encab-0.0.4/src/encab.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,53 @@
+Metadata-Version: 2.1
+Name: encab
+Version: 0.0.4
+Summary: Docker entrypoint tool
+Author-email: Sebastian Kuebeck <sebastian.kuebeck@encab.io>
+Project-URL: Homepage, https://github.com/sebastian-kuebeck/encab
+Project-URL: Documentation, https://encab.readthedocs.io
+Project-URL: Bug Tracker, https://github.com/sebastian-kuebeck/encab
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Encab: A Docker Entrypoint Tool
 
 **Encab** is essentially a replacement for complex, hand-written Docker Container Entrypoint scripts,
 especially when dockerizing complex legacy applications.
 
-Add it as your [Dockerfile Entrypoint][1],
+1. Add it as your [Dockerfile Entrypoint][1],
 together with the encab configuration file `encab.yml`,
 
 ```dockerfile
    ...
    ADD encab.yml .
    ENTRYPOINT ["encab"]
 ```
 
 [1]: https://docs.docker.com/engine/reference/builder/#entrypoint
 
-define what you want to run in your container in `encab.yml`,
+2. Define what you want to run in your container in `encab.yml`,
 
 ```yaml
    programs:
       cron:
          command: cron -f
       main:
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.0.1
+   INFO  encab: encab 0.0.3
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -54,127 +69,119 @@
 
 ## Documentation
 
 [Encab Documentation](https://encab.readthedocs.io)
 
 ## Installation
 
-### From Source
-
-Encab is not yet at pypi so installation from source is the only option right now.
+### Install locally
 
 #### Prerequisites
 
-- [Docker](https://www.docker.com/) from your Linux distribution or Docker Desktop.
-- [git](https://git-scm.com/) distributed version control system
 - [Python](https://www.python.org/) Version >= 3.7
 - activated Python virtual environment such as [miniconda][2] or [virtualenv][3]
 
-[2]: https://docs.conda.io/en/latest/miniconda.html
-[3]: https://virtualenv.pypa.io/en/latest/
-
-#### Download
-
 ```sh
-   git clone https://github.com/skuebeck/encab.git
-   cd encab
-   pip install -r requirements.txt
+   pip install -U encab
 ```
 
-#### Build Wheel
-
-```sh
-   make dist
-```
+#### Run locally
 
-If all goes well, the encab [wheel file](https://packaging.python.org/en/latest/tutorials/installing-packages/#source-distributions-vs-wheels) will be in the `dist` directory.
+1. Create sample encab file `encab.yml`
 
-It's named `encab-<version>-py3-none-any.whl`
-
-#### Testing (optional)
-
-run unit tests:
-
-```sh
-   make test
+```yml
+   encab:
+      dry_run: false
+   programs:
+      main:
+         sh:
+            - echo "Hello Encab!"
 ```
 
-run localy:
+2. Run locally:
 
 ```sh
-   python -m encab
+   encab
 ```
 
-It'll use the sample `encab.yml` file.
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.0.1
+INFO  encab: encab 0.0.3
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
-INFO  encab: Dry run. No program will be started.
-INFO  encab: settings are valid.
-INFO  encab: settings are valid.
-INFO  encab: settings are valid.
-INFO  encab: Dry run succeeded. Exiting.
-```
-
-## Deployment
-
-1. Copy the generated wheel file into your Docker project directory.
-2. Create a configuration file `encab.yml`(see Configuration section for details).
-
-   ```yaml
-      programs:
-         main:
-            sh: echo 'Hello World'
+INFO  main: Hello Encab!
+INFO  main: Exited with rc: 0
    ```
 
-3. Add Encab to your [Docker file][4].
+### Install in Container
+
+#### Prerequisites
+
+- [Docker](https://www.docker.com/) from your Linux distribution or Docker Desktop.
+
+#### Run in Container
+
+1. Create sample encab file `encab.yml`
+
+```yml
+   encab:
+      dry_run: false
+   programs:
+      main:
+         sh:
+            - echo "Hello Encab!"
+```
+
+2. Add Encab to your [Docker file][4].
 
    ```dockerfile
-   FROM python:3.10.8-slim-bullseye
 
+   FROM python:3.10.8-slim-bullseye
+   # --------------------------------------------
+   # Install Venv 
+   #
+   ENV VIRTUAL_ENV=/opt/encabenv
+   ENV PATH="$VIRTUAL_ENV/bin:$PATH"
+   RUN python3 -m venv $VIRTUAL_ENV && \
+      pip install --upgrade pip
    # --------------------------------------------
    # Install Encab 
    #
-   ARG ENCAB_WHEEL=encab-0.0.1-py3-none-any.whl
 
-   ENV PATH=$PATH:/root/.local/bin
-   RUN python3 -m pip install --user pipx
-   ADD ${ENCAB_WHEEL} .
-   RUN python3 -m pipx install ./${ENCAB_WHEEL}
+   RUN pip install encab
 
    # -------------------------------------------
    # add configuration file
    #
    ADD encab.yml .
 
    # -------------------------------------------
    # set encab as entrypoint
    ENTRYPOINT ["encab"]
+
    ```
 
    [4]: https://docs.docker.com/engine/reference/builder/
 
-4. Build container
+2. Build container
 
    ```sh
-   docker build --build-arg ENCAB_WHEEL=`ls encab-*.whl` -t encab_minimum .
+   docker build -t encab_minimum .
    ```
 
-5. Run container
+3. Run container
 
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.0.1
+   INFO  encab: encab 0.0.3
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.0.2/pyproject.toml` & `encab-0.0.4/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=63.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "encab"
-version = "0.0.2"
+version = "0.0.4"
 authors = [
   { name="Sebastian Kuebeck", email="sebastian.kuebeck@encab.io" },
 ]
-description = "Docker entypoint tool"
+description = "Docker entrypoint tool"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
```

### Comparing `encab-0.0.2/src/encab/config.py` & `encab-0.0.4/src/encab/config.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.2/src/encab/encab.py` & `encab-0.0.4/src/encab/encab.py`

 * *Files 0% similar despite different names*

```diff
@@ -183,15 +183,15 @@
     try:
         config, location = load_config(encab_stream)
 
         logger = set_up_logger(config)
 
         extra = {"program": ENCAB}
 
-        logger.info("encab 0.0.1", extra=extra)
+        logger.info("encab 0.0.4", extra=extra)
         logger.info("Using configuration %s", location, extra=extra)
 
         logger.debug(
             "Encab config: %s",
             shorten(str(config), width=127, placeholder="..."),
             extra=extra,
         )
```

### Comparing `encab-0.0.2/src/encab/ext/log_sanitizer.py` & `encab-0.0.4/src/encab/ext/log_sanitizer.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.2/src/encab/ext/startup_script.py` & `encab-0.0.4/src/encab/ext/startup_script.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.2/src/encab/ext/validation.py` & `encab-0.0.4/src/encab/ext/validation.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.2/src/encab/extensions.py` & `encab-0.0.4/src/encab/extensions.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.2/src/encab/program.py` & `encab-0.0.4/src/encab/program.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,18 @@
         thread = Thread(target=lambda: self._run(), name=name)
         thread.daemon = True
         self.thread = thread
         thread.start()
         return self
 
     def close(self):
+        try:
+            self.stream.flush()
+        except IOError:
+            pass
         self.stream.close()
 
 
 class ExecutionContext(object):
     """
     The context in which a program is executed
```

### Comparing `encab-0.0.2/src/encab/program_state.py` & `encab-0.0.4/src/encab/program_state.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.2/src/encab/programs.py` & `encab-0.0.4/src/encab/programs.py`

 * *Files identical despite different names*

### Comparing `encab-0.0.2/src/encab.egg-info/PKG-INFO` & `encab-0.0.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,53 +1,38 @@
-Metadata-Version: 2.1
-Name: encab
-Version: 0.0.2
-Summary: Docker entypoint tool
-Author-email: Sebastian Kuebeck <sebastian.kuebeck@encab.io>
-Project-URL: Homepage, https://github.com/sebastian-kuebeck/encab
-Project-URL: Documentation, https://encab.readthedocs.io
-Project-URL: Bug Tracker, https://github.com/sebastian-kuebeck/encab
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Encab: A Docker Entrypoint Tool
 
 **Encab** is essentially a replacement for complex, hand-written Docker Container Entrypoint scripts,
 especially when dockerizing complex legacy applications.
 
-Add it as your [Dockerfile Entrypoint][1],
+1. Add it as your [Dockerfile Entrypoint][1],
 together with the encab configuration file `encab.yml`,
 
 ```dockerfile
    ...
    ADD encab.yml .
    ENTRYPOINT ["encab"]
 ```
 
 [1]: https://docs.docker.com/engine/reference/builder/#entrypoint
 
-define what you want to run in your container in `encab.yml`,
+2. Define what you want to run in your container in `encab.yml`,
 
 ```yaml
    programs:
       cron:
          command: cron -f
       main:
          command: httpd-foreground
 ```
 
 and encab cares for the rest.
 Run it and you'll always know who's logging what...
 
 ```text
-   INFO  encab: encab 0.0.1
+   INFO  encab: encab 0.0.3
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: AH00558: httpd: Could not reliably determine the server's fully qualified domain name, using 172.17.0.2. Set the 'ServerName' directive globally to suppress this message
    ERROR main: [Wed Jan 18 09:47:12.417275 2023] [mpm_event:notice] [pid 12:tid 140142563044672] AH00489: Apache/2.4.54 (Unix) configured -- resuming normal operations
    ERROR main: [Wed Jan 18 09:47:12.417830 2023] [core:notice] [pid 12:tid 140142563044672] AH00094: Command line: 'httpd -D FOREGROUND'
    INFO  cron: Hello Wed Jan 18 09:48:01 UTC 2023
 ```
@@ -69,127 +54,119 @@
 
 ## Documentation
 
 [Encab Documentation](https://encab.readthedocs.io)
 
 ## Installation
 
-### From Source
-
-Encab is not yet at pypi so installation from source is the only option right now.
+### Install locally
 
 #### Prerequisites
 
-- [Docker](https://www.docker.com/) from your Linux distribution or Docker Desktop.
-- [git](https://git-scm.com/) distributed version control system
 - [Python](https://www.python.org/) Version >= 3.7
 - activated Python virtual environment such as [miniconda][2] or [virtualenv][3]
 
-[2]: https://docs.conda.io/en/latest/miniconda.html
-[3]: https://virtualenv.pypa.io/en/latest/
-
-#### Download
-
 ```sh
-   git clone https://github.com/skuebeck/encab.git
-   cd encab
-   pip install -r requirements.txt
+   pip install -U encab
 ```
 
-#### Build Wheel
-
-```sh
-   make dist
-```
+#### Run locally
 
-If all goes well, the encab [wheel file](https://packaging.python.org/en/latest/tutorials/installing-packages/#source-distributions-vs-wheels) will be in the `dist` directory.
+1. Create sample encab file `encab.yml`
 
-It's named `encab-<version>-py3-none-any.whl`
-
-#### Testing (optional)
-
-run unit tests:
-
-```sh
-   make test
+```yml
+   encab:
+      dry_run: false
+   programs:
+      main:
+         sh:
+            - echo "Hello Encab!"
 ```
 
-run localy:
+2. Run locally:
 
 ```sh
-   python -m encab
+   encab
 ```
 
-It'll use the sample `encab.yml` file.
 The result will be something like this:
 
 ```text
-INFO  encab: encab 0.0.1
+INFO  encab: encab 0.0.3
 INFO  encab: Using configuration file ./encab.yml, source: Default location.
-INFO  encab: Dry run. No program will be started.
-INFO  encab: settings are valid.
-INFO  encab: settings are valid.
-INFO  encab: settings are valid.
-INFO  encab: Dry run succeeded. Exiting.
-```
-
-## Deployment
-
-1. Copy the generated wheel file into your Docker project directory.
-2. Create a configuration file `encab.yml`(see Configuration section for details).
-
-   ```yaml
-      programs:
-         main:
-            sh: echo 'Hello World'
+INFO  main: Hello Encab!
+INFO  main: Exited with rc: 0
    ```
 
-3. Add Encab to your [Docker file][4].
+### Install in Container
+
+#### Prerequisites
+
+- [Docker](https://www.docker.com/) from your Linux distribution or Docker Desktop.
+
+#### Run in Container
+
+1. Create sample encab file `encab.yml`
+
+```yml
+   encab:
+      dry_run: false
+   programs:
+      main:
+         sh:
+            - echo "Hello Encab!"
+```
+
+2. Add Encab to your [Docker file][4].
 
    ```dockerfile
-   FROM python:3.10.8-slim-bullseye
 
+   FROM python:3.10.8-slim-bullseye
+   # --------------------------------------------
+   # Install Venv 
+   #
+   ENV VIRTUAL_ENV=/opt/encabenv
+   ENV PATH="$VIRTUAL_ENV/bin:$PATH"
+   RUN python3 -m venv $VIRTUAL_ENV && \
+      pip install --upgrade pip
    # --------------------------------------------
    # Install Encab 
    #
-   ARG ENCAB_WHEEL=encab-0.0.1-py3-none-any.whl
 
-   ENV PATH=$PATH:/root/.local/bin
-   RUN python3 -m pip install --user pipx
-   ADD ${ENCAB_WHEEL} .
-   RUN python3 -m pipx install ./${ENCAB_WHEEL}
+   RUN pip install encab
 
    # -------------------------------------------
    # add configuration file
    #
    ADD encab.yml .
 
    # -------------------------------------------
    # set encab as entrypoint
    ENTRYPOINT ["encab"]
+
    ```
 
    [4]: https://docs.docker.com/engine/reference/builder/
 
-4. Build container
+2. Build container
 
    ```sh
-   docker build --build-arg ENCAB_WHEEL=`ls encab-*.whl` -t encab_minimum .
+   docker build -t encab_minimum .
    ```
 
-5. Run container
+3. Run container
 
    ```sh
    docker run encab_minimum
    ```
 
    Result:
 
    ```text
-   INFO  encab: encab 0.0.1
+   INFO  encab: encab 0.0.3
    INFO  encab: Using configuration file ./encab.yml, source: Default location.
    INFO  main: Hello world!
    INFO  main: Exited with rc: 0
    ```
 
 ## Similar Projects
```

### Comparing `encab-0.0.2/src/encab.egg-info/SOURCES.txt` & `encab-0.0.4/src/encab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

