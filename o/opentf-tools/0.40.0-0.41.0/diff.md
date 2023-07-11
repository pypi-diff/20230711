# Comparing `tmp/opentf_tools-0.40.0-py3-none-any.whl.zip` & `tmp/opentf_tools-0.41.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,16 @@
-Zip file size: 36828 bytes, number of entries: 13
--rw-r--r--  2.0 unx    27203 b- defN 23-Apr-25 14:33 opentf/tools/ctl.py
--rw-r--r--  2.0 unx     7773 b- defN 23-Apr-25 14:33 opentf/tools/ctlcommons.py
--rw-r--r--  2.0 unx    29452 b- defN 23-Apr-25 14:33 opentf/tools/ctlconfig.py
--rw-r--r--  2.0 unx     8138 b- defN 23-Apr-25 14:33 opentf/tools/ctlnetworking.py
--rw-r--r--  2.0 unx    32205 b- defN 23-Apr-25 14:33 opentf/tools/ctlworkflows.py
--rw-r--r--  2.0 unx     3188 b- defN 23-Apr-25 14:33 opentf/tools/done.py
--rw-r--r--  2.0 unx     9391 b- defN 23-Apr-25 14:33 opentf/tools/ready.py
--rw-rw-rw-  2.0 unx    11357 b- defN 23-Apr-25 14:33 opentf_tools-0.40.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1737 b- defN 23-Apr-25 14:33 opentf_tools-0.40.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-25 14:33 opentf_tools-0.40.0.dist-info/WHEEL
--rw-r--r--  2.0 unx      139 b- defN 23-Apr-25 14:33 opentf_tools-0.40.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-25 14:33 opentf_tools-0.40.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1088 b- defN 23-Apr-25 14:33 opentf_tools-0.40.0.dist-info/RECORD
-13 files, 131770 bytes uncompressed, 35012 bytes compressed:  73.4%
+Zip file size: 39576 bytes, number of entries: 14
+-rw-r--r--  2.0 unx    27544 b- defN 23-Jul-11 10:24 opentf/tools/ctl.py
+-rw-r--r--  2.0 unx     7773 b- defN 23-Jul-11 10:24 opentf/tools/ctlcommons.py
+-rw-r--r--  2.0 unx    29452 b- defN 23-Jul-11 10:24 opentf/tools/ctlconfig.py
+-rw-r--r--  2.0 unx     8138 b- defN 23-Jul-11 10:24 opentf/tools/ctlnetworking.py
+-rw-r--r--  2.0 unx    10861 b- defN 23-Jul-11 10:24 opentf/tools/ctlqualitygate.py
+-rw-r--r--  2.0 unx    29356 b- defN 23-Jul-11 10:24 opentf/tools/ctlworkflows.py
+-rw-r--r--  2.0 unx     3188 b- defN 23-Jul-11 10:24 opentf/tools/done.py
+-rw-r--r--  2.0 unx     9391 b- defN 23-Jul-11 10:24 opentf/tools/ready.py
+-rw-rw-rw-  2.0 unx    11357 b- defN 23-Jul-11 10:25 opentf_tools-0.41.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1793 b- defN 23-Jul-11 10:25 opentf_tools-0.41.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 10:25 opentf_tools-0.41.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      139 b- defN 23-Jul-11 10:25 opentf_tools-0.41.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-Jul-11 10:25 opentf_tools-0.41.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1176 b- defN 23-Jul-11 10:25 opentf_tools-0.41.0.dist-info/RECORD
+14 files, 140267 bytes uncompressed, 37624 bytes compressed:  73.2%
```

## zipnote {}

```diff
@@ -6,35 +6,38 @@
 
 Filename: opentf/tools/ctlconfig.py
 Comment: 
 
 Filename: opentf/tools/ctlnetworking.py
 Comment: 
 
+Filename: opentf/tools/ctlqualitygate.py
+Comment: 
+
 Filename: opentf/tools/ctlworkflows.py
 Comment: 
 
 Filename: opentf/tools/done.py
 Comment: 
 
 Filename: opentf/tools/ready.py
 Comment: 
 
-Filename: opentf_tools-0.40.0.dist-info/LICENSE
+Filename: opentf_tools-0.41.0.dist-info/LICENSE
 Comment: 
 
-Filename: opentf_tools-0.40.0.dist-info/METADATA
+Filename: opentf_tools-0.41.0.dist-info/METADATA
 Comment: 
 
-Filename: opentf_tools-0.40.0.dist-info/WHEEL
+Filename: opentf_tools-0.41.0.dist-info/WHEEL
 Comment: 
 
-Filename: opentf_tools-0.40.0.dist-info/entry_points.txt
+Filename: opentf_tools-0.41.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: opentf_tools-0.40.0.dist-info/top_level.txt
+Filename: opentf_tools-0.41.0.dist-info/top_level.txt
 Comment: 
 
