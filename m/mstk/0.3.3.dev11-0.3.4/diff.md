# Comparing `tmp/mstk-0.3.3.dev11.tar.gz` & `tmp/mstk-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mstk-0.3.3.dev11.tar", last modified: Thu Feb  2 07:33:48 2023, max compression
+gzip compressed data, was "mstk-0.3.4.tar", last modified: Tue Jul 11 07:49:11 2023, max compression
```

## Comparing `mstk-0.3.3.dev11.tar` & `mstk-0.3.4.tar`

### file list

```diff
@@ -1,129 +1,129 @@
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.578225 mstk-0.3.3.dev11/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    26526 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/LICENSE
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2213 2023-02-02 07:33:48.577690 mstk-0.3.3.dev11/PKG-INFO
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     1799 2023-02-02 03:17:42.000000 mstk-0.3.3.dev11/README.md
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.268731 mstk-0.3.3.dev11/mstk/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     1045 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/__init__.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.319993 mstk-0.3.3.dev11/mstk/analyzer/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/analyzer/__init__.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4134 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/analyzer/canny.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    11884 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/analyzer/energy_kernels.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     8319 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/analyzer/ewald.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     8692 2023-01-30 09:29:48.000000 mstk-0.3.3.dev11/mstk/analyzer/fitting.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2275 2023-02-02 03:17:42.000000 mstk-0.3.3.dev11/mstk/analyzer/neighborlist.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4167 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/analyzer/series.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     1972 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/analyzer/structure.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4861 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/analyzer/vle.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.328359 mstk-0.3.3.dev11/mstk/chem/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/chem/__init__.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)      472 2023-01-30 03:30:28.000000 mstk-0.3.3.dev11/mstk/chem/constant.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2162 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/chem/element.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4819 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/chem/formula.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)      786 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/chem/rdkit.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.236996 mstk-0.3.3.dev11/mstk/data/
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.342072 mstk-0.3.3.dev11/mstk/data/forcefield/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    80183 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/data/forcefield/SPICA_v1.zfp
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     8120 2023-01-09 02:42:16.000000 mstk-0.3.3.dev11/mstk/data/forcefield/primitive.zff
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)      504 2023-01-09 02:42:16.000000 mstk-0.3.3.dev11/mstk/data/forcefield/primitive.zft
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)      325 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/errors.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.355013 mstk-0.3.3.dev11/mstk/forcefield/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)      193 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/forcefield/__init__.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4364 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/forcefield/dff_utils.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)      207 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/forcefield/errors.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    50916 2023-01-09 02:26:36.000000 mstk-0.3.3.dev11/mstk/forcefield/ffterm.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    36011 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/forcefield/forcefield.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.369326 mstk-0.3.3.dev11/mstk/forcefield/io/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/forcefield/io/__init__.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    15881 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/forcefield/io/padua.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     9327 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/forcefield/io/ppf.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     3764 2023-01-09 02:24:10.000000 mstk-0.3.3.dev11/mstk/forcefield/io/zff.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     5137 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/forcefield/io/zfp.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.374626 mstk-0.3.3.dev11/mstk/forcefield/typer/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)       68 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/forcefield/typer/__init__.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     1332 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/forcefield/typer/typer.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     8735 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/forcefield/typer/zft.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.381796 mstk-0.3.3.dev11/mstk/misc/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)       67 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/misc/__init__.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)      594 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/misc/docmeta.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)      219 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/misc/singleton.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.393077 mstk-0.3.3.dev11/mstk/ommhelper/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)      115 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/ommhelper/__init__.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    11581 2023-01-09 02:13:53.000000 mstk-0.3.3.dev11/mstk/ommhelper/force.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4908 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/ommhelper/grofile.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.417830 mstk-0.3.3.dev11/mstk/ommhelper/reporter/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)      248 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/ommhelper/reporter/__init__.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2851 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/ommhelper/reporter/checkpointreporter.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     6193 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/ommhelper/reporter/drudetemperaturereporter.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     3627 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/ommhelper/reporter/groreporter.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    22557 2023-01-29 11:56:20.000000 mstk-0.3.3.dev11/mstk/ommhelper/reporter/statedatareporter.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2796 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/ommhelper/reporter/viscosityreporter.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)      340 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/ommhelper/unit.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4229 2023-01-18 05:58:55.000000 mstk-0.3.3.dev11/mstk/ommhelper/utils.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.433085 mstk-0.3.3.dev11/mstk/scheduler/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)      122 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/scheduler/__init__.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     1662 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/scheduler/pbsjob.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     8305 2023-02-02 07:29:04.000000 mstk-0.3.3.dev11/mstk/scheduler/remote_slurm.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     8473 2023-01-18 06:47:49.000000 mstk-0.3.3.dev11/mstk/scheduler/scheduler.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     7940 2023-01-29 06:16:50.000000 mstk-0.3.3.dev11/mstk/scheduler/slurm.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.445541 mstk-0.3.3.dev11/mstk/simsys/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)      186 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/simsys/__init__.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    18560 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/simsys/gmxexporter.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    12785 2023-01-10 03:43:33.000000 mstk-0.3.3.dev11/mstk/simsys/lmpexporter.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     8339 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/simsys/namdexporter.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    31161 2023-01-09 06:37:05.000000 mstk-0.3.3.dev11/mstk/simsys/ommexporter.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    21437 2023-01-09 06:37:05.000000 mstk-0.3.3.dev11/mstk/simsys/system.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.478703 mstk-0.3.3.dev11/mstk/topology/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)      388 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/topology/__init__.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4677 2023-02-01 05:49:52.000000 mstk-0.3.3.dev11/mstk/topology/atom.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    11976 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/topology/connectivity.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     6778 2023-01-11 03:42:28.000000 mstk-0.3.3.dev11/mstk/topology/geometry.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.507316 mstk-0.3.3.dev11/mstk/topology/io/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/topology/io/__init__.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    10921 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/topology/io/lammps.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     3195 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/topology/io/msd.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     7215 2023-01-16 08:56:37.000000 mstk-0.3.3.dev11/mstk/topology/io/pdb.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    13233 2023-01-16 08:56:37.000000 mstk-0.3.3.dev11/mstk/topology/io/psf.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     1201 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/topology/io/smi.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2551 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/topology/io/xyz.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     9179 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/topology/io/zmat.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    52140 2023-01-18 07:51:51.000000 mstk-0.3.3.dev11/mstk/topology/molecule.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)      880 2023-01-18 03:05:53.000000 mstk-0.3.3.dev11/mstk/topology/residue.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    24007 2023-01-30 02:29:02.000000 mstk-0.3.3.dev11/mstk/topology/topology.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     8353 2023-01-11 02:42:39.000000 mstk-0.3.3.dev11/mstk/topology/unitcell.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4223 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/topology/virtualsite.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.517911 mstk-0.3.3.dev11/mstk/trajectory/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)      262 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/trajectory/__init__.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2866 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/trajectory/frame.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     3038 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/trajectory/handler.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.532810 mstk-0.3.3.dev11/mstk/trajectory/io/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/trajectory/io/__init__.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     1477 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/trajectory/io/combined_trj.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2192 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/trajectory/io/dcd.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4476 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/trajectory/io/gro.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4717 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/trajectory/io/lammps.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2192 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/trajectory/io/xtc.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2947 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/trajectory/io/xyz.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     7589 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/trajectory/trajectory.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.532810 mstk-0.3.3.dev11/mstk/utils/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4698 2023-02-01 02:28:01.000000 mstk-0.3.3.dev11/mstk/utils/__init__.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.555669 mstk-0.3.3.dev11/mstk/wrapper/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)       74 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/wrapper/__init__.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4740 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/wrapper/gauss.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    40192 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/wrapper/gmx.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     6449 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/wrapper/packmol.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)    14462 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/mstk/wrapper/panedr.py
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.294628 mstk-0.3.3.dev11/mstk.egg-info/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2213 2023-02-02 07:33:47.000000 mstk-0.3.3.dev11/mstk.egg-info/PKG-INFO
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2744 2023-02-02 07:33:47.000000 mstk-0.3.3.dev11/mstk.egg-info/SOURCES.txt
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)        1 2023-02-02 07:33:47.000000 mstk-0.3.3.dev11/mstk.egg-info/dependency_links.txt
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)        5 2023-02-02 07:33:47.000000 mstk-0.3.3.dev11/mstk.egg-info/top_level.txt
-drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-02-02 07:33:48.573629 mstk-0.3.3.dev11/scripts/
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     5172 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/scripts/analyze-rdf.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     1092 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/scripts/ffconv.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     5441 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/scripts/logplot.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     7761 2023-01-30 03:30:28.000000 mstk-0.3.3.dev11/scripts/quick-sim.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2661 2023-01-09 03:00:46.000000 mstk-0.3.3.dev11/scripts/topconv.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2841 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/scripts/trjconv.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)     3757 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/scripts/wham-pp.py
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)       38 2023-02-02 07:33:48.579240 mstk-0.3.3.dev11/setup.cfg
--rwxrwxrwx   0 zheng     (1000) zheng     (1000)      987 2023-01-09 02:13:54.000000 mstk-0.3.3.dev11/setup.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:11.704302 mstk-0.3.4/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    26526 2023-01-09 02:13:53.000000 mstk-0.3.4/LICENSE
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2493 2023-07-11 07:49:11.703290 mstk-0.3.4/PKG-INFO
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2085 2023-07-11 07:48:45.000000 mstk-0.3.4/README.md
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:09.430593 mstk-0.3.4/mstk/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     1045 2023-03-03 15:29:30.000000 mstk-0.3.4/mstk/__init__.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:09.601348 mstk-0.3.4/mstk/analyzer/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/analyzer/__init__.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4134 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/analyzer/canny.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    11884 2023-03-03 09:02:43.000000 mstk-0.3.4/mstk/analyzer/energy_kernels.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     8319 2023-03-03 09:02:43.000000 mstk-0.3.4/mstk/analyzer/ewald.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     8692 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/analyzer/fitting.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2275 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/analyzer/neighborlist.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4167 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/analyzer/series.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     1972 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/analyzer/structure.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4861 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/analyzer/vle.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:09.654093 mstk-0.3.4/mstk/chem/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-03-03 09:02:43.000000 mstk-0.3.4/mstk/chem/__init__.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)      472 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/chem/constant.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2162 2023-03-03 09:02:43.000000 mstk-0.3.4/mstk/chem/element.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4819 2023-03-03 09:02:43.000000 mstk-0.3.4/mstk/chem/formula.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)      786 2023-03-03 09:02:43.000000 mstk-0.3.4/mstk/chem/rdkit.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:09.356226 mstk-0.3.4/mstk/data/
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:09.689159 mstk-0.3.4/mstk/data/forcefield/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    80183 2023-03-03 09:02:43.000000 mstk-0.3.4/mstk/data/forcefield/SPICA_v1.zfp
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     8120 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/data/forcefield/primitive.zff
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)      504 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/data/forcefield/primitive.zft
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)      162 2023-03-10 06:03:23.000000 mstk-0.3.4/mstk/errors.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:09.796860 mstk-0.3.4/mstk/forcefield/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)      193 2023-03-03 15:29:30.000000 mstk-0.3.4/mstk/forcefield/__init__.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4364 2023-03-03 09:02:43.000000 mstk-0.3.4/mstk/forcefield/dff_utils.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)      207 2023-03-03 09:02:43.000000 mstk-0.3.4/mstk/forcefield/errors.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    50916 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/forcefield/ffterm.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    36011 2023-03-03 15:29:30.000000 mstk-0.3.4/mstk/forcefield/forcefield.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:09.922217 mstk-0.3.4/mstk/forcefield/io/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-03-03 09:02:43.000000 mstk-0.3.4/mstk/forcefield/io/__init__.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    15881 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/forcefield/io/padua.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     9327 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/forcefield/io/ppf.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     3764 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/forcefield/io/zff.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     5137 2023-03-03 09:02:43.000000 mstk-0.3.4/mstk/forcefield/io/zfp.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:09.970420 mstk-0.3.4/mstk/forcefield/typer/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)       68 2023-03-03 09:02:43.000000 mstk-0.3.4/mstk/forcefield/typer/__init__.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     1332 2023-03-03 09:02:43.000000 mstk-0.3.4/mstk/forcefield/typer/typer.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     8712 2023-03-10 06:03:23.000000 mstk-0.3.4/mstk/forcefield/typer/zft.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:10.022581 mstk-0.3.4/mstk/misc/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)       67 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/misc/__init__.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)      594 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/misc/docmeta.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)      219 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/misc/singleton.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:10.137466 mstk-0.3.4/mstk/ommhelper/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)      115 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/ommhelper/__init__.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    11581 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/ommhelper/force.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4908 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/ommhelper/grofile.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:10.297244 mstk-0.3.4/mstk/ommhelper/reporter/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)      248 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/ommhelper/reporter/__init__.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2851 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/ommhelper/reporter/checkpointreporter.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     6193 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/ommhelper/reporter/drudetemperaturereporter.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     3627 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/ommhelper/reporter/groreporter.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    22849 2023-05-08 03:39:52.000000 mstk-0.3.4/mstk/ommhelper/reporter/statedatareporter.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2796 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/ommhelper/reporter/viscosityreporter.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)      340 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/ommhelper/unit.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4377 2023-04-27 08:27:17.000000 mstk-0.3.4/mstk/ommhelper/utils.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:10.481864 mstk-0.3.4/mstk/scheduler/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)      122 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/scheduler/__init__.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     1662 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/scheduler/pbsjob.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     8305 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/scheduler/remote_slurm.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     8473 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/scheduler/scheduler.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     7894 2023-03-08 03:36:50.000000 mstk-0.3.4/mstk/scheduler/slurm.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:10.768644 mstk-0.3.4/mstk/simsys/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)      186 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/simsys/__init__.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    18560 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/simsys/gmxexporter.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    12785 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/simsys/lmpexporter.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     8339 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/simsys/namdexporter.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    31291 2023-03-24 02:48:27.000000 mstk-0.3.4/mstk/simsys/ommexporter.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    21437 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/simsys/system.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:11.067597 mstk-0.3.4/mstk/topology/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)      388 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/topology/__init__.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4677 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/topology/atom.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    12989 2023-03-10 06:03:23.000000 mstk-0.3.4/mstk/topology/connectivity.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     7599 2023-06-22 03:07:27.000000 mstk-0.3.4/mstk/topology/geometry.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:11.251839 mstk-0.3.4/mstk/topology/io/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/topology/io/__init__.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    10921 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/topology/io/lammps.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     3195 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/topology/io/msd.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     7216 2023-04-12 07:09:44.000000 mstk-0.3.4/mstk/topology/io/pdb.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    13233 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/topology/io/psf.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     1201 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/topology/io/smi.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2551 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/topology/io/xyz.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     9179 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/topology/io/zmat.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    53197 2023-03-24 02:12:19.000000 mstk-0.3.4/mstk/topology/molecule.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)      880 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/topology/residue.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    24007 2023-04-25 02:49:16.000000 mstk-0.3.4/mstk/topology/topology.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     8353 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/topology/unitcell.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4223 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/topology/virtualsite.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:11.359158 mstk-0.3.4/mstk/trajectory/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)      262 2023-03-03 15:29:30.000000 mstk-0.3.4/mstk/trajectory/__init__.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2866 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/trajectory/frame.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     3038 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/trajectory/handler.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:11.469947 mstk-0.3.4/mstk/trajectory/io/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/trajectory/io/__init__.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     1477 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/trajectory/io/combined_trj.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2192 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/trajectory/io/dcd.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4476 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/trajectory/io/gro.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4717 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/trajectory/io/lammps.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2192 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/trajectory/io/xtc.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2947 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/trajectory/io/xyz.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     7830 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/trajectory/trajectory.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:11.479036 mstk-0.3.4/mstk/utils/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4895 2023-05-23 05:10:07.000000 mstk-0.3.4/mstk/utils/__init__.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:11.580329 mstk-0.3.4/mstk/wrapper/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)       74 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/wrapper/__init__.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4740 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/wrapper/gauss.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    40192 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/wrapper/gmx.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     6449 2023-03-03 15:29:37.000000 mstk-0.3.4/mstk/wrapper/packmol.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)    14462 2023-03-03 09:02:44.000000 mstk-0.3.4/mstk/wrapper/panedr.py
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:09.452011 mstk-0.3.4/mstk.egg-info/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2493 2023-07-11 07:49:08.000000 mstk-0.3.4/mstk.egg-info/PKG-INFO
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     2744 2023-07-11 07:49:09.000000 mstk-0.3.4/mstk.egg-info/SOURCES.txt
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)        1 2023-07-11 07:49:09.000000 mstk-0.3.4/mstk.egg-info/dependency_links.txt
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)        5 2023-07-11 07:49:09.000000 mstk-0.3.4/mstk.egg-info/top_level.txt
+drwxrwxrwx   0 zheng     (1000) zheng     (1000)        0 2023-07-11 07:49:11.688953 mstk-0.3.4/scripts/
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     5512 2023-03-03 15:29:37.000000 mstk-0.3.4/scripts/analyze-rdf.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     1092 2023-03-03 09:02:44.000000 mstk-0.3.4/scripts/ffconv.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     8075 2023-05-31 03:28:15.000000 mstk-0.3.4/scripts/logplot.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     7761 2023-04-24 07:31:04.000000 mstk-0.3.4/scripts/quick-sim.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     3336 2023-03-03 15:29:37.000000 mstk-0.3.4/scripts/topconv.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     3558 2023-03-22 03:33:13.000000 mstk-0.3.4/scripts/trjconv.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)     4211 2023-03-03 15:29:37.000000 mstk-0.3.4/scripts/wham-pp.py
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)       38 2023-07-11 07:49:11.707219 mstk-0.3.4/setup.cfg
+-rwxrwxrwx   0 zheng     (1000) zheng     (1000)      981 2023-07-11 07:35:56.000000 mstk-0.3.4/setup.py
```

### Comparing `mstk-0.3.3.dev11/LICENSE` & `mstk-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/PKG-INFO` & `mstk-0.3.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mstk
-Version: 0.3.3.dev11
+Version: 0.3.4
 Summary: Molecular simulation toolkit
 Home-page: https://github.com/z-gong/mstk
 Author: Zheng Gong
 Author-email: z.gong@outlook.com
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -65,7 +65,15 @@
 
 https://mstk.readthedocs.io/en/latest/index.html
 
 ## TODO
 
 - [ ] Take bond order into consideration for force field assignment
 - [ ] Re-organize algorithms scattered in topology and analyzer modules
