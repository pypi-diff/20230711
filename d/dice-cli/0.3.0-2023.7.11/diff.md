# Comparing `tmp/dice_cli-0.3.0.tar.gz` & `tmp/dice_cli-2023.7.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dice_cli-0.3.0.tar", last modified: Fri Jan 14 15:06:33 2022, max compression
+gzip compressed data, was "dice_cli-2023.7.11.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dice_cli-0.3.0.tar` & `dice_cli-2023.7.11.tar`

### file list

```diff
@@ -1,22 +1,38 @@
--rw-r--r--   0        0        0     1522 2022-01-14 15:06:26.071479 dice_cli-0.3.0/LICENSE
--rw-r--r--   0        0        0     1433 2022-01-14 15:06:26.071479 dice_cli-0.3.0/README.md
--rw-r--r--   0        0        0     2306 2022-01-14 15:06:26.071479 dice_cli-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       50 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/__init__.py
--rw-r--r--   0        0        0      219 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/_io/__init__.py
--rw-r--r--   0        0        0      951 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/_io/_csv.py
--rw-r--r--   0        0        0      832 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/admin/__init__.py
--rw-r--r--   0        0        0     1252 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/admin/_print_unused_id_ranges.py
--rw-r--r--   0        0        0      898 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/admin/_print_used_id_ranges.py
--rw-r--r--   0        0        0     1543 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/admin/_scan_groups_and_users.py
--rw-r--r--   0        0        0     1245 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/admin/report/__init__.py
--rw-r--r--   0        0        0     1069 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/admin/report/_storage.py
--rw-r--r--   0        0        0      233 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/benchmark/__init__.py
--rw-r--r--   0        0        0      268 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/docs/__init__.py
--rw-r--r--   0        0        0      543 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/fs/__init__.py
--rw-r--r--   0        0        0      196 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/fs/copy_from_local.py
--rw-r--r--   0        0        0     1950 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/info/__init__.py
--rw-r--r--   0        0        0      359 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/job/__init__.py
--rw-r--r--   0        0        0     2459 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/logger.py
--rw-r--r--   0        0        0     2319 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/main.py
--rw-r--r--   0        0        0        0 2022-01-14 15:06:26.071479 dice_cli-0.3.0/src/dice_cli/py.typed
--rw-r--r--   0        0        0     3015 1970-01-01 00:00:00.000000 dice_cli-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1522 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/LICENSE
+-rw-r--r--   0        0        0     3558 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/README.md
+-rw-r--r--   0        0        0     2482 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/pyproject.toml
+-rw-r--r--   0        0        0       55 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/__init__.py
+-rw-r--r--   0        0        0     1501 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/_date.py
+-rw-r--r--   0        0        0      279 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/_io/__init__.py
+-rw-r--r--   0        0        0     1172 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/_io/_csv.py
+-rw-r--r--   0        0        0      655 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/_io/_remote.py
+-rw-r--r--   0        0        0      953 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/__init__.py
+-rw-r--r--   0        0        0     1256 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/_print_unused_id_ranges.py
+-rw-r--r--   0        0        0      902 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/_print_used_id_ranges.py
+-rw-r--r--   0        0        0     1547 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/_scan_groups_and_users.py
+-rw-r--r--   0        0        0      777 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/deploy/__init__.py
+-rw-r--r--   0        0        0     2659 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/deploy/_hdfs_mount.py
+-rw-r--r--   0        0        0     2783 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/investigate/__init__.py
+-rw-r--r--   0        0        0     6411 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/report/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/report/_consistency_check_grid.py
+-rw-r--r--   0        0        0      735 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/report/_dns.py
+-rw-r--r--   0        0        0     4942 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/report/_inventory.py
+-rw-r--r--   0        0        0     3845 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/report/_network.py
+-rw-r--r--   0        0        0     1122 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/admin/report/_storage.py
+-rw-r--r--   0        0        0     1015 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/benchmark/__init__.py
+-rw-r--r--   0        0        0      173 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/cache.py
+-rw-r--r--   0        0        0     1670 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/check/__init__.py
+-rw-r--r--   0        0        0     1783 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/check/_environment.py
+-rw-r--r--   0        0        0     1138 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/dicectl.py
+-rw-r--r--   0        0        0      268 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/docs/__init__.py
+-rw-r--r--   0        0        0     1044 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/fs/__init__.py
+-rw-r--r--   0        0        0      196 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/fs/_copy_from_local.py
+-rw-r--r--   0        0        0     1964 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/info/__init__.py
+-rw-r--r--   0        0        0      359 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/job/__init__.py
+-rw-r--r--   0        0        0     2459 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/logger.py
+-rw-r--r--   0        0        0     4166 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/main.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/migrate/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/py.typed
+-rw-r--r--   0        0        0        0 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/restore/__init__.py
+-rw-r--r--   0        0        0       81 2023-07-11 14:00:44.029929 dice_cli-2023.7.11/src/dice_cli/sync/__init__.py
+-rw-r--r--   0        0        0     5261 1970-01-01 00:00:00.000000 dice_cli-2023.7.11/PKG-INFO
```