-Filename: opentf_tools-0.40.0.dist-info/RECORD
+Filename: opentf_tools-0.41.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## opentf/tools/ctl.py

```diff
@@ -41,15 +41,15 @@
     _eventbus,
     _agentchannel,
     _observer,
     _get,
     _delete,
 )
 from opentf.tools.ctlworkflows import print_workflow_help, workflow_cmd
-
+from opentf.tools.ctlqualitygate import print_qualitygate_help, qualitygate_cmd
 
 ########################################################################
 
 # pylint: disable=broad-except
 
 DEFAULT_NAMESPACE = 'default'
 
@@ -72,14 +72,16 @@
   delete agent {agent_id}          De-register an agent
 
 Channel Commands:
   get channels                     List known channels
 
 Qualitygate Commands:
   get qualitygate {workflow_id}    Get qualitygate status for a workflow
+  describe qualitygate {workflow_id}
+                                   Get description of a qualitygate status for a workflow
 
 Token Commands:
   generate token using {key}       Interactively generate a signed token
   check token {token} using {key}  Check if token signature matches public key
   view token {token}               Show token payload
 
 Advanced Commands:
@@ -769,20 +771,20 @@
         print(GET_AGENTS_HELP)
     elif _is_command('get channels', args):
         print(GET_CHANNELS_HELP)
     elif _is_command('delete agent', args):
         print(DELETE_AGENT_HELP)
     elif _is_command('config', args):
         print_config_help(args)
-    elif (
-        _is_command('_ workflow', args)
-        or _is_command('_ workflows', args)
-        or _is_command('get qualitygate', args)
-    ):
+    elif _is_command('_ workflow', args) or _is_command('_ workflows', args):
         print_workflow_help(args)
+    elif _is_command('get qualitygate', args) or _is_command(
+        'describe qualitygate', args
+    ):
+        print_qualitygate_help(args)
     elif _is_command('get namespaces', args):
         print(GET_NAMESPACES_HELP)
     elif len(args) == 2:
         print(GENERAL_HELP)
     else:
         _error('Unknown command.  Use --help to list known commands.')
         sys.exit(1)
@@ -860,20 +862,20 @@
         )
         read_configuration()
         list_channels()
     elif _is_command('delete agent _', sys.argv):
         _ensure_options(sys.argv[4:])
         read_configuration()
         delete_agent(sys.argv[3])
-    elif (
-        _is_command('_ workflow', sys.argv)
-        or _is_command('_ workflows', sys.argv)
-        or _is_command('get qualitygate', sys.argv)
-    ):
+    elif _is_command('_ workflow', sys.argv) or _is_command('_ workflows', sys.argv):
         workflow_cmd()
+    elif _is_command('get qualitygate', sys.argv) or _is_command(
+        'describe qualitygate', sys.argv
+    ):
+        qualitygate_cmd()
     elif _is_command('config', sys.argv):
         config_cmd()
     else:
         _error('Unknown command.  Use --help to list known commands.')
         sys.exit(1)
```

## opentf/tools/ctlworkflows.py

