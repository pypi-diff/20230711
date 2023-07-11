# Comparing `tmp/cobaya_utilities-0.1.2.tar.gz` & `tmp/cobaya_utilities-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cobaya_utilities-0.1.2.tar", last modified: Mon Dec  5 16:54:52 2022, max compression
+gzip compressed data, was "cobaya_utilities-0.1.3.tar", last modified: Tue Jul 11 08:00:01 2023, max compression
```

## Comparing `cobaya_utilities-0.1.2.tar` & `cobaya_utilities-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 16:54:52.692356 cobaya_utilities-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (122)     2480 2022-12-05 16:54:52.692356 cobaya_utilities-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1817 2022-12-05 16:54:44.000000 cobaya_utilities-0.1.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 16:54:52.692356 cobaya_utilities-0.1.2/cobaya_utilities/
--rw-r--r--   0 runner    (1001) docker     (122)       73 2022-12-05 16:54:44.000000 cobaya_utilities-0.1.2/cobaya_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      497 2022-12-05 16:54:52.692356 cobaya_utilities-0.1.2/cobaya_utilities/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     9780 2022-12-05 16:54:44.000000 cobaya_utilities-0.1.2/cobaya_utilities/fisher.py
--rw-r--r--   0 runner    (1001) docker     (122)     9661 2022-12-05 16:54:44.000000 cobaya_utilities-0.1.2/cobaya_utilities/plots.py
--rw-r--r--   0 runner    (1001) docker     (122)    16200 2022-12-05 16:54:44.000000 cobaya_utilities-0.1.2/cobaya_utilities/tools.py
--rw-r--r--   0 runner    (1001) docker     (122)      284 2022-12-05 16:54:44.000000 cobaya_utilities-0.1.2/cobaya_utilities/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-05 16:54:52.692356 cobaya_utilities-0.1.2/cobaya_utilities.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2480 2022-12-05 16:54:52.000000 cobaya_utilities-0.1.2/cobaya_utilities.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      414 2022-12-05 16:54:52.000000 cobaya_utilities-0.1.2/cobaya_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-05 16:54:52.000000 cobaya_utilities-0.1.2/cobaya_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2022-12-05 16:54:52.000000 cobaya_utilities-0.1.2/cobaya_utilities.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2022-12-05 16:54:52.000000 cobaya_utilities-0.1.2/cobaya_utilities.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      766 2022-12-05 16:54:45.000000 cobaya_utilities-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-05 16:54:52.692356 cobaya_utilities-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1029 2022-12-05 16:54:45.000000 cobaya_utilities-0.1.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    83635 2022-12-05 16:54:45.000000 cobaya_utilities-0.1.2/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:00:01.850476 cobaya_utilities-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-11 08:00:01.850476 cobaya_utilities-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-07-11 07:59:58.000000 cobaya_utilities-0.1.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:00:01.850476 cobaya_utilities-0.1.3/cobaya_utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-07-11 07:59:58.000000 cobaya_utilities-0.1.3/cobaya_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-11 08:00:01.850476 cobaya_utilities-0.1.3/cobaya_utilities/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-07-11 07:59:58.000000 cobaya_utilities-0.1.3/cobaya_utilities/fisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13586 2023-07-11 07:59:58.000000 cobaya_utilities-0.1.3/cobaya_utilities/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17061 2023-07-11 07:59:58.000000 cobaya_utilities-0.1.3/cobaya_utilities/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-11 07:59:58.000000 cobaya_utilities-0.1.3/cobaya_utilities/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 08:00:01.850476 cobaya_utilities-0.1.3/cobaya_utilities.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-07-11 08:00:01.000000 cobaya_utilities-0.1.3/cobaya_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-11 08:00:01.000000 cobaya_utilities-0.1.3/cobaya_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 08:00:01.000000 cobaya_utilities-0.1.3/cobaya_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-11 08:00:01.000000 cobaya_utilities-0.1.3/cobaya_utilities.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-11 08:00:01.000000 cobaya_utilities-0.1.3/cobaya_utilities.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-11 07:59:58.000000 cobaya_utilities-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 08:00:01.850476 cobaya_utilities-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-07-11 07:59:58.000000 cobaya_utilities-0.1.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83635 2023-07-11 07:59:58.000000 cobaya_utilities-0.1.3/versioneer.py
```

### Comparing `cobaya_utilities-0.1.2/PKG-INFO` & `cobaya_utilities-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobaya_utilities
-Version: 0.1.2
+Version: 0.1.3
 Summary: A set of functions to deal with MCMC output from cobaya
 Home-page: https://github.com/xgarrido/cobaya_utilities.git
 Author: Xavier Garrido
 Author-email: xavier.garrido@lal.in2p3.fr
 Keywords: cobaya,MCMC,plot
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
@@ -22,16 +22,17 @@
 
 A set of tools to deal with MCMC chains and a complement to `cobaya
 <https://github.com/CobayaSampler/cobaya>`_ and `getdist <https://github.com/cmbant/getdist>`_.
 
 .. image:: https://img.shields.io/pypi/v/cobaya-utilities.svg?style=flat
    :target: https://pypi.python.org/pypi/cobaya-utilities
 