+
+## Known issue
+`mstk` use `chemfiles` to write `XTC` trajectory. However, lastest `chemfiles` is buggy under WSL for writing binary trajectory format. 
+If you are working under WSL, please install `chemfiles 0.10.2`.
+
+```
+conda install chemfiles-lib=0.10.2 chemfiles-python=0.10.2
+```
```

### Comparing `mstk-0.3.3.dev11/README.md` & `mstk-0.3.4/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -52,7 +52,15 @@
 
 https://mstk.readthedocs.io/en/latest/index.html
 
 ## TODO
 
 - [ ] Take bond order into consideration for force field assignment
 - [ ] Re-organize algorithms scattered in topology and analyzer modules
+
+## Known issue
+`mstk` use `chemfiles` to write `XTC` trajectory. However, lastest `chemfiles` is buggy under WSL for writing binary trajectory format. 
+If you are working under WSL, please install `chemfiles 0.10.2`.
+
+```
+conda install chemfiles-lib=0.10.2 chemfiles-python=0.10.2
+```
```

### Comparing `mstk-0.3.3.dev11/mstk/__init__.py` & `mstk-0.3.4/mstk/__init__.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/analyzer/canny.py` & `mstk-0.3.4/mstk/analyzer/canny.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/analyzer/energy_kernels.py` & `mstk-0.3.4/mstk/analyzer/energy_kernels.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/analyzer/ewald.py` & `mstk-0.3.4/mstk/analyzer/ewald.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/analyzer/fitting.py` & `mstk-0.3.4/mstk/analyzer/fitting.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/analyzer/neighborlist.py` & `mstk-0.3.4/mstk/analyzer/neighborlist.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/analyzer/series.py` & `mstk-0.3.4/mstk/analyzer/series.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/analyzer/structure.py` & `mstk-0.3.4/mstk/analyzer/structure.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/analyzer/vle.py` & `mstk-0.3.4/mstk/analyzer/vle.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/chem/element.py` & `mstk-0.3.4/mstk/chem/element.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/chem/formula.py` & `mstk-0.3.4/mstk/chem/formula.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/chem/rdkit.py` & `mstk-0.3.4/mstk/chem/rdkit.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/data/forcefield/SPICA_v1.zfp` & `mstk-0.3.4/mstk/data/forcefield/SPICA_v1.zfp`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/data/forcefield/primitive.zff` & `mstk-0.3.4/mstk/data/forcefield/primitive.zff`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/forcefield/dff_utils.py` & `mstk-0.3.4/mstk/forcefield/dff_utils.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/forcefield/ffterm.py` & `mstk-0.3.4/mstk/forcefield/ffterm.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/forcefield/forcefield.py` & `mstk-0.3.4/mstk/forcefield/forcefield.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/forcefield/io/padua.py` & `mstk-0.3.4/mstk/forcefield/io/padua.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/forcefield/io/ppf.py` & `mstk-0.3.4/mstk/forcefield/io/ppf.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/forcefield/io/zff.py` & `mstk-0.3.4/mstk/forcefield/io/zff.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/forcefield/io/zfp.py` & `mstk-0.3.4/mstk/forcefield/io/zfp.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/forcefield/typer/typer.py` & `mstk-0.3.4/mstk/forcefield/typer/typer.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/forcefield/typer/zft.py` & `mstk-0.3.4/mstk/forcefield/typer/zft.py`

 * *Files 4% similar despite different names*

```diff
@@ -94,15 +94,15 @@
     file : str or file-like object, optional
         Type definition file
     content : str, optional
         Content of type definition file
 
     Notes
     -----
