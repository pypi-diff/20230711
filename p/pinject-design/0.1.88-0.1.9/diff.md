# Comparing `tmp/pinject_design-0.1.88.tar.gz` & `tmp/pinject-design-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pinject_design-0.1.88.tar", max compression
+gzip compressed data, was "pinject-design-0.1.9.tar", max compression
```

## Comparing `pinject_design-0.1.88.tar` & `pinject-design-0.1.9.tar`

### file list

```diff
@@ -1,44 +1,13 @@
--rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.000000 pinject_design-0.1.88/LICENSE
--rw-r--r--   0        0        0      170 2022-12-05 13:41:50.000000 pinject_design-0.1.88/pinject_design/__init__.py
--rw-r--r--   0        0        0        0 2022-08-10 02:59:10.000000 pinject_design-0.1.88/pinject_design/di/__init__.py
--rw-r--r--   0        0        0     1786 2022-10-12 04:28:37.000000 pinject_design-0.1.88/pinject_design/di/app_designed.py
--rw-r--r--   0        0        0     2442 2023-05-06 03:52:35.678286 pinject_design-0.1.88/pinject_design/di/app_injected.py
--rw-r--r--   0        0        0      640 2022-10-09 04:01:27.000000 pinject_design-0.1.88/pinject_design/di/applicative.py
--rw-r--r--   0        0        0     6671 2023-05-08 06:26:47.063185 pinject_design-0.1.88/pinject_design/di/ast.py
--rw-r--r--   0        0        0     7338 2023-05-04 06:32:55.349238 pinject_design-0.1.88/pinject_design/di/design.py
--rw-r--r--   0        0        0     1943 2023-05-09 04:27:42.242474 pinject_design-0.1.88/pinject_design/di/designed.py
--rw-r--r--   0        0        0     1341 2022-11-10 03:41:15.000000 pinject_design-0.1.88/pinject_design/di/dynamic_proxy.py
--rw-r--r--   0        0        0    28337 2023-07-04 16:13:18.254578 pinject_design-0.1.88/pinject_design/di/graph.py
--rw-r--r--   0        0        0       27 2023-05-24 05:53:54.286111 pinject_design-0.1.88/pinject_design/di/implicit_globals.py
--rw-r--r--   0        0        0    29340 2023-07-11 07:44:55.289012 pinject_design-0.1.88/pinject_design/di/injected.py
--rw-r--r--   0        0        0     1285 2023-05-06 04:00:43.966962 pinject_design-0.1.88/pinject_design/di/injected_analysis.py
--rw-r--r--   0        0        0        0 2023-05-23 16:15:25.508899 pinject_design-0.1.88/pinject_design/di/permissioned/__init__.py
--rw-r--r--   0        0        0     7815 2023-05-24 05:53:54.289323 pinject_design-0.1.88/pinject_design/di/permissioned/blueprint.py
--rw-r--r--   0        0        0      147 2023-07-02 07:30:07.430121 pinject_design-0.1.88/pinject_design/di/playground.py
--rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinject_design-0.1.88/pinject_design/di/provider.py
--rw-r--r--   0        0        0     2113 2023-05-24 09:33:43.951004 pinject_design-0.1.88/pinject_design/di/proxiable.py
--rw-r--r--   0        0        0     3208 2023-05-04 14:37:38.150578 pinject_design-0.1.88/pinject_design/di/session.py
--rw-r--r--   0        0        0     2069 2022-10-12 04:28:37.000000 pinject_design-0.1.88/pinject_design/di/sessioned.py
--rw-r--r--   0        0        0     5730 2023-05-08 04:41:16.885893 pinject_design-0.1.88/pinject_design/di/static_proxy.py
--rw-r--r--   0        0        0      151 2022-10-12 04:42:16.000000 pinject_design-0.1.88/pinject_design/di/test_ast.py
--rw-r--r--   0        0        0      995 2022-10-08 11:27:55.000000 pinject_design-0.1.88/pinject_design/di/test_dynamic_proxy.py
--rw-r--r--   0        0        0     1505 2022-10-09 04:19:51.000000 pinject_design-0.1.88/pinject_design/di/test_graph.py
--rw-r--r--   0        0        0     2249 2023-04-19 08:08:57.197957 pinject_design-0.1.88/pinject_design/di/test_injected.py
--rw-r--r--   0        0        0      705 2022-10-12 04:28:37.000000 pinject_design-0.1.88/pinject_design/di/test_proxiable.py
--rw-r--r--   0        0        0    28581 2023-07-11 04:43:03.271241 pinject_design-0.1.88/pinject_design/di/util.py
--rw-r--r--   0        0        0     1011 2023-06-08 08:03:44.708591 pinject_design-0.1.88/pinject_design/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-08 06:25:57.424869 pinject_design-0.1.88/pinject_design/global_configs
--rw-r--r--   0        0        0       35 2023-05-08 06:26:47.054220 pinject_design-0.1.88/pinject_design/global_configs.py
--rw-r--r--   0        0        0     1316 2023-06-15 09:48:02.404293 pinject_design-0.1.88/pinject_design/graph_inspection.py
--rw-r--r--   0        0        0     2285 2023-07-11 08:45:24.185649 pinject_design-0.1.88/pinject_design/module_inspector.py
--rw-r--r--   0        0        0     1747 2023-07-04 04:35:00.683470 pinject_design-0.1.88/pinject_design/nx_graph_util.py
--rw-r--r--   0        0        0      467 2023-05-29 00:14:18.924421 pinject_design-0.1.88/pinject_design/pinject_design.iml
--rw-r--r--   0        0        0    29360 2023-07-11 09:12:45.323975 pinject_design-0.1.88/pinject_design/run_config_utils.py
--rw-r--r--   0        0        0      938 2023-07-11 04:43:03.272810 pinject_design-0.1.88/pinject_design/test_package/__init__.py
--rw-r--r--   0        0        0      234 2023-07-11 04:43:03.273171 pinject_design-0.1.88/pinject_design/test_package/child/__init__.py
--rw-r--r--   0        0        0      284 2023-07-11 08:16:07.010761 pinject_design-0.1.88/pinject_design/test_package/child/module1.py
--rw-r--r--   0        0        0    19787 2023-07-05 04:39:53.268769 pinject_design-0.1.88/pinject_design/visualize_di.py
--rw-r--r--   0        0        0        0 2022-04-27 03:40:35.000000 pinject_design-0.1.88/pinject_design/viz/__init__.py
--rw-r--r--   0        0        0       78 2022-04-27 03:51:47.000000 pinject_design-0.1.88/pinject_design/viz/graph.py
--rw-r--r--   0        0        0      639 2023-07-11 09:12:47.931889 pinject_design-0.1.88/pyproject.toml
--rw-r--r--   0        0        0      743 1970-01-01 00:00:00.000000 pinject_design-0.1.88/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-03-23 09:24:51.954701 pinject-design-0.1.9/LICENSE
+-rw-r--r--   0        0        0        0 2022-01-27 17:14:04.355211 pinject-design-0.1.9/pinject_design/__init__.py
+-rw-r--r--   0        0        0        0 2021-03-31 10:36:27.000000 pinject-design-0.1.9/pinject_design/di/__init__.py
+-rw-r--r--   0        0        0     7144 2022-04-27 08:04:25.209057 pinject-design-0.1.9/pinject_design/di/design.py
+-rw-r--r--   0        0        0     2155 2022-01-27 18:10:42.819773 pinject-design-0.1.9/pinject_design/di/graph.py
+-rw-r--r--   0        0        0    13823 2022-04-30 05:26:53.150771 pinject-design-0.1.9/pinject_design/di/injected.py
+-rw-r--r--   0        0        0      416 2021-07-14 13:45:34.000000 pinject-design-0.1.9/pinject_design/di/provider.py
+-rw-r--r--   0        0        0    23372 2022-04-27 10:14:06.845469 pinject-design-0.1.9/pinject_design/di/util.py
+-rw-r--r--   0        0        0        0 2022-04-27 03:40:35.011226 pinject-design-0.1.9/pinject_design/viz/__init__.py
+-rw-r--r--   0        0        0       78 2022-04-27 03:51:47.513177 pinject-design-0.1.9/pinject_design/viz/graph.py
+-rw-r--r--   0        0        0      463 2022-05-01 19:21:00.339822 pinject-design-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      755 2022-05-01 19:21:10.151308 pinject-design-0.1.9/setup.py
+-rw-r--r--   0        0        0      703 2022-05-01 19:21:10.151485 pinject-design-0.1.9/PKG-INFO
```

### Comparing `pinject_design-0.1.88/LICENSE` & `pinject-design-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pinject_design-0.1.88/pinject_design/di/design.py` & `pinject-design-0.1.9/pinject_design/di/design.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import abc
 import inspect
 from dataclasses import dataclass
 from functools import wraps
 from typing import TypeVar, Generic, Callable, Union, Dict, List
 
 from frozendict import frozendict