-.. image:: https://img.shields.io/github/workflow/status/xgarrido/cobaya_utilities/Unit%20test
+.. image:: https://img.shields.io/github/actions/workflow/status/xgarrido/cobaya_utilities/testing.yml?branch=master
    :target: https://github.com/xgarrido/cobaya_utilities/actions
+   :alt: GitHub Workflow Status
 
 .. image:: https://readthedocs.org/projects/cobaya-utilities/badge/?version=latest
    :target: https://cobaya-utilities.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/xgarrido/cobaya_utilities/master
```

### Comparing `cobaya_utilities-0.1.2/README.rst` & `cobaya_utilities-0.1.3/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 A set of tools to deal with MCMC chains and a complement to `cobaya
 <https://github.com/CobayaSampler/cobaya>`_ and `getdist <https://github.com/cmbant/getdist>`_.
 
 .. image:: https://img.shields.io/pypi/v/cobaya-utilities.svg?style=flat
    :target: https://pypi.python.org/pypi/cobaya-utilities
 
-.. image:: https://img.shields.io/github/workflow/status/xgarrido/cobaya_utilities/Unit%20test
+.. image:: https://img.shields.io/github/actions/workflow/status/xgarrido/cobaya_utilities/testing.yml?branch=master
    :target: https://github.com/xgarrido/cobaya_utilities/actions
+   :alt: GitHub Workflow Status
 
 .. image:: https://readthedocs.org/projects/cobaya-utilities/badge/?version=latest
    :target: https://cobaya-utilities.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/xgarrido/cobaya_utilities/master
```

### Comparing `cobaya_utilities-0.1.2/cobaya_utilities/fisher.py` & `cobaya_utilities-0.1.3/cobaya_utilities/fisher.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,15 +204,15 @@
                     sizes=(50, 200),
                     size_norm=(-1, 1),
                 )
                 .set(xlabel="", ylabel="", aspect="equal")
                 .set_xticklabels(rotation=90)
                 .despine(left=True, bottom=True)
             )
