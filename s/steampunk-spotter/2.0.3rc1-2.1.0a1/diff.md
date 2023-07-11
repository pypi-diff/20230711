# Comparing `tmp/steampunk_spotter-2.0.3rc1-py3-none-any.whl.zip` & `tmp/steampunk_spotter-2.1.0a1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,38 +1,43 @@
-Zip file size: 63297 bytes, number of entries: 36
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 11:39 spotter/__init__.py
+Zip file size: 65123 bytes, number of entries: 41
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 07:12 spotter/__init__.py
 -rw-r--r--  2.0 unx    22727 b- defN 23-Jun-09 10:45 spotter/api.py
--rw-r--r--  2.0 unx     5662 b- defN 23-Jun-27 06:19 spotter/cli.py
--rw-r--r--  2.0 unx    21661 b- defN 23-Jun-21 10:01 spotter/environment.py
--rw-r--r--  2.0 unx    24325 b- defN 23-Jun-21 10:42 spotter/parsing.py
+-rw-r--r--  2.0 unx     5923 b- defN 23-Jul-04 09:16 spotter/cli.py
+-rw-r--r--  2.0 unx    21522 b- defN 23-Jul-04 08:35 spotter/environment.py
 -rw-r--r--  2.0 unx     5697 b- defN 23-Jun-09 10:45 spotter/storage.py
 -rw-r--r--  2.0 unx     1311 b- defN 23-Jun-27 06:19 spotter/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 11:39 spotter/commands/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 07:12 spotter/commands/__init__.py
+-rw-r--r--  2.0 unx     3912 b- defN 23-Jul-04 09:16 spotter/commands/clear_config.py
 -rw-r--r--  2.0 unx     5468 b- defN 23-Jun-09 10:45 spotter/commands/clear_policies.py
+-rw-r--r--  2.0 unx     4025 b- defN 23-Jul-04 09:16 spotter/commands/get_config.py
 -rw-r--r--  2.0 unx     2446 b- defN 23-Jun-09 10:45 spotter/commands/login.py
 -rw-r--r--  2.0 unx     2253 b- defN 23-Jun-09 10:45 spotter/commands/logout.py
 -rw-r--r--  2.0 unx     1155 b- defN 23-May-29 11:32 spotter/commands/register.py
--rw-r--r--  2.0 unx    40462 b- defN 23-Jun-27 06:19 spotter/commands/scan.py
+-rw-r--r--  2.0 unx    40747 b- defN 23-Jul-04 08:35 spotter/commands/scan.py
+-rw-r--r--  2.0 unx     5257 b- defN 23-Jul-04 09:16 spotter/commands/set_config.py
 -rw-r--r--  2.0 unx     6692 b- defN 23-Jun-09 10:45 spotter/commands/set_policies.py
 -rw-r--r--  2.0 unx     3620 b- defN 23-Jun-09 10:45 spotter/commands/suggest.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 07:12 spotter/parsing/__init__.py
+-rw-r--r--  2.0 unx     4964 b- defN 23-Jul-04 08:35 spotter/parsing/noqa_comments.py
+-rw-r--r--  2.0 unx    25021 b- defN 23-Jul-11 06:41 spotter/parsing/parsing.py
 -rw-r--r--  2.0 unx       60 b- defN 23-Mar-14 07:59 spotter/reporting/__init__.py
--rw-r--r--  2.0 unx     3459 b- defN 23-Jun-27 09:55 spotter/reporting/report.py
--rw-r--r--  2.0 unx        0 b- defN 23-Jun-27 11:39 spotter/rewriting/__init__.py
+-rw-r--r--  2.0 unx     3461 b- defN 23-Jun-30 06:19 spotter/reporting/report.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 07:12 spotter/rewriting/__init__.py
 -rw-r--r--  2.0 unx     7545 b- defN 23-Apr-11 07:05 spotter/rewriting/models.py
--rw-r--r--  2.0 unx     7562 b- defN 23-Jun-21 10:01 spotter/rewriting/processor.py
+-rw-r--r--  2.0 unx     7588 b- defN 23-Jun-30 06:19 spotter/rewriting/processor.py
 -rw-r--r--  2.0 unx     1937 b- defN 23-Apr-11 07:05 spotter/rewriting/rewrite_action_inline.py
--rw-r--r--  2.0 unx     2318 b- defN 23-Apr-11 07:05 spotter/rewriting/rewrite_action_object.py
+-rw-r--r--  2.0 unx     2459 b- defN 23-Jul-06 06:23 spotter/rewriting/rewrite_action_object.py
 -rw-r--r--  2.0 unx      989 b- defN 23-Apr-11 07:05 spotter/rewriting/rewrite_always_run.py
 -rw-r--r--  2.0 unx      982 b- defN 23-Apr-11 07:05 spotter/rewriting/rewrite_fqcn.py