### Comparing `dice_cli-0.3.0/LICENSE` & `dice_cli-2023.7.11/LICENSE`

 * *Files identical despite different names*

### Comparing `dice_cli-0.3.0/pyproject.toml` & `dice_cli-2023.7.11/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -23,30 +23,33 @@
   "Topic :: Scientific/Engineering",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "License :: OSI Approved :: BSD License",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.6",
-  "Programming Language :: Python :: 3.7",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Development Status :: 1 - Planning",
 ]
 
 
 dynamic = ["version"]
 dependencies = [
   "colorama >=0.4.0",
-  "dice-lib >=0.3.1",
+  "dice-lib >=0.5.0",
+  "diskcache >=5.4.0",
+  "htcondor >=9.0.0",
+  "plumbum >=1.7.2",
+  "prettytable >=3.2.0",
   "tabulate >=0.8.9",
+  "tqdm < 5.0.0",
   "typer >=0.4.0",
   "typing_extensions >=3.7",
+  "requests < 3.0.0",
   "rich >=10.12.0",
   "shellingham >=1.4.0",
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest >=6",
@@ -56,14 +59,17 @@
 ]
 docs = [
   "Sphinx~=3.0",
   "myst_parser>=0.13",
   "sphinx-book-theme>=0.1.0",
   "sphinx_copybutton",
 ]
+admin = [
+  "python-nmap >=0.7.1",
+]
 
 [project.urls]
 homepage = "https://github.com/uobdic/dice-cli"
 
 
 [tool.pytest.ini_options]
 addopts = "-ra"
@@ -73,15 +79,15 @@
 
 [tool.pycln]
 all = true
 
 
 [tool.mypy]
 files = "src"
-python_version = "3.8"
+python_version = "3.9"
 warn_unused_configs = true
 
 disallow_any_generics = true
 disallow_subclassing_any = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
@@ -105,7 +111,10 @@
 
 [tool.isort]
 profile = "black"
 known_third_party = ["typer", "click"]
 
 [project.scripts]
 dice = "dice_cli.main:main"
+dicectl = "dice_cli.dicectl:main"
+dice-adm = "dice_cli.dicectl:main"
+# dicefs = "dice_cli.dicefs:main" # once `dice fs` is mature enough
```

### Comparing `dice_cli-0.3.0/src/dice_cli/_io/_csv.py` & `dice_cli-2023.7.11/src/dice_cli/_io/_csv.py`

 * *Files 15% similar despite different names*

```diff
@@ -27,7 +27,14 @@
 def write_list_data_to_csv(
     data: List[Any], fieldnames: List[str], output_file: Path
 ) -> None:
     with open(output_file, "w") as f:
         writer = csv.writer(f)
         writer.writerow(fieldnames)
         writer.writerows(data)
+
+
+def read_list_data_from_csv(filename: Path) -> List[Dict[str, Any]]:
+    with open(filename) as f:
+        reader = csv.DictReader(f, delimiter=",", quotechar='"')
+        data = [row for row in reader]
+    return data
```

### Comparing `dice_cli-0.3.0/src/dice_cli/admin/__init__.py` & `dice_cli-2023.7.11/src/dice_cli/admin/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import typer
 
 from . import (
     _print_unused_id_ranges,
     _print_used_id_ranges,
     _scan_groups_and_users,
+    deploy,
+    investigate,
     report,
 )
 
 app = typer.Typer(help="DICE admin commands")
+app.add_typer(deploy.app, name="deploy")
+app.add_typer(investigate.app, name="investigate")
 app.add_typer(report.app, name="report")
 
 
 @app.command()
 def scan_groups_and_users() -> None:
     _scan_groups_and_users.main()
```

### Comparing `dice_cli-0.3.0/src/dice_cli/admin/_print_unused_id_ranges.py` & `dice_cli-2023.7.11/src/dice_cli/admin/_print_unused_id_ranges.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from itertools import groupby
 from pathlib import Path
 from typing import List
 