-    * SMARTS is parsed by using OpenBabel package. Therefore `pybel` module should be installed.
+    * SMARTS is parsed by using RDKit package. Make sure it is installed.
     * In type definition file, empty lines are ignored, and comments should start with ##.
 
     '''
 
     def __init__(self, file=None):
         if not RDKIT_IMPORTER:
             raise Exception('RDKit is required for ZftTyper')
```

### Comparing `mstk-0.3.3.dev11/mstk/misc/docmeta.py` & `mstk-0.3.4/mstk/misc/docmeta.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/ommhelper/force.py` & `mstk-0.3.4/mstk/ommhelper/force.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/ommhelper/grofile.py` & `mstk-0.3.4/mstk/ommhelper/grofile.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/ommhelper/reporter/checkpointreporter.py` & `mstk-0.3.4/mstk/ommhelper/reporter/checkpointreporter.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/ommhelper/reporter/drudetemperaturereporter.py` & `mstk-0.3.4/mstk/ommhelper/reporter/drudetemperaturereporter.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/ommhelper/reporter/groreporter.py` & `mstk-0.3.4/mstk/ommhelper/reporter/groreporter.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/ommhelper/reporter/statedatareporter.py` & `mstk-0.3.4/mstk/ommhelper/reporter/statedatareporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         This is required if either progress or remainingTime is set to True,
         and defines how many steps will indicate 100% completion.
     cvs : list=[]
         Collective variables defined by CustomCVForce
     '''
 
     def __init__(self, file, reportInterval, step=True, time=False, potentialEnergy=True,
-                 kineticEnergy=False, totalEnergy=False, temperature=True, volume=False, box=True,
+                 kineticEnergy=False, totalEnergy=False, temperature=True, volume=True, box=True,
                  density=True, progress=False, remainingTime=False, speed=True, elapsedTime=False,
                  separator='\t', systemMass=None, totalSteps=None, append=False,
                  cvs=None, pressure=True, pxx=False, pyy=False, pzz=False, extra={}):
         self._reportInterval = reportInterval
         self._openedFile = isinstance(file, str)
         if (progress or remainingTime) and totalSteps is None:
             raise ValueError(
@@ -310,16 +310,15 @@
             values.append(value)
 
         for cv in self._cvs:
             values.append(cv.getCollectiveVariableValues(simulation.context)[0])
 
         bool_press = [self._pxx, self._pyy, self._pzz]
         if any(bool_press):
-            indexes = [i for i in range(3) if bool_press[i]]
-            values.extend(self._compute_anisotropic_pressure(simulation.context, state, indexes))
+            values.extend(self._compute_anisotropic_pressure(simulation.context, state, *bool_press))
 
         if self._extra:
             values.extend(self._extra.values())
 
         self._boxSizeList[0].append(box[0][0].value_in_unit(unit.nanometer)),
         self._boxSizeList[1].append(box[1][1].value_in_unit(unit.nanometer)),
         self._boxSizeList[2].append(box[2][2].value_in_unit(unit.nanometer)),
@@ -463,17 +462,28 @@
         p_virial = -(dU / dV).value_in_unit(unit.bar)
 
         context.setPeriodicBoxVectors(*box)
         context.setPositions(positions)
 
         return p_kinetic + p_virial
 
-    def _compute_anisotropic_pressure(self, context: mm.Context, state: mm.State, indexes: [bool]):
+    def _compute_anisotropic_pressure(self, context, state, pxx, pyy, pzz):
         '''
         Compute the anisotropic pressure of a rectangular system
+
+        Parameters
+        ----------
+        context : mm.Context
+        state : mm.State
+        pxx : bool
+            Whether or not the Pxx be calculated
+        pyy : bool
+            Whether or not the Pyy be calculated
+        pzz : bool
+            Whether or not the Pzz be calculated
         '''
         box = state.getPeriodicBoxVectors(asNumpy=True)
         positions = state.getPositions(asNumpy=True)
         volume = box[0][0] * box[1][1] * box[2][2]
 
         # TODO Assume kinetic energies are well-partitioned to each DOF
         p_kinetic = (2 * state.getKineticEnergy() * unit.item / 3 / volume).value_in_unit(unit.bar)
@@ -481,15 +491,17 @@
         # Because the contribution of constraints to the pressure cannot be evaluated,
         # here I approximate it by removing the kinetic contribution of the internal motion of each constrained group.
         # TODO I'm not confident about this formula
         p_kinetic *= len(self._constrained_groups) * 3 / self._dof
 
         scale = 0.0001
         pressures = []
-        for index in indexes:
+        for index, _bool in enumerate([pxx, pyy, pzz]):
+            if not _bool:
+                continue
             scale_array = np.array([1.0, 1.0, 1.0])
             scale_array[index] = 1 + scale
 
             box_scaled = box._value.copy()
             box_scaled[index][index] = box_scaled[index][index] * (1 + scale)
 
             context.setPeriodicBoxVectors(*box_scaled)
```

### Comparing `mstk-0.3.3.dev11/mstk/ommhelper/reporter/viscosityreporter.py` & `mstk-0.3.4/mstk/ommhelper/reporter/viscosityreporter.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/ommhelper/utils.py` & `mstk-0.3.4/mstk/ommhelper/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-import openmm
-import openmm.openmm as mm
 import numpy as np
-from openmm import app
+import openmm
+from openmm import openmm as mm, app
 from .grofile import GroFile
 from .unit import kelvin, bar, nm, ps
 
 
 class CONST:
     PI = 3.1415926535
     EPS0 = 8.8541878128E-12  # F/m
@@ -64,27 +63,33 @@
         GroFile.writeFile(sim.topology, state.getPositions(), state.getPeriodicBoxVectors(), gro_out)
 
 
 def apply_mc_barostat(system, pcoupl, P, T, nsteps=100, logger=None):
     '''
     Add a MonteCarlo barostat to the system and return the index of the added barostat
 
+    Parameters
+    ----------
+    system : mm.System
+    pcoupl : str
+        The type of barostat. Can be one of the following: iso, semi-iso, aniso, xy, z.
+
     Returns
     -------
     idx : index of the added barostat force
     '''
     if pcoupl == 'iso':
         msg = 'Isotropic barostat'
         force = mm.MonteCarloBarostat(P * bar, T * kelvin, nsteps)
     elif pcoupl == 'semi-iso':
         msg = 'Anisotropic barostat with coupled XY'
         force = mm.MonteCarloMembraneBarostat(P * bar, 0 * bar * nm, T * kelvin,
                                               mm.MonteCarloMembraneBarostat.XYIsotropic,
                                               mm.MonteCarloMembraneBarostat.ZFree, nsteps)
-    elif pcoupl == 'xyz':
+    elif pcoupl == 'aniso':
         msg = 'Anisotropic barostat'
         force = mm.MonteCarloAnisotropicBarostat([P * bar] * 3, T * kelvin, True, True, True, nsteps)
     elif pcoupl == 'xy':
         msg = 'Anisotropic barostat only for X and Y'
         force = mm.MonteCarloAnisotropicBarostat([P * bar] * 3, T * kelvin, True, True, False, nsteps)
     elif pcoupl == 'z':
         msg = 'Anisotropic barostat only for Z'
```

### Comparing `mstk-0.3.3.dev11/mstk/scheduler/pbsjob.py` & `mstk-0.3.4/mstk/scheduler/pbsjob.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/scheduler/remote_slurm.py` & `mstk-0.3.4/mstk/scheduler/remote_slurm.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/scheduler/scheduler.py` & `mstk-0.3.4/mstk/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/scheduler/slurm.py` & `mstk-0.3.4/mstk/scheduler/slurm.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,16 +105,16 @@
             The name (path) of shell script to be generated.
             If not set, will use the default :attr:`sh`.
         '''
         workdir = workdir or (self.remote_dir if self.is_remote else os.getcwd())
         workdir = Path(workdir).absolute().as_posix()
         sh = sh or self.sh
         sh_basename = Path(sh).stem
-        out = os.path.join(workdir, sh_basename + '.out')
-        err = os.path.join(workdir, sh_basename + '.err')
+        out = sh_basename + '.out'
+        err = sh_basename + '.err'
         node_cmd = f'#SBATCH --nodes={self.n_node}\n' if self.n_node > 0 else ''
         gpu_cmd = f'#SBATCH --gres=gpu:{self.n_gpu}\n' if self.n_gpu > 0 else ''
         dep_cmd = f'#SBATCH --dependency=afterok:{id_prior}\n' if id_prior is not None else ''  # id_prior can be 0
         exclude_cmd = f'#SBATCH --exclude={self.exclude}\n' if self.exclude else ''
 
         with open(sh, 'w') as f:
             f.write(f'#!/bin/bash\n'
```

### Comparing `mstk-0.3.3.dev11/mstk/simsys/gmxexporter.py` & `mstk-0.3.4/mstk/simsys/gmxexporter.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/simsys/lmpexporter.py` & `mstk-0.3.4/mstk/simsys/lmpexporter.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/simsys/namdexporter.py` & `mstk-0.3.4/mstk/simsys/namdexporter.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/simsys/ommexporter.py` & `mstk-0.3.4/mstk/simsys/ommexporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,34 +139,37 @@
                     aterm = system.angle_terms[angle]
                     if type(aterm) == HarmonicAngleTerm:
                         aforce.addAngle(angle.atom1.id, angle.atom2.id, angle.atom3.id,
                                         aterm.theta, aterm.k * 2)
             elif angle_class == SDKAngleTerm:
                 logger.debug('Setting up SDK angles...')
                 aforce = mm.CustomCompoundBondForce(
-                    3, 'k*(theta-theta0)^2+step(rmin-r)*LJ96;'
-                       'LJ96=6.75*epsilon*((sigma/r)^9-(sigma/r)^6)+epsilon;'
+                    3, 'k*(theta-theta0)^2+step(rmin-r)*LJ;'
+                       'LJ=C*epsilon*((sigma/r)^n-(sigma/r)^m)+epsilon;'
                        'theta=angle(p1,p2,p3);'
                        'r=distance(p1,p3);'
-                       'rmin=1.144714*sigma')
+                       'C=n/(n-m)*(n/m)^(m/(n-m));'
+                       'rmin=(n/m)^(1/(n-m))*sigma')
                 aforce.addPerBondParameter('theta0')
                 aforce.addPerBondParameter('k')
                 aforce.addPerBondParameter('epsilon')
                 aforce.addPerBondParameter('sigma')
+                aforce.addPerBondParameter('n')
+                aforce.addPerBondParameter('m')
                 for angle in top.angles:
                     if angle in system.constrain_angles:
                         continue
                     aterm = system.angle_terms[angle]
                     if type(aterm) != SDKAngleTerm:
                         continue
-                    vdw = ff.get_vdw_term(ff.atom_types[angle.atom1.type], ff.atom_types[angle.atom2.type])
-                    if type(vdw) != MieTerm or vdw.repulsion != 9 or vdw.attraction != 6:
-                        raise Exception(f'Corresponding 9-6 MieTerm for {aterm} not found in FF')
+                    vdw = ff.get_vdw_term(ff.atom_types[angle.atom1.type], ff.atom_types[angle.atom3.type])
+                    if type(vdw) != MieTerm:
+                        raise Exception(f'Corresponding MieTerm for {aterm} not found in FF')
                     aforce.addBond([angle.atom1.id, angle.atom2.id, angle.atom3.id],
-                                   [aterm.theta, aterm.k, vdw.epsilon, vdw.sigma])
+                                   [aterm.theta, aterm.k, vdw.epsilon, vdw.sigma, vdw.repulsion, vdw.attraction])
             elif angle_class == LinearAngleTerm:
                 logger.debug('Setting up linear angles...')
                 aforce = mm.CustomCompoundBondForce(
                     3, 'k_linear*r^2;'
                        'r=pointdistance(xref,yref,zref,x2,y2,z2);'
                        'xref=x1*a+x3*(1-a);'
                        'yref=y1*a+y3*(1-a);'
```

### Comparing `mstk-0.3.3.dev11/mstk/simsys/system.py` & `mstk-0.3.4/mstk/simsys/system.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/topology/atom.py` & `mstk-0.3.4/mstk/topology/atom.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/topology/connectivity.py` & `mstk-0.3.4/mstk/topology/connectivity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import numpy as np
 from .atom import Atom
+from .geometry import periodic_distance, periodic_angle, periodic_dihedral
 
 __all__ = [
     'Bond',
     'Angle',
     'Dihedral',
     'Improper',
 ]
@@ -111,22 +112,29 @@
 
         Returns
         -------
         is : bool
         '''
         return self.atom1.is_drude or self.atom2.is_drude
 
-    def evaluate(self):
+    def evaluate(self, cell=None):
         '''
         Evaluate the length of this bond
 
+        Parameters
+        ----------
+        box : UnitCell, Optional
+
         Returns
         -------
         value : float
         '''
+        if cell:
+            return periodic_distance(self.atom1.position, self.atom2.position, cell.size)
+
         delta = self.atom2.position - self.atom1.position
         return float(np.sqrt(delta.dot(delta)))
 
     @property
     def is_aromatic(self):
         rdbond = self.atom1.molecule.rdmol.GetBondBetweenAtoms(self.atom1.id_in_mol, self.atom2.id_in_mol)
         return rdbond.GetIsAromatic()
@@ -221,22 +229,29 @@
         try:
             bond23 = next(b for b in self.atom2.bonds if b.equals(_bond23))
         except StopIteration:
             raise Exception(f'{_bond23} not found in {self.atom2.molecule}')
 
         return bond12, bond23
 
-    def evaluate(self):
+    def evaluate(self, cell=None):
         '''
         Evaluate the value of this angle in unit of radian
 
+        Parameters
+        ----------
+        cell : UnitCell, Optional
+
         Returns
         -------
         value : float
         '''
+        if cell:
+            return periodic_angle(self.atom1.position, self.atom2.position, self.atom3.position, cell)
+
         vec1 = self.atom1.position - self.atom2.position
         vec2 = self.atom3.position - self.atom2.position
         cos = vec1.dot(vec2) / np.sqrt(vec1.dot(vec1) * vec2.dot(vec2))
         return float(np.arccos(np.clip(cos, -1, 1)))
 
 
 class Dihedral():
@@ -357,22 +372,30 @@
         try:
             angle234 = next(a for a in mol.angles if a.equals(_angle234))
         except StopIteration:
             raise Exception(f'{_angle234} not found in {mol}')
 
         return angle123, angle234
 
-    def evaluate(self):
+    def evaluate(self, cell=None):
         '''
         Evaluate the value of this dihedral in unit of radian
 
+        Parameters
+        ----------
+        cell : UnitCell, Optional
+
         Returns
         -------
         value : float
         '''
+        if cell:
+            return periodic_dihedral(self.atom1.position, self.atom2.position, self.atom3.position, self.atom4.position,
+                                     cell.size)
+
         vec1 = self.atom2.position - self.atom1.position
         vec2 = self.atom3.position - self.atom2.position
         vec3 = self.atom4.position - self.atom3.position
         n1 = np.cross(vec1, vec2)
         n2 = np.cross(vec2, vec3)
         cos = n1.dot(n2) / np.sqrt(n1.dot(n1) * n2.dot(n2))
         value = float(np.arccos(np.clip(cos, -1, 1)))
@@ -446,23 +469,31 @@
 
         Returns
         -------
         atoms : tuple of Atom
         '''
         return self.atom1, self.atom2, self.atom3, self.atom4
 
-    def evaluate(self):
+    def evaluate(self, cell=None):
         '''
         Evaluate the value of this improper torsion in unit of radian.
         The improper is defined as the angle between plane a1-a2-a3 and a2-a3-a4.
 
+        Parameters
+        ----------
+        cell : UnitCell, Optional
+
         Returns
         -------
         value : float
         '''
+        if cell:
+            return periodic_dihedral(self.atom1.position, self.atom2.position, self.atom3.position, self.atom4.position,
+                                     cell.size)
+
         vec1 = self.atom2.position - self.atom1.position
         vec2 = self.atom3.position - self.atom2.position
         vec3 = self.atom4.position - self.atom3.position
         n1 = np.cross(vec1, vec2)
         n2 = np.cross(vec2, vec3)
         cos = n1.dot(n2) / np.sqrt(n1.dot(n1) * n2.dot(n2))
         value = float(np.arccos(np.clip(cos, -1, 1)))
```

### Comparing `mstk-0.3.3.dev11/mstk/topology/geometry.py` & `mstk-0.3.4/mstk/topology/geometry.py`

 * *Files 12% similar despite different names*

```diff
@@ -58,14 +58,30 @@
 
     phi = np.random.random() * 2 * np.pi
     w = np.sin(angle) * np.cos(phi) * xb + np.sin(angle) * np.sin(phi) * yb + np.cos(angle) * v
 
     return pos2 + w * bond
 
 
+def relocate_hydrogen(hydrogen):
+    '''
+    Update the position of a hydrogen atom according to the parent atom and other neighbors of parent
+
+    Parameters
+    ----------
+    hydrogen : Atom
+    '''
+    vector = np.array([0., 0., 0.])
+    parent = hydrogen.bond_partners[0]
+    for atom in parent.bond_partners:
+        if atom is not hydrogen:
+            vector += atom.position - parent.position
+    hydrogen.position = parent.position - vector / np.sqrt(np.dot(vector, vector)) * 0.1  # bXH = 0.1 nm
+
+
 def periodic_distance(pos1, pos2, box, distance_max=None):
     '''
     Calculate the distance between two points under periodic boundary condition
     
     Parameters
     ----------
     pos1 : np.ndarray
@@ -151,15 +167,15 @@
     n2 = np.cross(vec2, vec3)
     cos = n1.dot(n2) / np.sqrt(n1.dot(n1) * n2.dot(n2))
     value = float(np.arccos(np.clip(cos, -1, 1)))
     sign = 1 if vec1.dot(n2) >= 0 else -1
     return sign * value
 
 
-def find_clusters(elements, func):
+def find_clusters(elements, func, show_progress=False):
     '''
     Group elements into clusters
 
     Parameters
     ----------
     elements : Iterable
     func : func
@@ -171,15 +187,20 @@
     clusters : list of list of int
         The clusters formed by elements. Each cluster is represented by a list of the index of elements.
     '''
     n_element = len(elements)
     flag = [0] * n_element
     n_cluster = 0
     clusters = []
-    for i in range(n_element):
+    if show_progress:
+        from tqdm import tqdm
+        _iterator = tqdm(range(n_element))
+    else:
+        _iterator = range(n_element)
+    for i in _iterator:
         if flag[i]:
             continue
         path = {i}
         expand = set()
         n_cluster += 1
         flag[i] = n_cluster
         for j in range(i + 1, n_element):
@@ -199,15 +220,15 @@
                     expand.add(n)
                     flag[n] = n_cluster
         clusters.append(list(path))
 
     return clusters
 
 
-def find_clusters_consecutive(elements, func):
+def find_clusters_consecutive(elements, func, show_progress=False):
     '''
     Group elements into clusters. If element i and j are in the same group, all elements between i and j will also be put in the same group.
 
     Parameters
     ----------
     elements : Iterable
     func : func
@@ -219,15 +240,20 @@
     clusters : list of list of int
         The clusters formed by elements. Each cluster is represented by a list of the index of elements.
     '''
     n_element = len(elements)
     flag = [0] * n_element
     n_cluster = 0
     clusters = []
-    for i in range(n_element):
+    if show_progress:
+        from tqdm import tqdm
+        _iterator = tqdm(range(n_element))
+    else:
+        _iterator = range(n_element)
+    for i in _iterator:
         if not flag[i]:
             n_cluster += 1
             flag[i] = n_cluster
             clusters.append({i})
         for j in reversed(range(i + 1, n_element)):
             if flag[j]:
                 break
```

### Comparing `mstk-0.3.3.dev11/mstk/topology/io/lammps.py` & `mstk-0.3.4/mstk/topology/io/lammps.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/topology/io/msd.py` & `mstk-0.3.4/mstk/topology/io/msd.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/topology/io/pdb.py` & `mstk-0.3.4/mstk/topology/io/pdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
             lengths[0], lengths[1], lengths[2], angles[0] * RAD2DEG, angles[1] * RAD2DEG, angles[2] * RAD2DEG)
 
         for atom in top.atoms:
             pos = atom.position * 10  # convert from nm to A
             atom_name = atom.type if atom_type else atom.name
             resname = atom.residue.name
             resid = atom.residue.id + 1
