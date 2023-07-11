# Comparing `tmp/torchlpc-0.1.tar.gz` & `tmp/torchlpc-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchlpc-0.1.tar", last modified: Sun Jul  9 03:25:04 2023, max compression
+gzip compressed data, was "torchlpc-0.2.tar", last modified: Tue Jul 11 17:14:14 2023, max compression
```

## Comparing `torchlpc-0.1.tar` & `torchlpc-0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:25:04.353730 torchlpc-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-09 03:24:54.000000 torchlpc-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-09 03:25:04.349730 torchlpc-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-09 03:24:54.000000 torchlpc-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-09 03:25:04.353730 torchlpc-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-09 03:24:54.000000 torchlpc-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:25:04.349730 torchlpc-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-07-09 03:24:54.000000 torchlpc-0.1/tests/test_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:25:04.349730 torchlpc-0.1/torchlpc/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-09 03:24:54.000000 torchlpc-0.1/torchlpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5204 2023-07-09 03:24:54.000000 torchlpc-0.1/torchlpc/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-09 03:25:04.349730 torchlpc-0.1/torchlpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-09 03:25:04.000000 torchlpc-0.1/torchlpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-09 03:25:04.000000 torchlpc-0.1/torchlpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-09 03:25:04.000000 torchlpc-0.1/torchlpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-09 03:25:04.000000 torchlpc-0.1/torchlpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-09 03:25:04.000000 torchlpc-0.1/torchlpc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:14:14.446075 torchlpc-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-11 17:14:04.000000 torchlpc-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-11 17:14:14.446075 torchlpc-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-11 17:14:04.000000 torchlpc-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 17:14:14.446075 torchlpc-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-11 17:14:04.000000 torchlpc-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:14:14.446075 torchlpc-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-11 17:14:04.000000 torchlpc-0.2/tests/test_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:14:14.446075 torchlpc-0.2/torchlpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-07-11 17:14:04.000000 torchlpc-0.2/torchlpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5186 2023-07-11 17:14:04.000000 torchlpc-0.2/torchlpc/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 17:14:14.446075 torchlpc-0.2/torchlpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-11 17:14:14.000000 torchlpc-0.2/torchlpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-11 17:14:14.000000 torchlpc-0.2/torchlpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 17:14:14.000000 torchlpc-0.2/torchlpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-11 17:14:14.000000 torchlpc-0.2/torchlpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 17:14:14.000000 torchlpc-0.2/torchlpc.egg-info/top_level.txt
```

### Comparing `torchlpc-0.1/LICENSE` & `torchlpc-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torchlpc-0.1/PKG-INFO` & `torchlpc-0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlpc
-Version: 0.1
+Version: 0.2
 Summary: Fast, efficient, and differentiable time-varying LPC filtering in PyTorch.
 Home-page: https://github.com/yoyololicon/torchlpc
 Author: Chin-Yun Yu
 Author-email: chin-yun.yu@qmul.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 `torchlpc` provides a PyTorch implementation of the Linear Predictive Coding (LPC) filtering operation, also known as IIR filtering.
 It's fast, differentiable, and supports batched inputs with time-varying filter coefficients.
 The computation is done as follows:
 
 Given an input signal $\mathbf{x} \in \mathbb{R}^T$ and time-varying LPC coefficients $\mathbf{A} \in \mathbb{R}^{T \times N}$ with an order of $N$, the LPC filtering operation is defined as:
 
 ```math
-\mathbf{y}_t = \mathbf{x}_t - \sum_{i=1}^N \mathbf{A}_{t,i} \mathbf{x}_{t-i}.
+\mathbf{y}_t = \mathbf{x}_t - \sum_{i=1}^N \mathbf{A}_{t,i} \mathbf{y}_{t-i}.
 ```
 
 It's still in early development, so please open an issue if you find any bugs.
 
 ## Usage
 
 ```python
```