--rw-r--r--  2.0 unx     2087 b- defN 23-Jun-21 10:01 spotter/rewriting/rewrite_inline.py
--rw-r--r--  2.0 unx     2527 b- defN 23-Jun-21 10:01 spotter/rewriting/rewrite_local_action_inline.py
--rw-r--r--  2.0 unx     2312 b- defN 23-Jun-21 10:01 spotter/rewriting/rewrite_local_object.py
+-rw-r--r--  2.0 unx     2124 b- defN 23-Jun-30 06:19 spotter/rewriting/rewrite_inline.py
+-rw-r--r--  2.0 unx     2553 b- defN 23-Jun-30 06:19 spotter/rewriting/rewrite_local_action_inline.py
+-rw-r--r--  2.0 unx     2559 b- defN 23-Jul-06 06:23 spotter/rewriting/rewrite_local_object.py
 -rw-r--r--  2.0 unx      989 b- defN 23-Apr-11 07:05 spotter/rewriting/rewrite_module_inline.py
 -rw-r--r--  2.0 unx      888 b- defN 23-Apr-11 07:05 spotter/rewriting/rewrite_module_object.py
--rw-rw-rw-  2.0 unx    11358 b- defN 23-Jun-27 11:39 steampunk_spotter-2.0.3rc1.dist-info/LICENSE
--rw-r--r--  2.0 unx    23429 b- defN 23-Jun-27 11:39 steampunk_spotter-2.0.3rc1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-27 11:39 steampunk_spotter-2.0.3rc1.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 23-Jun-27 11:39 steampunk_spotter-2.0.3rc1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-27 11:39 steampunk_spotter-2.0.3rc1.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-27 11:39 steampunk_spotter-2.0.3rc1.dist-info/zip-safe
--rw-rw-r--  2.0 unx     3152 b- defN 23-Jun-27 11:39 steampunk_spotter-2.0.3rc1.dist-info/RECORD
-36 files, 215219 bytes uncompressed, 58193 bytes compressed:  73.0%
+-rw-rw-rw-  2.0 unx    11358 b- defN 23-Jul-11 07:12 steampunk_spotter-2.1.0a1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7269 b- defN 23-Jul-11 07:12 steampunk_spotter-2.1.0a1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 07:12 steampunk_spotter-2.1.0a1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 23-Jul-11 07:12 steampunk_spotter-2.1.0a1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-Jul-11 07:12 steampunk_spotter-2.1.0a1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Jul-11 07:12 steampunk_spotter-2.1.0a1.dist-info/zip-safe
+-rw-rw-r--  2.0 unx     3585 b- defN 23-Jul-11 07:12 steampunk_spotter-2.1.0a1.dist-info/RECORD
+41 files, 219232 bytes uncompressed, 59335 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -6,47 +6,62 @@
 
 Filename: spotter/cli.py
 Comment: 
 
 Filename: spotter/environment.py
 Comment: 
 
-Filename: spotter/parsing.py
-Comment: 
-
 Filename: spotter/storage.py
 Comment: 
 
 Filename: spotter/utils.py
 Comment: 
 
 Filename: spotter/commands/__init__.py
 Comment: 
 
+Filename: spotter/commands/clear_config.py
+Comment: 
+
 Filename: spotter/commands/clear_policies.py
 Comment: 
 
+Filename: spotter/commands/get_config.py
+Comment: 
+
 Filename: spotter/commands/login.py
 Comment: 
 
 Filename: spotter/commands/logout.py
 Comment: 
 
 Filename: spotter/commands/register.py
 Comment: 
 
 Filename: spotter/commands/scan.py
 Comment: 
 
+Filename: spotter/commands/set_config.py
+Comment: 
+
 Filename: spotter/commands/set_policies.py
 Comment: 
 
 Filename: spotter/commands/suggest.py
 Comment: 
 
+Filename: spotter/parsing/__init__.py
+Comment: 
+
+Filename: spotter/parsing/noqa_comments.py
+Comment: 
+
+Filename: spotter/parsing/parsing.py
+Comment: 
+
 Filename: spotter/reporting/__init__.py
 Comment: 
 
 Filename: spotter/reporting/report.py
 Comment: 
 
 Filename: spotter/rewriting/__init__.py
@@ -81,29 +96,29 @@
 
 Filename: spotter/rewriting/rewrite_module_inline.py
 Comment: 
 
 Filename: spotter/rewriting/rewrite_module_object.py
 Comment: 
 
-Filename: steampunk_spotter-2.0.3rc1.dist-info/LICENSE
+Filename: steampunk_spotter-2.1.0a1.dist-info/LICENSE
 Comment: 
 