-from dice_lib.ranges import as_range, groupby_inverse_range
-
 from .._io import read_ints_from_csv
 from ..logger import admin_logger
 
 
 def _read_userids(filename: str) -> List[int]:
     return read_ints_from_csv(Path(filename), "uid")
 
@@ -16,14 +14,16 @@
     return read_ints_from_csv(Path(filename), "gid")
 
 
 def main(users_file: str, group_file: str) -> None:
     """
     Prints the unused ID ranges for all groups and users.
     """
+    from dice_lib.ranges import as_range, groupby_inverse_range
+
     userids = _read_userids(users_file)
     groupids = _read_groupids(group_file)
 
     unused_uids = sorted({i for i in range(max(userids))} - set(userids))
     unused_uids_ranges = ",".join(
         as_range(g) for _, g in groupby(unused_uids, key=groupby_inverse_range)
     )
```

### Comparing `dice_cli-0.3.0/src/dice_cli/admin/_print_used_id_ranges.py` & `dice_cli-2023.7.11/src/dice_cli/admin/_print_used_id_ranges.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from itertools import groupby
 from pathlib import Path
 from typing import List
 
-from dice_lib.ranges import as_range, groupby_range
-
 from .._io import read_ints_from_csv
 from ..logger import admin_logger
 
 
 def _read_userids(filename: str) -> List[int]:
     return read_ints_from_csv(Path(filename), "uid")
 
@@ -16,14 +14,16 @@
     return read_ints_from_csv(Path(filename), "gid")
 
 
 def main(users_file: str, group_file: str) -> None:
     """
     Prints the used ID ranges for all groups and users.
     """
+    from dice_lib.ranges import as_range, groupby_range
+
     userids = _read_userids(users_file)
     groupids = _read_groupids(group_file)
 
     uid_ranges = ",".join(as_range(g) for _, g in groupby(userids, groupby_range))
     gid_ranges = ",".join(as_range(g) for _, g in groupby(groupids, groupby_range))
 
     admin_logger.info(f"Used UID ranges: {uid_ranges}")
```

### Comparing `dice_cli-0.3.0/src/dice_cli/admin/_scan_groups_and_users.py` & `dice_cli-2023.7.11/src/dice_cli/admin/_scan_groups_and_users.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from pathlib import Path
 from typing import Any, Dict, List
 
-from dice_lib.host import current_fqdn
-
 from .._io import write_list_data_as_dict_to_csv
 from ..logger import admin_logger
 
 
 def _read_groups() -> List[Dict[str, str]]:
     with open("/etc/group") as f:
         group_lines = f.readlines()
@@ -37,14 +35,16 @@
 def _write_groups_to_csv(
     groups: List[Dict[str, Any]], output_file: str = "/tmp/groups.csv"
 ) -> None:
     write_list_data_as_dict_to_csv(groups, ["name", "gid"], Path(output_file))
 
 
 def main() -> None:
+    from dice_lib.host import current_fqdn
+
     groups = _read_groups()
     users = _read_users()
     hostname = current_fqdn()
 
     user_output = f"/tmp/00_{hostname}_users.csv"
     group_output = f"/tmp/01_{hostname}_groups.csv"
```

### Comparing `dice_cli-0.3.0/src/dice_cli/admin/report/_storage.py` & `dice_cli-2023.7.11/src/dice_cli/admin/report/_storage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from pathlib import Path
 from typing import Any, List, Tuple
 
-from dice_lib.fs import get_owner, size_of_paths
+from dice_lib.fs import FSClient
 from dice_lib.user import get_user_full_name
 
 
-def _resolve_usernames_in_report(report: List[Any]) -> List[Any]:
+def _resolve_usernames_in_report(report: List[Any], fs: FSClient) -> List[Any]:
     new_report = []
     for row in report:
         path = row[0]