### Comparing `torchlpc-0.1/README.md` & `torchlpc-0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 `torchlpc` provides a PyTorch implementation of the Linear Predictive Coding (LPC) filtering operation, also known as IIR filtering.
 It's fast, differentiable, and supports batched inputs with time-varying filter coefficients.
 The computation is done as follows:
 
 Given an input signal $\mathbf{x} \in \mathbb{R}^T$ and time-varying LPC coefficients $\mathbf{A} \in \mathbb{R}^{T \times N}$ with an order of $N$, the LPC filtering operation is defined as:
 
 ```math
-\mathbf{y}_t = \mathbf{x}_t - \sum_{i=1}^N \mathbf{A}_{t,i} \mathbf{x}_{t-i}.
+\mathbf{y}_t = \mathbf{x}_t - \sum_{i=1}^N \mathbf{A}_{t,i} \mathbf{y}_{t-i}.
 ```
 
 It's still in early development, so please open an issue if you find any bugs.
 
 ## Usage
 
 ```python
```

### Comparing `torchlpc-0.1/setup.py` & `torchlpc-0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 
 NAME = "torchlpc"
-VERSION = "0.1"
+VERSION = "0.2"
 MAINTAINER = "Chin-Yun Yu"
 EMAIL = "chin-yun.yu@qmul.ac.uk"
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
```

### Comparing `torchlpc-0.1/tests/test_grad.py` & `torchlpc-0.2/tests/test_grad.py`

 * *Files 18% similar despite different names*

```diff
@@ -73,19 +73,39 @@
 def test_low_order_cuda(
     x_requires_grad: bool,
     a_requires_grad: bool,
     zi_requires_grad: bool,
     samples: int,
 ):
     batch_size = 4
-    samples = 32
     x, A, zi = create_test_inputs(batch_size, samples)
     x = x.cuda()
     A = A.cuda()
     zi = zi.cuda()
 
     A.requires_grad = a_requires_grad
     x.requires_grad = x_requires_grad
     zi.requires_grad = zi_requires_grad
 
     assert gradcheck(LPC.apply, (x, A, zi))
     assert gradgradcheck(LPC.apply, (x, A, zi))
+
+
+@pytest.mark.skipif(not torch.cuda.is_available(), reason="CUDA not available")
+def test_float64_vs_32_cuda():
+    batch_size = 4
+    samples = 32
+    x, A, zi = create_test_inputs(batch_size, samples)
+    x = x.cuda()
+    A = A.cuda()
+    zi = zi.cuda()
+
+    x32 = x.float()
+    A32 = A.float()
+    zi32 = zi.float()
+
+    y64 = LPC.apply(x, A, zi)
+    y32 = LPC.apply(x32, A32, zi32)
+
+    assert torch.allclose(y64, y32.double(), atol=1e-6), torch.max(
+        torch.abs(y64 - y32.double())
+    )
```

### Comparing `torchlpc-0.1/torchlpc/__init__.py` & `torchlpc-0.2/torchlpc/__init__.py`

 * *Files identical despite different names*

### Comparing `torchlpc-0.1/torchlpc/core.py` & `torchlpc-0.2/torchlpc/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,16 +26,18 @@
         circular_idx = t % order
         if i == (order - 1):
             sm[circular_idx] *= -A[b, t, i]
         cuda.syncthreads()
 
         if i == (order - 1):
             v = padded_y[b, t + order]
+        elif i > circular_idx - 1:
+            v = -A[b, t, i] * sm[circular_idx - i - 1 + order]
         else:
-            v = -A[b, t, i] * sm[(circular_idx - i - 1 + order) % order]
+            v = -A[b, t, i] * sm[circular_idx - i - 1]
         cuda.atomic.add(sm, circular_idx, v)
         cuda.syncthreads()
 
         if i == (order - 1):
             padded_y[b, t + order] = sm[circular_idx]
 
 
@@ -58,16 +60,18 @@
         circular_idx = t % order
         if i == (order - 1):
             sm[circular_idx] *= -A[b, t, i]
         cuda.syncthreads()
 
         if i == (order - 1):
             v = padded_y[b, t + order]
+        elif i > circular_idx - 1:
+            v = -A[b, t, i] * sm[circular_idx - i - 1 + order]
         else:
-            v = -A[b, t, i] * sm[(circular_idx - i - 1 + order) % order]
+            v = -A[b, t, i] * sm[circular_idx - i - 1]
         cuda.atomic.add(sm, circular_idx, v)
         cuda.syncthreads()
 
         if i == (order - 1):
             padded_y[b, t + order] = sm[circular_idx]
 
 
@@ -111,29 +115,28 @@
             padded_y[b, t + order] = ref
 
     return padded_y[:, order:]
 
 
 class LPC(Function):
     @staticmethod
-    def forward(x: torch.Tensor, A: torch.Tensor, zi: torch.Tensor) -> torch.Tensor:
+    def forward(
+        ctx: Any, x: torch.Tensor, A: torch.Tensor, zi: torch.Tensor
+    ) -> torch.Tensor:
         if x.is_cuda:
-            return lpc_cuda(x.detach(), A.detach(), zi.detach())
-
-        y = lpc_np(
-            x.detach().cpu().numpy(),
-            A.detach().cpu().numpy(),
-            zi.detach().cpu().numpy(),
-        )
-        return torch.from_numpy(y).to(x.device, x.dtype)
-
-    @staticmethod
-    def setup_context(ctx: Any, inputs: Tuple[Any], output: Any) -> Any:
-        _, A, zi = inputs
-        ctx.save_for_backward(A, zi, output)
+            y = lpc_cuda(x.detach(), A.detach(), zi.detach())
+        else:
+            y = lpc_np(
+                x.detach().cpu().numpy(),
+                A.detach().cpu().numpy(),
+                zi.detach().cpu().numpy(),
+            )
+            y = torch.from_numpy(y).to(x.device, x.dtype)
+        ctx.save_for_backward(A, zi, y)
+        return y
 
     @staticmethod
     def backward(
         ctx, grad_y: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor, Optional[torch.Tensor]]:
         A, zi, y = ctx.saved_tensors
         grad_x = grad_A = grad_zi = None
@@ -163,16 +166,13 @@
             flipped_grad_x = flipped_grad_x[:, :-order]
 
         if ctx.needs_input_grad[0]:
             grad_x = flipped_grad_x.flip(1)
 
         if ctx.needs_input_grad[1]:
             valid_y = y[:, :-1]
-            if zi is None:
-                padded_y = F.pad(valid_y.unsqueeze(1), (order, 0)).squeeze(1)
-            else:
-                padded_y = torch.cat([zi.flip(1), valid_y], dim=1)
+            padded_y = torch.cat([zi.flip(1), valid_y], dim=1)
 
             unfolded_y = padded_y.unfold(1, order, 1).flip(2)
             grad_A = unfolded_y * -flipped_grad_x.flip(1).unsqueeze(2)
 
         return grad_x, grad_A, grad_zi
```

### Comparing `torchlpc-0.1/torchlpc.egg-info/PKG-INFO` & `torchlpc-0.2/torchlpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchlpc
-Version: 0.1
+Version: 0.2
 Summary: Fast, efficient, and differentiable time-varying LPC filtering in PyTorch.
 Home-page: https://github.com/yoyololicon/torchlpc
 Author: Chin-Yun Yu
 Author-email: chin-yun.yu@qmul.ac.uk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -16,15 +16,15 @@
 `torchlpc` provides a PyTorch implementation of the Linear Predictive Coding (LPC) filtering operation, also known as IIR filtering.
 It's fast, differentiable, and supports batched inputs with time-varying filter coefficients.
 The computation is done as follows:
 
 Given an input signal $\mathbf{x} \in \mathbb{R}^T$ and time-varying LPC coefficients $\mathbf{A} \in \mathbb{R}^{T \times N}$ with an order of $N$, the LPC filtering operation is defined as:
 
 ```math
-\mathbf{y}_t = \mathbf{x}_t - \sum_{i=1}^N \mathbf{A}_{t,i} \mathbf{x}_{t-i}.
+\mathbf{y}_t = \mathbf{x}_t - \sum_{i=1}^N \mathbf{A}_{t,i} \mathbf{y}_{t-i}.
 ```
 
 It's still in early development, so please open an issue if you find any bugs.
 
 ## Usage
 
 ```python
```