-Filename: steampunk_spotter-2.0.3rc1.dist-info/METADATA
+Filename: steampunk_spotter-2.1.0a1.dist-info/METADATA
 Comment: 
 
-Filename: steampunk_spotter-2.0.3rc1.dist-info/WHEEL
+Filename: steampunk_spotter-2.1.0a1.dist-info/WHEEL
 Comment: 
 
-Filename: steampunk_spotter-2.0.3rc1.dist-info/entry_points.txt
+Filename: steampunk_spotter-2.1.0a1.dist-info/entry_points.txt
 Comment: 
 
-Filename: steampunk_spotter-2.0.3rc1.dist-info/top_level.txt
+Filename: steampunk_spotter-2.1.0a1.dist-info/top_level.txt
 Comment: 
 
-Filename: steampunk_spotter-2.0.3rc1.dist-info/zip-safe
+Filename: steampunk_spotter-2.1.0a1.dist-info/zip-safe
 Comment: 
 
-Filename: steampunk_spotter-2.0.3rc1.dist-info/RECORD
+Filename: steampunk_spotter-2.1.0a1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## spotter/cli.py

```diff
@@ -4,15 +4,16 @@
 import sys
 from pathlib import Path
 from typing import Dict, Union, Sequence, Optional, Any, NoReturn
 
 import colorama
 
 from spotter.api import ApiClient
-from spotter.commands import login, logout, register, scan, suggest, set_policies, clear_policies
+from spotter.commands import login, logout, register, scan, suggest, set_policies, clear_policies, get_config, \
+    set_config, clear_config
 from spotter.storage import Storage
 from spotter.utils import get_current_cli_version, validate_url
 
 
 class ArgParser(argparse.ArgumentParser):
     """An argument parser that displays help on error."""
 
@@ -91,15 +92,18 @@
     cmds = [
         (register.__name__.rsplit(".", maxsplit=1)[-1], register),
         (login.__name__.rsplit(".", maxsplit=1)[-1], login),
         (logout.__name__.rsplit(".", maxsplit=1)[-1], logout),
         (scan.__name__.rsplit(".", maxsplit=1)[-1], scan),
         (suggest.__name__.rsplit(".", maxsplit=1)[-1], suggest),
         (set_policies.__name__.rsplit(".", maxsplit=1)[-1], set_policies),
-        (clear_policies.__name__.rsplit(".", maxsplit=1)[-1], clear_policies)
+        (clear_policies.__name__.rsplit(".", maxsplit=1)[-1], clear_policies),
+        (get_config.__name__.rsplit(".", maxsplit=1)[-1], get_config),
+        (set_config.__name__.rsplit(".", maxsplit=1)[-1], set_config),
+        (clear_config.__name__.rsplit(".", maxsplit=1)[-1], clear_config)
     ]
     for command_name, module in cmds:
         # FIXME: Remove this if we decide that suggest command can be used standalone
         if command_name != "suggest":
             subparsers_metavar += f"{command_name.replace('_', '-')},"
         module.add_parser(subparsers)
```

## spotter/environment.py

```diff
@@ -7,17 +7,19 @@
 import sys
 from copy import deepcopy
 from pathlib import Path
 from typing import Optional, List, Dict, Any
 
 import pkg_resources
 import pydantic.dataclasses
-import yaml
+import ruamel.yaml as yaml
 from pydantic.json import pydantic_encoder
 
+from spotter.parsing.noqa_comments import SpotterNoqa
+
 
 class _EnvironmentDataclassConfig:
     extra = "forbid"
     # all dataclass arguments are optional because this is a discovery process
     # but use
     allow_mutation = False
 
@@ -27,23 +29,14 @@
     """Discovered Ansible versions (per edition, i.e. full, base, core)."""
 
     ansible_core: Optional[str] = None
     ansible_base: Optional[str] = None
     ansible: Optional[str] = None
 
 
-@pydantic.dataclasses.dataclass
-class SpotterNoqa:
-    """Data class with options for skipping and enforcing checks."""
-
-    event: str
-    subevent_code: Optional[str] = None
-    fqcn: Optional[str] = None
-
-
 @pydantic.dataclasses.dataclass(config=_EnvironmentDataclassConfig)
 class Environment:
     """User environment/workspace state discovery (retrieves system info and versions of installed packages)."""
 
     python_version: Optional[str] = None
     ansible_version: Optional[EnvironmentAnsibleVersion] = None
     installed_collections: Optional[List[Dict[str, Optional[str]]]] = None
```

## spotter/commands/scan.py