-        owner = get_owner(path)
+        owner = fs.get_owner(path)
         full_name = get_user_full_name(owner)
         new_report.append(row + (owner, full_name))
     return new_report
 
 
 def generate_storage_report(
     paths: List[Path], resolve_usernames: bool
@@ -21,14 +21,16 @@
     """
     Generates a storage report for a list of paths.
 
     :param paths: List of paths to generate a report for.
     :param resolve_usernames: Whether to resolve usernames to full names.
     :return: Tuple of (headers, report)
     """
+    fs = FSClient()
+
     headers = ["Path", "Size [B]", "Size [human-readable]", "Unit [human-readable]"]
-    report = size_of_paths(paths)
+    report = fs.size_of_paths([str(path) for path in paths])
     if resolve_usernames:
         headers += ["Owner", "Owner full name"]
-        report = _resolve_usernames_in_report(report)
+        report = _resolve_usernames_in_report(report, fs)
 
     return headers, report
```

### Comparing `dice_cli-0.3.0/src/dice_cli/info/__init__.py` & `dice_cli-2023.7.11/src/dice_cli/info/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Dict, List
 
 import typer
-from dice_lib import parameters as dice_params
+from dice_lib import load_config
 
 from ..logger import user_logger
 
+dice_params = load_config()
 app = typer.Typer(help="DICE info commands")
 
 
 def _print_storage_element_info(
     storage_elemet: str, se_endpoints: Dict[str, str], se_mount_point: str
 ) -> None:
     user_logger.info(f"Storage element: {storage_elemet}")
```

### Comparing `dice_cli-0.3.0/src/dice_cli/logger.py` & `dice_cli-2023.7.11/src/dice_cli/logger.py`

 * *Files identical despite different names*

### Comparing `dice_cli-0.3.0/src/dice_cli/main.py` & `dice_cli-2023.7.11/src/dice_cli/dicectl.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,30 +1,15 @@
 import logging
-from typing import Any, Optional
+from typing import Any
 
-import dice_lib.parameters as dice_params
 import rich
 import typer
 
-from . import __version__, admin, benchmark, docs, info, job
-from .logger import admin_logger, console_handler, user_logger
-
-
-def user_callback(
-    verbose: bool = typer.Option(False, "--verbose", "-v", help="Verbose output"),
-    debug: bool = typer.Option(False, "--debug", "-d", help="Debug output"),
-) -> Any:
-    # verbose is debug
-    verbose = debug or verbose
-    debug = verbose
-
-    if debug:
-        user_logger.setLevel(logging.DEBUG)
-        # workaround for rich
-        console_handler.setLevel(logging.DEBUG)
+from . import __version__, _date, admin
+from .logger import admin_logger, console_handler
 
 
 def admin_callback(
     verbose: bool = typer.Option(False, "--verbose", "-v", help="Verbose output"),
     debug: bool = typer.Option(False, "--debug", "-d", help="Debug output"),
 ) -> Any:
     # verbose is debug
@@ -33,49 +18,37 @@
 
     if debug:
         admin_logger.setLevel(logging.DEBUG)
         # workaround for rich
         console_handler.setLevel(logging.DEBUG)
 
 
-app = typer.Typer()
-app.add_typer(admin.app, name="admin", callback=admin_callback)
-app.add_typer(benchmark.app, name="benchmark", callback=user_callback)
-app.add_typer(docs.app, name="docs", callback=user_callback)
-app.add_typer(info.app, name="info", callback=user_callback)
-app.add_typer(job.app, name="job", callback=user_callback)
+app = admin.app
+app.callback = admin_callback
 
 
 @app.command()
 def version() -> None:
     """
     Show version
     """
     rich.print(f"[blue]DICE CLI Version[/]: [magenta]{__version__}[/]")
 
 
 @app.command()
-def glossary(
-    word: Optional[str] = typer.Argument(None, help="Word to search for"),
-    print_all: bool = typer.Option(
-        False, "--all", "-a", help="Print all glossary entries"
-    ),
+def date(
+    date_format: _date.DateOptions = typer.Option(
+        _date.DateOptions.ISO8601_JUST_Y_M_D,
+        "--format",
+        "-f",
+        help="Format to print",
+        case_sensitive=False,
+    )
 ) -> None:
     """
-    Show the meaning of a given word (in DICE context)
+    Print the current date in ISO8601 format
     """
-    if print_all:
-        rich.print("[blue]All items[/]:")
-        for w, meaning in dice_params.GLOSSARY.items():
-            rich.print(f"[blue]{w}[/]: [magenta]{meaning}[/]")
-        return
-
-    if word not in dice_params.GLOSSARY:
-        rich.print(f"[red]Word '{word}' not found[/]")
-        typer.echo("To list all glossary items use 'dice glossary -a'")
-        return
-
-    rich.print(f"[blue]{word}[/]: [magenta]{dice_params.GLOSSARY[word]}[/]")
+    rich.print(_date.formatted_date(date_format))
 
 
 def main() -> Any:
     return app()
```