-            line = 'HETATM%5d %4s %4s %4d    %8.3f%8.3f%8.3f                      %2s\n' % (
+            line = 'HETATM%5d %4s %-4s %4d    %8.3f%8.3f%8.3f                      %2s\n' % (
                 (atom.id + 1) % 100000, atom_name[:4], resname[:4], resid % 10000,
                 pos[0], pos[1], pos[2], atom.symbol[:2])
             string += line
 
         for atom in top.atoms:
             partners = [a for a in atom.bond_partners if a.id > atom.id]
             if len(partners) > 0:
```

### Comparing `mstk-0.3.3.dev11/mstk/topology/io/psf.py` & `mstk-0.3.4/mstk/topology/io/psf.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/topology/io/smi.py` & `mstk-0.3.4/mstk/topology/io/smi.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/topology/io/xyz.py` & `mstk-0.3.4/mstk/topology/io/xyz.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/topology/io/zmat.py` & `mstk-0.3.4/mstk/topology/io/zmat.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/topology/molecule.py` & `mstk-0.3.4/mstk/topology/molecule.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,35 +210,30 @@
 
     @property
     def rdmol(self):
         '''
         The `rdkit.Chem.Mol` object associated with this molecule.
 
         It is required by ZftTyper typing engine, which performs SMARTS matching on the molecule.
-        The obmol attribute will be assigned if the molecule is initialized from SMILES or Pybel Molecule.
-        If this information is not available, an Exception will be raised.
+        The `rdmol` attribute will be assigned if the molecule is initialized from SMILES or RDKit Molecule.
+        If it is not available, a RDKit molecule will be constructed from atoms and bonds.
+        The positions will not be preserved.
 
         Returns
         -------
         rdmol : rdkit.Chem.Mol
         '''
-        if not self._is_rdmol_valid:
-            self._construct_rdmol()
-
-        return self._rdmol
-
-    def _construct_rdmol(self):
-        '''
-        Construct a RDKit molecule from atoms and bonds. The positions will not be preserved.
-        '''
         try:
             from rdkit import Chem
         except ImportError:
             raise ImportError('RDKit not found')
 
+        if self._is_rdmol_valid:
+            return self._rdmol
+
         if any(b.order == Bond.Order.UNSPECIFIED for b in self.bonds):
             logger.warning(f'Not all bond orders are specified in {self}')
 
         rwmol = Chem.RWMol()
         for atom in self.atoms:
             rdatom = Chem.Atom(atom.symbol)
             rdatom.SetFormalCharge(atom.formal_charge)
@@ -252,14 +247,46 @@
                 Bond.Order.TRIPLE     : Chem.rdchem.BondType.TRIPLE,
             }
             rwmol.AddBond(bond.atom1.id_in_mol, bond.atom2.id_in_mol, d_bond_order[bond.order])
         Chem.SanitizeMol(rwmol)
         self._rdmol = rwmol.GetMol()
         self._is_rdmol_valid = True
 