-
+from loguru import logger
 from makefun import create_function
 
 from pinject_design.di.injected import Injected, extract_dependency_including_self, extract_dependency
 
 T = TypeVar("T")
 U = TypeVar("U")
 
@@ -21,23 +21,22 @@
     def __hash__(self):
         return hash(frozendict(**self.kwargs))
 
 
 @dataclass
 class PinjectProvider:
     method: Callable  # a callable with (self,dep1,dep2) signatures...
-
     # might be annotated with pinject's annotations..
     # pinject ads an attribute to an annotated function for marking..
     # which is not something I prefer though...
     # ok I should stop using pinject's features
 
     def __post_init__(self):
         # if self is not in method signature, this will add it.
-        assert self.method is not None, "PinjectProvider created with method==None!"
+        assert self.method is not None,"PinjectProvider created with method==None!"
         if callable(self.method):
             self.method = ensure_self_arg(self.method)
             # we need to make sure the function's name starts with provide_
         else:
             # may this class is used for pampy pattern matching..
             pass
 
@@ -104,33 +103,33 @@
         return PinjectProvider(mapped)
 
 
 def remove_kwargs_from_func(f, kwargs: List[str]):
     deps = extract_dependency_including_self(f)
     to_remove = set(kwargs)
     new_kwargs = deps - to_remove