```diff
@@ -9,21 +9,22 @@
 import xml
 from enum import Enum
 from io import StringIO
 from pathlib import Path
 from typing import List, Dict, Any, Optional, Tuple, cast
 
 import pydantic.dataclasses
-import yaml
+import ruamel.yaml as yaml
 from colorama import Fore, Style
 from pydantic.json import pydantic_encoder
 
 from spotter.api import ApiClient
-from spotter.environment import Environment, SpotterNoqa
-from spotter.parsing import parse_ansible_artifacts, ParsingResult
+from spotter.environment import Environment
+from spotter.parsing.noqa_comments import SpotterNoqa
+from spotter.parsing.parsing import parse_ansible_artifacts, ParsingResult
 from spotter.reporting.report import JUnitXml
 from spotter.rewriting.models import RewriteSuggestion, CheckType
 from spotter.rewriting.processor import update_files
 from spotter.storage import Storage
 
 
 class DisplayLevel(Enum):
@@ -597,16 +598,16 @@
         """
         Format scan result as YAML.
 
         :param disable_docs_url: Disable outputting URL to documentation
         :return: A formatted string
         """
         stream = StringIO()
-        yaml.dump(
-            self._format_dict(disable_docs_url), stream=stream, indent=2, default_flow_style=False, sort_keys=False
+        yaml.round_trip_dump(
+            self._format_dict(disable_docs_url), stream=stream, indent=2, default_flow_style=False
         )
         return stream.getvalue()
 
     def _format_junit_xml(self, disable_docs_url: bool = False) -> str:
         """
         Format scan result as JUnitXML.
 
@@ -859,17 +860,21 @@
 
     cli_scan_args_skip_checks = []
     cli_scan_args_enforce_checks = []
     if environment.cli_scan_args:
         cli_scan_args_skip_checks = environment.cli_scan_args.get("skip_checks", [])
         cli_scan_args_enforce_checks = environment.cli_scan_args.get("enforce_checks", [])
     if skip_checks:
-        cli_scan_args_skip_checks = [SpotterNoqa(event=e) for e in skip_checks]
+        cli_scan_args_skip_checks = []
+        for skip_check in skip_checks:
+            cli_scan_args_skip_checks.extend(SpotterNoqa.parse_noqa_comment(skip_check, use_noqa_regex=False))
     if enforce_checks:
-        cli_scan_args_enforce_checks = [SpotterNoqa(event=e) for e in enforce_checks]
+        cli_scan_args_enforce_checks = []
+        for enforce_check in enforce_checks:
+            cli_scan_args_enforce_checks.extend(SpotterNoqa.parse_noqa_comment(enforce_check, use_noqa_regex=False))
 
     environment = environment.combine(
         Environment(cli_scan_args={
             "parse_values": include_values,
             # FIXME: Remove this deprecated option that is currently mandatory on backend.
             "include_values": include_values,
             "include_metadata": include_metadata,
```

## spotter/reporting/report.py

```diff
@@ -1,13 +1,13 @@
 """This is an interface for generating modular reports in various formats."""
 
+import itertools
+import sys
 import xml.etree.ElementTree as ET
 from abc import ABC, abstractmethod
-import itertools
-from xml.dom import minidom
 from typing import List, TYPE_CHECKING
 
 if TYPE_CHECKING:
     # cylic import
     from spotter.commands.scan import CheckResult
 
 
@@ -80,10 +80,12 @@
                 )
 
                 check_count += 1
 
             self.add_attribute(test_suite, "tests", str(check_count))
             self.add_attribute(test_suite, "errors", str(check_count))
 
-        return str(minidom.parseString(
-            ET.tostring(root_node, encoding="unicode", method="xml")
-        ).toprettyxml(indent="  ", encoding="utf-8").decode("utf-8"))
+        if sys.version_info >= (3, 9):
+            # ET.indent works only for Python >= 3.9
+            ET.indent(root_node)
+
+        return ET.tostring(root_node, encoding="unicode", method="xml")
```

## spotter/rewriting/processor.py

```diff
@@ -1,24 +1,24 @@
 """Entry point of rewriting functionality."""
-from typing import Optional, List, cast
 
-import os
 import itertools
+import os
+from typing import Optional, List, cast
 
-import yaml
+import ruamel.yaml as yaml
 
+from spotter.rewriting.models import Replacement, RewriteResult
+from spotter.rewriting.models import RewriteSuggestion
 from spotter.rewriting.rewrite_action_inline import RewriteActionInline
 from spotter.rewriting.rewrite_action_object import RewriteActionObject
 from spotter.rewriting.rewrite_always_run import RewriteAlwaysRun
 from spotter.rewriting.rewrite_fqcn import RewriteFqcn
 from spotter.rewriting.rewrite_inline import RewriteInline
 from spotter.rewriting.rewrite_local_action_inline import RewriteLocalActionInline
 from spotter.rewriting.rewrite_local_object import RewriteLocalActionObject
-from spotter.rewriting.models import Replacement, RewriteResult
-from spotter.rewriting.models import RewriteSuggestion
 
 
 class RewriteProcessor:
     """Factory that will use correct implementation depending on 'action' inside 'suggestion'."""
 
     rewriter_mapping = {
         "FIX_FQCN": RewriteFqcn,
@@ -166,8 +166,8 @@
                 continue
             if "collections" not in data or ("collections" in data and data["collections"] is None):
                 data["collections"] = []
 
             data["collections"].append({"name": collection_name, "version": collection_version})
             requirements_file.seek(0)
             requirements_file.truncate()
-            requirements_file.write(yaml.dump(data, default_flow_style=False))
+            requirements_file.write(yaml.round_trip_dump(data, default_flow_style=False))
```