```diff
@@ -1,8 +1,8 @@
-# Copyright 2021, 2022 Henix, henix.fr
+# Copyright 2021-2023 Henix, henix.fr
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -38,15 +38,14 @@
     _debug,
 )
 from opentf.tools.ctlconfig import read_configuration, CONFIG
 from opentf.tools.ctlnetworking import (
     _observer,
     _receptionist,
     _killswitch,
-    _qualitygate,
     _get,
     _get_json,
     _delete,
     _post,
 )
 
 
@@ -149,32 +148,14 @@
 
 Usage:
   opentf-ctl get workflow WORKFLOW_ID [--step_depth=value] [--job_depth=value] [--watch] [options]
 
 Use "opentf-ctl options" for a list of global command-line options (applies to all commands).
 '''
 
-GET_QUALITYGATE_HELP = '''Get qualitygate status for a workflow
-
-Examples:
-  # Get the current qualitygate status of a workflow
-  opentf-ctl get qualitygate 9ea3be45-ee90-4135-b47f-e66e4f793383
-
-  # Get the qualitygate status of a workflow for a specific mode
-  opentf-ctl get qualitygate 9ea3be45-ee90-4135-b47f-e66e4f793383 --mode=strict
-
-Options:
-  --mode=strict|passing|... or -m=...: use the specific qualitygate mode
-
-Usage:
-  opentf-ctl get qualitygate WORKFLOW_ID [--mode=mode] [options]
-
-Use "opentf-ctl options" for a list of global command-line options (applies to all commands).
-'''
-
 GET_WORKFLOWS_HELP = '''List active and recent workflows
 
 Examples:
   # List the IDs of active and recent workflows
   opentf-ctl get workflows
 
   # Get the status of active and recent workflows
@@ -344,25 +325,32 @@
         _error(
             'Could not get workflows list.  Return code was %d.',
             response.status_code,
         )
     sys.exit(2)
 
 
-def list_workflows() -> None:
-    """List active and recent workflows."""
+def _retrieve_columns_to_display(
+    wide_columns: tuple, default_columns: tuple
+) -> Iterable[str]:
+    """Safely retrieve columns to display when listing workflow or quality gate results."""
     try:
-        columns = _get_columns(WIDE_COLUMNS, DEFAULT_COLUMNS)
+        return _get_columns(wide_columns, default_columns)
     except ValueError as err:
         _error('Invalid parameters: %s.', err)
         sys.exit(2)
     except Exception as err:
         _error('Could not get columns specification: %s.', err)
         sys.exit(2)
 
+
+def list_workflows() -> None:
+    """List active and recent workflows."""
+    columns = _retrieve_columns_to_display(WIDE_COLUMNS, DEFAULT_COLUMNS)
+
     response = _get_json(
         _observer(),
         '/workflows',
         'Could not get workflows list',
         handler=_handler_maybe_outdated,
     )
     workflows_ids = response['details']['items']
@@ -841,95 +829,28 @@
     _ensure_uuid(workflow_id)
 
     _ = _get(_observer(), f'/workflows/{workflow_id}/status', handler=_notknown)
     _ = _delete(_killswitch(), f'/workflows/{workflow_id}')
     print(f'Killing workflow {workflow_id}.')
 
 
-def get_qualitygate(workflow_id: str, mode: str) -> None:
-    """Get qualitygate status.
-
-    # Required parameter
-
-    - workflow_id: a non-empty string (an UUID)
-    - mode: a string
-
-    # Raised exceptions
-
-    Abort with an error code of 2 if the specified `workflow_id` is
-    invalid or if an error occurred while contacting the orchestrator.
-
-    Abort with an error code of 101 if the workflow is still running.
-
-    Abort with an error code of 102 if the qualitygate failed.
-    """
-    _ensure_uuid(workflow_id)
-    result = _get_json(
-        _qualitygate(),
-        f'/workflows/{workflow_id}/qualitygate?mode={mode}',
-        statuses=(200, 404, 422),
-    )
-    if result.get('code') == 404:
-        _error(
-            'Unknown workflow %s.  It is either too new, too old, or the provided '
-            + 'workflow ID is incorrect.  You can use "opentf-ctl get workflows" to list '
-            + 'the known workflow IDs.',
-            workflow_id,
-        )
-        sys.exit(2)
-    if result.get('code') == 422:
-        _error(result.get('message'))
-        sys.exit(2)
-    if 'details' not in result or 'status' not in result.get('details', {}):
-        _error(
-            'Unexpected response from qualitygate.  Was expecting a JSON object'
-            + ' with a .details.status entry, got: %s',
-            str(result),
-        )
-        sys.exit(2)
-    status = result['details']['status']
-    if status not in ('SUCCESS', 'NOTEST', 'FAILURE', 'RUNNING'):
-        _error(
-            'Unexpected status from qualitygate: %s (was expecting SUCCESS, NOTEST,'
-            + ' FAILURE, or RUNNING).',
-            status,
-        )
-        sys.exit(2)
-    if status == 'RUNNING':
-        print(
-            f'Workflow {workflow_id} is still running.  Please retry after workflow completion.'
-        )
-        sys.exit(101)
-    if status == 'FAILURE':
-        print(f'Workflow {workflow_id} failed the qualitygate using mode {mode}.')
-        sys.exit(102)
-    if status == 'NOTEST':
-        print(f'Workflow {workflow_id} contains no test.')
-    else:
-        print(
-            f'Workflow {workflow_id} successfully passed the qualitygate using mode {mode}.'
-        )
-
-
 ########################################################################
 # Helpers
 
 
 def print_workflow_help(args: List[str]):
     """Display help."""
     if _is_command('run workflow', args):
         print(RUN_WORKFLOW_HELP)
     elif _is_command('get workflows', args):
         print(GET_WORKFLOWS_HELP)
     elif _is_command('get workflow', args):
         print(GET_WORKFLOW_HELP)
     elif _is_command('kill workflow', args):
         print(KILL_WORKFLOW_HELP)
-    elif _is_command('get qualitygate', args):
-        print(GET_QUALITYGATE_HELP)
     else:
         _error('Unknown command.  Use --help to list known commands.')
         sys.exit(1)
 
 
 def workflow_cmd():
     """Interact with workflows."""
@@ -971,14 +892,10 @@
         )
         read_configuration()
         get_workflow(sys.argv[3], '--watch' in sys.argv or '-w' in sys.argv)
     elif _is_command('kill workflow _', sys.argv):
         _ensure_options(sys.argv[4:])
         read_configuration()
         kill_workflow(sys.argv[3])
-    elif _is_command('get qualitygate _', sys.argv):
-        _ensure_options(sys.argv[4:], [('--mode', '-m')])
-        read_configuration()
-        get_qualitygate(sys.argv[3], _get_arg('--mode=') or _get_arg('-m=') or 'strict')
     else:
         _error('Unknown command.  Use --help to list known commands.')
         sys.exit(1)
```