-            for artist in g.legend.legendHandles:
+            for artist in g.legend.legend_handles:
                 artist.set_edgecolor("0.7")
     else:
         mask = np.triu(np.ones_like(matrix, dtype=bool))
         sns.heatmap(
             matrix,
             mask=mask,
             cmap=cmap,
```

### Comparing `cobaya_utilities-0.1.2/cobaya_utilities/plots.py` & `cobaya_utilities-0.1.3/cobaya_utilities/plots.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,103 +1,217 @@
+import os
+from dataclasses import dataclass
+from typing import Optional
+
+import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from scipy import stats
 
-_use_seaborn = False
+
+@dataclass
+class Sample:
+    path: str
+    label: str
+    color: Optional[str] = None
+
+
+@dataclass
+class SampleCollection:
+    samples: list[Sample] = None
 
 
 def set_style(
-    use_seaborn=True, seaborn_style="ticks", use_svg=True, print_load_details=False, **rc
+    use_seaborn=False,
+    seaborn_style="ticks",
+    seaborn_context="paper",
+    palette="tab10",
+    use_svg=False,
+    use_tex=False,
+    print_load_details=False,
+    **rc,
 ):
     """Set default plot settings
 
     Parameters
     ----------
     use_seaborn: bool
       use seaborn theming option
     seaborn_style: str
       set seaborn style (default: `ticks`)
+    seaborn_context: str
+      set seaborn context (default: `paper`)
+    palette: str
+      color palette name to be used for individual colors (default: tab10)
     use_svg: bool
       use `svg` output format for figure
+    use_tex: bool
+      use LaTeX axis labels
     print_load_details: bool
       print load details when getdist loads samples
     rc: dict
       overload matplotlib rc parameters
     """
+
+    colors = None
+    if palette == "the-lab":
+        colors = dict(
+            blue="#015692",
+            orange="#b75501",
+            green="#54790d",
+            red="#c02d2e",
+            purple="#803378",
+            gray="#656e77",
+        )
+    elif palette == "getdist":
+        colors = dict(blue="#006FED", red="#E03424", green="#009966")
+    elif use_seaborn:
+        palette = "deep"
+
+    _default_color_cycle = [
+        "blue",
+        "orange",
+        "green",
+        "red",
+        "purple",
+        "brown",
+        "pink",
+        "gray",
+        "yellow",
+        "cyan",
+    ]
+    if colors:
+        for color, code in colors.items():
+            rgb = mpl.colors.colorConverter.to_rgb(color)
+            mpl.colors.colorConverter.colors[code] = rgb
+            mpl.colors.colorConverter.cache[code] = rgb
+
+        _default_prop_cycle = mpl.rcParams["axes.prop_cycle"].by_key()["color"]
+        mpl.rcParams["axes.prop_cycle"] = mpl.cycler(
+            color=[
+                colors.get(color, _default_prop_cycle[i])
+                for i, k in enumerate(_default_color_cycle)
+            ]
+        )
+    elif palette in ["tab10", "pastel", "muted", "bright", "deep", "colorblind", "dark"]:
+        for code, color in zip(_default_color_cycle, sns.color_palette(palette)):
+            rgb = mpl.colors.colorConverter.to_rgb(color)
+            mpl.colors.colorConverter.colors[code] = rgb
+            mpl.colors.colorConverter.cache[code] = rgb
+    else:
+        sns.set_palette(palette, n_colors=10)
+
     import getdist
 
     getdist.chains.print_load_details = print_load_details
 
+    if use_tex and use_svg:
+        print("Using latex text with svg output format does not play well. Disable the later one")
+        use_svg = False
+
     if use_svg:
         import matplotlib_inline
 
         matplotlib_inline.backend_inline.set_matplotlib_formats("svg")
 
-    rc = rc or {"axes.spines.top": False, "axes.spines.right": False, "figure.figsize": (8, 6)}
+    rc = rc or {"axes.spines.top": False, "axes.spines.right": False}
+    if use_tex:
+        rc.update({"text.usetex": True})
     if use_seaborn:
-        _use_seaborn = True
-        sns.set_theme(rc=rc, style=seaborn_style)
+        sns.set_theme(rc=rc, style=seaborn_style, context=None if use_tex else seaborn_context)
+    else:
+        plt.rcParams.update(rc)
+
 
+def get_default_settings(colors=None, linewidth=2, num_plot_contours=3):
+    """Set default getdist plot settings
+
+    Parameters
+    ----------
+    colors: list
+      list of colors to be used
+    linewidth: float
+      line width of contours and KDE distributions (default: 2)
+    num_plot_contours: int
+      number of contour levels (default: 3)
+    """
+    if not colors:
+        colors = plt.rcParams["axes.prop_cycle"].by_key()["color"]
 
-def get_default_settings():
-    """Set default getdist plot settings"""
     from getdist.plots import GetDistPlotSettings
 
     plot_settings = GetDistPlotSettings()
-    plot_settings.num_plot_contours = 3
-    plot_settings.solid_colors = "tab10"
-    plot_settings.line_styles = "tab10"
-    plot_settings.linewidth = 2
+    plot_settings.solid_colors = colors
+    plot_settings.line_styles = colors
+    plot_settings.num_plot_contours = num_plot_contours
+    plot_settings.linewidth = linewidth
     plot_settings.legend_fontsize = 15
     plot_settings.legend_colored_text = True
     return plot_settings
 
 
-def show_inputs(axes, inputs, colors=None):
-    """Show inputs values on a given set of axes
+def get_mc_samples(mcmc_samples, prefix="mcmc", burnin=0.4, no_cache=False):
+    from getdist.plots import loadMCSamples
+
+    samples = [
+        loadMCSamples(
+            os.path.join(path, prefix), settings={"ignore_rows": burnin}, no_cache=no_cache
+        )
+        for path in mcmc_samples.values()
+    ]
+    return list(mcmc_samples.keys()), samples
 
+
+def show_inputs(g, inputs, color=None, ls="--"):
+    """Show input/reference values on a given set of axes
     Parameters
     ----------
-    axes: array
-      array of matplotlib axes
+    g: getdist.plots
+      the getdist plotter instance
     inputs: dict
       dictionary holding loc/scale value for normal distribution
-    colors: list
-      list of colors to be applied
+    color: str
+      the color name
+    ls: str
+      the line style
     """
-    for i, ax in enumerate(axes):
-        x = np.linspace(*ax.get_xlim(), 100)
-        for j, values in enumerate(inputs):
-            mean, sigma = values[i]
-            if mean is None:
-                continue
-            y = stats.norm.pdf(x, mean, sigma)
-            color = colors[j] if colors is not None else f"C{j}"
-            ax.plot(x, y / np.max(y), color=color, ls="--")
+    for par, val in inputs.items():
+        if not (ax := g.get_axes_for_params(par)):
+            continue
+        if isinstance(val, float):
+            ax.axvline(val, color=color, ls=ls)
+        else:
+            x = np.linspace(*ax.get_xlim(), 100)
+            y = stats.norm.pdf(x, *val)
+            ax.plot(x, y / y.max(), color=color, ls=ls)
 
 
-def show_tau_prior(ax, loc=0.054, scale=0.0073):
+def show_tau_prior(g, loc=0.054, scale=0.0073, color="gray", ls="--"):
     """Dedicated function to plot tau prior
 
     Parameters
     ----------
-    ax: matplotlib.axis
-      the axis where to plot tau prior
+    g: getdist.plots
+      the getdist plotter instance
     loc: float
       the central tau value
     scale: float
       the scale/sigma of tau value
+    color: str
+      the color name
+    ls: str
+      the line style
     """
     from matplotlib.lines import Line2D
 
-    show_inputs([ax], inputs=[[(loc, scale)]], colors=["gray"])
-    ax.legend(
-        [Line2D([0], [0], color="gray", ls="--")],
+    show_inputs(g, inputs=dict(tau=(loc, scale)), color=color, ls=ls)
+    g.get_axes_for_params("tau").legend(
+        [Line2D([0], [0], color=color, ls=ls)],
         [r"$\tau$ prior"],
         loc="upper left",
         bbox_to_anchor=(1, 1),
     )
 
 
 def despine(g, all_axes=False, **kwargs):
@@ -272,7 +386,30 @@
                 prop={"size": 16},
             )
         results[ax.get_xlabel()] = {"value rec.": mu, "$\sigma$ rec.": sigma}
         ax.spines.left.set_visible(False)
 
     if return_results:
         return pd.DataFrame.from_dict(results, orient="index")
+
+
+def add_legend(fig=None, ax=None, labels=None, colors=None, ls=None, **kwargs):
+    from matplotlib.lines import Line2D
+
+    if not fig and not ax:
+        raise ValueError("Missing either fig or axis instance!")
+
+    colors = colors or [None for label in labels]
+    ls = ls or ["-" for label in labels]
+    handles = [Line2D([0], [0], color=colors[i], ls=ls[i]) for i, label in enumerate(labels)]
+
+    obj = fig or ax
+    leg = obj.legend(
+        handles,
+        labels,
+        bbox_to_anchor=kwargs.get("bbox_to_anchor", (0.5, 1)),
+        labelcolor=kwargs.get("labelcolor", "linecolor"),
+        loc=kwargs.get("loc", "center"),
+        title=kwargs.get("title"),
+        ncol=kwargs.get("ncol", 1),
+    )
+    leg._legend_box.align = "left"
```

### Comparing `cobaya_utilities-0.1.2/cobaya_utilities/tools.py` & `cobaya_utilities-0.1.3/cobaya_utilities/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,36 +95,44 @@
       prefix for chain names (default is "mcmc.")
     """
     create_symlink(mcmc_samples, prefix)
     r = re.compile(r"\[mcmc\] Progress @ (.*) : (.*) steps taken, and (.*) accepted.")
     regex_log = re.compile(r".*mcmc\.([0-9]+).log")
     regex_progress = re.compile(r".*mcmc\.([0-9]+).progress")
 
+    found_rminus1 = []
     data = {}
     for irow, (name, path) in enumerate(mcmc_samples.items()):
         files = _get_chain_filenames(path, prefix=prefix, suffix=".log")
         if not files:
             print(f"Missing log files for chains '{name}' within path '{path}'!")
             return
         for fn in sorted(files):
+            total_steps = 0
             idx = 1 if not (m := regex_log.match(fn)) else m.group(1)
             mcmc_name = f"mcmc {idx}"
             status = dict(done="[mcmc] The run has converged!", error="[mcmc] *ERROR*")
             data.setdefault(name, {}).update({(mcmc_name, "status"): "running"})
             with open(fn) as f:
                 for line in f:
                     for state, msg in status.items():
                         if msg in line:
                             data[name].update({(mcmc_name, "status"): state})
 
                     found = r.findall(line)
                     if len(found) == 0:
                         continue
-                    time, total_steps, accepted_steps = found[0]
-            total_steps, accepted_steps = int(total_steps), int(accepted_steps)
+                    time, current_steps, accepted_steps = found[0]
+                    current_steps = int(current_steps)
+                    total_steps = (
+                        current_steps
+                        if current_steps > total_steps
+                        else total_steps + current_steps
+                    )
+            accepted_steps = int(accepted_steps)
             rate = accepted_steps / total_steps
             for field, content in zip(
                 ["accept.", "total", "rate", "R-1"], [accepted_steps, total_steps, rate, None]
             ):
                 data[name].update({(mcmc_name, field): content})
         if with_gelman_rubin:
             files = _get_chain_filenames(path, suffix=".progress")
@@ -133,14 +141,15 @@
                 mcmc_name = f"mcmc {idx}"
                 with open(fn) as f:
                     for line in f:
                         pass
                     if line.startswith("#"):
                         continue
                     data[name].update({(mcmc_name, "R-1"): f"{float(line.split()[-2]):.2f}"})
+                    found_rminus1 += [mcmc_name]
 
     df = pd.DataFrame.from_dict(data, orient="index")
     df.dropna(axis=1, how="all", inplace=True)
 
     mcmc_names = list(df.columns.get_level_values(0).unique())
 
     # Append total count
@@ -164,18 +173,22 @@
             color=bar_color,
             height=50,
             width=60,
         )
     if with_color_gradient:
         cm = sns.color_palette(color_palette, as_cmap=True)
         s.background_gradient(subset=[(name, "rate") for name in mcmc_names], cmap=cm, axis=None)