## spotter/rewriting/rewrite_action_object.py

```diff
@@ -1,18 +1,20 @@
 """RewriteLocalActionInline implementation."""
 
 import re
 from typing import Optional, Tuple
 
+import yaml
+
 from spotter.rewriting.rewrite_module_object import RewriteModuleObject
 from spotter.rewriting.models import Replacement, RewriteBase, RewriteSuggestion
 
 
 class RewriteActionObject(RewriteBase):
-    """RewriteActionInline implementation."""
+    """RewriteActionObject implementation."""
 
     def get_regex(self, text_before: str) -> str:  # noqa: D102
         return rf"^(\s*({text_before}\s*):)"
 
     def remove_module_row(self, content: str, suggestion: RewriteSuggestion) -> Tuple[str, RewriteSuggestion]:
         """
         Remove module line from content.
@@ -25,32 +27,31 @@
             module_name = suggestion.suggestion_spec["data"]["module_name"]
             print(f"Applying suggestion failed: could not find \"{module_name}\" to replace.")
             raise TypeError()
         rewrite_result = module_replacement.apply()
         suggestion.end_mark += rewrite_result.diff_size
         return rewrite_result.content, suggestion
 
-    def get_indent_index(self, content: str, start_mark: int) -> int:
-        """
-        Get index of first character.
-
-        :param content: content block (usually a whole task).
-        :param start_mark: starting mark index of task in content
-        """
-        l_content = content[:start_mark]
-        index = l_content.find("\n") + 1
-        return start_mark - index
-
     def get_replacement(self, content: str, suggestion: RewriteSuggestion) -> Optional[Replacement]:  # noqa: D102
+        # 1. Remove line "module: ..." from task arguments
+        suggestion_data = suggestion.suggestion_spec["data"]
         content, suggestion = self.remove_module_row(content, suggestion)
         part = self.get_context(content, suggestion)
-        suggestion_data = suggestion.suggestion_spec["data"]
+
+        # 2. Add "delegate_to": localhost
+        if suggestion_data["additional"]:
+            index = self.get_indent_index(content, suggestion.start_mark)
+            additional = " " * index + yaml.dump(suggestion_data["additional"][0])
+            new_content = content[:suggestion.end_mark] + additional + content[suggestion.end_mark]
+        else:
+            new_content = content
+
+        # 3. Replace "action:" with "<module_name>:"
         before = suggestion_data["original_module_name"]
         after = suggestion_data["module_name"]
-
         regex = self.get_regex(before)
         match = re.search(regex, part, re.MULTILINE)
         if match is None:
             print("Applying suggestion failed: could not find string to replace.")
             return None
-        replacement = Replacement(content, suggestion, match, after)
+        replacement = Replacement(new_content, suggestion, match, after)
         return replacement
```

## spotter/rewriting/rewrite_inline.py

```diff
@@ -1,13 +1,13 @@
 """RewriteInline implementation."""
 
 import re
 from typing import Optional
 
-import yaml
+import ruamel.yaml as yaml
 
 from spotter.rewriting.models import Replacement, RewriteBase, RewriteSuggestion
 
 
 class RewriteInline(RewriteBase):
     """RewriteInline implementation."""
 
@@ -33,17 +33,17 @@
         indent = self.get_indent_index(content, suggestion.start_mark)
         before = suggestion_dict["data"]["module_name"]
         offset = 2
 
         args = ""
         variables = ""
         if "args" in suggestion_dict["data"] and suggestion_dict["data"]["args"]:
-            args = self.get_indent_block(yaml.dump(suggestion_dict["data"]["args"]), offset, "\n")
+            args = self.get_indent_block(yaml.round_trip_dump(suggestion_dict["data"]["args"]), offset, "\n")
         if "vars" in suggestion_dict["data"] and suggestion_dict["data"]["vars"]:
-            variables = "\n" + yaml.dump({"vars": suggestion_dict["data"]["vars"]})
+            variables = "\n" + yaml.round_trip_dump({"vars": suggestion_dict["data"]["vars"]})
         after = self.get_indent_block("".join([args, variables]), indent, "\n").rstrip("\n")
 
         regex = self.get_regex(before)
         match = re.search(regex, part, re.MULTILINE)
         if match is None:
             print("Applying suggestion failed: could not find string to replace.")
             return None
```