## Comparing `opentf_tools-0.40.0.dist-info/LICENSE` & `opentf_tools-0.41.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `opentf_tools-0.40.0.dist-info/METADATA` & `opentf_tools-0.41.0.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: opentf-tools
-Version: 0.40.0
+Version: 0.41.0
 Summary: OpenTestFactory Orchestrator Tools
-Home-page: https://gitlab.com/opentestfactory/tools
+Home-page: https://opentestfactory.org/tools/
 Author: Martin Lafaix
 Author-email: mlafaix@henix.com
+Maintainer: Henix
+Maintainer-email: opentestfactory@henix.com
 License: Apache Software License (https://www.apache.org/licenses/LICENSE-2.0)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
@@ -32,15 +34,15 @@
 
 The package documentation is part of the
 [OpenTestFactory orchestrator](https://opentestfactory.org/tools/)
 documentation, in the **Tools** section.
 
 ## License
 
-Copyright 2021, 2022 Henix, henix.fr
+Copyright 2021, 2023 Henix, henix.fr
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
     http://www.apache.org/licenses/LICENSE-2.0
```

## Comparing `opentf_tools-0.40.0.dist-info/RECORD` & `opentf_tools-0.41.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-opentf/tools/ctl.py,sha256=59d875hZl21XlK7jloMn2mMKg0-Xk0uFwTdhgAoG3O0,27203
+opentf/tools/ctl.py,sha256=H930DQ1e0Iv3zwpL_ZiXXxiixVrF55A89N8MH9deftI,27544
 opentf/tools/ctlcommons.py,sha256=A1HKWqLQfQY1BFJA0ugXERK2klC23c8u0jn5lYz8uxE,7773
 opentf/tools/ctlconfig.py,sha256=dWY0RHgpa7GeC1GMMBniUctuCQKrnXyY-AcNm5xhrNQ,29452
 opentf/tools/ctlnetworking.py,sha256=92hK0xQSwocMiMitkEkdi5jmmJ-LEjg3_tbL2wj2Ggg,8138
-opentf/tools/ctlworkflows.py,sha256=x7SENaZNqNxn3mHWWiJcETzW32HpJH8-1hAO9HlGgfg,32205
+opentf/tools/ctlqualitygate.py,sha256=p4B7t-taQq-EeHxfBNOKsg66aJriEiIcCesGobLAcFc,10861
+opentf/tools/ctlworkflows.py,sha256=KwSPOrkpkt5-x0GUbdSqpXZBOQPp5qL2vkOAeewWGdg,29356
 opentf/tools/done.py,sha256=1X5s9IjpphD0LZvcQ0h36mKHkbLjjYDzlqqwat6kKdE,3188
 opentf/tools/ready.py,sha256=WHPdnWCMOKLCxLlF0FTCCpW-8y0BF7rrGCl7H2AJ-DM,9391
-opentf_tools-0.40.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-opentf_tools-0.40.0.dist-info/METADATA,sha256=F9rXjprST79TNgSemNhIrdnZFqS9MLboHSzCJpoqSgY,1737
-opentf_tools-0.40.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-opentf_tools-0.40.0.dist-info/entry_points.txt,sha256=u5qYtmUbgIMcq8360YobnI9CtDvrjptf4lDkmKojoa0,139
-opentf_tools-0.40.0.dist-info/top_level.txt,sha256=_gPuE6GTT6UNXy1DjtmQSfCcZb_qYA2vWmjg7a30AGk,7
-opentf_tools-0.40.0.dist-info/RECORD,,
+opentf_tools-0.41.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+opentf_tools-0.41.0.dist-info/METADATA,sha256=1jMCjx8fXbIFB7V3yqdvJbB20faAuoZ27HG5Yi267CM,1793
+opentf_tools-0.41.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+opentf_tools-0.41.0.dist-info/entry_points.txt,sha256=u5qYtmUbgIMcq8360YobnI9CtDvrjptf4lDkmKojoa0,139
+opentf_tools-0.41.0.dist-info/top_level.txt,sha256=_gPuE6GTT6UNXy1DjtmQSfCcZb_qYA2vWmjg7a30AGk,7
+opentf_tools-0.41.0.dist-info/RECORD,,
```