-    func_name = f.__name__.replace("<lambda>", "_lambda_")
+    func_name = f.__name__.replace("<lambda>","_lambda_")
     sig = f"""{func_name}({",".join(new_kwargs)})"""
 
     def impl(**called_kwargs):
         deleted = deps & to_remove
         # for self, you must check whether f is method or not
         if inspect.ismethod(f):
             deleted = deleted - {"self"}
         d_kwargs = {k: None for k in deleted}
         return f(**called_kwargs, **d_kwargs)
 
     return create_function(sig, impl)
 
 
 def bind_to_injected(bind: Bind):
-    if isinstance(bind, PinjectBind) and "to_class" in bind.kwargs:
+    if isinstance(bind,PinjectBind) and "to_class" in bind.kwargs:
         cls = bind.kwargs["to_class"]
         return Injected.bind(cls)
-    elif isinstance(bind, InjectedProvider):
+    elif isinstance(bind,InjectedProvider):
         return bind.src
     pb = bind.to_pinject_binding()
     provider = pinject_to_provider(pb)
     provider = remove_kwargs_from_func(provider, ["self"])
     return Injected.bind(provider)
 
 
@@ -145,19 +144,19 @@
     @property
     @abc.abstractmethod
     def provider(self):
         pass
 
     def to_pinject_binding(self) -> Union["PinjectConfigure", "PinjectProvider"]:
         provider = self.provider
-        assert provider is not None, "provider is None for some reason!"
+        assert provider is not None,"provider is None for some reason!"
         return PinjectProvider(provider)
 
 
-@dataclass
+@dataclass(frozen=True)
 class InjectedProvider(ProviderTrait[T]):
     src: Injected[T]
 
     @property
     def provider(self):
         return self.src.get_provider()
 
@@ -203,15 +202,14 @@
             lines, ln = inspect.getsourcelines(func)
             fn = func.__name__.replace("<", "").replace(">", "")
             fname = f"""{module.__name__.replace(".", "_")}_ln_{ln}_{fn}"""
         except OSError as ose:
             fn = func.__name__.replace("<", "").replace(">", "")
             fname = f"""{module.__name__.replace(".", "_")}_{fn}"""
         except AttributeError as ae:
-            from loguru import logger
             logger.warning(f"could not set reasonable func name. better provide fname as argument!")
             fname = f"""unknwon_module_function"""
 
     assert not isinstance(argspec.args, str)
     signature = f"""{fname}({" ,".join(["self"] + (argspec.args or []))})"""
 
     # logger.error(source)
@@ -228,14 +226,7 @@
     kwargs: Dict
 
     def __hash__(self):
         return hash(frozendict(**self.kwargs))
 
     def to_pinject_binding(self) -> Union[PinjectConfigure, PinjectProvider]:
         return PinjectConfigure(self.kwargs)
-
-@dataclass
-class MetaBind(Bind):
-    src:Bind
-    metadata:dict
-    def to_pinject_binding(self) -> Union[PinjectConfigure, PinjectProvider]:
-        return self.src.to_pinject_binding()
```

### Comparing `pinject_design-0.1.88/pinject_design/di/util.py` & `pinject-design-0.1.9/pinject_design/di/util.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,99 +1,50 @@
 import abc
 import inspect
 from copy import copy
 from dataclasses import dataclass, field, replace
 from functools import wraps
 from itertools import chain
-from pprint import pformat
+from pickle import PicklingError
 from typing import Union, Type, TypeVar, Callable, Dict, Any
 
-import cloudpickle
 import pinject
-from cytoolz import merge
+import cloudpickle
+from cytoolz import merge, valmap
+from expression import Some, Nothing
+from expression.collections import Map
+from loguru import logger
 from makefun import create_function, wraps
 from pampy import match
 from pinject import BindingSpec