## spotter/rewriting/rewrite_local_action_inline.py

```diff
@@ -1,16 +1,16 @@
 """RewriteActionInline implementation."""
 
 import re
 from typing import Optional, Tuple
 
-import yaml
+import ruamel.yaml as yaml
 
-from spotter.rewriting.rewrite_module_inline import RewriteModuleInline
 from spotter.rewriting.models import Replacement, RewriteBase, RewriteSuggestion
+from spotter.rewriting.rewrite_module_inline import RewriteModuleInline
 
 
 class RewriteLocalActionInline(RewriteBase):
     """RewriteActionInline implementation."""
 
     def get_regex(self, text_before: str) -> str:  # noqa: D102
         return rf"^(\s*({text_before}\s*):)"
@@ -37,15 +37,15 @@
 
         # 1. remove module name from arguments
         content, suggestion = self.remove_module_name(content, suggestion)
 
         # 2. add delegate_to: localhost
         suggestion_data = suggestion.suggestion_spec["data"]
         index = self.get_indent_index(content, suggestion.start_mark)
-        additional = start_char + " " * index + yaml.dump(suggestion_data["additional"][0])
+        additional = start_char + " " * index + yaml.round_trip_dump(suggestion_data["additional"][0])
         new_content = content[:suggestion.end_mark] + additional + content[suggestion.end_mark:]
         suggestion.end_mark += len(additional)
 
         # 3. replace local_action keyword with module name
         part = self.get_context(content, suggestion)
         before = suggestion_data["original_module_name"]
         after = suggestion_data["module_name"]
```

## spotter/rewriting/rewrite_local_object.py

```diff
@@ -1,16 +1,16 @@
 """RewriteLocalActionInline implementation."""
 
 import re
 from typing import Optional, Tuple
 
-import yaml
+import ruamel.yaml as yaml
 
-from spotter.rewriting.rewrite_module_object import RewriteModuleObject
 from spotter.rewriting.models import Replacement, RewriteBase, RewriteSuggestion
+from spotter.rewriting.rewrite_module_object import RewriteModuleObject
 
 
 class RewriteLocalActionObject(RewriteBase):
     """RewriteLocalActionInline implementation."""
 
     def get_regex(self, text_before: str) -> str:  # noqa: D102
         return rf"^(\s*({text_before}\s*):)"
@@ -28,27 +28,32 @@
             print(f'Applying suggestion failed: could not find "{module_name}" to replace.')
             raise TypeError()
         rewrite_result = module_replacement.apply()
         suggestion.end_mark += rewrite_result.diff_size
         return rewrite_result.content, suggestion
 
     def get_replacement(self, content: str, suggestion: RewriteSuggestion) -> Optional[Replacement]:  # noqa: D102
-        # 1. Remove line "module: ..." from task arguments
-        suggestion_data = suggestion.suggestion_spec["data"]
+        # 0. clean spaces in suggestion
+        suggestion, start_char = self.shorten_match(content, suggestion)
+
+        # 1. remove module name from arguments
         content, suggestion = self.remove_module_row(content, suggestion)
-        part = self.get_context(content, suggestion)
 
-        # 2. Add "delegate_to": localhost
+        # 2. add delegate_to: localhost
+        suggestion_data = suggestion.suggestion_spec["data"]
         index = self.get_indent_index(content, suggestion.start_mark)
-        additional = " " * index + yaml.dump(suggestion_data["additional"][0])
-        new_content = content + additional
+        additional = start_char + " " * index + yaml.round_trip_dump(suggestion_data["additional"][0])
+        new_content = content[:suggestion.end_mark] + additional + content[suggestion.end_mark:]
+        suggestion.end_mark += len(additional)
 
-        # 3. Replace "action:" with "<module_name>:"
+        # 3. replace local_action keyword with module name
+        part = self.get_context(content, suggestion)
         before = suggestion_data["original_module_name"]
         after = suggestion_data["module_name"]
+
         regex = self.get_regex(before)
         match = re.search(regex, part, re.MULTILINE)
         if match is None:
             print("Applying suggestion failed: could not find string to replace.")
             return None
         replacement = Replacement(new_content, suggestion, match, after)
         return replacement
```

## Comparing `spotter/parsing.py` & `spotter/parsing/parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Provide methods for parsing Ansible artifacts."""
-
 import sys
 import uuid
 from enum import Enum
 from pathlib import Path
 from typing import Dict, List, Tuple, Any, cast, Optional, Union, Callable
 
 import pydantic.dataclasses
