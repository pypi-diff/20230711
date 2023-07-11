# Comparing `tmp/nir-0.0.5.tar.gz` & `tmp/nir-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nir-0.0.5.tar", last modified: Sat Jul  8 23:58:59 2023, max compression
+gzip compressed data, was "nir-0.0.6.tar", last modified: Tue Jul 11 02:14:02 2023, max compression
```

## Comparing `nir-0.0.5.tar` & `nir-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:58:59.248926 nir-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-08 23:58:59.248926 nir-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-08 23:58:51.000000 nir-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:58:59.248926 nir-0.0.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:58:59.248926 nir-0.0.5/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-07-08 23:58:51.000000 nir-0.0.5/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:58:59.248926 nir-0.0.5/nir/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-08 23:58:51.000000 nir-0.0.5/nir/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-07-08 23:58:51.000000 nir-0.0.5/nir/ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-08 23:58:51.000000 nir-0.0.5/nir/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-07-08 23:58:51.000000 nir-0.0.5/nir/write.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:58:59.248926 nir-0.0.5/nir.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-07-08 23:58:59.000000 nir-0.0.5/nir.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-08 23:58:59.000000 nir-0.0.5/nir.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 23:58:59.000000 nir-0.0.5/nir.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 23:58:59.000000 nir-0.0.5/nir.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-08 23:58:59.000000 nir-0.0.5/nir.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-08 23:58:51.000000 nir-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 23:58:59.248926 nir-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 23:58:59.248926 nir-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 23:58:51.000000 nir-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-08 23:58:51.000000 nir-0.0.5/tests/test_ir.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-08 23:58:51.000000 nir-0.0.5/tests/test_readwrite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:14:02.646000 nir-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-11 02:14:02.646000 nir-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-07-11 02:13:53.000000 nir-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:14:02.642000 nir-0.0.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:14:02.642000 nir-0.0.6/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-11 02:13:53.000000 nir-0.0.6/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:14:02.642000 nir-0.0.6/nir/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-11 02:13:53.000000 nir-0.0.6/nir/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5395 2023-07-11 02:13:53.000000 nir-0.0.6/nir/ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-11 02:13:53.000000 nir-0.0.6/nir/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-07-11 02:13:53.000000 nir-0.0.6/nir/write.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:14:02.646000 nir-0.0.6/nir.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4729 2023-07-11 02:14:02.000000 nir-0.0.6/nir.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-11 02:14:02.000000 nir-0.0.6/nir.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 02:14:02.000000 nir-0.0.6/nir.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-11 02:14:02.000000 nir-0.0.6/nir.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-11 02:14:02.000000 nir-0.0.6/nir.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-11 02:13:53.000000 nir-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 02:14:02.646000 nir-0.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 02:14:02.646000 nir-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 02:13:53.000000 nir-0.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-07-11 02:13:53.000000 nir-0.0.6/tests/test_ir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-07-11 02:13:53.000000 nir-0.0.6/tests/test_readwrite.py
```

### Comparing `nir-0.0.5/PKG-INFO` & `nir-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nir
-Version: 0.0.5
+Version: 0.0.6
 Summary: Neuromorphic Intermediate Representation
 Author-email: Steven Abreu <s.abreu@rug.nl>, Felix Bauer <felix.bauer@synsense.ai>, Jason Eshraghian <jeshragh@ucsc.edu>, Matthias Jobst <matthias.jobst2@tu-dresden.de>, Gregor Lenz <mail@lenzgregor.com>, Jens Egholm Pedersen <jens@jepedersen.dk>, Sadique Sheik <sadique.sheik@synsense.ai>
 Project-URL: homepage, https://github.com/neuromorphs/nir
 Keywords: neuromorphic,intermediate,representation
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -20,30 +20,32 @@
 # NIR: Neuromorphic Intermediate Representation specification
 
 NIR defines neuron models and connectivity for arbitrary networks that include spiking neurons. Neuron models are defined as dynamical system equations, because time is an essential component of neuromorphic systems. The goal is to provide a common format that different spiking neural network (SNN) frameworks can convert to. That allows a user to train an SNN in framework X and convert it to framework Y. Framework X might offer particularly fast training while framework Y might offer deployment to neuromorphic hardware.
 
 ## Computational units
 On top of popular primitives such as convolutional or fully connected/linear computations, we define additional compuational primitives that are specific to neuromorphic computing and hardware implementations thereof. Computational units that are not specifically neuromorphic take inspiration from the Pytorch ecosystem in terms of naming and parameters (such as Conv2d that uses groups/strides). Example definitons of computational units:
 
-$$\text{I}: [ R ]$$
+$$\text{Affine}: \mathbb{R}^{m \times n},  \mathbb{R}^n$$
 
-$$\text{LI}: [ \tau, R, v_{leak}]$$
+$$\text{Conv1d}: \mathbb{R}^{c_{out} \times c_{in} \times x},  \text{Strides}, \text{Groups}, ... $$ 
 
-$$\text{LIF}: [ \tau, R, v_{leak}, v_{threshold} ]$$
+$$\text{Conv2d}: \mathbb{R}^{c_{out} \times c_{in} \times y \times x},  \text{Strides}, \text{Groups}, ... $$ 
 
-$$\text{Linear}: \mathbb{R}^{m \times n},  \mathbb{R}^n$$
+$$\text{I}: [ R ]$$
 
-$$\text{Conv1d}: \mathbb{R}^{c_{out} \times c_{in} \times x},  \text{Strides}, \text{Groups}, ... $$ 
+$$\text{LI}: [ \tau, R, v_{leak}]$$
 
-$$\text{Conv2d}: \mathbb{R}^{c_{out} \times c_{in} \times y \times x},  \text{Strides}, \text{Groups}, ... $$ 
+$$\text{LIF}: [ \tau, R, v_{leak}, v_{threshold} ]$$
 
 where LIF is defined as a dynamical equation:
 
 $$ \tau \dot{v} = v_{leak} - v + R i $$ 
 