-from pinject.scoping import SingletonScope, BindableScopes, SINGLETON
-from returns.result import safe, Failure, Success
+from pinject.scoping import SingletonScope
+from returns.result import safe, Failure
+from tabulate import tabulate
 
 from pinject_design.di.design import Bind, FunctionProvider, ProviderTrait, InjectedProvider, PinjectConfigure, \
     PinjectProvider, ensure_self_arg, PinjectBind
-from pinject_design.di.graph import ExtendedObjectGraph, MyObjectGraph, IObjectGraph
+from pinject_design.di.graph import ExtendedObjectGraph
 from pinject_design.di.injected import Injected
-from pinject_design.di.proxiable import DelegatedVar
-from pinject_design.di.session import SessionScope
 
 prototype = pinject.provides(in_scope=pinject.PROTOTYPE)
 # is it possible to create a binding class which also has an ability to dynamically add..?
 # yes. actually.
 T = TypeVar("T")
 
 
-def rec_valmap(f, tgt: dict):
-    res = dict()
-    for k, v in tgt.items():
-        if isinstance(v, dict):
-            res[k] = rec_valmap(f, v)
-        else:
-            res[k] = f(v)
-    return res
-
-
-def rec_val_filter(f, tgt: dict):
-    res = dict()
-    for k, v in tgt.items():
-        if isinstance(v, dict):
-            res[k] = rec_val_filter(f, v)
-        elif f(v):
-            res[k] = v
-    return res
-
-class ErrorWithTrace(BaseException):
-    def __init__(self,src: BaseException, trace: str):
-        super().__init__()
-        self.src = src
-        self.trace = trace
-    def __reduce__(self):
-        return (ErrorWithTrace, (self.src, self.trace))
-
-    def __str__(self):
-        return f"{self.src}\n {self.trace}"
-
-def my_safe(f):
-    def impl(*args, **kwargs):
-        try:
-            return Success(f(*args, **kwargs))
-        except Exception as e:
-            import traceback
-            trace = "\n".join(traceback.format_exception(e))
-
-            return Failure(ErrorWithTrace(
-                e,
-                trace
-            ))
-    return impl
-
 def check_picklable(tgt: dict):
-    cloud_dumps_try = my_safe(cloudpickle.dumps)
-    cloud_loads_try = my_safe(cloudpickle.loads)
-    res = cloud_dumps_try(tgt).bind(cloud_loads_try)
-
-    if isinstance(res, Failure):
-        # target_check = valmap(cloud_dumps_try, tgt)
-        rec_check = rec_valmap(lambda v: (cloud_dumps_try(v), v), tgt)
-        failures = rec_val_filter(lambda v: isinstance(v[0], Failure), rec_check)
-        # failures = [(k, v, tgt[k]) for k, v in target_check.items() if isinstance(v, Failure)]
-
-        from loguru import logger
-        logger.error(f"Failed to pickle target: {pformat(failures)}")
+    cloud_dumps_try = safe(cloudpickle.dumps)
+    res = cloud_dumps_try(tgt)
+    if isinstance(res,Failure):
+        target_check = Map.of(**valmap(cloud_dumps_try, tgt))
+        logger.error(
+            "failed pickling:\n" + tabulate(target_check.filter(lambda k, v: isinstance(v, Failure)).to_list()))
         logger.error(f"if the error message contains EncodedFile pickling error, "
                      f"check whether the logging module is included in the target object or not.")
-        raise RuntimeError("this object is not picklable. check the error messages above.") from res.failure()
-    # logger.info(res)
+        raise RuntimeError("this object is not picklable. check the error messages above.")
 
 
 def inject_proto(all_except=None, arg_names=None):
     """injects provider with prototype context"""
 
     def _inner(f):
         return pinject.inject(all_except=all_except, arg_names=arg_names)(prototype(f))
@@ -131,15 +82,14 @@
 
 class DesignBindContext:
     def __init__(self, src: "Design", key: str):
         self.src = src
         self.key = key
 
     def to_class(self, cls: type, **kwargs):