-import yaml
+import ruamel.yaml as yaml
 from detect_secrets.core.secrets_collection import SecretsCollection
 from detect_secrets.settings import default_settings
 from pydantic.json import pydantic_encoder
-from yaml import MappingNode
+
+from spotter.parsing.noqa_comments import match_comments_with_task
 
 
 @pydantic.dataclasses.dataclass
 class SpotterObfuscated:
     """Class where we save metadata about which fields were obfuscated."""
 
     type: str
@@ -50,15 +50,16 @@
         Remove sensitive data from input tasks.
 
         :return: Cleaned list of input tasks
         """
         return [
             {
                 "task_id": t["task_id"],
-                "task_args": t["task_args"]
+                "task_args": t["task_args"],
+                "spotter_noqa": t["spotter_noqa"]
             } for t in self.tasks
         ]
 
     def playbooks_without_metadata(self) -> List[Dict[str, Union[str, List[Dict[str, Any]]]]]:
         """
         Remove sensitive data from input playbooks.
 
@@ -74,53 +75,50 @@
                     }
                     for x in t["plays"]
                 ]
             } for t in self.playbooks
         ]
 
 
-class SafeLineLoader(yaml.loader.SafeLoader):
+class SafeLineLoader(yaml.RoundTripLoader):  # type: ignore
     """YAML loader that adds line numbers."""
 
-    yaml_implicit_resolvers = {
-        k: [r for r in v if r[0] != "tag:yaml.org,2002:timestamp"] for
-        k, v in yaml.SafeLoader.yaml_implicit_resolvers.items()
-    }
-
-    def __init__(self, stream: Any) -> None:
+    def __init__(self, stream: yaml.StreamTextType, version: Optional[yaml.VersionType] = None,
+                 preserve_quotes: Optional[bool] = None) -> None:
         """
         Initialize the YAML loader.
 
         :param stream: YAML stream
         """
-        super().__init__(stream)
+        super().__init__(stream, version, preserve_quotes)
         # add constructors for !vault and !unsafe tags, throw away their values because they are sensitive
         construct_unsafe_or_vault: Callable[[yaml.SafeLoader, yaml.Node], Any] = lambda loader, node: None
         self.add_constructor("!unsafe", construct_unsafe_or_vault)
         self.add_constructor("!vault", construct_unsafe_or_vault)
+        self.add_constructor("tag:yaml.org,2002:timestamp", yaml.SafeLoader.construct_yaml_str)
 
-    def construct_mapping(self, node: MappingNode, deep: bool = False) -> Dict[Any, Any]:
+    def construct_mapping(self, node: yaml.MappingNode, maptyp: Any, deep: bool = False) -> Dict[Any, Any]:
         """
         Overridden the original construct_mapping method.
 
         :param node: YAML node object
+        :param maptyp: YAML map type
         :param deep: Build objects recursively
         :return: A dict with loaded YAML
         """
-        mapping: Dict[Any, Any] = \
-            cast(Dict[Any, Any], super().construct_mapping(node, deep=deep))
+        super().construct_mapping(node, maptyp, deep=deep)
 
         meta = {}
         meta["__line__"] = node.start_mark.line + 1
         meta["__column__"] = node.start_mark.column + 1
         meta["__start_mark_index__"] = node.start_mark.index
         meta["__end_mark_index__"] = node.end_mark.index
-        mapping["__meta__"] = meta
+        maptyp["__meta__"] = meta
 
-        return mapping
+        return maptyp  # type: ignore
 
 
 class AnsibleArtifact(Enum):
     """Enum that can distinct between different Ansible artifacts (i.e., types of Ansible files)."""
 
     TASK = 1
     PLAYBOOK = 2
@@ -169,15 +167,15 @@
     Load YAML file and return corresponding Python object if parsing has been successful.
 
     :param path: Path to YAML file
     :return: Parsed YAML file as a Python object
     """
     with path.open("r", encoding="utf-8") as stream:
         try:
-            return yaml.load(stream, Loader=SafeLineLoader)
+            return yaml.load(stream, SafeLineLoader, "1.1")
         except yaml.YAMLError as e:
             print(e, file=sys.stderr)
             return None
         except UnicodeDecodeError as e:
             print(f"{stream.name}: {e}", file=sys.stderr)
             return None
 
@@ -286,14 +284,16 @@
 
     :param task: Ansible task
     :param params_to_keep: List of parameters that should not be removed
     """
     for task_key in task:
         if isinstance(task[task_key], dict):
             for key in list(task[task_key]):
+                if task_key in ["action", "local_action"] and key == "module":
+                    continue
                 if key != "__meta__":
                     task[task_key][key] = None
         else:
             if not params_to_keep or task_key not in params_to_keep:
                 task[task_key] = None
 
 