+        return self._rdmol
+
+    def generate_conformers(self, n_conformer=1):
+        '''
+        Generate several conformers with RDKit.
+
+        The positions will be generated from only elements and bonds. The chiral center will not be respected.
+
+        Parameters
+        ----------
+        n_conformer : int
+            How many conformers to generate
+
+        Returns
+        -------
+        molecules : list of Molecule
+            Each conformer will be a independent molecule object
+        '''
+        try:
+            from rdkit.Chem import AllChem as Chem
+        except ImportError:
+            raise ImportError('RDKit not found')
+
+        molecules = []
+        rdmol = Chem.Mol(self.rdmol)
+        Chem.EmbedMultipleConfs(rdmol, numConfs=n_conformer, clearConfs=True)
+        for i in range(rdmol.GetNumConformers()):
+            molecules.append(Molecule.from_rdmol(rdmol, name=self.name))
+            rdmol.RemoveConformer(i)
+
+        return molecules
+
     @property
     def topology(self):
         '''
         The topology this molecule belongs to
 
         Returns
         -------
@@ -313,14 +340,16 @@
         Remove an atom and all the bonds connected to the atom from this molecule.
 
         The atom will also be removed from its residue.
         The id_in_mol attribute of all atoms will be updated after removal.
         The angle, dihedral and improper involving this atom are untouched.
         Therefore, you may call `generate_angle_dihedral_improper` to refresh the connectivity.
 
+        # TODO This operation is extremely slow
+
         Parameters
         ----------
         atom : Atom
         update_topology : bool
             If update_topology is True, the topology this molecule belongs to will update its atom list and assign id for all atoms and residues.
             Otherwise, you have to re-init the topology manually so that the topological information is correct.
         '''
@@ -347,42 +376,45 @@
 
         Parameters
         ----------
         update_topology : bool
             If update_topology is True, the topology this molecule belongs to will update its atom list and assign id for all atoms and residues.
             Otherwise, you have to re-init the topology manually so that the topological information is correct.
 
+        # TODO This operation is extremely slow
+
         Returns
         -------
         ids_removed : list of int
             The number of atoms removed
         '''
         hydrogens = []
-        ids_removed = []
         for atom in self.atoms[:]:
             if atom.symbol != 'H' or len(atom.bonds) != 1:
                 continue
             neigh = atom.bond_partners[0]
             if neigh.symbol not in ('C', 'Si'):
                 continue
             neigh.mass += atom.mass
             neigh.charge += atom.charge
-            for conn in self.bonds[:] + self.angles[:] + self.dihedrals[:] + self.impropers[:]:
-                if atom in conn.atoms:
-                    self.remove_connectivity(conn)
-            ids_removed.append(atom.id_in_mol)
             hydrogens.append(atom)
+        ids_hydrogens = [atom.id_in_mol for atom in hydrogens]
+
+        for conn in self.bonds[:] + self.angles[:] + self.dihedrals[:] + self.impropers[:]:
+            ids_set = {atom.id_in_mol for atom in conn.atoms}
+            if ids_set.intersection(ids_hydrogens):
+                self.remove_connectivity(conn)
 
         for atom in hydrogens:
             self.remove_atom(atom, update_topology=False)
 
         if self._topology is not None and update_topology:
             self._topology.update_molecules(self._topology.molecules, deepcopy=False)
 
-        return ids_removed
+        return ids_hydrogens
 
     def add_residue(self, name, atoms, update_topology=True):
         '''
         Put a group of atoms into a new residue. These atoms will be removed from their old residues.
 
         Make sure that these atoms belong to this molecule.
         For performance issue, this is not checked.
@@ -559,14 +591,16 @@
 
         Make sure that this connectivity belongs to this molecule.
         For performance issue, this is not checked.
 
         Note that when a bond get removed, the relevant angles, dihedrals and impropers are still there.
         You may call `generate_angle_dihedral_improper` to refresh connectivity.
 
+        # TODO This operation is extremely slow
+
         Parameters
         ----------
         connectivity : [Bond, Angle, Dihedral, Improper]
         '''
         if type(connectivity) is Bond:
             bond = connectivity
             self._bonds.remove(bond)
```

### Comparing `mstk-0.3.3.dev11/mstk/topology/residue.py` & `mstk-0.3.4/mstk/topology/residue.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/topology/topology.py` & `mstk-0.3.4/mstk/topology/topology.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/topology/unitcell.py` & `mstk-0.3.4/mstk/topology/unitcell.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/topology/virtualsite.py` & `mstk-0.3.4/mstk/topology/virtualsite.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/trajectory/frame.py` & `mstk-0.3.4/mstk/trajectory/frame.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/trajectory/handler.py` & `mstk-0.3.4/mstk/trajectory/handler.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/trajectory/io/combined_trj.py` & `mstk-0.3.4/mstk/trajectory/io/combined_trj.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/trajectory/io/dcd.py` & `mstk-0.3.4/mstk/trajectory/io/dcd.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/trajectory/io/gro.py` & `mstk-0.3.4/mstk/trajectory/io/gro.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/trajectory/io/lammps.py` & `mstk-0.3.4/mstk/trajectory/io/lammps.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/trajectory/io/xtc.py` & `mstk-0.3.4/mstk/trajectory/io/xtc.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/trajectory/io/xyz.py` & `mstk-0.3.4/mstk/trajectory/io/xyz.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/trajectory/trajectory.py` & `mstk-0.3.4/mstk/trajectory/trajectory.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,14 +72,17 @@
 
         if mode == 'r':
             self.n_atom, self.n_frame = self._handler.get_info()
 
     def __del__(self):
         self.close()
 
+    def __repr__(self):
+        return f'<Trajectory: {self.n_frame} frames {self.n_atom} atoms>'
+
     def close(self):
         '''
         Close the opened trajectory file(s).
         '''
         try:
             self._handler.close()
         except:
@@ -93,15 +96,16 @@
         For the best of performance, a cached frame is used.
         When this method is called, the position and cell etc in the cached frame are updated,
         and the reference of this frame will be returned.
         Therefore, if you want to handle several different frames at the same time,
         this method should not be used because all the frames actually point to the same frame.
         In this case, use :func:`read_frames` instead.
 
-        i_frame should be in the range of [0, n_frame), otherwise and Exception will be raised.
+        i_frame should be in the range of [-1, n_frame), otherwise and Exception will be raised.
+        -1 means the last frame.
 
         Parameters
         ----------
         i_frame : int
             The index of the frame in trajectory.
 
         Returns
@@ -119,26 +123,29 @@
             if self.n_atom == -1:
                 raise Exception('Invalid number of atoms')
             self.frame = Frame(self.n_atom)
 
         # Reset the information in self.frame in case the frames read from different trajectory files pollute each other for CombinedTrajectory
         self.frame.reset()
 
+        if i_frame == -1:
+            i_frame = self.n_frame - 1
         self._handler.read_frame(i_frame, self.frame)
         return self.frame
 
     def read_frames(self, i_frames: [int]):
         '''
         Read a bunch of frames from the trajectory.
 
         Unlike :func:`read_frame`, the cached frame is not used.
         Instead, a new Frame object is constructed for each frame.
         This method should be called when you want to multiprocess several frames in parallel.
 
-        All the items in i_frames should be in the range of (0, n_frame), otherwise and Exception will be raised.
+        All the items in i_frames should be in the range of [-1, n_frame), otherwise and Exception will be raised.
+        -1 means the last frame.
 
         Parameters
         ----------
         i_frames : list of int
 
         Returns
         -------
@@ -149,14 +156,16 @@
             raise Exception('mode != "r" or closed trajectory')
 
         if any(i >= self.n_frame for i in i_frames):
             raise Exception('i_frame should be smaller than %i' % self.n_frame)
 
         frames = [Frame(self.n_atom) for _ in i_frames]
         for ii, i_frame in enumerate(i_frames):
+            if i_frame == -1:
+                i_frame = self.n_frame - 1
             self._handler.read_frame(i_frame, frames[ii])
         return frames
 
     def write_frame(self, frame, topology=None, subset=None, **kwargs):
         '''
         Write one frame to the opened trajectory file.
 
@@ -215,12 +224,10 @@
 
         Returns
         -------
         frame : Frame
 
         '''
         trj = Trajectory(file, 'r')
-        if i_frame == -1:
-            i_frame = trj.n_frame - 1
         frame = trj.read_frame(i_frame)
         trj.close()
         return frame
```

### Comparing `mstk-0.3.3.dev11/mstk/utils/__init__.py` & `mstk-0.3.4/mstk/utils/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 '''
 
 import os
 import subprocess
 import random
 import string
 import numpy as np
+from typing import Iterable
 
 
 def greatest_common_divisor(numbers):
     '''
     Calculate the greatest common divisor.
 
     Parameters
@@ -183,7 +184,15 @@
             if ratio1 > ratio2:
                 ylims2[1] = -ylims2[0] * ratio1
             else:
                 ylims1[1] = -ylims1[0] * ratio2
 
     ax1.set(ylim=ylims1)
     ax2.set(ylim=ylims2)
+
+
+def flatten(it):
+    for x in it:
+        if (isinstance(x, Iterable) and not isinstance(x, str)):
+            yield from flatten(x)
+        else:
+            yield x
```

### Comparing `mstk-0.3.3.dev11/mstk/wrapper/gauss.py` & `mstk-0.3.4/mstk/wrapper/gauss.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/wrapper/gmx.py` & `mstk-0.3.4/mstk/wrapper/gmx.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/wrapper/packmol.py` & `mstk-0.3.4/mstk/wrapper/packmol.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk/wrapper/panedr.py` & `mstk-0.3.4/mstk/wrapper/panedr.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/mstk.egg-info/PKG-INFO` & `mstk-0.3.4/mstk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mstk
-Version: 0.3.3.dev11
+Version: 0.3.4
 Summary: Molecular simulation toolkit
 Home-page: https://github.com/z-gong/mstk
 Author: Zheng Gong
 Author-email: z.gong@outlook.com
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
@@ -65,7 +65,15 @@
 
 https://mstk.readthedocs.io/en/latest/index.html
 
 ## TODO
 
 - [ ] Take bond order into consideration for force field assignment
 - [ ] Re-organize algorithms scattered in topology and analyzer modules