-        assert isinstance(cls, type), f"binding must be a class! got:{cls} for key:{self.src}"
         return self.src.bind_imm(self.key, to_class=cls, **kwargs)
 
     def to_instance(self, instance, **kwargs):
         return self.src.bind_imm(self.key, to_instance=instance, **kwargs)
 
     def to_provider(self, provider, all_except=None, arg_names=None, in_scope=None):
         return self.src.bind_provider_imm(self.key, provider, all_except=all_except, arg_names=arg_names,
@@ -155,15 +105,18 @@
     args = inspect.getfullargspec(f).args
     if isinstance(f, type) and "self" in args:
         args.remove("self")
     return args
 
 
 def getitem_opt(o, k):
-    return safe(o.__getitem__)(k)
+    if k in o:
+        return Some(o[k])
+    else:
+        return Nothing
 
 
 def to_readable_name(o):
     from pampy import match, _
     return match(o,
                  DirectPinjectProvider(_), lambda method: method.__name__,
                  PinjectProviderBind, lambda ppb: (ppb.f.__name__),
@@ -189,16 +142,16 @@
     # all_keys.remove("base_train_transform_design")
     # all_keys.remove("base_test_transform_design")
     all_keys.remove("design")
     data = []
     Subject = try_import_subject()
     for k in all_keys:
 
-        ak = getitem_opt(a, k).map(to_readable_name).value_or(None)
-        bk = getitem_opt(b, k).map(to_readable_name).value_or(None)
+        ak = getitem_opt(a, k).map(to_readable_name).or_else(Some(None)).value
+        bk = getitem_opt(b, k).map(to_readable_name).or_else(Some(None)).value
         flag = match((ak, bk),
                      (Subject, Subject), lambda a, b: True,
                      # (np.ndarray, np.ndarray), lambda a, b: (a != b).any(),
                      # (np.ndarray, Any),lambda a,b:False,
                      # (Any,np.ndarray),lambda a,b:False,
                      (Any, Any), lambda a, b: a != b
                      )
@@ -226,16 +179,15 @@
     def __getstate__(self):
         res = dict(
             bindings=self.bindings,
             multi_binds=self.multi_binds,
             modules=[m.__name__ for m in self.modules],
             classes=self.classes,
         )
-        # ah, so this pickling checker is a bit of a problem
-        # check_picklable(self.bindings)
+        check_picklable(self.bindings)
         return res
 
     def __setstate__(self, state):
         mods = state["modules"]
         import importlib
         mods = [importlib.import_module(
             name=m
@@ -248,31 +200,26 @@
         other = self._ensure_dbc(other)
         return self.merged(other)
 
     def bind(self, key: str) -> DesignBindContext:
         return DesignBindContext(self, key)
 
     def _ensure_dbc(self, other: Union["Design", BindingSpec, Dict[str, Bind]]):
-        match other:
-            case BindingSpec():
-                return Design.gather_spec(other)
-            case Design():
-                return other
-            case dict() if all([isinstance(v, Bind) for v in other.values()]):
-                return Design(other)
-            case _:
-                raise ValueError(f"cannot add {type(other)} to Design")
+        return match(other,
+                     BindingSpec, lambda o: Design.gather_spec(o),
+                     Design, lambda d: d,
+                     Dict[str, Bind], lambda d: Design(d)
+                     )
 
     def _merge_multi_binds(self, src, dst):
-        # src = Map.of(**src)
-        # dst = Map.of(**dst)
+        src = Map.of(**src)
+        dst = Map.of(**dst)
         keys = src.keys() | dst.keys()
         multi = {k: (
-                getitem_opt(src, k).value_or([]) +
-                getitem_opt(dst, k).value_or([])
+                    src.try_find(k).default_value([]) + dst.try_find(k).default_value([])
         ) for k in keys}
         return multi
 
     def merged(self, other: "Design"):
         """creates another instance with merged bindings. does not modify self"""
         # logger.debug(f"merging:\n\t{self} to \n\t{other}")
         assert isinstance(other, Design), f"merge target is not a Design. type:{type(other)}:{other}"
@@ -284,21 +231,18 @@
             classes=list(set(self.classes) | set(other.classes)),
         )
         return res
 
     def bind_provider_imm(self, key, f, all_except=None, arg_names=None, in_scope=None):
         def raise_unhandled(any):
             raise RuntimeError(f"unknown input type for bind_provider_imm! key:{key}, provider:{f}")
-
         bind = match(f,
                      Injected, lambda i: Design({key: InjectedProvider(i)}),
                      ProviderTrait, lambda pt: Design({key: pt}),
-                     DelegatedVar, lambda dv: Design({key: InjectedProvider(dv.eval())}),
-                     callable, lambda c: Design(
-                {key: PinjectProviderBind(f, all_except=all_except, arg_names=arg_names, in_scope=in_scope)}),
+                     callable, lambda c: Design({key: PinjectProviderBind(f, all_except=all_except, arg_names=arg_names, in_scope=in_scope)}),
                      Any, raise_unhandled
                      )
         res = self + bind
         return res
 
     def bind_imm(self, key, **kwargs):
         from pampy import _
@@ -306,88 +250,58 @@
                             {"to_class": Injected}, lambda injected: Design(bindings={key: InjectedProvider(injected)}),
                             _, Design(bindings={key: PinjectBind(kwargs)})
                             )
 
     def bind_instance(self, **kwargs):
         x = self
         for k, v in kwargs.items():
-            if isinstance(v, type):
-                from loguru import logger
+            if isinstance(v,type):
                 logger.warning(f"{k} is bound to class {v} with 'bind_instance' do you mean 'bind_class'?")
             x = x.bind(k).to_instance(v)
         return x
 
-    def bind_provider(self, **kwargs: Union[Callable, Injected]):
-        from loguru import logger
+    def bind_provider(self, **kwargs):
         x = self
         for k, v in kwargs.items():
             # logger.info(f"binding provider:{k}=>{v}")
-            def parse(item):
-                match item:
-                    case type():
-                        logger.warning(f"{k}->{v}: class is used for bind_provider. fixing automatically.")
-                        return x.bind(k).to_class(item)
-                    case Injected():
-                        return x.bind(k).to_provider(item)
-                    case DelegatedVar():
-                        return parse(item.eval())
-                    case non_func if not callable(non_func):
-                        logger.warning(
-                            f"{k}->{item}: non-callable or non-injected is passed to bind_provider. fixing automatically.")
-                        return x.bind(k).to_instance(v)
-                    case _:
-                        return x.bind(k).to_provider(item)
-
-            x = parse(v)
+            if isinstance(v,type):
+                logger.warning(f"{k}->{v}: class is used for bind_provider. fixing automatically.")
+                x = x.bind(k).to_class(v)
+            else:
+                x = x.bind(k).to_provider(v)
         return x
 
     def bind_class(self, **kwargs):
-        from loguru import logger
         x = self
         for k, v in kwargs.items():
-            if isinstance(v, Injected):
-                logger.warning(f"{k}->{v}: Injected instance is used for bind_class. fixing automatically.")
-                x = x.bind(k).to_provider(v)
-            else:
-                x = x.bind(k).to_class(v)
+            x = x.bind(k).to_class(v)
         return x
 
-    def to_graph(self, modules=None, classes=None) -> IObjectGraph:
-        #So MyObjectGraph's session is still corrupt?
-        design = self + Design(
-            modules=modules or [],
-            classes=classes or []
-        )
-        return MyObjectGraph.root(design)
-
-    def _old_to_graph(self,modules=None, classes=None) -> IObjectGraph:
-        from loguru import logger
+    def to_graph(self, modules=None, classes=None) -> ExtendedObjectGraph:
         modules = self.modules + (modules or [])
         classes = self.classes + (classes or [])
-        logger.info(f"to_graph:\n\t{pformat(modules)}\n\t{pformat(classes)}")
-        g = pinject.new_object_graph(
-            modules=modules,
-            binding_specs=[self.to_binding_spec()],
-            classes=classes
-        )
-        g._obj_provider._bindable_scopes = BindableScopes(
-            id_to_scope={SINGLETON: SessionScope()}
-        )
-        return ExtendedObjectGraph(self, g)
+        # logger.info(f"to_graph:\n\t{pformat(modules)}\n\t{pformat(classes)}")
+        return ExtendedObjectGraph(
+            self,
+            pinject.new_object_graph(
+                modules=modules,
+                binding_specs=[self.to_binding_spec()],
+                classes=classes
+            ))
 
     def run(self, f, modules=None, classes=None):
         return self.to_graph(modules, classes).run(f)
 
     def provide(self, target: Union[str, Type[T]], modules=None, classes=None) -> T:
         """
         :param target: provided name
         :param modules: modules to use for graph construction
         :return:
         """
-        return self.to_graph(modules=modules, classes=classes).provide(target,level=4)
+        return self.to_graph(modules=modules, classes=classes).provide(target)
 
     @staticmethod
     def gather_spec(b: BindingSpec) -> "Design":
         assert isinstance(b, BindingSpec)
         dep_spec = Design()
         for dep in b.dependencies() or []:
             spec = Design.gather_spec(dep)
@@ -470,63 +384,54 @@
     def __contains__(self, item):
         return item in self.bindings
 
     def __getitem__(self, item):
         return self.bindings[item]
 
     def __str__(self):
-        return f"Design(len={len(self.bindings) + len(self.multi_binds)})"
-
-    def __repr__(self):
-        return str(self)
-
-    def table_str(self):
         import tabulate
         binds = tabulate.tabulate(sorted(list(self.bindings.items())))
         multis = tabulate.tabulate(sorted(list(self.multi_binds.items())))
         return binds + "\n" + multis
 
+    def __repr__(self):
+        return str(self)
+
     def to_str_dict(self):
         res = dict()
         from pampy import _
         for k, v in self.bindings.items():
             res[k] = match(v,
                            FunctionProvider, lambda fp: fp.f.__name__,
                            InjectedProvider, lambda i: str(i),
                            PinjectBind({'to_class': _}), lambda cls: str(cls),
                            PinjectBind({'to_instance': _}), lambda ins: str(ins),
                            _, lambda any: str(any)
                            )
         return res
 
     def build(self):
-        design = self
+        design= self
         for k, providers in self.multi_binds.items():
             # assert k not in self.bindings,f"multi binding key overwrapping with normal binding key,{k}"
             if len(providers) == 0:
                 design = design.bind_instance(**{k: set()})
             else:
                 design = self._add_multi_binding(design, k, providers)
         return design
 
     def to_binding_spec(self):
         """Generate a BindingSpec class for pinject and returns its instance."""
 
         design = self.build()
-        bindings = {k: v.to_pinject_binding() for k, v in design.bindings.items()}
-        configures = {k: v for k, v in bindings.items() if isinstance(v, PinjectConfigure)}
-        # configures = bindings.filter(lambda k, v: isinstance(v, PinjectConfigure))
-        providers = {k: v for k, v in bindings.items() if isinstance(v, PinjectProvider)}
-        providers = {k: self._ensure_provider_name(k, v.method) for k, v in providers.items()}
-
-        # providers = itemmap(lambda t: self._ensure_provider_name(t[0], t[1].method), providers)
-
-        # providers = bindings.filter(lambda k, v: isinstance(v, PinjectProvider)).map(
-        #     lambda k, v: self._ensure_provider_name(k, v.method)
-        # )
+        bindings = Map.of(**design.bindings).map(lambda k, v: v.to_pinject_binding())
+        configures = bindings.filter(lambda k, v: isinstance(v, PinjectConfigure))
+        providers = bindings.filter(lambda k, v: isinstance(v, PinjectProvider)).map(
+            lambda k, v: self._ensure_provider_name(k, v.method)
+        )
 
         def configure(self, bind):
             for c, v in dict(configures).items():
                 # logger.info(f"bind :{v.kwargs}")
                 bind(c, **v.kwargs)
 
         DynamicBinding = type("DynamicBinding", (BindingSpec,),
@@ -535,15 +440,14 @@
                                   **{f"provide_{k}": v for k, v in providers.items()},
                               })
 
         return DynamicBinding()
 
     def _ensure_provider_name(self, k, method):
         """set appropriate name for provider function to be recognized by pinject"""
-        from loguru import logger
         name = f"provide_{k}"
         if not method.__name__ == name:
             # there are cases where you cannot directly set __name__ attribute.
             # and sometimes pinject.inject decorator is already applied so wrapping that again is not appropriate
             # so, the solution is to first try setting __name__ and then try wrapping if failed.
             try:
                 method.__name__ = name
@@ -575,85 +479,63 @@
         """:key returns a new design which returns a [] for "key" as default value. """
         # None works as a signal to remove
         return self + Design(
             multi_binds={
                 k: [None] for k in keys
             }
         )
-
-    def _acc_multi_provider(self, providers):
+    def _acc_multi_provider(self,providers):
+        if providers:
+            logger.info("--------")
+            logger.info(providers)
         res = []
         for p in providers:
-            if p is None:  # this is set by empty_multi_provider call
+            if p is None:# this is set by empty_multi_provider call
                 res = []
             else:
                 res.append(p)
+        if providers:
+            logger.info(res)
+            logger.info("--------")
         return res
 
-    def _add_multi_binding(self, design, k, providers: list):
-        # TODO use Injected's mzip.
+    def _add_multi_binding(self, design, k, providers:list):
         providers = self._acc_multi_provider(providers)
-        deps = [f.dependencies() if isinstance(f, Injected) else get_class_aware_args(f) for f in providers]
+        deps = [get_class_aware_args(f) for f in providers]
         dep_set = set(chain(*deps))
         if "self" in dep_set:
             dep_set.remove("self")
         f_signature = f"multi_bind_provider_{k}({','.join(dep_set)})"
-        # logger.info(f_signature)
+        logger.info(f_signature)
         for ds in deps:
             for d in ds:
                 assert d in dep_set
 
         def create_impl(tgt_providers, tgt_dependencies):
             def f_impl(**kwargs):
-                # from loguru import logger
-
-                # logger.info(f"{f_signature} called with {list(kwargs.keys())}")
+                logger.info(f"{f_signature} called with {list(kwargs.keys())}")
                 values = []
                 for provider, ds in zip(tgt_providers, tgt_dependencies):
                     p_deps = {k: kwargs[k] for k in ds}
                     v = provider(**p_deps)
                     values.append(v)  # unhashable type...
                 return values
 
             return f_impl
 
         new_f = create_function(f_signature, create_impl(providers, deps))
         binding = {k: new_f}
-        # logger.info(binding)
+        logger.info(binding)
         design = design.bind_provider(**binding)
         return design
 
     def diff(self, other):
         d = get_dict_diff(self.bindings, other.bindings)
         return d
 
-    def inspect_picklability(self):
-        from loguru import logger
-        logger.info(f"checking picklability of bindings")
-        check_picklable(self.bindings)
-        logger.info(f"checking picklability of multi-binds")
-        check_picklable(self.multi_binds)
-        logger.info(f"checking picklability of modules")
-        check_picklable(self.modules)
-        logger.info(f"checking picklability of classes")
-        check_picklable(self.classes)
-
-    def add_modules(self, *modules):
-        return self + Design(modules=list(modules))
-
-    def add_classes(self, *classes):
-        return self + Design(classes=list(classes))
-
-    def to_vis_graph(self):
-        from pinject_design.visualize_di import DIGraph
-        return DIGraph(self)
-
-
-EmptyDesign = Design()
-
 
 @dataclass
 class DirectPinjectProvider(Bind):
     method: Callable
 
     def to_pinject_binding(self) -> Union[PinjectConfigure, PinjectProvider]:
         return PinjectProvider(self.method)
@@ -691,15 +573,14 @@
         if binding_key not in d:
             val = default_provider_fn()
             d[binding_key] = val
         return d[binding_key]
 
 
 def patch_pinject_singleton_scope():
-    from loguru import logger
     logger.warning(f"patching pinject's SingletonScope to produce better exception")
     SingletonScope.provide = _patched_provide
     logger.warning(f"patching done")
 
 
 patch_pinject_singleton_scope()
 
@@ -717,15 +598,14 @@
     if res is None:
         return "unknown_module"
     return res.__name__
 
 
 def patch_pinject_get_external_type_name():
     import pinject.locations
-    from loguru import logger
     logger.warning(f"patching pinject's _get_external_type_name to accept pickled function")
     pinject.locations._get_external_type_name = _get_external_type_name
 
 
 patch_pinject_get_external_type_name()
 
 
@@ -735,24 +615,22 @@
     """use this to keep things picklable"""
     f: Callable
     all_except: Any
     arg_names: Any
     in_scope: Any
 
     def __post_init__(self):
-        assert self.f is not None, "PinjectProviderBind cannot have None as f."
         if self.f.__name__ == "<lambda>":
             self.f.__name__ = "_lambda_"
         self._fname = self.f.__name__
         assert self._fname is not None, f"provided function has no name.:{self.f}"
         self._signature = inspect.signature(self.f)
 
     def provider_for_binding_spec(self):
         # so first you need to convert a method in to function
-        assert self.f is not None
         f = self.f
         if "__name__" not in dir(f):
             f = method_to_function(f)
         # now ensure the function has self arg
         f = ensure_self_arg(f, fname=self._fname)
 
         @wraps(f)  # called 78 times
@@ -781,27 +659,7 @@
             _fname=self._fname,
             _signature=self._signature
         )
 
     def __setstate__(self, state):
         for k, v in state.items():
             setattr(self, k, v)