+$$\text{Linear}: \mathbb{R}^{m \times n}$$
+
 
 ## Connectivity 
 Each computational unit is a node in a static graph. Given 3 nodes $A$ which is a LIF node, $B$ which is a Linear node and $C$ which is another LIF node, we can define edges in the graph such as:
 
 $$
 A \rightarrow B \\
 B \rightarrow C
@@ -56,15 +58,15 @@
 
 | **Framework** | **Write to NIR** | **Read from NIR** |
 | --------------- | :--: | :--: |
 | [Lava-DL](https://github.com/lava-nc/lava-dl) | ⬚ | ⬚ |
 | [Nengo](https://nengo.ai) | ⬚ | ⬚ |
 | [Norse](https://github.com/norse/norse) | ✓ | ⬚ |
 | [Rockpool](https://rockpool.ai) | ⬚ | ⬚ |
-| [Sinabs](https://sinabs.readthedocs.io) | ⬚ | ⬚ |
+| [Sinabs](https://sinabs.readthedocs.io) | ✓ | ✓ |
 | [SpiNNaker2](https://spinncloud.com/portfolio/spinnaker2/) | ⬚ | ⬚ |
 | [SynSense Speck](https://www.synsense.ai/products/speck-2/) | ⬚ | ⬚ |
 | [SynSense Xylo](https://www.synsense.ai/products/xylo/) | ⬚ | ⬚ |
 
 
 ## Acknowledgements
 Authors (in alphabetical order):
```

### Comparing `nir-0.0.5/README.md` & `nir-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 # NIR: Neuromorphic Intermediate Representation specification
 
 NIR defines neuron models and connectivity for arbitrary networks that include spiking neurons. Neuron models are defined as dynamical system equations, because time is an essential component of neuromorphic systems. The goal is to provide a common format that different spiking neural network (SNN) frameworks can convert to. That allows a user to train an SNN in framework X and convert it to framework Y. Framework X might offer particularly fast training while framework Y might offer deployment to neuromorphic hardware.
 
 ## Computational units
 On top of popular primitives such as convolutional or fully connected/linear computations, we define additional compuational primitives that are specific to neuromorphic computing and hardware implementations thereof. Computational units that are not specifically neuromorphic take inspiration from the Pytorch ecosystem in terms of naming and parameters (such as Conv2d that uses groups/strides). Example definitons of computational units:
 
-$$\text{I}: [ R ]$$
+$$\text{Affine}: \mathbb{R}^{m \times n},  \mathbb{R}^n$$
 
-$$\text{LI}: [ \tau, R, v_{leak}]$$
+$$\text{Conv1d}: \mathbb{R}^{c_{out} \times c_{in} \times x},  \text{Strides}, \text{Groups}, ... $$ 
 
-$$\text{LIF}: [ \tau, R, v_{leak}, v_{threshold} ]$$
+$$\text{Conv2d}: \mathbb{R}^{c_{out} \times c_{in} \times y \times x},  \text{Strides}, \text{Groups}, ... $$ 
 
-$$\text{Linear}: \mathbb{R}^{m \times n},  \mathbb{R}^n$$
+$$\text{I}: [ R ]$$
 
-$$\text{Conv1d}: \mathbb{R}^{c_{out} \times c_{in} \times x},  \text{Strides}, \text{Groups}, ... $$ 
+$$\text{LI}: [ \tau, R, v_{leak}]$$
 
-$$\text{Conv2d}: \mathbb{R}^{c_{out} \times c_{in} \times y \times x},  \text{Strides}, \text{Groups}, ... $$ 
+$$\text{LIF}: [ \tau, R, v_{leak}, v_{threshold} ]$$
 
 where LIF is defined as a dynamical equation:
 
 $$ \tau \dot{v} = v_{leak} - v + R i $$ 
 
+$$\text{Linear}: \mathbb{R}^{m \times n}$$
+
 
 ## Connectivity 
 Each computational unit is a node in a static graph. Given 3 nodes $A$ which is a LIF node, $B$ which is a Linear node and $C$ which is another LIF node, we can define edges in the graph such as:
 
 $$
 A \rightarrow B \\
 B \rightarrow C
@@ -37,15 +39,15 @@
 
 | **Framework** | **Write to NIR** | **Read from NIR** |
 | --------------- | :--: | :--: |
 | [Lava-DL](https://github.com/lava-nc/lava-dl) | ⬚ | ⬚ |
 | [Nengo](https://nengo.ai) | ⬚ | ⬚ |
 | [Norse](https://github.com/norse/norse) | ✓ | ⬚ |
 | [Rockpool](https://rockpool.ai) | ⬚ | ⬚ |
-| [Sinabs](https://sinabs.readthedocs.io) | ⬚ | ⬚ |
+| [Sinabs](https://sinabs.readthedocs.io) | ✓ | ✓ |
 | [SpiNNaker2](https://spinncloud.com/portfolio/spinnaker2/) | ⬚ | ⬚ |
 | [SynSense Speck](https://www.synsense.ai/products/speck-2/) | ⬚ | ⬚ |
 | [SynSense Xylo](https://www.synsense.ai/products/xylo/) | ⬚ | ⬚ |
 
 
 ## Acknowledgements
 Authors (in alphabetical order):
```

### Comparing `nir-0.0.5/docs/source/conf.py` & `nir-0.0.6/docs/source/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,11 +43,20 @@
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 # html_theme = 'alabaster'
 html_theme = "sphinx_book_theme"
 
+html_theme_options = {
+    "search_bar_text": "Search this book...",
+    "repository_url": "https://github.com/neuromorphs/nir",
+    "repository_branch": "docs",
+    "use_repository_button": True,
+    "use_edit_page_button": False,
+    "use_issues_button": True,
+}
+
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
```

### Comparing `nir-0.0.5/nir/ir.py` & `nir-0.0.6/nir/ir.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,86 +3,130 @@
 
 import numpy as np
 
 
 Edges = typing.NewType("Edges", typing.List[typing.Tuple[int, int]])
 
 
+class NIRNode:
+    """Base superclass of Neural Intermediate Representation Unit (NIR).
+    All NIR primitives inherit from this class, but NIRNodes should never be
+    instantiated.
+    """
+
+
 @dataclass
-class NIR:
-    """Neural Intermediate Representation (NIR)"""
+class NIRGraph(NIRNode):
+    """Neural Intermediate Representation (NIR) Graph containing a number
+    of nodes and edges.
 
-    nodes: typing.List[typing.Any]  # List of computational nodes
+    A graph of computational nodes and identity edges."""
+
+    nodes: typing.List[NIRNode]  # List of computational nodes
     edges: Edges
 
 
-class NIRNode:
-    """Basic Neural Intermediate Representation Unit (NIRUnit)"""
+@dataclass
+class Affine(NIRNode):
+    r"""Affine transform:
 
-    pass
+    .. math::
+        y(t) = W*x(t) + b
+    """
+    weight: np.ndarray  # Weight term
+    bias: np.ndarray  # Bias term
 
 
 @dataclass
-class Input(NIRNode):
-    """Input Node.
+class Conv1d(NIRNode):
+    """Convolutional layer in 1d"""
 
-    This is a virtual node, which allows feeding in data into the graph.
-    """
+    weight: np.ndarray  # Weight C_out * C_in * X
+    stride: int  # Stride
+    padding: int  # Padding
+    dilation: int  # Dilation
+    groups: int  # Groups
+    bias: np.ndarray  # Bias C_out
 
-    shape: np.ndarray  # Shape of input data
+
+@dataclass
+class Conv2d(NIRNode):
+    """Convolutional layer in 2d"""
+
+    weight: np.ndarray  # Weight C_out * C_in * X * Y
+    stride: int  # Stride
+    padding: int  # Padding
+    dilation: int  # Dilation
+    groups: int  # Groups
+    bias: np.ndarray  # Bias C_out
 
 
 @dataclass
-class Output(NIRNode):
-    """Output Node.
+class Delay(NIRNode):
+    """Simple delay node.
 
-    Defines an output of the graph.
+    This node implements a simple delay:
+
+    .. math::
+        y(t) = x(t - \tau)
     """
 
-    pass
+    delay: np.ndarray  # Delay
 
 
 @dataclass
-class I(NIRNode):
-    """Integrator
+class I(NIRNode):  # noqa: E742
+    r"""Integrator
 
     The integrator neuron model is defined by the following equation:
 
     .. math::
         \dot{v} = R I
     """
 
     r: np.ndarray
 
 
 @dataclass
 class IF(NIRNode):
-    """Integrate-and-fire neuron model.
+    r"""Integrate-and-fire neuron model.
 
-   The integrate-and-fire neuron model is defined by the following equations:
+    The integrate-and-fire neuron model is defined by the following equations:
 
-   .. math::
-        \dot{V} = R I
+    .. math::
+        \dot{v} = R I
 
+    .. math::
         z = \begin{cases} 
-            1 & v > v_{threshold} \\ 
+            1 & v > v_{thr} \\ 
             0 & else
         \end{cases}
 
+    .. math::
         v = \begin{cases}
             v-v_{thr} & z=1 \\
             v & else
-            \end{cases}
+        \end{cases}
     """
 
     r: np.ndarray  # Resistance
     v_threshold: np.ndarray  # Firing threshold
 
 
 @dataclass
+class Input(NIRNode):
+    """Input Node.
+
+    This is a virtual node, which allows feeding in data into the graph.
+    """
+
+    shape: np.ndarray  # Shape of input data
+
+
+@dataclass
 class LI(NIRNode):
     r"""Leaky integrator neuron model.
 
     The leaky integrator neuron model is defined by the following equation:
 
     .. math::
         \tau \dot{v} = (v_{leak} - v) + R I
@@ -94,78 +138,112 @@
 
     tau: np.ndarray  # Time constant
     r: np.ndarray  # Resistance
     v_leak: np.ndarray  # Leak voltage
 
 
 @dataclass
+class Linear(NIRNode):
+    r"""Linear transform without bias:
+
+    .. math::
+        y(t) = W*x(t)
+    """
+    weight: np.ndarray  # Weight term
+
+
+@dataclass
 class LIF(NIRNode):
     r"""Leaky integrate and-fire-neuron model.
 
     The leaky integrate-and-fire neuron model is defined by the following equations:
     
     .. math::
         \tau \dot{v} = (v_{leak} - v) + R I
-    
+
+    .. math::
         z = \begin{cases} 
             1 & v > v_{thr} \\ 
             0 & else
         \end{cases}
 
+    .. math::
         v = \begin{cases}
             v-v_{thr} & z=1 \\
             v & else
         \end{cases}
 
-    Where $\tau$ is the time constant, $v$ is the membrane potential,
-    $v_{leak}$ is the leak voltage, $R$ is the resistance, $v_th$ is
-    the firing threshold, and $I$ is the input current.
+    Where :math:`\tau` is the time constant, :math:`v` is the membrane potential,
+    :math:`v_{leak}` is the leak voltage, :math:`R` is the resistance, 
+    :math:`v_{threshold}` is the firing threshold, and :math:`I` is the input current.
     """
 
     tau: np.ndarray  # Time constant
     r: np.ndarray  # Resistance
     v_leak: np.ndarray  # Leak voltage
     v_threshold: np.ndarray  # Firing threshold
 
 
 @dataclass
-class Linear(NIRNode):
-    weights: np.ndarray  # Weights M * N
-    bias: np.ndarray  # Bias M
+class CubaLIF(NIRNode):
+    r"""Current based leaky integrate and-fire-neuron model.
 
+    The current based leaky integrate-and-fire neuron model
+    is defined by the following equations:
 
-@dataclass
-class Conv1d(NIRNode):
-    """Convolutional layer in 1d"""
+    .. math::
+        \tau_syn \ dot{I} = - I + S
 
-    weights: np.ndarray  # Weights C_out * C_in * X
-    stride: int  # Stride
-    padding: int  # Padding
-    dilation: int  # Dilation
-    groups: int  # Groups
-    bias: np.ndarray  # Bias C_out
+        \tau_mem \dot{v} = (v_{leak} - v) + R I
 
+    .. math::
+        z = \begin{cases}
+            1 & v > v_{thr} \\
+            0 & else
+        \end{cases}
 
-@dataclass
-class Conv2d(NIRNode):
-    """Convolutional layer in 2d"""
+    .. math::
+        v = \begin{cases}
+            v-v_{thr} & z=1 \\
+            v & else
+        \end{cases}
 
-    weights: np.ndarray  # Weights C_out * C_in * X * Y
-    stride: int  # Stride
-    padding: int  # Padding
-    dilation: int  # Dilation
-    groups: int  # Groups
-    bias: np.ndarray  # Bias C_out
+    Where :math:`\tau_syn` is the synaptic time constant,
+    :math:`\tau_mem` is the membrane time constant,
+    :math:`v` is the membrane potential,
+    :math:`v_{leak}` is the leak voltage,
+    :math:`R` is the resistance,
+    :math:`v_{threshold}` is the firing threshold,
+    and :math:`S` is the input spike.
+    """
+
+    tau_syn: np.ndarray  # Time constant
+    tau_mem: np.ndarray  # Time constant
+    r: np.ndarray  # Resistance
+    v_leak: np.ndarray  # Leak voltage
+    v_threshold: np.ndarray  # Firing threshold
 
 
 @dataclass
-class Threshold(NIRNode):
-    """Threshold node."""
+class Output(NIRNode):
+    """Output Node.
 
-    threshold: np.ndarray  # Firing threshold
+    Defines an output of the graph.
+    """
+
+    pass
 
 
 @dataclass
-class Delay(NIRNode):
-    """Simple delay node."""
+class Threshold(NIRNode):
+    r"""Threshold node.
 
-    delay: np.ndarray  # Delay
+    This node implements the heaviside step function:
+
+    .. math::
+        z = \begin{cases}
+            1 & v > v_{thr} \\
+            0 & else
+        \end{cases}
+    """
+
+    threshold: np.ndarray  # Firing threshold
```

### Comparing `nir-0.0.5/nir/read.py` & `nir-0.0.6/nir/read.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,95 +1,93 @@
 import typing
 import h5py
 import pathlib
 
 import nir
 
 
-def read(filename: typing.Union[str, pathlib.Path]) -> nir.NIR:
+def read_node(node: typing.Any) -> nir.NIRNode:
+    """Read a graph from a HDF/conn5 file."""
+    if node["type"][()] == b"Affine":
+        return nir.Affine(
+            weight=node["weight"][()],
+            bias=node["bias"][()],
+        )
+    elif node["type"][()] == b"Conv1d":
+        return nir.Conv1d(
+            weight=node["weight"][()],
+            stride=node["stride"][()],
+            padding=node["padding"][()],
+            dilation=node["dilation"][()],
+            groups=node["groups"][()],
+            bias=node["bias"][()],
+        )
+    elif node["type"][()] == b"Conv2d":
+        return nir.Conv2d(
+            weight=node["weight"][()],
+            stride=node["stride"][()],
+            padding=node["padding"][()],
+            dilation=node["dilation"][()],
+            groups=node["groups"][()],
+            bias=node["bias"][()],
+        )
+    elif node["type"][()] == b"Delay":
+        return nir.Delay(
+            delay=node["delay"][()],
+        )
+    elif node["type"][()] == b"I":
+        return nir.I(
+            r=node["r"][()],
+        )
+    elif node["type"][()] == b"IF":
+        return nir.IF(
+            r=node["r"][()],
+            v_threshold=node["v_threshold"][()],
+        )
+    elif node["type"][()] == b"Input":
+        return nir.Input(
+            shape=node["shape"][()],
+        )
+    elif node["type"][()] == b"LI":
+        return nir.LI(
+            tau=node["tau"][()],
+            r=node["r"][()],
+            v_leak=node["v_leak"][()],
+        )
+    elif node["type"][()] == b"Linear":
+        return nir.Linear(
+            weight=node["weight"][()],
+        )
+    elif node["type"][()] == b"LIF":
+        return nir.LIF(
+            tau=node["tau"][()],
+            r=node["r"][()],
+            v_leak=node["v_leak"][()],
+            v_threshold=node["v_threshold"][()],
+        )
+    elif node["type"][()] == b"CubaLIF":
+        return nir.CubaLIF(
+            tau_mem=node["tau_mem"][()],
+            tau_syn=node["tau_syn"][()],
+            r=node["r"][()],
+            v_leak=node["v_leak"][()],
+            v_threshold=node["v_threshold"][()],
+        )
+    elif node["type"][()] == b"NIRGraph":
+        return nir.NIRGraph(
+            nodes=[read_node(n) for n in node["nodes"].values()],
+            edges=node["edges"][()],
+        )
+    elif node["type"][()] == b"Output":
+        return nir.Output()
+    elif node["type"][()] == b"Threshold":
+        return nir.Threshold(
+            threshold=node["threshold"][()],
+        )
+    else:
+        raise ValueError(f"Unknown unit type: {node['type'][()]}")
+
+
+def read(filename: typing.Union[str, pathlib.Path]) -> nir.NIRGraph:
     """Load a NIR from a HDF/conn5 file."""
     with h5py.File(filename, "r") as f:
-        nodes = []
-        for k, node in f["nodes"].items():
-            if node["type"][()] == b"Delay":
-                nodes.append(
-                    nir.Delay(
-                        delay=node["delay"][()],
-                    )
-                )
-            elif node["type"][()] == b"I":
-                nodes.append(
-                    nir.I(
-                        r=node["r"][()],
-                    )
-                )
-            elif node["type"][()] == b"IF":
-                nodes.append(
-                    nir.IF(
-                        r=node["r"][()],
-                        v_threshold=node["v_threshold"][()],
-                    )
-                )
-            elif node["type"][()] == b"Input":
-                nodes.append(
-                    nir.Input(
-                        shape=node["shape"][()],
-                    )
-                )
-            elif node["type"][()] == b"Output":
-                nodes.append(nir.Output())
-            elif node["type"][()] == b"LI":
-                nodes.append(
-                    nir.LI(
-                        tau=node["tau"][()],
-                        r=node["r"][()],
-                        v_leak=node["v_leak"][()],
-                    )
-                )
-            elif node["type"][()] == b"LIF":
-                nodes.append(
-                    nir.LIF(
-                        tau=node["tau"][()],
-                        r=node["r"][()],
-                        v_leak=node["v_leak"][()],
-                        v_threshold=node["v_threshold"][()],
-                    )
-                )
-            elif node["type"][()] == b"Linear":
-                nodes.append(
-                    nir.Linear(
-                        weights=node["weights"][()],
-                        bias=node["bias"][()],
-                    )
-                )
-            elif node["type"][()] == b"Conv1d":
-                nodes.append(
-                    nir.Conv1d(
-                        weights=node["weights"][()],
-                        stride=node["stride"][()],
-                        padding=node["padding"][()],
-                        dilation=node["dilation"][()],
-                        groups=node["groups"][()],
-                        bias=node["bias"][()],
-                    )
-                )
-            elif node["type"][()] == b"Conv2d":
-                nodes.append(
-                    nir.Conv2d(
-                        weights=node["weights"][()],
-                        stride=node["stride"][()],
-                        padding=node["padding"][()],
-                        dilation=node["dilation"][()],
-                        groups=node["groups"][()],
-                        bias=node["bias"][()],
-                    )
-                )
-            elif node["type"][()] == b"Threshold":
-                nodes.append(
-                    nir.Threshold(
-                        threshold=node["threshold"][()],
-                    )
-                )
-            else:
-                raise ValueError(f"Unknown unit type: {node['type'][()]}")
-        edges = f["edges"][()]
-        return nir.NIR(nodes=nodes, edges=edges)
+        return read_node(f["node"])
```

### Comparing `nir-0.0.5/nir/write.py` & `nir-0.0.6/nir/write.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,85 +3,107 @@
 
 import h5py
 import numpy as np
 
 import nir
 
 
-def write(filename: typing.Union[str, pathlib.Path], graph: nir.NIR) -> None:
-    def convert_node(node: nir.NIRNode) -> dict:
-        if isinstance(node, nir.Delay):
-            return {"type": "Delay", "delay": node.delay}
-        elif isinstance(node, nir.I):
-            return {"type": "I", "r": node.r}
-        elif isinstance(node, nir.IF):
-            return {"type": "IF", "r": node.r, "v_threshold": node.v_threshold}
-        elif isinstance(node, nir.Input):
-            return {
-                "type": "Input",
-                "shape": node.shape,
-            }
-        elif isinstance(node, nir.LI):
-            return {
-                "type": "LI",
-                "tau": node.tau,
-                "r": node.r,
-                "v_leak": node.v_leak,
-            }
-        elif isinstance(node, nir.LIF):
-            return {
-                "type": "LIF",
-                "tau": node.tau,
-                "r": node.r,
-                "v_leak": node.v_leak,
-                "v_threshold": node.v_threshold,
-            }
-        elif isinstance(node, nir.Linear):
-            return {
-                "type": "Linear",
-                "weights": node.weights,
-                "bias": node.bias,
-            }
-        elif isinstance(node, nir.Conv1d):
-            return {
-                "type": "Conv1d",
-                "weights": node.weights,
-                "stride": node.stride,
-                "padding": node.padding,
-                "dilation": node.dilation,
-                "groups": node.groups,
-                "bias": node.bias,
-            }
-        elif isinstance(node, nir.Conv2d):
-            return {
-                "type": "Conv2d",
-                "weights": node.weights,
-                "stride": node.stride,
-                "padding": node.padding,
-                "dilation": node.dilation,
-                "groups": node.groups,
-                "bias": node.bias,
-            }
-        elif isinstance(node, nir.Output):
-            return {
-                "type": "Output",
-            }
-        elif isinstance(node, nir.Threshold):
-            return {"type": "Threshold", "threshold": node.threshold}
-        else:
-            raise ValueError(f"Unknown node type: {node}")
+def _convert_node(node: nir.NIRNode) -> dict:
+    if isinstance(node, nir.Affine):
+        return {
+            "type": "Affine",
+            "weight": node.weight,
+            "bias": node.bias,
+        }
+    elif isinstance(node, nir.Conv1d):
+        return {
+            "type": "Conv1d",
+            "weight": node.weight,
+            "stride": node.stride,
+            "padding": node.padding,
+            "dilation": node.dilation,
+            "groups": node.groups,
+            "bias": node.bias,
+        }
+    elif isinstance(node, nir.Conv2d):
+        return {
+            "type": "Conv2d",
+            "weight": node.weight,
+            "stride": node.stride,
+            "padding": node.padding,
+            "dilation": node.dilation,
+            "groups": node.groups,
+            "bias": node.bias,
+        }
+    elif isinstance(node, nir.Delay):
+        return {"type": "Delay", "delay": node.delay}
+    elif isinstance(node, nir.I):
+        return {"type": "I", "r": node.r}
+    elif isinstance(node, nir.IF):
+        return {"type": "IF", "r": node.r, "v_threshold": node.v_threshold}
+    elif isinstance(node, nir.Input):
+        return {
+            "type": "Input",
+            "shape": node.shape,
+        }
+    elif isinstance(node, nir.LI):
+        return {
+            "type": "LI",
+            "tau": node.tau,
+            "r": node.r,
+            "v_leak": node.v_leak,
+        }
+    elif isinstance(node, nir.Linear):
+        return {
+            "type": "Linear",
+            "weight": node.weight,
+        }
+    elif isinstance(node, nir.LIF):
+        return {
+            "type": "LIF",
+            "tau": node.tau,
+            "r": node.r,
+            "v_leak": node.v_leak,
+            "v_threshold": node.v_threshold,
+        }
+    elif isinstance(node, nir.CubaLIF):
+        return {
+            "type": "CubaLIF",
+            "tau_mem": node.tau_mem,
+            "tau_syn": node.tau_syn,
+            "r": node.r,
+            "v_leak": node.v_leak,
+            "v_threshold": node.v_threshold,
+        }
+    elif isinstance(node, nir.NIRGraph):
+        return {
+            "type": "NIRGraph",
+            "nodes": {i: _convert_node(n) for i, n in enumerate(node.nodes)},
+            "edges": node.edges,
+        }
+    elif isinstance(node, nir.Output):
+        return {
+            "type": "Output",
+        }
+    elif isinstance(node, nir.Threshold):
+        return {"type": "Threshold", "threshold": node.threshold}
+    else:
+        raise ValueError(f"Unknown node type: {node}")
 
+
+def write(filename: typing.Union[str, pathlib.Path], graph: nir.NIRNode) -> None:
     """Write a NIR to a HDF5 file."""
+
+    def write_recursive(group: h5py.Group, node: dict) -> None:
+        for k, v in node.items():
+            if isinstance(v, str):
+                group.create_dataset(k, data=v, dtype=h5py.string_dtype())
+            elif isinstance(v, np.ndarray):
+                group.create_dataset(k, data=v, dtype=v.dtype)
+            elif isinstance(v, dict):
+                write_recursive(group.create_group(str(k)), v)
+            else:
+                group.create_dataset(k, data=v)
+
     with h5py.File(filename, "w") as f:
-        nodes_group = f.create_group("nodes")
-        for i, node in enumerate(graph.nodes):
-            d = convert_node(node)
-            node_group = nodes_group.create_group(str(i))
-            for k, v in d.items():
-                if isinstance(v, str):
-                    node_group.create_dataset(k, data=v, dtype=h5py.string_dtype())
-                elif isinstance(v, np.ndarray):
-                    node_group.create_dataset(k, data=v, dtype=v.dtype)
-                else:
-                    node_group.create_dataset(k, data=v)
-                    # raise ValueError(f"Unknown type: {type(v)}")
-        f.create_dataset("edges", data=graph.edges)
+        node_group = f.create_group("node")
+        write_recursive(node_group, _convert_node(graph))
```

### Comparing `nir-0.0.5/nir.egg-info/PKG-INFO` & `nir-0.0.6/nir.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nir
-Version: 0.0.5
+Version: 0.0.6
 Summary: Neuromorphic Intermediate Representation
 Author-email: Steven Abreu <s.abreu@rug.nl>, Felix Bauer <felix.bauer@synsense.ai>, Jason Eshraghian <jeshragh@ucsc.edu>, Matthias Jobst <matthias.jobst2@tu-dresden.de>, Gregor Lenz <mail@lenzgregor.com>, Jens Egholm Pedersen <jens@jepedersen.dk>, Sadique Sheik <sadique.sheik@synsense.ai>
 Project-URL: homepage, https://github.com/neuromorphs/nir
 Keywords: neuromorphic,intermediate,representation
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -20,30 +20,32 @@
 # NIR: Neuromorphic Intermediate Representation specification
 
 NIR defines neuron models and connectivity for arbitrary networks that include spiking neurons. Neuron models are defined as dynamical system equations, because time is an essential component of neuromorphic systems. The goal is to provide a common format that different spiking neural network (SNN) frameworks can convert to. That allows a user to train an SNN in framework X and convert it to framework Y. Framework X might offer particularly fast training while framework Y might offer deployment to neuromorphic hardware.
 
 ## Computational units
 On top of popular primitives such as convolutional or fully connected/linear computations, we define additional compuational primitives that are specific to neuromorphic computing and hardware implementations thereof. Computational units that are not specifically neuromorphic take inspiration from the Pytorch ecosystem in terms of naming and parameters (such as Conv2d that uses groups/strides). Example definitons of computational units:
 
-$$\text{I}: [ R ]$$
+$$\text{Affine}: \mathbb{R}^{m \times n},  \mathbb{R}^n$$
 
-$$\text{LI}: [ \tau, R, v_{leak}]$$
+$$\text{Conv1d}: \mathbb{R}^{c_{out} \times c_{in} \times x},  \text{Strides}, \text{Groups}, ... $$ 
 
-$$\text{LIF}: [ \tau, R, v_{leak}, v_{threshold} ]$$
+$$\text{Conv2d}: \mathbb{R}^{c_{out} \times c_{in} \times y \times x},  \text{Strides}, \text{Groups}, ... $$ 
 
-$$\text{Linear}: \mathbb{R}^{m \times n},  \mathbb{R}^n$$
+$$\text{I}: [ R ]$$
 
-$$\text{Conv1d}: \mathbb{R}^{c_{out} \times c_{in} \times x},  \text{Strides}, \text{Groups}, ... $$ 
+$$\text{LI}: [ \tau, R, v_{leak}]$$
 
-$$\text{Conv2d}: \mathbb{R}^{c_{out} \times c_{in} \times y \times x},  \text{Strides}, \text{Groups}, ... $$ 
+$$\text{LIF}: [ \tau, R, v_{leak}, v_{threshold} ]$$
 
 where LIF is defined as a dynamical equation:
 
 $$ \tau \dot{v} = v_{leak} - v + R i $$ 
 
+$$\text{Linear}: \mathbb{R}^{m \times n}$$
+
 
 ## Connectivity 
 Each computational unit is a node in a static graph. Given 3 nodes $A$ which is a LIF node, $B$ which is a Linear node and $C$ which is another LIF node, we can define edges in the graph such as:
 
 $$
 A \rightarrow B \\
 B \rightarrow C
@@ -56,15 +58,15 @@
 
 | **Framework** | **Write to NIR** | **Read from NIR** |
 | --------------- | :--: | :--: |
 | [Lava-DL](https://github.com/lava-nc/lava-dl) | ⬚ | ⬚ |
 | [Nengo](https://nengo.ai) | ⬚ | ⬚ |
 | [Norse](https://github.com/norse/norse) | ✓ | ⬚ |
 | [Rockpool](https://rockpool.ai) | ⬚ | ⬚ |
-| [Sinabs](https://sinabs.readthedocs.io) | ⬚ | ⬚ |
+| [Sinabs](https://sinabs.readthedocs.io) | ✓ | ✓ |
 | [SpiNNaker2](https://spinncloud.com/portfolio/spinnaker2/) | ⬚ | ⬚ |
 | [SynSense Speck](https://www.synsense.ai/products/speck-2/) | ⬚ | ⬚ |
 | [SynSense Xylo](https://www.synsense.ai/products/xylo/) | ⬚ | ⬚ |
 
 
 ## Acknowledgements
 Authors (in alphabetical order):
```

### Comparing `nir-0.0.5/pyproject.toml` & `nir-0.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools"]
 
 [project]
 name = "nir"
-version = "0.0.5"
+version = "0.0.6"
 description = "Neuromorphic Intermediate Representation"
 authors = [
   { name = "Steven Abreu", email = "s.abreu@rug.nl" },
   { name = "Felix Bauer", email = "felix.bauer@synsense.ai" },
   { name = "Jason Eshraghian", email = "jeshragh@ucsc.edu" },
   { name = "Matthias Jobst", email = "matthias.jobst2@tu-dresden.de" },
   { name = "Gregor Lenz", email = "mail@lenzgregor.com" },
```

### Comparing `nir-0.0.5/tests/test_ir.py` & `nir-0.0.6/tests/test_ir.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,40 +1,58 @@
 import nir
 
 
 def test_simple():
-    ir = nir.NIR(nodes=[nir.Linear(weights=[1, 2, 3], bias=4)], edges=[(0, 0)])
-    assert ir.nodes[0].weights == [1, 2, 3]
+    ir = nir.NIRGraph(nodes=[nir.Affine(weight=[1, 2, 3], bias=4)], edges=[(0, 0)])
+    assert ir.nodes[0].weight == [1, 2, 3]
     assert ir.nodes[0].bias == 4
     assert ir.edges == [(0, 0)]
 
 
+def test_nested():
+    nested = nir.NIRGraph(
+        nodes=[
+            nir.I(r=[1, 1]),
+            nir.Delay([2, 2]),
+        ],
+        edges=[(0, 1), (1, 0)]
+    )
+    ir = nir.NIRGraph(
+        nodes=[nir.Affine(weight=[1, 2], bias=4), nested],
+        edges=[(0, 1)],
+    )
+    assert ir.nodes[0].weight == [1, 2]
+    assert ir.nodes[1].nodes[0].r == [1, 1]
+    assert ir.nodes[1].nodes[1].delay == [2, 2]
+    assert ir.nodes[1].edges == [(0, 1), (1, 0)]
+
+
 def test_simple_with_input_output():
-    ir = nir.NIR(
+    ir = nir.NIRGraph(
         nodes=[
             nir.Input(
                 shape=[
                     3,
                 ]
             ),
-            nir.Linear(weights=[1, 2, 3], bias=4),
+            nir.Affine(weight=[1, 2, 3], bias=4),
             nir.Output(),
         ],
         edges=[(0, 1), (1, 2)],
     )
     assert ir.nodes[0].shape == [
         3,
     ]
-    assert ir.nodes[1].weights == [1, 2, 3]
+    assert ir.nodes[1].weight == [1, 2, 3]
     assert ir.nodes[1].bias == 4
     assert ir.edges == [(0, 1), (1, 2)]
 
 
 def test_delay():
-    ir = nir.NIR(
+    ir = nir.NIRGraph(
         nodes=[
             nir.Input(
                 shape=[
                     3,
                 ]
             ),
             nir.Delay(delay=[1, 2, 3]),
@@ -46,15 +64,15 @@
         3,
     ]
     assert ir.nodes[1].delay == [1, 2, 3]
     assert ir.edges == [(0, 1), (1, 2)]
 
 
 def test_threshold():
-    ir = nir.NIR(
+    ir = nir.NIRGraph(
         nodes=[
             nir.Input(
                 shape=[
                     3,
                 ]
             ),
             nir.Threshold(threshold=[2.0, 2.5, 2.8]),
@@ -63,7 +81,13 @@
         edges=[(0, 1), (1, 2)],
     )
     assert ir.nodes[0].shape == [
         3,
     ]
     assert ir.nodes[1].threshold == [2.0, 2.5, 2.8]
     assert ir.edges == [(0, 1), (1, 2)]
+
+
+def test_linear():
+    ir = nir.NIRGraph(nodes=[nir.Linear(weight=[1, 2, 3])], edges=[(0, 0)])
+    assert ir.nodes[0].weight == [1, 2, 3]
+    assert ir.edges == [(0, 0)]
```

### Comparing `nir-0.0.5/tests/test_readwrite.py` & `nir-0.0.6/tests/test_readwrite.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,84 +1,126 @@
 import tempfile
 
 import numpy as np
 
 import nir
 
 
-def factory_test_graph(ir: nir.NIR):
+def assert_equivalence(ir: nir.NIRGraph, ir2: nir.NIRGraph):
+    for i in range(len(ir.nodes)):
+        if isinstance (ir.nodes[i], nir.NIRGraph):
+            # Handle nested graphs
+            assert isinstance(ir2.nodes[i], nir.NIRGraph)
+            assert_equivalence(ir.nodes[i], ir2.nodes[i])
+        else:
+            for k, v in ir.nodes[i].__dict__.items():
+                if isinstance(v, np.ndarray) or isinstance(v, list):
+                    assert np.array_equal(v, getattr(ir2.nodes[i], k))
+                else:
+                    assert v == getattr(ir2.nodes[i], k)
+
+
+def factory_test_graph(ir: nir.NIRGraph):
     tmp = tempfile.mktemp()
     nir.write(tmp, ir)
     ir2 = nir.read(tmp)
-    for i in range(len(ir.nodes)):
-        for k, v in ir.nodes[i].__dict__.items():
-            if isinstance(v, np.ndarray) or isinstance(v, list):
-                assert np.array_equal(v, getattr(ir2.nodes[i], k))
-            else:
-                assert v == getattr(ir2.nodes[i], k)
+    assert_equivalence(ir, ir2)
 
 
 def test_simple():
-    ir = nir.NIR(nodes=[nir.Linear(weights=[1, 2, 3], bias=4)], edges=[(0, 0)])
+    ir = nir.NIRGraph(nodes=[nir.Affine(weight=[1, 2, 3], bias=4)], edges=[(0, 0)])
+    factory_test_graph(ir)
+
+
+def test_nested():
+    nested = nir.NIRGraph(
+        nodes=[
+            nir.I(r=[1, 1]),
+            nir.Delay([2, 2]),
+        ],
+        edges=[(0, 1), (1, 0)]
+    )
+    ir = nir.NIRGraph(
+        nodes=[nir.Affine(weight=[1, 2], bias=4), nested],
+        edges=[(0, 1)],
+    )
     factory_test_graph(ir)
 
 
 def test_integrator():
-    ir = nir.NIR(
-        nodes=[nir.Linear(weights=[1], bias=0), nir.I(r=2)],
+    ir = nir.NIRGraph(
+        nodes=[nir.Affine(weight=[1], bias=0), nir.I(r=2)],
         edges=[(0, 0)],
     )
     factory_test_graph(ir)
 
 
-def test_integrator():
-    ir = nir.NIR(
-        nodes=[nir.Linear(weights=[1], bias=0), nir.IF(r=2, v_threshold=3)],
+def test_integrate_and_fire():
+    ir = nir.NIRGraph(
+        nodes=[nir.Affine(weight=[1], bias=0), nir.IF(r=2, v_threshold=3)],
         edges=[(0, 0)],
     )
     factory_test_graph(ir)
 
 
 def test_leaky_integrator():
-    ir = nir.NIR(
-        nodes=[nir.Linear(weights=[1], bias=0), nir.LI(tau=1, r=2, v_leak=3)],
+    ir = nir.NIRGraph(
+        nodes=[nir.Affine(weight=[1], bias=0), nir.LI(tau=1, r=2, v_leak=3)],
+        edges=[(0, 0)],
+    )
+    factory_test_graph(ir)
+
+
+def test_linear():
+    ir = nir.NIRGraph(
+        nodes=[nir.Linear(weight=[1]), nir.LI(tau=1, r=2, v_leak=3)],
         edges=[(0, 0)],
     )
     factory_test_graph(ir)
 
 
 def test_leaky_integrator_and_fire():
-    ir = nir.NIR(
+    ir = nir.NIRGraph(
         nodes=[
-            nir.Linear(weights=[1], bias=0),
+            nir.Affine(weight=[1], bias=0),
             nir.LIF(tau=1, r=2, v_leak=3, v_threshold=4),
         ],
         edges=[(0, 0)],
     )
     factory_test_graph(ir)
 
+def test_current_based_leaky_integrator_and_fire():
+    ir = nir.NIRGraph(
+        nodes=[
+            nir.Linear(weight=[1]),
+            nir.CubaLIF(tau_mem=1, tau_syn=1, r=2, v_leak=3, v_threshold=4),
+        ],
+        edges=[(0, 0)],
+    )
+    factory_test_graph(ir)
+
 
 def test_simple_with_read_write():
-    ir = nir.NIR(
+    ir = nir.NIRGraph(
         nodes=[
             nir.Input(
                 shape=[
                     3,
                 ]
             ),
-            nir.Linear(weights=[1, 2, 3], bias=4),
+            nir.Affine(weight=[1, 2, 3], bias=4),
             nir.Output(),
         ],
         edges=[(0, 1), (1, 2)],
     )
     factory_test_graph(ir)
 
 
 def test_delay():
-    ir = nir.NIR(
+    ir = nir.NIRGraph(
         nodes=[
             nir.Input(
                 shape=[
                     3,
                 ]
             ),
             nir.Delay(delay=[1, 2, 3]),
@@ -86,15 +128,15 @@
         ],
         edges=[(0, 1), (1, 2)],
     )
     factory_test_graph(ir)
 
 
 def test_threshold():
-    ir = nir.NIR(
+    ir = nir.NIRGraph(
         nodes=[
             nir.Input(
                 shape=[
                     3,
                 ]
             ),
             nir.Threshold(threshold=[2.0, 2.5, 2.8]),
```