-        if with_gelman_rubin:
-            cm = sns.color_palette(color_palette + "_r", as_cmap=True)
-            s.text_gradient(subset=[(name, "R-1") for name in mcmc_names], cmap=cm, axis=None)
-            # s.highlight_null(color="white")
+        # if with_gelman_rubin and found_rminus1:
+        #     cm = sns.color_palette(color_palette + "_r", as_cmap=True)
+        #     s.text_gradient(
+        #         subset=[(name, "R-1") for name in mcmc_names if name in found_rminus1],
+        #         cmap=cm,
+        #         axis=None,
+        #     )
+        #     # s.highlight_null(color="white")
         s.background_gradient(
             subset=[(all_name, "total")], cmap=sns.color_palette("Blues", as_cmap=True)
         )
         s.background_gradient(
             subset=[(all_name, "rate")], cmap=sns.color_palette("Reds", as_cmap=True)
         )
 
@@ -210,39 +223,42 @@
     labels: list
       a list of labels to be used a row index.
     limit: int
       the confidence limit of the results (default: 1 i.e. 68%).
     """
     params = params if isinstance(params, list) else list(params.keys())
     labels = labels if isinstance(labels, list) else list(labels.keys())
-    d = {}
+    d, cols = {}, {}
     r = re.compile(r"(.*)(=|<|>)(.*)")
     for param in params:
         for sample in samples:
             latex = None
             for par in param.split("|"):
                 if sample.getParamNames().hasParam(par):
                     latex = sample.getInlineLatex(par, limit=limit)
                     if "<" in latex or ">" in latex:
                         latex = sample.getInlineLatex(par, limit=2)
                     break
-            assert latex is not None, f"Parameter '{param}' not found!"
-            found = r.findall(latex)
-            assert (
-                len(found) == 1
-            ), f"Something gets wrong when retrieving limits for '{param}' parameter!"
-            name, sign, value = found[0]
-            name = name.replace(" ", "")
+            if not latex:
+                value = " "
+            else:
+                # assert latex is not None, f"Parameter '{param}' not found!"
+                found = r.findall(latex)
+                assert (
+                    len(found) == 1
+                ), f"Something gets wrong when retrieving limits for '{param}' parameter!"
+                name, sign, value = found[0]
+                name = name.replace(" ", "")
+                if param not in cols:
+                    cols[param] = f"${name}$"
             if "---" in value:
-                value = "$-$"
-            d.setdefault(f"${name}$", []).append(
-                f"${value}$" if sign == "=" else f"${sign}{value}$"
-            )
+                value = "-"
+            d.setdefault(param, []).append(f"${value}$" if sign == "=" else f"${sign}{value}$")
     df = pd.DataFrame(d, index=labels[: len(samples)])
-    return df
+    return df.rename(columns=cols)
 
 
 def plot_chains(
     mcmc_samples,
     params,
     ncol=None,
     highlight_burnin=0.4,
@@ -252,39 +268,39 @@
     no_cache=False,
     markers=None,
     markers_args=None,
     prefix="mcmc",
 ):
     """Plot MCMC sample evolution
 