-        assert self.f is not None
-
-
-def instances(**kwargs):
-    for k,v in kwargs.items():
-        assert not isinstance(v, DelegatedVar), f"passing delegated var with Injected context is forbidden, to prevent human error."
-        assert not isinstance(v, Injected), f"passing Injected to 'instances' is forbidden, to prevent human error. use bind_instance instead."
-    return Design().bind_instance(**kwargs)
-
-
-def providers(**kwargs):
-    return Design().bind_provider(**kwargs)
-
-
-def classes(**kwargs):
-    return Design().bind_class(**kwargs)
-
-
-def injecteds(**kwargs):
-    return Design().bind_provider(**kwargs)
```

### Comparing `pinject_design-0.1.88/PKG-INFO` & `pinject-design-0.1.9/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,23 @@
 Metadata-Version: 2.1
 Name: pinject-design
-Version: 0.1.88
+Version: 0.1.9
 Summary: immutable wrapper for pinject
 License: MIT
 Author: proboscis
 Author-email: nameissoap@gmail.com
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: cloudpickle
 Requires-Dist: cytoolz
 Requires-Dist: expression
-Requires-Dist: fire
-Requires-Dist: frozendict
 Requires-Dist: loguru
 Requires-Dist: makefun
-Requires-Dist: networkx
 Requires-Dist: pampy
 Requires-Dist: pinject
-Requires-Dist: pydantic
-Requires-Dist: pyvis
-Requires-Dist: pyyaml
 Requires-Dist: returns
 Requires-Dist: tabulate
```