+
+## Known issue
+`mstk` use `chemfiles` to write `XTC` trajectory. However, lastest `chemfiles` is buggy under WSL for writing binary trajectory format. 
+If you are working under WSL, please install `chemfiles 0.10.2`.
+
+```
+conda install chemfiles-lib=0.10.2 chemfiles-python=0.10.2
+```
```

### Comparing `mstk-0.3.3.dev11/mstk.egg-info/SOURCES.txt` & `mstk-0.3.4/mstk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/scripts/analyze-rdf.py` & `mstk-0.3.4/scripts/analyze-rdf.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,124 +6,131 @@
 import numpy as np
 import matplotlib
 import matplotlib.pyplot as plt
 from mstk.topology import Topology
 from mstk.trajectory import Trajectory
 from mstk.utils import print_data_to_file
 from mstk.topology.geometry import periodic_distance
+from mstk import logger
 
 np.seterr(all='raise')
 matplotlib.use('Agg')
 matplotlib.rcParams.update({'font.size': 15})
 
-parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-parser.add_argument('input', nargs='+', type=str,
-                    help='trajectory files for atomic positions and charges')
-parser.add_argument('-t', '--topology', required=True, type=str,
-                    help='psf or lammps data file for topology information')
-parser.add_argument('--a1', type=str, nargs='+', help='type of central atoms')
-parser.add_argument('--a2', type=str, nargs='+', help='type of coordinate atoms')
-parser.add_argument('--m1', type=str, help='name of central molecules')
-parser.add_argument('--m2', type=str, help='name of coordinate molecules')
-parser.add_argument('-o', '--output', required=True, type=str, help='Output prefix')
-parser.add_argument('-b', '--begin', default=0, type=int,
-                    help='first frame to analyze. Index starts from 0')
-parser.add_argument('-e', '--end', default=-1, type=int,
-                    help='last frame (not included) to analyze. Index starts from 0. '
-                         '-1 means until last frames (included)')
-parser.add_argument('--maxr', default=1.0, type=float,
-                    help='max distance (nm) for calculation of distribution')
-parser.add_argument('--dr', default=0.01, type=float,
-                    help='bin size (nm) for calculation of distribution')
-parser.add_argument('--ignore', nargs='+', default=[], type=str,
-                    help='ignore these molecules in topology in case topology and trajectory do not match')
-parser.add_argument('--skip', default=1, type=int, help='skip frames in trajectory')
-args = parser.parse_args()
-
-top = Topology.open(args.topology)
-if args.ignore != []:
-    molecules = [mol for mol in top.molecules if mol.name not in args.ignore]
-    top.update_molecules(molecules)
-print('Topology info: ', top.n_atom, 'atoms;', top.n_molecule, 'molecules')
-
-trj = Trajectory.open(args.input)
-print('Trajectory info: ', trj.n_atom, 'atoms;', trj.n_frame, 'frames')
-
-if (top.n_atom != trj.n_atom):
-    raise Exception('Number of atoms in topology and trajectory files do not match')
-
-if args.m1 is None:
-    group1 = [[atom] for atom in top.atoms if atom.type in args.a1]
-else:
-    group1 = [[atom for atom in mol.atoms if atom.type in args.a1]
-              for mol in top.molecules if mol.name == args.m1]
-ids_group1 = [[atom.id for atom in atoms] for atoms in group1]
-masses_group1 = [[atom.mass for atom in atoms] for atoms in group1]
-
-if args.m2 is None:
-    group2 = [[atom] for atom in top.atoms if atom.type in args.a2]
-else:
-    group2 = [[atom for atom in mol.atoms if atom.type in args.a2]
-              for mol in top.molecules if mol.name == args.m2]
-ids_group2 = [[atom.id for atom in atoms] for atoms in group2]
-masses_group2 = [[atom.mass for atom in atoms] for atoms in group2]
-
-if args.end > trj.n_frame or args.end == -1:
-    args.end = trj.n_frame
-
-dr = args.dr
-n_bin = math.ceil(args.maxr / dr) + 1
-edges = np.array([dr * (i - 0.5) for i in range(n_bin + 1)], dtype=np.float32)
-r_array = (edges[1:] + edges[:-1]) / 2
-rdf_array = np.zeros(n_bin, dtype=np.float32)
-
-
-def _get_weighted_center(positions, weight):
-    return np.sum(positions * np.array(weight)[:, np.newaxis], axis=0) / sum(weight)
-
-
-def _get_com_group(positions, ids_group, masses_group):
-    com_group = []
-    for ids, masses in zip(ids_group, masses_group):
-        poss = positions[ids]
-        if len(ids) == 1:
-            pos = poss[0]
-        else:
-            pos = _get_weighted_center(poss, masses)
-        com_group.append(pos)
-    return com_group
-
-
-n_frame = 0
-for i in range(args.begin, args.end, args.skip):
-    n_frame += 1
-    frame = trj.read_frame(i)
-    sys.stdout.write('\r    frame %i' % i)
-
-    com_group1 = _get_com_group(frame.positions, ids_group1, masses_group1)
-    com_group2 = _get_com_group(frame.positions, ids_group2, masses_group2)
-
-    vol = frame.cell.volume
-    density_pair = len(group1) * len(group2) / vol
-
-    density_array = np.zeros(len(r_array), dtype=np.float32)
-    for com1 in com_group1:
-        for com2 in com_group2:
-            distance = periodic_distance(com1, com2, frame.cell.size, args.maxr + dr / 2)
-            if distance is not None and distance < args.maxr + dr / 2:
-                idx_r = int((distance - edges[0]) / dr)
-                density_array[idx_r] += 1
-
-    rdf_array[1:] += density_array[1:] / (4 * np.pi * r_array[1:] ** 2 * dr) / density_pair
-
-rdf_array = rdf_array / n_frame
-
-name_column_dict = {'r'  : r_array,
-                    'rdf': rdf_array}
-print_data_to_file(name_column_dict, f'{args.output}-rdf.txt')
-
-fig, ax = plt.subplots()
-ax.set(xlabel='r (nm)', ylabel='RDF')
-ax.plot(r_array, rdf_array, label='RDF')
-ax.legend()
-fig.tight_layout()
-fig.savefig(f'{args.output}-rdf.png')
+
+def parse_args():
+    parser = argparse.ArgumentParser(formatter_class=argparse.ArgumentDefaultsHelpFormatter)
+    parser.add_argument('input', nargs='+', type=str,
+                        help='trajectory files for atomic positions and charges')
+    parser.add_argument('-p', '--top', required=True, type=str,
+                        help='psf or lammps data file for topology information')
+    parser.add_argument('--a1', type=str, nargs='+', help='type of central atoms')
+    parser.add_argument('--a2', type=str, nargs='+', help='type of coordinate atoms')
+    parser.add_argument('--m1', type=str, help='name of central molecules')
+    parser.add_argument('--m2', type=str, help='name of coordinate molecules')
+    parser.add_argument('-o', '--output', required=True, type=str, help='Output prefix')
+    parser.add_argument('-b', '--begin', default=0, type=int,
+                        help='first frame to analyze. Index starts from 0')
+    parser.add_argument('-e', '--end', default=-1, type=int,
+                        help='last frame (not included) to analyze. Index starts from 0. '
+                             '-1 means until last frames (included)')
+    parser.add_argument('--maxr', default=1.0, type=float,
+                        help='max distance (nm) for calculation of distribution')
+    parser.add_argument('--dr', default=0.01, type=float,
+                        help='bin size (nm) for calculation of distribution')
+    parser.add_argument('--ignore', nargs='+', default=[], type=str,
+                        help='ignore these molecules in topology in case topology and trajectory do not match')
+    parser.add_argument('--skip', default=1, type=int, help='skip frames in trajectory')
+
+    return parser.parse_args()
+
+
+if __name__ == '__main__':
+    args = parse_args()
+    top = Topology.open(args.top)
+    if args.ignore != []:
+        molecules = [mol for mol in top.molecules if mol.name not in args.ignore]
+        top.update_molecules(molecules)
+    logger.info(top)
+
+    trj = Trajectory.open(args.input)
+    logger.info(trj)
+
+    if (top.n_atom != trj.n_atom):
+        raise Exception('Number of atoms in topology and trajectory files do not match')
+
+    if args.m1 is None:
+        group1 = [[atom] for atom in top.atoms if atom.type in args.a1]
+    else:
+        group1 = [[atom for atom in mol.atoms if atom.type in args.a1]
+                  for mol in top.molecules if mol.name == args.m1]
+    ids_group1 = [[atom.id for atom in atoms] for atoms in group1]
+    masses_group1 = [[atom.mass for atom in atoms] for atoms in group1]
+
+    if args.m2 is None:
+        group2 = [[atom] for atom in top.atoms if atom.type in args.a2]
+    else:
+        group2 = [[atom for atom in mol.atoms if atom.type in args.a2]
+                  for mol in top.molecules if mol.name == args.m2]
+    ids_group2 = [[atom.id for atom in atoms] for atoms in group2]
+    masses_group2 = [[atom.mass for atom in atoms] for atoms in group2]
+
+    if args.end > trj.n_frame or args.end == -1:
+        args.end = trj.n_frame
+
+    dr = args.dr
+    n_bin = math.ceil(args.maxr / dr) + 1
+    edges = np.array([dr * (i - 0.5) for i in range(n_bin + 1)], dtype=np.float32)
+    r_array = (edges[1:] + edges[:-1]) / 2
+    rdf_array = np.zeros(n_bin, dtype=np.float32)
+
+
+    def _get_weighted_center(positions, weight):
+        return np.sum(positions * np.array(weight)[:, np.newaxis], axis=0) / sum(weight)
+
+
+    def _get_com_group(positions, ids_group, masses_group):
+        com_group = []
+        for ids, masses in zip(ids_group, masses_group):
+            poss = positions[ids]
+            if len(ids) == 1:
+                pos = poss[0]
+            else:
+                pos = _get_weighted_center(poss, masses)
+            com_group.append(pos)
+        return com_group
+
+
+    n_frame = 0
+    for i in range(args.begin, args.end, args.skip):
+        n_frame += 1
+        frame = trj.read_frame(i)
+        sys.stdout.write('\r    frame %i' % i)
+
+        com_group1 = _get_com_group(frame.positions, ids_group1, masses_group1)
+        com_group2 = _get_com_group(frame.positions, ids_group2, masses_group2)
+
+        vol = frame.cell.volume
+        density_pair = len(group1) * len(group2) / vol
+
+        density_array = np.zeros(len(r_array), dtype=np.float32)
+        for com1 in com_group1:
+            for com2 in com_group2:
+                distance = periodic_distance(com1, com2, frame.cell.size, args.maxr + dr / 2)
+                if distance is not None and distance < args.maxr + dr / 2:
+                    idx_r = int((distance - edges[0]) / dr)
+                    density_array[idx_r] += 1
+
+        rdf_array[1:] += density_array[1:] / (4 * np.pi * r_array[1:] ** 2 * dr) / density_pair
+
+    rdf_array = rdf_array / n_frame
+
+    name_column_dict = {'r'  : r_array,
+                        'rdf': rdf_array}
+    print_data_to_file(name_column_dict, f'{args.output}-rdf.txt')
+
+    fig, ax = plt.subplots()
+    ax.set(xlabel='r (nm)', ylabel='RDF')
+    ax.plot(r_array, rdf_array, label='RDF')
+    ax.legend()
+    fig.tight_layout()
+    fig.savefig(f'{args.output}-rdf.png')
```

### Comparing `mstk-0.3.3.dev11/scripts/ffconv.py` & `mstk-0.3.4/scripts/ffconv.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/scripts/quick-sim.py` & `mstk-0.3.4/scripts/quick-sim.py`

 * *Files identical despite different names*

### Comparing `mstk-0.3.3.dev11/scripts/topconv.py` & `mstk-0.3.4/scripts/topconv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,87 @@
 #!/usr/bin/env python3
 
 import argparse
 from mstk.topology import Topology