@@ -352,61 +352,69 @@
 
     if isinstance(yaml_key, str) and any(secret_value in yaml_key for secret_value in secret_values):
         return None, [SpotterObfuscated(type="str", path=[])]
 
     return yaml_key, []
 
 
+# pylint: disable=too-many-locals
 def _parse_tasks(tasks: List[Dict[str, Any]], file_name: str, parse_values: bool = False) -> List[Dict[str, Any]]:
     """
     Parse Ansible tasks and prepare them for scanning.
 
     :param tasks: List of Ansible task dicts
     :param file_name: Name of the original file with tasks
     :param parse_values: True if also read values (apart from parameter names) from task parameters, False if not
     :return: List of parsed Ansible tasks
     """
     try:
         parsed_tasks = []
         secrets = detect_secrets_in_file(file_name)
+
         for task in [t for t in tasks if t is not None]:
-            _clean_action_and_local_action(task, parse_values)
+            # _clean_action_and_local_action(task, parse_values)
 
             contains_block_section = False
             for block_section in ("block", "rescue", "always"):
                 if block_section in task:
                     contains_block_section = True
                     if isinstance(task[block_section], list):
                         parsed_tasks += _parse_tasks(task[block_section], file_name, parse_values)
             if contains_block_section:
                 continue
 
-            task_meta = task.pop("__meta__", None)
+            if isinstance(task, yaml.CommentedMap):
+                match_comments_with_task(task)
+
+            task_copy: Dict[str, Any] = dict(task)
+            task_meta = task_copy.pop("__meta__", None)
+            task_noqa = task_copy.pop("__noqa__", [])
             obfuscated: ObfuscatedInput = []
 
             if not parse_values:
-                _remove_parameter_values(task)
+                _remove_parameter_values(task_copy)
             else:
-                for task_key in task:
-                    task[task_key], hidden = _remove_secret_parameter_values(task[task_key], secrets)
+                for task_key in task_copy:
+                    task_copy[task_key], hidden = _remove_secret_parameter_values(task_copy[task_key], secrets)
                     obfuscated.extend(item.to_parent(task_key) for item in hidden)
 
             meta = {
                 "file": file_name,
                 "line": task_meta["__line__"],
                 "column": task_meta["__column__"],
                 "start_mark_index": task_meta["__start_mark_index__"],
                 "end_mark_index": task_meta["__end_mark_index__"]
             }
 
             task_dict = {
                 "task_id": str(uuid.uuid4()),
-                "task_args": _remove_deep_metadata(task),
+                "task_args": _remove_deep_metadata(task_copy),
                 "spotter_metadata": meta,
-                "spotter_obfuscated": [pydantic_encoder(x) for x in obfuscated]
+                "spotter_obfuscated": [pydantic_encoder(x) for x in obfuscated],
+                "spotter_noqa": [pydantic_encoder(x) for x in task_noqa]
             }
             parsed_tasks.append(task_dict)
 
         return parsed_tasks
     except Exception as e:  # pylint: disable=broad-except
         print(f"Error while parsing tasks from {file_name}: {e}", file=sys.stderr)
         return []
@@ -468,24 +476,25 @@
     parsed_plays = []
     for play in [p for p in playbook if p is not None]:
         tasks = play.pop("tasks", [])
         pre_tasks = play.pop("pre_tasks", [])
         post_tasks = play.pop("post_tasks", [])
         handlers = play.pop("handlers", [])
 
-        if not isinstance(tasks, list):
-            tasks = []
-        if not isinstance(handlers, list):
-            handlers = []
-        if not isinstance(post_tasks, list):
-            post_tasks = []
-        if not isinstance(pre_tasks, list):
-            pre_tasks = []
+        all_tasks = yaml.CommentedSeq()
+        if isinstance(tasks, list):
+            all_tasks.extend(tasks)
+        if isinstance(pre_tasks, list):
+            all_tasks.extend(pre_tasks)
+        if isinstance(post_tasks, list):
+            all_tasks.extend(post_tasks)
+        if isinstance(handlers, list):
+            all_tasks.extend(handlers)
 
-        parsed_tasks += _parse_tasks(tasks + handlers + pre_tasks + post_tasks, file_name, parse_values)
+        parsed_tasks += _parse_tasks(all_tasks, file_name, parse_values)
         parsed_plays.append(_parse_play(play, file_name, parse_values))
 
     parsed_playbook = {"playbook_id": str(uuid.uuid4()), "plays": parsed_plays}
     return parsed_tasks, [parsed_playbook]
 
 
 def _parse_role(directory: Path, parse_values: bool = False) -> Tuple[List[Dict[str, Any]], List[Dict[str, Any]]]:
```

## Comparing `steampunk_spotter-2.0.3rc1.dist-info/LICENSE` & `steampunk_spotter-2.1.0a1.dist-info/LICENSE`

 * *Files identical despite different names*

