# Comparing `tmp/energy_tools-1.1.1.tar.gz` & `tmp/energy_tools-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "energy_tools-1.1.1.tar", last modified: Wed Feb  8 19:34:52 2023, max compression
+gzip compressed data, was "energy_tools-1.1.2.tar", last modified: Tue Jul 11 01:51:21 2023, max compression
```

## Comparing `energy_tools-1.1.1.tar` & `energy_tools-1.1.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-02-08 19:34:52.345016 energy_tools-1.1.1/
--rw-rw-rw-   0        0        0     1091 2021-07-06 13:36:54.000000 energy_tools-1.1.1/LICENSE
--rw-rw-rw-   0        0        0     6985 2023-02-08 19:34:52.343891 energy_tools-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     6299 2023-02-08 19:33:21.000000 energy_tools-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-02-08 19:34:52.327891 energy_tools-1.1.1/energy_tools/
--rw-rw-rw-   0        0        0        2 2021-07-06 13:36:54.000000 energy_tools-1.1.1/energy_tools/__init__.py
--rw-rw-rw-   0        0        0     5901 2021-07-06 13:36:54.000000 energy_tools-1.1.1/energy_tools/complex.py
--rw-rw-rw-   0        0        0     1357 2021-07-06 13:39:19.000000 energy_tools-1.1.1/energy_tools/energy_factors.py
--rw-rw-rw-   0        0        0     1459 2021-07-06 13:36:54.000000 energy_tools-1.1.1/energy_tools/misc.py
--rw-rw-rw-   0        0        0     1386 2021-07-06 13:36:54.000000 energy_tools-1.1.1/energy_tools/per_unit.py
--rw-rw-rw-   0        0        0     8460 2021-07-06 13:36:54.000000 energy_tools-1.1.1/energy_tools/phasor.py
--rw-rw-rw-   0        0        0     1289 2023-02-08 19:15:11.000000 energy_tools-1.1.1/energy_tools/power.py
-drwxrwxrwx   0        0        0        0 2023-02-08 19:34:52.341891 energy_tools-1.1.1/energy_tools.egg-info/
--rw-rw-rw-   0        0        0     6985 2023-02-08 19:34:52.000000 energy_tools-1.1.1/energy_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-02-08 19:34:52.000000 energy_tools-1.1.1/energy_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-08 19:34:52.000000 energy_tools-1.1.1/energy_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-02-08 19:34:52.000000 energy_tools-1.1.1/energy_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-02-08 19:34:52.000000 energy_tools-1.1.1/energy_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-08 19:34:52.345894 energy_tools-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3891 2023-02-08 19:29:31.000000 energy_tools-1.1.1/setup.py
+drwxrwxr-x   0 michel    (1000) michel    (1000)        0 2023-07-11 01:51:21.121758 energy_tools-1.1.2/
+-rw-rw-r--   0 michel    (1000) michel    (1000)     8341 2023-07-11 01:51:21.121758 energy_tools-1.1.2/PKG-INFO
+-rw-rw-r--   0 michel    (1000) michel    (1000)     6105 2023-07-11 01:13:41.000000 energy_tools-1.1.2/README.md
+drwxrwxr-x   0 michel    (1000) michel    (1000)        0 2023-07-11 01:51:21.109757 energy_tools-1.1.2/energy_tools/
+-rw-rw-r--   0 michel    (1000) michel    (1000)        1 2022-12-23 00:41:15.000000 energy_tools-1.1.2/energy_tools/__init__.py
+-rw-rw-r--   0 michel    (1000) michel    (1000)     5687 2022-12-23 00:41:15.000000 energy_tools-1.1.2/energy_tools/complex.py
+-rw-rw-r--   0 michel    (1000) michel    (1000)     1312 2022-12-23 00:41:15.000000 energy_tools-1.1.2/energy_tools/energy_factors.py
+-rw-rw-r--   0 michel    (1000) michel    (1000)     1401 2022-12-23 00:41:15.000000 energy_tools-1.1.2/energy_tools/misc.py
+-rw-rw-r--   0 michel    (1000) michel    (1000)     1335 2022-12-23 00:41:15.000000 energy_tools-1.1.2/energy_tools/per_unit.py
+-rw-rw-r--   0 michel    (1000) michel    (1000)     7222 2023-07-11 01:47:43.000000 energy_tools-1.1.2/energy_tools/phasor.py
+-rw-rw-r--   0 michel    (1000) michel    (1000)     1246 2023-07-11 01:13:41.000000 energy_tools-1.1.2/energy_tools/power.py
+drwxrwxr-x   0 michel    (1000) michel    (1000)        0 2023-07-11 01:51:21.117757 energy_tools-1.1.2/energy_tools.egg-info/
+-rw-rw-r--   0 michel    (1000) michel    (1000)     8341 2023-07-11 01:51:20.000000 energy_tools-1.1.2/energy_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 michel    (1000) michel    (1000)      368 2023-07-11 01:51:21.000000 energy_tools-1.1.2/energy_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 michel    (1000) michel    (1000)        1 2023-07-11 01:51:20.000000 energy_tools-1.1.2/energy_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 michel    (1000) michel    (1000)        6 2023-07-11 01:51:20.000000 energy_tools-1.1.2/energy_tools.egg-info/requires.txt
+-rw-rw-r--   0 michel    (1000) michel    (1000)       13 2023-07-11 01:51:20.000000 energy_tools-1.1.2/energy_tools.egg-info/top_level.txt
+-rw-rw-r--   0 michel    (1000) michel    (1000)       38 2023-07-11 01:51:21.121758 energy_tools-1.1.2/setup.cfg
+-rw-rw-r--   0 michel    (1000) michel    (1000)     3765 2023-07-11 01:49:58.000000 energy_tools-1.1.2/setup.py
```

### Comparing `energy_tools-1.1.1/PKG-INFO` & `energy_tools-1.1.2/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,213 +1,194 @@
-Metadata-Version: 2.1
-Name: energy_tools
-Version: 1.1.1
-Summary: Modest collection of electrical energy calculation tools.
-Home-page: https://gitlab.com/miek770/energy_tools
-Author: Michel Lavoie
-Author-email: lavoie.michel@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# energy_tools
-
-Modest collection of electrical energy calculation tools.
-
-**Content:**
-
-- [Installation](#installation)
-    - [Requirements](#requirements)
-    - [Installing energy_tools](#installing-energy_tools)
-        - [With pip](#with-pip)
-        - [Without pip](#without-pip)
-        - [Development version](#development-version)
-    - [Test your installation](#test-your-installation)
-- [Features](#features)
-    - [complex](#complex)
-    - [energy_factors](#energy_factors)
-    - [misc](#misc)
-    - [per_unit](#per_unit)
-    - [phasor](#phasor)
-    - [power](#power)
-- [Usage](#usage)
-- [Contributing](#contributing)
-
-## Installation
-
-### Requirements
-
-Basic requirements:
-
-- [Python 3.8+](http://www.python.org/download/releases/);
-- numpy.
-
-Development additional requirements:
-
-- black;
-- pre-commit;
-- pytest;
-- twine.
-
-### Installing energy_tools
-
-#### With pip
-
-1. Open a command prompt (e.g. Start > cmd on windows systems);
-2. Install energy_tools by running:
-
-```
-pip install -U --user energy_tools
-```
-
-#### Without pip
-
-If you don’t have internet access on your system or don’t want to use pip for some other reason, energy_tools can also be installed without using pip:
-
-1. Download and unzip the current energy_tools distribution from PyPi under “Download files”.
-2. Open a command prompt (e.g. Start > cmd on Windows) and navigate to the folder that contains the setup.py file with the command cd <folder> :
-
-```
-cd %path_to_energy_tools%\energy_tools-x.x.x\
-```
-
-Install energy_tools by running :
-
-```
-python setup.py install
-```
-
-#### Development version
-
-To install the latest development version of energy_tools from GitLab, simply follow these steps:
-
-1. Download and install git.
-2. Open a git shell and navigate to the directory where you want to keep your energy_tools files.
-3. Run the following commands:
-
-```
-python -m venv energy_tools
-cd energy_tools
-git clone https://gitlab.com/miek770/energy_tools.git
-source Scripts/activate
-pip install -U pip
-pip install -U wheel
-pip install -r energy_tools/requirements-dev.txt
-```
-
-4. Navigate inside the repository and check out the develop branch:
-
-```
-cd energy_tools
-git checkout develop
-```
-
-5. Install [Black](https://github.com/ambv/black#version-control-integration) using pre-commit:
-
-```
-pre-commit install
-```
-
-### Test your installation
-
-To test your installed development version, run pytest from the energy_tools' base directory:
-
-```
-pytest
-```
-
-## Features
-
-`energy_tools` currently includes the following modules:
-
-### complex
-
-The `complex` module includes an improved `EleComplex` class which adds the following attributes (properties): `phase`, `module`.
-
-- `EleComplex.phase` returns the complex number's phase in degrees.
-- `EleComplex.module` returns the complex number's amplitude.
-
-The `complex` module also includes a `complex_impedance` function that returns an improved `EleComplex` number, based on a provided real impedance *z* and an *X/R* ratio.
-
-The `EleComplex` class must be imported in order for some of the other tools to be usable:
-
-``` python
-from energy_tools.complex import EleComplex
-```
-
-See [Usage](#usage) below for more details.
-
-### energy_factors
-
-The `energy_factors` module includes functions to calculate yearly energy factors for special calculations. Currently, it includes the `utilisation_factor` and `loss_factor` functions.
-
-### misc
-
-The `misc` module includes basic functions to manipulate impedances, including `serie`, `parallel`, `zCap` and `zInd`. These calculate series impedance, parallel impedances, capacitance impedance and inductance impedance respectively.
-
-### per_unit
-
-The `per_unit` module includes functions that return the base current, impedance and power.
-
-### phasor
-
-The `phasor` module includes a new data type `Phasor` for the electrical phasor used in power systems.
-
-A phasor is defined by an amplitude and a phase. The instance can be created either using those, or by providing a complex amplitude (in this case the phase is ignored). Several operations are supported, including: addition, substraction, multiplication, division, power, inversion and equality with either another phasor, a float or an integer.
-
-It also provides a nice representation in this form: 120.000 @ 0.000°
-
-Attributes:
-
-- amp: The unitless phasor amplitude.
-- pha: The phasor's phase in degrees.
-- real: The phasor's real part (interpreted as a complex number).
-- imag: The phasor's imaginary part (interpreted as a complex number).
-
-The `phasor` module also includes functions `sequences` and `phasors`. The former retuns phase A's sequence voltages from phase A, B and C's voltages. The latter does the opposite, i.e. it returns phase A, B and C's voltages from phases A's sequence voltages.
-
-### power
-
-The `power` module includes 2 functions `p()` and `q()` which calculate the active power and reactive power based on at least 2 of the following arguments:
-
-- `p`: Active power (for `q()`).
-- `q`: Reactive power (for `p()`).
-- `s`: Apparent power.
-- `pf`: Power factor.
-
-The arguments and return value are unitless.
-
-## Usage
-
-Sample usage may be found in the [tests](https://gitlab.com/miek770/energy_tools/tree/master/energy_tools/tests) directory. Most of these tools are straightforward (or aim to be), so the tests and docstrings should be helpful enough.
-
-As mentioned [above](#complex), the `EleComplex` class must be imported in order for many of the other tools to be usable:
-
-``` python
-from energy_tools.complex import EleComplex
-```
-
-When the improved `EleComplex` type is imported this way, the following call will result in variable `a` being an `energy_tools.complex.EleComplex` instance, as expected:
-
-```
-a = EleComplex(1, 1)
-a.phase #  Will return 45 degrees
-```
-
-Implicitly declaring a complex number, however, will return the built-in `complex` type:
-
-```
-a = 1 + 1j
-a.phase #  Will raise AttributeError
-```
-
-## Contributing
-
-If you wish to contribute, please follow the development version instructions above and refer to the project's [contribution guide](https://gitlab.com/miek770/energy_tools/blob/master/CONTRIBUTING.md).
+# energy_tools
+
+Modest collection of electrical energy calculation tools.
+
+**Content:**
+
+- [Installation](#installation)
+    - [Requirements](#requirements)
+    - [Installing energy_tools](#installing-energy_tools)
+        - [With pip](#with-pip)
+        - [Without pip](#without-pip)
+        - [Development version](#development-version)
+    - [Test your installation](#test-your-installation)
+- [Features](#features)
+    - [complex](#complex)
+    - [energy_factors](#energy_factors)
+    - [misc](#misc)
+    - [per_unit](#per_unit)
+    - [phasor](#phasor)
+    - [power](#power)
+- [Usage](#usage)
+- [Contributing](#contributing)
+
+## Installation
+
+### Requirements
+
+Basic requirements:
+
+- [Python 3.8+](http://www.python.org/download/releases/);
+- numpy.
+
+Development additional requirements:
+
+- black;
+- pre-commit;
+- pytest;
+- twine.
+
+### Installing energy_tools
+
+#### With pip
+
+1. Open a command prompt (e.g. Start > cmd on windows systems);
+2. Install energy_tools by running:
+
+```
+pip install -U --user energy_tools
+```
+
+#### Without pip
+
+If you don’t have internet access on your system or don’t want to use pip for some other reason, energy_tools can also be installed without using pip:
+
+1. Download and unzip the current energy_tools distribution from PyPi under “Download files”.
+2. Open a command prompt (e.g. Start > cmd on Windows) and navigate to the folder that contains the setup.py file with the command cd <folder> :
+
+```
+cd %path_to_energy_tools%\energy_tools-x.x.x\
+```
+
+Install energy_tools by running :
+
+```
+python setup.py install
+```
+
+#### Development version
+
+To install the latest development version of energy_tools from GitLab, simply follow these steps:
+
+1. Download and install git.
+2. Open a git shell and navigate to the directory where you want to keep your energy_tools files.
+3. Run the following commands:
+
+```
+python -m venv energy_tools
+cd energy_tools
+git clone https://gitlab.com/miek770/energy_tools.git
+source Scripts/activate
+pip install -U pip
+pip install -U wheel
+pip install -r energy_tools/requirements-dev.txt
+```
+
+4. Navigate inside the repository and check out the develop branch:
+
+```
+cd energy_tools
+git checkout develop
+```
+
+5. Install [Black](https://github.com/ambv/black#version-control-integration) using pre-commit:
+
+```
+pre-commit install
+```
+
+### Test your installation
+
+To test your installed development version, run pytest from the energy_tools' base directory:
+
+```
+pytest
+```
+
+## Features
+
+`energy_tools` currently includes the following modules:
+
+### complex
+
+The `complex` module includes an improved `EleComplex` class which adds the following attributes (properties): `phase`, `module`.
+
+- `EleComplex.phase` returns the complex number's phase in degrees.
+- `EleComplex.module` returns the complex number's amplitude.
+
+The `complex` module also includes a `complex_impedance` function that returns an improved `EleComplex` number, based on a provided real impedance *z* and an *X/R* ratio.
+
+The `EleComplex` class must be imported in order for some of the other tools to be usable:
+
+``` python
+from energy_tools.complex import EleComplex
+```
+
+See [Usage](#usage) below for more details.
+
+### energy_factors
+
+The `energy_factors` module includes functions to calculate yearly energy factors for special calculations. Currently, it includes the `utilisation_factor` and `loss_factor` functions.
+
+### misc
+
+The `misc` module includes basic functions to manipulate impedances, including `serie`, `parallel`, `zCap` and `zInd`. These calculate series impedance, parallel impedances, capacitance impedance and inductance impedance respectively.
+
+### per_unit
+
+The `per_unit` module includes functions that return the base current, impedance and power.
+
+### phasor
+
+The `phasor` module includes a new data type `Phasor` for the electrical phasor used in power systems.
+
+A phasor is defined by an amplitude and a phase. The instance can be created either using those, or by providing a complex amplitude (in this case the phase is ignored). Several operations are supported, including: addition, substraction, multiplication, division, power, inversion and equality with either another phasor, a float or an integer.
+
+It also provides a nice representation in this form: 120.000 @ 0.000°
+
+Attributes:
+
+- amp: The unitless phasor amplitude.
+- pha: The phasor's phase in degrees.
+- real: The phasor's real part (interpreted as a complex number).
+- imag: The phasor's imaginary part (interpreted as a complex number).
+
+The `phasor` module also includes functions `sequences` and `phasors`. The former retuns phase A's sequence voltages from phase A, B and C's voltages. The latter does the opposite, i.e. it returns phase A, B and C's voltages from phases A's sequence voltages.
+
+### power
+
+The `power` module includes 2 functions `p()` and `q()` which calculate the active power and reactive power based on at least 2 of the following arguments:
+
+- `p`: Active power (for `q()`).
+- `q`: Reactive power (for `p()`).
+- `s`: Apparent power.
+- `pf`: Power factor.
+
+The arguments and return value are unitless.
+
+## Usage
+
+Sample usage may be found in the [tests](https://gitlab.com/miek770/energy_tools/tree/master/energy_tools/tests) directory. Most of these tools are straightforward (or aim to be), so the tests and docstrings should be helpful enough.
+
+As mentioned [above](#complex), the `EleComplex` class must be imported in order for many of the other tools to be usable:
+
+``` python
+from energy_tools.complex import EleComplex
+```
+
+When the improved `EleComplex` type is imported this way, the following call will result in variable `a` being an `energy_tools.complex.EleComplex` instance, as expected:
+
+```
+a = EleComplex(1, 1)
+a.phase #  Will return 45 degrees
+```
+
+Implicitly declaring a complex number, however, will return the built-in `complex` type:
+
+```
+a = 1 + 1j
+a.phase #  Will raise AttributeError
+```
+
+## Contributing
+
+If you wish to contribute, please follow the development version instructions above and refer to the project's [contribution guide](https://gitlab.com/miek770/energy_tools/blob/master/CONTRIBUTING.md).
```

### Comparing `energy_tools-1.1.1/energy_tools/energy_factors.py` & `energy_tools-1.1.2/energy_tools/energy_factors.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-def utilisation_factor(hours_list, p_list, p):
-    """Returns the utilisation factor based on the active power during a year.
-
-    Args:
-        hours_list: List of duration in hours for each active power in p_list.
-        p_list: List of active power at each hour.
-        p: Nominal active power (single value).
-
-    Returns:
-        Utilisation factor in per unit.
-    """
-    if len(hours_list) != len(p_list):
-        raise ValueError("hours_list and p_mw_list must have the same length.")
-
-    p_pu = []
-    for i in range(len(hours_list)):
-        p_pu.append(p_list[i] / p)
-
-    e_pu = []
-    for i in range(len(hours_list)):
-        e_pu.append(hours_list[i] * p_pu[i])
-
-    return sum(e_pu) / sum(hours_list)
-
-
-def loss_factor(hours_list, p_list, p):
-    """Returns the loss factor based on the active power during a year.
-
-    Args:
-        hours_list: List of duration in hours for each active power in p_list.
-        p_list: List of active power at each hour.
-        p: Nominal active power (single value).
-
-    Returns:
-        Loss factor in per unit.
-    """
-    p_pu = []
-    for i in range(len(hours_list)):
-        p_pu.append(p_list[i] / p)
-
-    e2_pu = []
-    for i in range(len(hours_list)):
-        e2_pu.append(hours_list[i] * pow(p_pu[i], 2))
-
-    return sum(e2_pu) / sum(hours_list)
+def utilisation_factor(hours_list, p_list, p):
+    """Returns the utilisation factor based on the active power during a year.
+
+    Args:
+        hours_list: List of duration in hours for each active power in p_list.
+        p_list: List of active power at each hour.
+        p: Nominal active power (single value).
+
+    Returns:
+        Utilisation factor in per unit.
+    """
+    if len(hours_list) != len(p_list):
+        raise ValueError("hours_list and p_mw_list must have the same length.")
+
+    p_pu = []
+    for i in range(len(hours_list)):
+        p_pu.append(p_list[i] / p)
+
+    e_pu = []
+    for i in range(len(hours_list)):
+        e_pu.append(hours_list[i] * p_pu[i])
+
+    return sum(e_pu) / sum(hours_list)
+
+
+def loss_factor(hours_list, p_list, p):
+    """Returns the loss factor based on the active power during a year.
+
+    Args:
+        hours_list: List of duration in hours for each active power in p_list.
+        p_list: List of active power at each hour.
+        p: Nominal active power (single value).
+
+    Returns:
+        Loss factor in per unit.
+    """
+    p_pu = []
+    for i in range(len(hours_list)):
+        p_pu.append(p_list[i] / p)
+
+    e2_pu = []
+    for i in range(len(hours_list)):
+        e2_pu.append(hours_list[i] * pow(p_pu[i], 2))
+
+    return sum(e2_pu) / sum(hours_list)
```

### Comparing `energy_tools-1.1.1/energy_tools/misc.py` & `energy_tools-1.1.2/energy_tools/misc.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,58 @@
-# Standard library
-from math import pi
-from collections.abc import Iterable
-
-# Current module
-from energy_tools.complex import EleComplex
-
-
-def serie(*args):
-    """Puts impedances in serie (yep, simple summation).
-
-    Args:
-        z: List of impedances (either complex or real or a combination of both).
-
-    Returns:
-        Serie impedance.
-    """
-
-    # Check if an iterable was supplied instead of multiple arguments
-    if len(args) == 1 and isinstance(args[0], Iterable):
-        args = args[0]
-
-    return sum(args)
-
-
-def parallel(*args):
-    """Puts impedances in parallel.
-
-    Args:
-        z: List of impedances (either complex or real or a combination of both).
-
-    Returns:
-        Parallel impedance.
-    """
-
-    # Check if an iterable was supplied instead of multiple arguments
-    if len(args) == 1 and isinstance(args[0], Iterable):
-        args = args[0]
-
-    try:
-        return 1 / sum([1.0 / y for y in args])
-
-    except ZeroDivisionError:
-        return 0.0
-
-
-def zCap(C, f=60):
-    """Retourne l'impédance complexe d'un banc de condensateurs en fonction de
-    la capacitance et de la fréquence (à 60Hz par défaut).
-    """
-    return EleComplex(1 / (2j * pi * f * C))
-
-
-def zInd(L, f=60):
-    """Retourne l'impédance complexe d'une inductance en fonction de
-    l'inductance et de la fréquence (à 60Hz par défaut).
-    """
-    return EleComplex(2j * pi * f * L)
+# Standard library
+from math import pi
+from collections.abc import Iterable
+
+# Current module
+from energy_tools.complex import EleComplex
+
+
+def serie(*args):
+    """Puts impedances in serie (yep, simple summation).
+
+    Args:
+        z: List of impedances (either complex or real or a combination of both).
+
+    Returns:
+        Serie impedance.
+    """
+
+    # Check if an iterable was supplied instead of multiple arguments
+    if len(args) == 1 and isinstance(args[0], Iterable):
+        args = args[0]
+
+    return sum(args)
+
+
+def parallel(*args):
+    """Puts impedances in parallel.
+
+    Args:
+        z: List of impedances (either complex or real or a combination of both).
+
+    Returns:
+        Parallel impedance.
+    """
+
+    # Check if an iterable was supplied instead of multiple arguments
+    if len(args) == 1 and isinstance(args[0], Iterable):
+        args = args[0]
+
+    try:
+        return 1 / sum([1.0 / y for y in args])
+
+    except ZeroDivisionError:
+        return 0.0
+
+
+def zCap(C, f=60):
+    """Retourne l'impédance complexe d'un banc de condensateurs en fonction de
+    la capacitance et de la fréquence (à 60Hz par défaut).
+    """
+    return EleComplex(1 / (2j * pi * f * C))
+
+
+def zInd(L, f=60):
+    """Retourne l'impédance complexe d'une inductance en fonction de
+    l'inductance et de la fréquence (à 60Hz par défaut).
+    """
+    return EleComplex(2j * pi * f * L)
```

### Comparing `energy_tools-1.1.1/energy_tools/per_unit.py` & `energy_tools-1.1.2/energy_tools/per_unit.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-def i_base_ka(sb_mva, vbll_kv):
-    """Returns the base current based on the base power and voltage.
-
-    Args:
-        sb_mva: Base power in MVA.
-        vbll_kv: Base voltage in kV.
-
-    Returns:
-        Base current in kA.
-    """
-    sb_mva = float(sb_mva)
-    vbll_kv = float(vbll_kv)
-    return sb_mva / (vbll_kv * 3 ** 0.5)
-
-
-def z_base_ohm(vbll_kv, ib_ka=None, sb_mva=None):
-    """Returns the base impedance based on the base voltage and either the base current
-    or the base power.
-
-    Args:
-        vbll_kv: Base voltage in kV.
-        sb_mva: Base power in MVA.
-        ib_ka: Base current in kA.
-
-    Returns:
-        Base impedance in ohms.
-    """
-    vbll_kv = float(vbll_kv)
-    if ib_ka is None and sb_mva is not None:
-        sb_mva = float(sb_mva)
-        return (vbll_kv ** 2) / sb_mva
-    elif sb_mva is None and ib_ka is not None:
-        ib_ka = float(ib_ka)
-        return vbll_kv / (ib_ka * 3 ** 0.5)
-    else:
-        raise ValueError("You must provide either ib_ka or sb_mva")
-
-
-def s_base_mva(vbll_kv, ib_ka):
-    """Returns the base power based on the base voltage and current.
-
-    Args:
-        vbll_kv: Base voltage in kV.
-        ib_ka: Base current in kA.
-
-    Returns:
-        Base power in MVA.
-    """
-    vbll_kv = float(vbll_kv)
-    ib_ka = float(ib_ka)
-    return ib_ka * vbll_kv * 3 ** 0.5
+def i_base_ka(sb_mva, vbll_kv):
+    """Returns the base current based on the base power and voltage.
+
+    Args:
+        sb_mva: Base power in MVA.
+        vbll_kv: Base voltage in kV.
+
+    Returns:
+        Base current in kA.
+    """
+    sb_mva = float(sb_mva)
+    vbll_kv = float(vbll_kv)
+    return sb_mva / (vbll_kv * 3 ** 0.5)
+
+
+def z_base_ohm(vbll_kv, ib_ka=None, sb_mva=None):
+    """Returns the base impedance based on the base voltage and either the base current
+    or the base power.
+
+    Args:
+        vbll_kv: Base voltage in kV.
+        sb_mva: Base power in MVA.
+        ib_ka: Base current in kA.
+
+    Returns:
+        Base impedance in ohms.
+    """
+    vbll_kv = float(vbll_kv)
+    if ib_ka is None and sb_mva is not None:
+        sb_mva = float(sb_mva)
+        return (vbll_kv ** 2) / sb_mva
+    elif sb_mva is None and ib_ka is not None:
+        ib_ka = float(ib_ka)
+        return vbll_kv / (ib_ka * 3 ** 0.5)
+    else:
+        raise ValueError("You must provide either ib_ka or sb_mva")
+
+
+def s_base_mva(vbll_kv, ib_ka):
+    """Returns the base power based on the base voltage and current.
+
+    Args:
+        vbll_kv: Base voltage in kV.
+        ib_ka: Base current in kA.
+
+    Returns:
+        Base power in MVA.
+    """
+    vbll_kv = float(vbll_kv)
+    ib_ka = float(ib_ka)
+    return ib_ka * vbll_kv * 3 ** 0.5
```

### Comparing `energy_tools-1.1.1/energy_tools/power.py` & `energy_tools-1.1.2/energy_tools/power.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from math import sqrt
-
-
-def q(s=None, p=None, pf=None):
-    """Calculates the reactive power `p` (unitless) from the apparent power `s`,
-    the active power `p`, or the power factor `pf` (2 values required).
-    """
-
-    if pf is not None:
-        if not -1 <= pf <= 1:
-            raise ValueError("PF must be between -1 and 1.")
-
-    if p is not None and pf is not None:
-        return sqrt(p**2 * ((1 / pf**2) - 1))
-
-    if s is not None and pf is not None:
-        return sqrt(s**2 - (s * pf) ** 2)
-
-    if p is not None and s is not None:
-        return sqrt(s**2 - p**2)
-
-    raise ValueError("You must provide at least two arguments.")
-
-
-def p(s=None, q=None, pf=None):
-    """Calculates the active power `p` (unitless) from the apparent power `s`,
-    the reactive power `q`, or the power factor `pf` (2 values required).
-    """
-
-    if pf is not None:
-        if not -1 <= pf <= 1:
-            raise ValueError("PF must be between -1 and 1.")
-
-    if q is not None and pf is not None:
-        return sqrt(q**2 / ((1 / pf**2) - 1))
-
-    if s is not None and pf is not None:
-        return s * pf
-
-    if q is not None and s is not None:
-        return sqrt(s**2 - q**2)
-
-    raise ValueError("You must provide at least two arguments.")
+from math import sqrt
+
+
+def q(s=None, p=None, pf=None):
+    """Calculates the reactive power `p` (unitless) from the apparent power `s`,
+    the active power `p`, or the power factor `pf` (2 values required).
+    """
+
+    if pf is not None:
+        if not -1 <= pf <= 1:
+            raise ValueError("PF must be between -1 and 1.")
+
+    if p is not None and pf is not None:
+        return sqrt(p**2 * ((1 / pf**2) - 1))
+
+    if s is not None and pf is not None:
+        return sqrt(s**2 - (s * pf) ** 2)
+
+    if p is not None and s is not None:
+        return sqrt(s**2 - p**2)
+
+    raise ValueError("You must provide at least two arguments.")
+
+
+def p(s=None, q=None, pf=None):
+    """Calculates the active power `p` (unitless) from the apparent power `s`,
+    the reactive power `q`, or the power factor `pf` (2 values required).
+    """
+
+    if pf is not None:
+        if not -1 <= pf <= 1:
+            raise ValueError("PF must be between -1 and 1.")
+
+    if q is not None and pf is not None:
+        return sqrt(q**2 / ((1 / pf**2) - 1))
+
+    if s is not None and pf is not None:
+        return s * pf
+
+    if q is not None and s is not None:
+        return sqrt(s**2 - q**2)
+
+    raise ValueError("You must provide at least two arguments.")
```

### Comparing `energy_tools-1.1.1/setup.py` & `energy_tools-1.1.2/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,126 +1,126 @@
-#!/usr/bin/env python
-# -*- coding: utf-8 -*-
-
-# Note: To use the 'upload' functionality of this file, you must:
-#   $ pip install twine
-
-import io
-import os
-import sys
-from shutil import rmtree
-
-from setuptools import find_packages, setup, Command
-
-# Package meta-data.
-NAME = "energy_tools"
-DESCRIPTION = "Modest collection of electrical energy calculation tools."
-URL = "https://gitlab.com/miek770/energy_tools"
-EMAIL = "lavoie.michel@gmail.com"
-AUTHOR = "Michel Lavoie"
-REQUIRES_PYTHON = ">=3.8"
-VERSION = "1.1.1"
-
-# What packages are required for this module to be executed?
-REQUIRED = ["numpy"]
-
-# What packages are optional?
-EXTRAS = {
-    # 'fancy feature': ['django'],
-}
-
-# The rest you shouldn't have to touch too much :)
-# ------------------------------------------------
-# Except, perhaps the License and Trove Classifiers!
-# If you do change the License, remember to change the Trove Classifier for that!
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-# Import the README and use it as the long-description.
-# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
-try:
-    with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
-        long_description = "\n" + f.read()
-except FileNotFoundError:
-    long_description = DESCRIPTION
-
-# Load the package's __version__.py module as a dictionary.
-about = {}
-if not VERSION:
-    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
-    with open(os.path.join(here, project_slug, "__version__.py")) as f:
-        exec(f.read(), about)
-else:
-    about["__version__"] = VERSION
-
-
-class UploadCommand(Command):
-    """Support setup.py upload."""
-
-    description = "Build and publish the package."
-    user_options = []
-
-    @staticmethod
-    def status(s):
-        """Prints things in bold."""
-        print("\033[1m{0}\033[0m".format(s))
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        try:
-            self.status("Removing previous builds…")
-            rmtree(os.path.join(here, "dist"))
-        except OSError:
-            pass
-
-        self.status("Building Source and Wheel (universal) distribution…")
-        os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
-
-        self.status("Uploading the package to PyPI via Twine…")
-        os.system("twine upload dist/*")
-
-        self.status("Pushing git tags…")
-        os.system("git tag v{0}".format(about["__version__"]))
-        os.system("git push --tags")
-
-        sys.exit()
-
-
-# Where the magic happens:
-setup(
-    name=NAME,
-    version=about["__version__"],
-    description=DESCRIPTION,
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    author=AUTHOR,
-    author_email=EMAIL,
-    python_requires=REQUIRES_PYTHON,
-    url=URL,
-    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    # If your package is a single module, use this instead of 'packages':
-    # py_modules=['mypackage'],
-    # entry_points={
-    #     'console_scripts': ['mycli=mymodule:cli'],
-    # },
-    install_requires=REQUIRED,
-    extras_require=EXTRAS,
-    include_package_data=True,
-    license="MIT",
-    classifiers=[
-        # Trove classifiers
-        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: Implementation :: CPython",
-        "Programming Language :: Python :: Implementation :: PyPy",
-    ],
-    # $ setup.py publish support.
-    cmdclass={"upload": UploadCommand},
-)
+#!/usr/bin/env python
+# -*- coding: utf-8 -*-
+
+# Note: To use the 'upload' functionality of this file, you must:
+#   $ pip install twine
+
+import io
+import os
+import sys
+from shutil import rmtree
+
+from setuptools import find_packages, setup, Command
+
+# Package meta-data.
+NAME = "energy_tools"
+DESCRIPTION = "Modest collection of electrical energy calculation tools."
+URL = "https://gitlab.com/miek770/energy_tools"
+EMAIL = "lavoie.michel@gmail.com"
+AUTHOR = "Michel Lavoie"
+REQUIRES_PYTHON = ">=3.8"
+VERSION = "1.1.2"
+
+# What packages are required for this module to be executed?
+REQUIRED = ["numpy"]
+
+# What packages are optional?
+EXTRAS = {
+    # 'fancy feature': ['django'],
+}
+
+# The rest you shouldn't have to touch too much :)
+# ------------------------------------------------
+# Except, perhaps the License and Trove Classifiers!
+# If you do change the License, remember to change the Trove Classifier for that!
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+# Import the README and use it as the long-description.
+# Note: this will only work if 'README.md' is present in your MANIFEST.in file!
+try:
+    with io.open(os.path.join(here, "README.md"), encoding="utf-8") as f:
+        long_description = "\n" + f.read()
+except FileNotFoundError:
+    long_description = DESCRIPTION
+
+# Load the package's __version__.py module as a dictionary.
+about = {}
+if not VERSION:
+    project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
+    with open(os.path.join(here, project_slug, "__version__.py")) as f:
+        exec(f.read(), about)
+else:
+    about["__version__"] = VERSION
+
+
+class UploadCommand(Command):
+    """Support setup.py upload."""
+
+    description = "Build and publish the package."
+    user_options = []
+
+    @staticmethod
+    def status(s):
+        """Prints things in bold."""
+        print("\033[1m{0}\033[0m".format(s))
+
+    def initialize_options(self):
+        pass
+
+    def finalize_options(self):
+        pass
+
+    def run(self):
+        try:
+            self.status("Removing previous builds…")
+            rmtree(os.path.join(here, "dist"))
+        except OSError:
+            pass
+
+        self.status("Building Source and Wheel (universal) distribution…")
+        os.system("{0} setup.py sdist bdist_wheel --universal".format(sys.executable))
+
+        self.status("Uploading the package to PyPI via Twine…")
+        os.system("twine upload dist/*")
+
+        self.status("Pushing git tags…")
+        os.system("git tag v{0}".format(about["__version__"]))
+        os.system("git push --tags")
+
+        sys.exit()
+
+
+# Where the magic happens:
+setup(
+    name=NAME,
+    version=about["__version__"],
+    description=DESCRIPTION,
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    author=AUTHOR,
+    author_email=EMAIL,
+    python_requires=REQUIRES_PYTHON,
+    url=URL,
+    packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
+    # If your package is a single module, use this instead of 'packages':
+    # py_modules=['mypackage'],
+    # entry_points={
+    #     'console_scripts': ['mycli=mymodule:cli'],
+    # },
+    install_requires=REQUIRED,
+    extras_require=EXTRAS,
+    include_package_data=True,
+    license="MIT",
+    classifiers=[
+        # Trove classifiers
+        # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
+        "License :: OSI Approved :: MIT License",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: Implementation :: CPython",
+        "Programming Language :: Python :: Implementation :: PyPy",
+    ],
+    # $ setup.py publish support.
+    cmdclass={"upload": UploadCommand},
+)
```