+from mstk.trajectory import Trajectory
 from mstk.forcefield import ForceField
+from mstk import logger
 
-parser = argparse.ArgumentParser()
-parser.add_argument('input', nargs='+', type=str, help='topology file')
-parser.add_argument('-n', '--number', nargs='+', type=int, help='number of molecules')
-parser.add_argument('-o', '--output', required=True, type=str, help='output trajectory file')
-parser.add_argument('--ignore', nargs='+', default=[], type=str, help='ignore these molecule types')
-parser.add_argument('-f', '--ff', type=str, help='reassign charge from FF')
-parser.add_argument('--qscale', default=1, type=float, help='scale the charge of atoms')
-parser.add_argument('--qscaleignore', nargs='+', default=[], type=str,
-                    help='ignore these molecule names for charge scaling')
-parser.add_argument('--qscaleignoreatom', nargs='+', default=[], type=str,
-                    help='ignore these atom types for charge scaling')
-parser.add_argument('--box', nargs=3, default=[-1, -1, -1], type=float,
-                    help='overwrite the box dimensions')
-parser.add_argument('--shift', nargs=3, default=[0, 0, 0], type=float,
-                    help='shift the positions of all atoms')
-parser.add_argument('--ua', action='store_true',
-                    help='remove non-polar hydrogen atoms and relevant connectivities. '
-                         'Hydrogens bonded to O/N/S/P are kept intact')
-args = parser.parse_args()
-
-top_list = [Topology.open(inp) for inp in args.input]
-if args.number is None:
-    args.number = [1] * len(top_list)
-
-molecules = []
-for top, n in zip(top_list, args.number):
-    molecules.extend(top.molecules * n)
-if args.ignore:
-    molecules = [mol for mol in molecules if mol.name not in args.ignore]
-
-top = top_list[0]
-top.update_molecules(molecules)
-print(f'Topology info: {top.n_atom} atoms {top.n_molecule} molecules')
-
-if args.ua:
-    for mol in top.molecules:
-        mol.remove_non_polar_hydrogens(update_topology=False)
-    top.update_molecules(top.molecules)
-    print(f'United-atom topology info: {top.n_atom} atoms')
-
-if args.ff:
-    ff = ForceField.open(args.ff)
-    ff.assign_charge(top)
-    print(f'Net charge = {sum(a.charge for a in top.atoms)}')
-
-if args.qscale != 1:
-    for atom in top.atoms:
-        if atom.type in args.qscaleignoreatom or atom.molecule.name in args.qscaleignore:
-            continue
-        atom.charge *= args.qscale
-
-box = [args.box[k] if args.box[k] != -1 else top.cell.size[k] for k in range(3)]
-top.cell.set_box(box)
-
-if top.has_position and set(args.shift) != {0}:
-    for atom in top.atoms:
-        atom.position += args.shift
 
-top.write(args.output)
+def parse_args():
+    parser = argparse.ArgumentParser()
+    parser.add_argument('input', nargs='+', type=str, help='topology file')
+    parser.add_argument('-n', '--number', nargs='+', type=int, help='number of molecules')
+    parser.add_argument('-c', '--conf', type=str,
+                        help='configuration file with positions and box. The last frame will be used. '
+                             'This is for writing topology in formats supporting positions, e.g. PDB, XYZ')
+    parser.add_argument('-o', '--output', required=True, type=str, help='output topology file')
+    parser.add_argument('--ignore', nargs='+', default=[], type=str, help='ignore these molecule types')
+    parser.add_argument('-f', '--ff', type=str, help='reassign charge from FF')
+    parser.add_argument('--qscale', default=1, type=float, help='scale the charge of atoms')
+    parser.add_argument('--qscaleignore', nargs='+', default=[], type=str,
+                        help='ignore these molecule names for charge scaling')
+    parser.add_argument('--box', nargs='+', type=float,
+                        help='overwrite the box dimensions')
+    parser.add_argument('--shift', nargs=3, default=[0, 0, 0], type=float,
+                        help='shift the positions of all atoms')
+    parser.add_argument('--ua', action='store_true',
+                        help='remove hydrogen atoms bonded to C/Si. '
+                             'Also remove the relevant bonds/angles/dihedrals/impropers')
+
+    return parser.parse_args()
+
+
+if __name__ == '__main__':
+    args = parse_args()
+
+    top_list = [Topology.open(inp) for inp in args.input]
+    if args.number is None:
+        args.number = [1] * len(top_list)
+
+    molecules = []
+    for top, n in zip(top_list, args.number):
+        molecules.extend(top.molecules * n)
+    if args.ignore:
+        molecules = [mol for mol in molecules if mol.name not in args.ignore]
+
+    top = top_list[0]
+    top.update_molecules(molecules)
+    logger.info(str(top))
+
+    if args.conf:
+        frame = Trajectory.read_frame_from_file(args.conf, -1)
+        top.cell.set_box(frame.cell.vectors)
+        top.set_positions(frame.positions)
+
+    if args.ua:
+        for mol in top.molecules:
+            mol.remove_non_polar_hydrogens(update_topology=False)
+        top.update_molecules(top.molecules)
+        logger.info(str(top))
+
+    if args.ff:
+        ff = ForceField.open(args.ff)
+        ff.assign_charge(top)
+        logger.info(f'Net charge = {sum(a.charge for a in top.atoms)}')
+
+    if args.qscale != 1:
+        for mol in top.molecules:
+            if mol.name in args.qscaleignore:
+                continue
+            for atom in mol.atoms:
+                atom.charge *= args.qscale
+
+    if args.box is not None:
+        if len(args.box) == 3:
+            box = args.box
+        elif len(args.box) == 1:
+            box = args.box * 3
+        else:
+            raise Exception('box should be float or list of three floats')
+        top.cell.set_box(box)
+
+    if top.has_position and set(args.shift) != {0}:
+        for atom in top.atoms:
+            atom.position += args.shift
+
+    top.write(args.output, atom_type=True)
```

### Comparing `mstk-0.3.3.dev11/scripts/trjconv.py` & `mstk-0.3.4/scripts/trjconv.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,65 +2,86 @@
 
 import sys
 import argparse
 import numpy as np
 
 from mstk.topology import Topology
 from mstk.trajectory import Trajectory
+from mstk import logger
 
-parser = argparse.ArgumentParser()
-parser.add_argument('input', nargs='+', type=str,
-                    help='trajectory file for atomic positions')
-parser.add_argument('-p', '--top', required=True, type=str,
-                    help='psf or lammps data file for topology information')
-parser.add_argument('-o', '--output', required=True, type=str, help='output trajectory file')
-parser.add_argument('-b', '--begin', default=0, type=int, help='first frame to output')
-parser.add_argument('-e', '--end', default=-1, type=int,
-                    help='last frame (not included unless set to -1) to output')
-parser.add_argument('--skip', default=1, type=int, help='skip frames between output')
-parser.add_argument('--topignore', nargs='+', default=[], type=str,
-                    help='ignore these molecule names in topology in case topology and trajectory do not match')
-parser.add_argument('--ignore', nargs='+', default=[], type=str, help='ignore these molecule names')
-parser.add_argument('--ignoreatom', nargs='+', default=[], type=str, help='ignore these atom types')
-parser.add_argument('--box', nargs=3, default=[-1, -1, -1], type=float,
-                    help='overwrite the box dimensions')
-parser.add_argument('--shift', nargs=3, default=[0, 0, 0], type=float,
-                    help='shift the positions of all atoms')
-args = parser.parse_args()
-
-top = Topology.open(args.top)
-if args.topignore != []:
-    molecules = [mol for mol in top.molecules if mol.name not in args.topignore]
-    top = Topology()
-    top.update_molecules(molecules)
-print('Topology info: ', top.n_atom, 'atoms;', top.n_molecule, 'molecules')
-trj = Trajectory.open(args.input)
-print('Trajectory info: ', trj.n_atom, 'atoms;', trj.n_frame, 'frames')
-
-if (top.n_atom != trj.n_atom):
-    raise Exception('Number of atoms in topology and trajectory files do not match')
-
-trj_out = Trajectory.open(args.output, 'w')
-
-if args.ignore or args.ignoreatom:
-    subset = [atom.id for atom in top.atoms
-              if atom.type not in args.ignoreatom and atom.molecule.name not in args.ignore]
-else:
-    subset = None
-
-if args.end > trj.n_frame or args.end == -1:
-    args.end = trj.n_frame
-
-if args.shift[0] != 0 or args.shift[1] != 0 or args.shift[2] != 0:
-    pos_shift = np.array([args.shift] * top.n_atom)
-else:
-    pos_shift = None
-
-for i in range(args.begin, args.end, args.skip):
-    sys.stdout.write('\r    %i' % i)
-    frame = trj.read_frame(i)
-    box = np.array([args.box[k] if args.box[k] != -1 else frame.cell.size[k] for k in range(3)])
-    frame.cell.set_box(box)
-    if pos_shift is not None:
-        frame.positions += pos_shift
-    trj_out.write_frame(frame, top, subset=subset)
-trj_out.close()
+
+def parse_args():
+    parser = argparse.ArgumentParser()
+    parser.add_argument('input', nargs='+', type=str, help='trajectory files')
+    parser.add_argument('-p', '--top', required=True, type=str, help='topology file')
+    parser.add_argument('-o', '--output', required=True, type=str, help='output trajectory file')
+    parser.add_argument('-b', '--begin', default=0, type=int,
+                        help='read from this frame (included). '
+                             'A negative value has the same meaning as in Python list')
+    parser.add_argument('-e', '--end', type=int,
+                        help='read until this frame (not included). '
+                             'A negative value has the same meaning as in Python list. '
+                             'If not set, will read until the end of the trajectory')
+    parser.add_argument('--skip', default=1, type=int, help='read every N frames')
+    parser.add_argument('--ignore', nargs='+', default=[], type=str, help='ignore these molecule names')
+    parser.add_argument('--ignoreatom', nargs='+', default=[], type=str, help='ignore these atom types')
+    parser.add_argument('--wrapfirst', action='store_true',
+                        help='shift the positions of all atoms so that all residues in the first frame are in the main cell')
+    parser.add_argument('--box', nargs=3, default=[-1, -1, -1], type=float,
+                        help='overwrite the box dimensions')
+    parser.add_argument('--shift', nargs=3, default=[0, 0, 0], type=float,
+                        help='shift the positions of all atoms')
+    return parser.parse_args()
+
+
+if __name__ == '__main__':
+    args = parse_args()
+
+    top = Topology.open(args.top)
+    logger.info(top)
+
+    trj = Trajectory.open(args.input)
+    logger.info(trj)
+
+    if (top.n_atom != trj.n_atom):
+        raise Exception('Number of atoms in topology and trajectory files do not match')
+
+    trj_out = Trajectory.open(args.output, 'w')
+
+    if args.ignore or args.ignoreatom:
+        subset = [atom.id for atom in top.atoms
+                  if atom.type not in args.ignoreatom and atom.molecule.name not in args.ignore]
+    else:
+        subset = None
+
+    if args.begin < 0:
+        args.begin += trj.n_frame
+    if args.end is None or args.end > trj.n_frame:
+        args.end = trj.n_frame
+    elif args.end < 0:
+        args.end += trj.n_frame
+
+    cell_offset = np.zeros((top.n_atom, 3), dtype=int)
+    if args.wrapfirst:
+        frame = trj.read_frame(args.begin)
+        for res in top.residues:
+            ids = [atom.id for atom in res.atoms]
+            positions = frame.positions[ids]
+            center = np.sum(positions, axis=0) / len(positions)
+            cell_offset[ids] = np.floor(center / frame.cell.size).astype(int)
+
+    if any(val != 0 for val in args.shift):
+        pos_shift = np.array([args.shift] * top.n_atom)
+    else:
+        pos_shift = None
+
+    for i in range(args.begin, args.end, args.skip):
+        sys.stdout.write('\r    %i' % i)
+        frame = trj.read_frame(i)
+        box = np.array([args.box[k] if args.box[k] != -1 else frame.cell.size[k] for k in range(3)])
+        frame.cell.set_box(box)
+        if args.wrapfirst:
+            frame.positions -= cell_offset * box
+        if pos_shift is not None:
+            frame.positions += pos_shift
+        trj_out.write_frame(frame, top, subset=subset)
+    trj_out.close()
```

### Comparing `mstk-0.3.3.dev11/scripts/wham-pp.py` & `mstk-0.3.4/scripts/wham-pp.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,108 +1,115 @@
 #!/usr/bin/env python3
 
 import os
 import argparse
 import numpy as np
 