-    Parameters
-    ----------
-    mcmc_samples: dict
-      a dict holding a name as key for the sample and a corresponding directory as value.
-    params: dict or list
-      a dict holding the parameter names for the different mcmc_samples or
-      a unique list of parameter names
-    ncol: int
-      the number of columns within the plot
-    highlight_burnin: float
-      the fraction of samples to highlight (below the burnin value, the color is faded)
-    ignore_rows: float
-      the fraction of samples to ignore
-    show_mean_std: bool
-      show the mean/std values over the different samples
-    show_only_mcmc: int or list
-      only show chains given their number
-    no_cache: bool
-      remove the getdist cache
-    markers: dict
-      dictionnary holding the "expected" value for a parameter
-    markers_args: dict
-      marker kwargs to pass to plt.axhline
-    prefix: str
-      prefix name of chains
+        Parameters
+        ----------
+        mcmc_samples: dict
+          a dict holding a name as key for the sample and a corresponding directory as value.
+        params: dict or list
+          a dict holding the parameter names for the different mcmc_samples or
+          a unique list of parameter names
+        ncol: int
+          the number of columns within the plot
+        highlight_burnin: float
+          the fraction of samples to highlight (below the burnin value, the color is faded)
+        ignore_rows: float
+          the fraction of samples to ignore
+        show_mean_std: bool
+          show the mean/std values over the different samples
+        show_only_mcmc: int or list
+          only show chains given their number
+        no_cache: bool
+          remove the getdist cache
+        markers: dict
+    :      dictionnary holding the "expected" value for a parameter
+        markers_args: dict
+          marker kwargs to pass to plt.axhline
+        prefix: str
+          prefix name of chains
     """
     create_symlink(mcmc_samples, prefix)
     from getdist import loadMCSamples
     from matplotlib.lines import Line2D
 
     if not isinstance(params, (list, dict)):
         raise ValueError("Parameter list must be either a list or a dict!")
@@ -335,16 +351,16 @@
                 # Keep only relevant parameters
                 selected_params = [par for par in params if par in lookup]
                 if ncol is None:
                     ncol, nrow = len(selected_params), 1
                 else:
                     nrow = len(selected_params) // ncol
                     nrow += 1 if len(selected_params) > nrow * ncol else 0
-                fig = plt.figure(figsize=(15, 2 * nrow))
-                axes = [plt.subplot(nrow, ncol, i + 1) for i in range(len(selected_params))]
+                fig, axes = plt.subplots(nrow, ncol, sharex=True, figsize=(15, 2 * nrow))
+                axes = axes.flatten()
 
             color = f"C{imcmc}"
             if samples.shape[0] < min_chain_size:
                 min_chain_size = samples.shape[0]
             for i, p in enumerate(selected_params):
                 axes[i].set_ylabel(r"${}$".format(lookup[p].get("label")))
                 y = samples[:, lookup[p].get("pos")]
@@ -361,14 +377,16 @@
             for i, p in enumerate(selected_params):
                 data = np.array([chain[:min_chain_size] for chain in chains[p]])
                 mu, std = np.mean(data), np.std(data)
                 axes[i].axhline(mu, color="0.6", lw=1)
                 for sign in [-1, +1]:
                     axes[i].axhline(mu + std * sign, color="0.6", ls="--", lw=1)
 
+        # Remove axes with no data inside
+        _ = [fig.delaxes(ax) for ax in axes if not len(ax.get_lines())]
         leg = fig.legend(
             [Line2D([0], [0], color=f"C{f.split('.')[-2]}") for f in files],
             [f"mcmc #{f.split('.')[-2]}" for f in files],
             bbox_to_anchor=(1.0, 0.5 if nrow > 1 else 1.0),
             labelcolor="linecolor",
             loc="center left",
             title=name,
@@ -394,20 +412,21 @@
     ncols = 2
     fig, axes = plt.subplots(nrows, ncols, figsize=(15, 3 * nrows), sharex=sharex)
     axes = np.atleast_2d(axes)
 
     regex = re.compile(r".*mcmc\.([0-9]+).progress")
     for i, (k, v) in enumerate(mcmc_samples.items()):
         files = _get_chain_filenames(v, suffix=".progress")
-        for f in files:
-            cols = [a.strip() for a in open(f).readline().lstrip("#").split()]
+        for fn in files:
+            with open(fn) as f:
+                cols = [a.strip() for a in f.readline().lstrip("#").split()]
             df = pd.read_csv(
-                f, names=cols, comment="#", sep=" ", skipinitialspace=True, index_col=False
+                fn, names=cols, comment="#", sep=" ", skipinitialspace=True, index_col=False
             )
-            idx = 1 if not (m := regex.match(f)) else m.group(1)
+            idx = 1 if not (m := regex.match(fn)) else m.group(1)
             kwargs = dict(label=f"mcmc" + (f" #{idx}" if idx else ""), color=f"C{idx}", alpha=0.75)
             axes[i, 0].semilogy(df.N, df.Rminus1, "-o", **kwargs)
             axes[i, 0].set_ylabel(r"$R-1$")
 
             axes[i, 1].plot(df.N, df.acceptance_rate, "-o", **kwargs)
             axes[i, 1].set_ylabel(r"acceptance rate")
         if len(files) > 1:
```

### Comparing `cobaya_utilities-0.1.2/cobaya_utilities.egg-info/PKG-INFO` & `cobaya_utilities-0.1.3/cobaya_utilities.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cobaya-utilities
-Version: 0.1.2
+Version: 0.1.3
 Summary: A set of functions to deal with MCMC output from cobaya
 Home-page: https://github.com/xgarrido/cobaya_utilities.git
 Author: Xavier Garrido
 Author-email: xavier.garrido@lal.in2p3.fr
 Keywords: cobaya,MCMC,plot
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Education
@@ -22,16 +22,17 @@
 
 A set of tools to deal with MCMC chains and a complement to `cobaya
 <https://github.com/CobayaSampler/cobaya>`_ and `getdist <https://github.com/cmbant/getdist>`_.
 
 .. image:: https://img.shields.io/pypi/v/cobaya-utilities.svg?style=flat
    :target: https://pypi.python.org/pypi/cobaya-utilities
 
-.. image:: https://img.shields.io/github/workflow/status/xgarrido/cobaya_utilities/Unit%20test
+.. image:: https://img.shields.io/github/actions/workflow/status/xgarrido/cobaya_utilities/testing.yml?branch=master
    :target: https://github.com/xgarrido/cobaya_utilities/actions
+   :alt: GitHub Workflow Status
 
 .. image:: https://readthedocs.org/projects/cobaya-utilities/badge/?version=latest
    :target: https://cobaya-utilities.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation Status
 
 .. image:: https://mybinder.org/badge_logo.svg
    :target: https://mybinder.org/v2/gh/xgarrido/cobaya_utilities/master
```

### Comparing `cobaya_utilities-0.1.2/pyproject.toml` & `cobaya_utilities-0.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cobaya_utilities-0.1.2/setup.py` & `cobaya_utilities-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `cobaya_utilities-0.1.2/versioneer.py` & `cobaya_utilities-0.1.3/versioneer.py`

 * *Files identical despite different names*