-parser = argparse.ArgumentParser()
-parser.add_argument('-b', '--begin', type=float, default=0)
-parser.add_argument('-p', '--plot', action='store_true', help='plot the histogram')
-parser.add_argument('--skip', type=int, default=1)
-parser.add_argument('--nbin', type=int, help='number of bins for histogram')
-parser.add_argument('--type', type=str, default='openmm', choices=['openmm', 'lammps', 'plumed'])
-args = parser.parse_args()
-
-BEGIN = args.begin
-SKIP = args.skip
-
-r0_k_list = []
-files = filter(os.path.isdir, os.listdir(os.getcwd()))
-for i in files:
-    if os.path.isdir(i) and '-' in i and \
-            (i[0].isdigit() or i[0].startswith('_')) and i[-1].isdigit():
-        r0 = i.split('-')[0]
-        k = i.split('-')[1]
-        r0_k_list.append((r0, k))
-r0_k_list.sort(key=lambda x: float(x[0].replace('_', '-')))
-
-outf_meta = open('wham-meta', 'w')
-for r0, k in r0_k_list:
-    outfile = 'wham-' + r0 + '-' + k + '.txt'
-    outf = open(outfile, 'w')
-    if args.type == 'openmm':
-        _START = False
-        with open(r0 + '-' + k + '/_job.out') as f:
-            lines = f.read().splitlines()
-        for line in lines:
-            if line.startswith('#"'):
-                _START = True
-                continue
-            if not _START:
-                continue
-            try:
-                words = line.strip().split()
-                step = int(words[0])
-            except:
-                continue
-            if step >= BEGIN and step % SKIP == 0:
-                str = line.strip().split()
-                time = float(words[0])
-                r = float(words[-1])
-                outf.write('%.1f %.6f\n' % (time, r))
-    elif args.type == 'lammps':
-        _CYCLE = 0
-        _START = False
-        countline = 0
-        with open(r0 + '-' + k + '/log') as f:
-            lines = f.read().splitlines()
-        for line in lines:
-            if line.startswith('Loop') and _CYCLE == 2:
-                break
-            if line.startswith('Step'):
-                _CYCLE += 1
-                if _CYCLE == 2:
+
+def parse_args():
+    parser = argparse.ArgumentParser()
+    parser.add_argument('-b', '--begin', type=float, default=0)
+    parser.add_argument('-p', '--plot', action='store_true', help='plot the histogram')
+    parser.add_argument('--skip', type=int, default=1)
+    parser.add_argument('--nbin', type=int, help='number of bins for histogram')
+    parser.add_argument('--type', type=str, default='openmm', choices=['openmm', 'lammps', 'plumed'])
+
+    return parser.parse_args()
+
+
+if __name__ == '__main__':
+    args = parse_args()
+
+    BEGIN = args.begin
+    SKIP = args.skip
+
+    r0_k_list = []
+    files = filter(os.path.isdir, os.listdir(os.getcwd()))
+    for i in files:
+        if os.path.isdir(i) and '-' in i and \
+                (i[0].isdigit() or i[0].startswith('_')) and i[-1].isdigit():
+            r0 = i.split('-')[0]
+            k = i.split('-')[1]
+            r0_k_list.append((r0, k))
+    r0_k_list.sort(key=lambda x: float(x[0].replace('_', '-')))
+
+    outf_meta = open('wham-meta', 'w')
+    for r0, k in r0_k_list:
+        outfile = 'wham-' + r0 + '-' + k + '.txt'
+        outf = open(outfile, 'w')
+        if args.type == 'openmm':
+            _START = False
+            with open(r0 + '-' + k + '/_job.out') as f:
+                lines = f.read().splitlines()
+            for line in lines:
+                if line.startswith('#"'):
                     _START = True
-            if _START:
+                    continue
+                if not _START:
+                    continue
+                try:
+                    words = line.strip().split()
+                    step = int(words[0])
+                except:
+                    continue
+                if step >= BEGIN and step % SKIP == 0:
+                    str = line.strip().split()
+                    time = float(words[0])
+                    r = float(words[-1])
+                    outf.write('%.1f %.6f\n' % (time, r))
+        elif args.type == 'lammps':
+            _CYCLE = 0
+            _START = False
+            countline = 0
+            with open(r0 + '-' + k + '/log') as f:
+                lines = f.read().splitlines()
+            for line in lines:
+                if line.startswith('Loop') and _CYCLE == 2:
+                    break
+                if line.startswith('Step'):
+                    _CYCLE += 1
+                    if _CYCLE == 2:
+                        _START = True
+                if _START:
+                    countline += 1
+                    if countline > BEGIN + 1 and countline % SKIP == 0:
+                        str = line.strip().split()
+                        time = float(str[0])
+                        r = float(str[6])
+                        outf.write('%.1f %.6f\n' % (time, r))
+        elif args.type == 'plumed':
+            countline = 0
+            with open(r0 + '-' + k + '/DIS.txt') as f:
+                lines = f.read().splitlines()
+            for line in lines:
                 countline += 1
                 if countline > BEGIN + 1 and countline % SKIP == 0:
                     str = line.strip().split()
                     time = float(str[0])
-                    r = float(str[6])
+                    r = float(str[1])
                     outf.write('%.1f %.6f\n' % (time, r))
-    elif args.type == 'plumed':
-        countline = 0
-        with open(r0 + '-' + k + '/DIS.txt') as f:
-            lines = f.read().splitlines()
-        for line in lines:
-            countline += 1
-            if countline > BEGIN + 1 and countline % SKIP == 0:
-                str = line.strip().split()
-                time = float(str[0])
-                r = float(str[1])
-                outf.write('%.1f %.6f\n' % (time, r))
-    outf.close()
-    outf_meta.write('%s %s %s\n' % (outfile, r0.replace('_', '-'), k))  # replace the leading _ with -
-outf_meta.close()
-
-if args.plot:
-    import matplotlib
-
-    matplotlib.use('Agg')
-    import matplotlib.pyplot as plt
-
-    fig = plt.gcf()
-    fig.set_size_inches(16, 8)
-    plt.grid(True)
-    files = filter(lambda x: x.startswith('wham-') and x.endswith('.txt'), os.listdir(os.getcwd()))
-    for r0, k in r0_k_list:
-        array = np.genfromtxt('wham-%s-%s.txt' %(r0, k))
-        data = array[:, 1]
-        if args.nbin:
-            hist, bins = np.histogram(data, bins=args.nbin)
-        else:
-            hist, bins = np.histogram(data)
-        center = (bins[:-1] + bins[1:]) / 2.
-        plt.plot(center, hist, linewidth=2)
-    plt.savefig('wham-hist.png')
+        outf.close()
+        outf_meta.write('%s %s %s\n' % (outfile, r0.replace('_', '-'), k))  # replace the leading _ with -
+    outf_meta.close()
+
+    if args.plot:
+        import matplotlib
+
+        matplotlib.use('Agg')
+        import matplotlib.pyplot as plt
+
+        fig = plt.gcf()
+        fig.set_size_inches(16, 8)
+        plt.grid(True)
+        files = filter(lambda x: x.startswith('wham-') and x.endswith('.txt'), os.listdir(os.getcwd()))
+        for r0, k in r0_k_list:
+            array = np.genfromtxt('wham-%s-%s.txt' % (r0, k))
+            data = array[:, 1]
+            if args.nbin:
+                hist, bins = np.histogram(data, bins=args.nbin)
+            else:
+                hist, bins = np.histogram(data)
+            center = (bins[:-1] + bins[1:]) / 2.
+            plt.plot(center, hist, linewidth=2)
+        plt.savefig('wham-hist.png')
 
-# os.system('wham %f %f %s %s 298.15 0 wham-meta wham-pmf' %(hist_min, hist_max, bins, tol))
+    # os.system('wham %f %f %s %s 298.15 0 wham-meta wham-pmf' %(hist_min, hist_max, bins, tol))
```

### Comparing `mstk-0.3.3.dev11/setup.py` & `mstk-0.3.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     long_description = f.read()
 
 dir_scripts = 'scripts'
 scripts = [os.path.join(dir_scripts, f) for f in os.listdir(dir_scripts)]
 
 setuptools.setup(
     name='mstk',
-    version='0.3.3.dev11',
+    version='0.3.4',
     author='Zheng Gong',
     author_email='z.gong@outlook.com',
     description='Molecular simulation toolkit',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/z-gong/mstk',
     packages=setuptools.find_packages(),
```

