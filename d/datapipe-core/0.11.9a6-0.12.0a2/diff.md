# Comparing `tmp/datapipe_core-0.11.9a6.tar.gz` & `tmp/datapipe_core-0.12.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapipe_core-0.11.9a6.tar", max compression
+gzip compressed data, was "datapipe_core-0.12.0a2.tar", max compression
```

## Comparing `datapipe_core-0.11.9a6.tar` & `datapipe_core-0.12.0a2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
--rw-r--r--   0        0        0     1514 2022-10-22 17:08:42.777947 datapipe_core-0.11.9a6/LICENSE
--rw-r--r--   0        0        0        0 2022-10-22 17:08:42.777947 datapipe_core-0.11.9a6/datapipe/__init__.py
--rw-r--r--   0        0        0    10924 2022-11-18 13:05:23.822285 datapipe_core-0.11.9a6/datapipe/compute.py
--rw-r--r--   0        0        0    14198 2022-11-18 13:05:23.822285 datapipe_core-0.11.9a6/datapipe/core_steps.py
--rw-r--r--   0        0        0    13380 2022-11-18 13:05:23.822285 datapipe_core-0.11.9a6/datapipe/datatable.py
--rw-r--r--   0        0        0     3549 2022-10-22 17:08:42.777947 datapipe_core-0.11.9a6/datapipe/event_logger.py
--rw-r--r--   0        0        0    16808 2022-11-18 13:05:23.822285 datapipe_core-0.11.9a6/datapipe/metastore.py
--rw-r--r--   0        0        0      969 2022-10-22 17:08:42.777947 datapipe_core-0.11.9a6/datapipe/run_config.py
--rw-r--r--   0        0        0        0 2022-10-22 17:08:42.777947 datapipe_core-0.11.9a6/datapipe/store/__init__.py
--rw-r--r--   0        0        0     7804 2022-10-30 21:46:50.060594 datapipe_core-0.11.9a6/datapipe/store/database.py
--rw-r--r--   0        0        0    17107 2022-11-18 13:05:23.822285 datapipe_core-0.11.9a6/datapipe/store/filedir.py
--rw-r--r--   0        0        0     3631 2022-10-22 17:08:42.777947 datapipe_core-0.11.9a6/datapipe/store/milvus.py
--rw-r--r--   0        0        0     1337 2022-10-22 17:08:42.777947 datapipe_core-0.11.9a6/datapipe/store/pandas.py
--rw-r--r--   0        0        0     3518 2022-10-22 17:08:42.777947 datapipe_core-0.11.9a6/datapipe/store/redis.py
--rw-r--r--   0        0        0     3742 2022-10-22 17:11:48.441249 datapipe_core-0.11.9a6/datapipe/store/table_store.py
--rw-r--r--   0        0        0     2853 2022-10-22 17:11:48.441249 datapipe_core-0.11.9a6/datapipe/types.py
--rw-r--r--   0        0        0     1233 2022-11-18 14:16:56.729673 datapipe_core-0.11.9a6/pyproject.toml
--rw-r--r--   0        0        0     1231 1970-01-01 00:00:00.000000 datapipe_core-0.11.9a6/setup.py
--rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 datapipe_core-0.11.9a6/PKG-INFO
+-rw-r--r--   0        0        0     1514 2022-12-26 14:30:45.008686 datapipe_core-0.12.0a2/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-29 09:25:17.932322 datapipe_core-0.12.0a2/datapipe/__init__.py
+-rw-r--r--   0        0        0    13255 2023-07-10 21:00:32.210382 datapipe_core-0.12.0a2/datapipe/cli.py
+-rw-r--r--   0        0        0    13446 2023-07-10 20:51:13.239026 datapipe_core-0.12.0a2/datapipe/compute.py
+-rw-r--r--   0        0        0    15105 2023-07-10 21:09:16.890168 datapipe_core-0.12.0a2/datapipe/core_steps.py
+-rw-r--r--   0        0        0    13484 2023-07-10 20:51:13.239026 datapipe_core-0.12.0a2/datapipe/datatable.py
+-rw-r--r--   0        0        0     4540 2023-07-10 20:51:13.239026 datapipe_core-0.12.0a2/datapipe/event_logger.py
+-rw-r--r--   0        0        0     4197 2023-07-10 20:51:13.239026 datapipe_core-0.12.0a2/datapipe/lints.py
+-rw-r--r--   0        0        0    17490 2023-07-10 20:51:13.239026 datapipe_core-0.12.0a2/datapipe/metastore.py
+-rw-r--r--   0        0        0      969 2023-07-10 20:51:13.239026 datapipe_core-0.12.0a2/datapipe/run_config.py
+-rw-r--r--   0        0        0        0 2022-12-26 14:30:45.008686 datapipe_core-0.12.0a2/datapipe/store/__init__.py
+-rw-r--r--   0        0        0     7854 2023-07-10 20:51:13.239026 datapipe_core-0.12.0a2/datapipe/store/database.py
+-rw-r--r--   0        0        0    16835 2023-07-10 20:51:13.239026 datapipe_core-0.12.0a2/datapipe/store/filedir.py
+-rw-r--r--   0        0        0     3595 2023-07-10 20:51:13.239026 datapipe_core-0.12.0a2/datapipe/store/milvus.py
+-rw-r--r--   0        0        0     1337 2023-07-10 20:51:13.239026 datapipe_core-0.12.0a2/datapipe/store/pandas.py
+-rw-r--r--   0        0        0     8570 2023-07-10 21:04:41.709164 datapipe_core-0.12.0a2/datapipe/store/qdrant.py
+-rw-r--r--   0        0        0     3210 2023-07-10 20:51:13.239026 datapipe_core-0.12.0a2/datapipe/store/redis.py
+-rw-r--r--   0        0        0     3877 2023-03-18 21:02:58.537544 datapipe_core-0.12.0a2/datapipe/store/table_store.py
+-rw-r--r--   0        0        0     3015 2023-07-10 20:51:13.239026 datapipe_core-0.12.0a2/datapipe/types.py
+-rw-r--r--   0        0        0     1907 2023-07-10 21:58:08.970134 datapipe_core-0.12.0a2/pyproject.toml
+-rw-r--r--   0        0        0     1906 1970-01-01 00:00:00.000000 datapipe_core-0.12.0a2/PKG-INFO
```

### Comparing `datapipe_core-0.11.9a6/LICENSE` & `datapipe_core-0.12.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `datapipe_core-0.11.9a6/datapipe/compute.py` & `datapipe_core-0.12.0a2/datapipe/compute.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import hashlib
 import logging
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
-from typing import Any, Dict, List, Optional, Protocol
+from typing import Dict, Iterable, List, Optional, Tuple
 
 from opentelemetry import trace
+import tqdm
 
 from datapipe.datatable import DataStore, DataTable
 from datapipe.run_config import RunConfig
 from datapipe.store.table_store import TableStore
-from datapipe.types import ChangeList
+from datapipe.types import ChangeList, DataDF, IndexDF, Labels, TransformResult
 
 logger = logging.getLogger("datapipe.compute")
 tracer = trace.get_tracer("datapipe.compute")
 
 
 @dataclass
 class Table:
@@ -32,217 +33,288 @@
         del self.catalog[name]
 
     def init_all_tables(self, ds: DataStore):
         for name in self.catalog.keys():
             self.get_datatable(ds, name)
 
     def get_datatable(self, ds: DataStore, name: str) -> DataTable:
-        return ds.get_or_create_table(
-            name=name,
-            table_store=self.catalog[name].store
-        )
+        return ds.get_or_create_table(name=name, table_store=self.catalog[name].store)
 
 
-@dataclass
-class Pipeline:
-    steps: List['PipelineStep']
-
-
-class PipelineStep(ABC):
+class ComputeStep:
     """
-    Пайплайн описывается через PipelineStep.
-
-    Для выполнения у каждого pipeline_step выполняется build_compute на
-    основании которых создается граф вычислений.
-    """
-
-    @abstractmethod
-    def build_compute(self, ds: DataStore, catalog: Catalog) -> List['ComputeStep']:
-        raise NotImplementedError
-
-
-class DatatableTransformFunc(Protocol):
-    # __name__: str
-
-    def __call__(
-        self,
-        ds: DataStore,
-        input_dts: List[DataTable],
-        output_dts: List[DataTable],
-        run_config: Optional[RunConfig],
-
-        # Возможно, лучше передавать как переменную, а не  **
-        **kwargs
-    ) -> None:
-        ...
-
-
-class DatatableTransform(PipelineStep):
-    def __init__(
-        self,
-        func: DatatableTransformFunc,
-        inputs: List[str],
-        outputs: List[str],
-        check_for_changes: bool = True,
-        kwargs: Optional[Dict] = None,
-    ) -> None:
-        self.func = func
-        self.inputs = inputs
-        self.outputs = outputs
-        self.check_for_changes = check_for_changes
-        self.kwargs = kwargs
-
-    def build_compute(self, ds: DataStore, catalog: Catalog) -> List['ComputeStep']:
-        return [
-            DatatableTransformStep(
-                name=self.func.__name__,    # type: ignore # mypy bug: https://github.com/python/mypy/issues/10976
-                input_dts=[catalog.get_datatable(ds, i) for i in self.inputs],
-                output_dts=[catalog.get_datatable(ds, i) for i in self.outputs],
-                func=self.func,
-                kwargs=self.kwargs,
-                check_for_changes=self.check_for_changes,
-            )
-        ]
-
-
-class ComputeStep(ABC):
-    '''
     Шаг вычислений в графе вычислений.
 
     Каждый шаг должен уметь отвечать на вопросы:
     - какие таблицы приходят на вход
     - какие таблицы изменяются в результате трансформации
 
     Шаг может запускаться в режиме полной обработки, то есть без указания какие
     объекты изменились. Или в changelist-режиме, когда на вход поступают
     измененные индексы для каждой из входных таблиц.
 
     В changelist-режиме шаг обрабатывает только минимально необходимое
     количество батчей, которые покрывают все измененные индексы.
-    '''
+    """
 
-    def __init__(self, name: str) -> None:
+    def __init__(
+        self,
+        name: str,
+        input_dts: List[DataTable],
+        output_dts: List[DataTable],
+        labels: Optional[Labels] = None,
+    ) -> None:
         self._name = name
+        self.input_dts = input_dts
+        self.output_dts = output_dts
+        self._labels = labels
 
     def get_name(self) -> str:
         ss = [
             self.__class__.__name__,
             self._name,
-            *[i.name for i in self.get_input_dts()],
-            *[o.name for o in self.get_output_dts()],
+            *[i.name for i in self.input_dts],
+            *[o.name for o in self.output_dts],
         ]
 
         m = hashlib.shake_128()
-        m.update(''.join(ss).encode('utf-8'))
+        m.update("".join(ss).encode("utf-8"))
 
         return f"{self._name}_{m.hexdigest(5)}"
 
     @property
     def name(self) -> str:
         return self.get_name()
 
-    @abstractmethod
-    def get_input_dts(self) -> List[DataTable]:
-        pass
-
-    @abstractmethod
-    def get_output_dts(self) -> List[DataTable]:
-        pass
+    @property
+    def labels(self) -> Labels:
+        return self._labels if self._labels else []
 
-    def validate(self):
-        inp_p_keys_arr = [set(inp.primary_keys) for inp in self.get_input_dts() if inp]
-        out_p_keys_arr = [set(out.primary_keys) for out in self.get_output_dts() if out]
+    def validate(self) -> None:
+        inp_p_keys_arr = [set(inp.primary_keys) for inp in self.input_dts if inp]
+        out_p_keys_arr = [set(out.primary_keys) for out in self.output_dts if out]
 
         inp_p_keys = set.intersection(*inp_p_keys_arr) if len(inp_p_keys_arr) else set()
         out_p_keys = set.intersection(*out_p_keys_arr) if len(out_p_keys_arr) else set()
         join_keys = set.intersection(inp_p_keys, out_p_keys)
 
         key_to_column_type_inp = {
             column.name: type(column.type)
-            for inp in self.get_input_dts()
-            for column in inp.primary_schema if column.name in join_keys
+            for inp in self.input_dts
+            for column in inp.primary_schema
+            if column.name in join_keys
         }
         key_to_column_type_out = {
             column.name: type(column.type)
-            for inp in self.get_output_dts()
-            for column in inp.primary_schema if column.name in join_keys
+            for inp in self.output_dts
+            for column in inp.primary_schema
+            if column.name in join_keys
         }
 
         for key in join_keys:
             if key_to_column_type_inp[key] != key_to_column_type_out[key]:
                 raise ValueError(
                     f'Primary key "{key}" in inputs and outputs must have same column\'s type: '
-                    f'{key_to_column_type_inp[key]} != {key_to_column_type_out[key]}'
+                    f"{key_to_column_type_inp[key]} != {key_to_column_type_out[key]}"
                 )
 
-    def run_full(self, ds: DataStore, run_config: RunConfig = None) -> None:
-        pass
-
-    def run_changelist(self, ds: DataStore, changelist: ChangeList, run_config: RunConfig = None) -> ChangeList:
-        return ChangeList()
-
-# TODO move to `core_steps`
-class DatatableTransformStep(ComputeStep):
-    def __init__(
+    def get_full_process_ids(
         self,
-        name: str,
-        input_dts: List[DataTable],
-        output_dts: List[DataTable],
+        ds: DataStore,
+        run_config: Optional[RunConfig] = None,
+    ) -> Tuple[int, Iterable[IndexDF]]:
+        raise NotImplementedError()
 
-        func: DatatableTransformFunc,
-        kwargs: Dict[str, Any] = None,
-        check_for_changes: bool = True,
-    ) -> None:
-        ComputeStep.__init__(self, name)
+    def get_change_list_process_ids(
+        self,
+        ds: DataStore,
+        change_list: ChangeList,
+        run_config: Optional[RunConfig] = None,
+    ) -> Tuple[int, Iterable[IndexDF]]:
+        raise NotImplementedError()
 
-        self.input_dts = input_dts
-        self.output_dts = output_dts
+    def get_batch_input_dfs(
+        self,
+        ds: DataStore,
+        idx: IndexDF,
+        run_config: Optional[RunConfig] = None,
+    ) -> List[DataDF]:
+        return [inp.get_data(idx) for inp in self.input_dts]
 
-        self.func = func
-        self.kwargs = kwargs or {}
-        self.check_for_changes = check_for_changes
-
-    def get_input_dts(self) -> List[DataTable]:
-        return self.input_dts
-
-    def get_output_dts(self) -> List[DataTable]:
-        return self.output_dts
-
-    def run_full(self, ds: DataStore, run_config: RunConfig = None) -> None:
-        if len(self.input_dts) > 0 and self.check_for_changes:
-            with tracer.start_as_current_span("check for changes"):
-                changed_idx_count = ds.get_changed_idx_count(
-                    inputs=self.input_dts,
-                    outputs=self.output_dts,
-                    run_config=run_config
-                )
+    def process_batch_dfs(
+        self,
+        ds: DataStore,
+        idx: IndexDF,
+        input_dfs: List[DataDF],
+        run_config: Optional[RunConfig] = None,
+    ) -> TransformResult:
+        raise NotImplementedError()
 
-                if changed_idx_count == 0:
-                    logger.debug(f'Skipping {self.get_name()} execution - nothing to compute')
+    def process_batch_dts(
+        self,
+        ds: DataStore,
+        idx: IndexDF,
+        run_config: Optional[RunConfig] = None,
+    ) -> Optional[TransformResult]:
+        with tracer.start_as_current_span("get input data"):
+            input_dfs = self.get_batch_input_dfs(ds, idx, run_config)
+
+        if sum(len(j) for j in input_dfs) == 0:
+            return None
+
+        with tracer.start_as_current_span("run transform"):
+            output_dfs = self.process_batch_dfs(
+                ds=ds,
+                idx=idx,
+                input_dfs=input_dfs,
+                run_config=run_config,
+            )
 
-                    return
+        return output_dfs
 
-        run_config = RunConfig.add_labels(run_config, {'step_name': self.get_name()})
+    def process_batch(
+        self,
+        ds: DataStore,
+        idx: IndexDF,
+        run_config: Optional[RunConfig] = None,
+    ) -> ChangeList:
+        with tracer.start_as_current_span("process batch"):
+            logger.debug(f"Idx to process: {idx.to_records()}")
 
-        with tracer.start_as_current_span(f"Run {self.func.__name__}"):
             try:
-                self.func(
-                    ds=ds,
-                    input_dts=self.input_dts,
-                    output_dts=self.output_dts,
-                    run_config=run_config,
-                    **self.kwargs
-                )
+                output_dfs = self.process_batch_dts(ds, idx, run_config)
             except Exception as e:
-                logger.error(f"Datatable transform ({self.func.__name__}) run failed: {str(e)}")
+                logger.error(f"Transform failed: {str(e)}")
                 ds.event_logger.log_exception(
                     e,
-                    run_config=run_config
+                    run_config=RunConfig.add_labels(run_config, {"idx": idx.to_dict(orient="records")}),
                 )
 
+                return ChangeList()
+
+            changes = ChangeList()
+
+            if output_dfs is not None:
+                if isinstance(output_dfs, (list, tuple)):
+                    assert len(output_dfs) == len(self.output_dts)
+                else:
+                    assert len(self.output_dts) == 1
+                    output_dfs = [output_dfs]
+
+                with tracer.start_as_current_span("store output batch"):
+                    try:
+                        for k, res_dt in enumerate(self.output_dts):
+                            # Берем k-ое значение функции для k-ой таблички
+                            # Добавляем результат в результирующие чанки
+                            change_idx = res_dt.store_chunk(
+                                data_df=output_dfs[k],
+                                processed_idx=idx,
+                                run_config=run_config,
+                            )
+
+                            changes.append(res_dt.name, change_idx)
+                    except Exception as e:
+                        logger.error(f"Store output batch failed: {str(e)}")
+                        ds.event_logger.log_exception(
+                            e,
+                            run_config=RunConfig.add_labels(run_config, {"idx": idx.to_dict(orient="records")}),
+                        )
+
+                        return ChangeList()
+
+            else:
+                with tracer.start_as_current_span("delete missing data from output"):
+                    for k, res_dt in enumerate(self.output_dts):
+                        del_idx = res_dt.meta_table.get_existing_idx(idx)
+
+                        res_dt.delete_by_idx(del_idx, run_config=run_config)
+
+                        changes.append(res_dt.name, del_idx)
+
+            return changes
+
+    def run_full(
+        self,
+        ds: DataStore,
+        run_config: Optional[RunConfig] = None,
+    ) -> None:
+        logger.info(f"Running: {self.name}")
+        run_config = RunConfig.add_labels(run_config, {"step_name": self.name})
+
+        (idx_count, idx_gen) = self.get_full_process_ids(ds, run_config)
+
+        logger.info(f"Batches to process {idx_count}")
+
+        if idx_count is not None and idx_count == 0:
+            return
+
+        for idx in tqdm.tqdm(idx_gen, total=idx_count):
+            self.process_batch(
+                ds=ds,
+                idx=idx,
+                run_config=run_config,
+            )
+
+        ds.event_logger.log_step_full_complete(self.name)
+
+    def run_changelist(
+        self,
+        ds: DataStore,
+        change_list: ChangeList,
+        run_config: Optional[RunConfig] = None,
+    ) -> ChangeList:
+        logger.info(f"Running: {self.name}")
+        run_config = RunConfig.add_labels(run_config, {"step_name": self.name})
+
+        (idx_count, idx_gen) = self.get_change_list_process_ids(ds, change_list, run_config)
+
+        logger.info(f"Batches to process {idx_count}")
+
+        if idx_count is not None and idx_count == 0:
+            return ChangeList()
+
+        res_changelist = ChangeList()
+
+        for idx in tqdm.tqdm(idx_gen, total=idx_count):
+            changes = self.process_batch(
+                ds=ds,
+                idx=idx,
+                run_config=run_config,
+            )
+            res_changelist.extend(changes)
+
+        return res_changelist
+
+
+class PipelineStep(ABC):
+    """
+    Пайплайн описывается через PipelineStep.
+
+    Для выполнения у каждого pipeline_step выполняется build_compute на
+    основании которых создается граф вычислений.
+    """
+
+    @abstractmethod
+    def build_compute(self, ds: DataStore, catalog: Catalog) -> List[ComputeStep]:
+        raise NotImplementedError
+
+
+@dataclass
+class Pipeline:
+    steps: List[PipelineStep]
+
+
+class DatapipeApp:
+    def __init__(self, ds: DataStore, catalog: Catalog, pipeline: Pipeline):
+        self.ds = ds
+        self.catalog = catalog
+        self.pipeline = pipeline
+
+        self.steps = build_compute(ds, catalog, pipeline)
+
 
 def build_compute(ds: DataStore, catalog: Catalog, pipeline: Pipeline) -> List[ComputeStep]:
     with tracer.start_as_current_span("build_compute"):
         catalog.init_all_tables(ds)
 
         compute_pipeline: List[ComputeStep] = []
 
@@ -253,77 +325,79 @@
             compute_step.validate()
 
         return compute_pipeline
 
 
 def print_compute(steps: List[ComputeStep]) -> None:
     import pprint
-    pprint.pp(
-        steps
-    )
 
+    pprint.pp(steps)
 
-def run_steps(ds: DataStore, steps: List[ComputeStep], run_config: RunConfig = None) -> None:
-    with tracer.start_as_current_span("run_steps"):
-        for step in steps:
-            with tracer.start_as_current_span(
-                f'{step.get_name()} {[i.name for i in step.get_input_dts()]} -> {[i.name for i in step.get_output_dts()]}'
-            ):
-                logger.info(
-                    f'Running {step.get_name()} '
-                    f'{[i.name for i in step.get_input_dts()]} -> {[i.name for i in step.get_output_dts()]}'
-                )
 
-                step.run_full(ds, run_config)
+def run_steps(ds: DataStore, steps: List[ComputeStep], run_config: Optional[RunConfig] = None) -> None:
+    for step in steps:
+        with tracer.start_as_current_span(
+            f"{step.get_name()} {[i.name for i in step.input_dts]} -> {[i.name for i in step.output_dts]}"
+        ):
+            logger.info(
+                f"Running {step.get_name()} "
+                f"{[i.name for i in step.input_dts]} -> {[i.name for i in step.output_dts]}"
+            )
+
+        step.run_full(ds, run_config)
 
 
 def run_pipeline(
     ds: DataStore,
     catalog: Catalog,
     pipeline: Pipeline,
-    run_config: RunConfig = None,
+    run_config: Optional[RunConfig] = None,
 ) -> None:
     steps = build_compute(ds, catalog, pipeline)
     run_steps(ds, steps, run_config)
 
 
 def run_changelist(
     ds: DataStore,
     catalog: Catalog,
     pipeline: Pipeline,
     changelist: ChangeList,
-    run_config: RunConfig = None,
+    run_config: Optional[RunConfig] = None,
 ) -> None:
     steps = build_compute(ds, catalog, pipeline)
 
     return run_steps_changelist(ds, steps, changelist, run_config)
 
 
 def run_steps_changelist(
     ds: DataStore,
     steps: List[ComputeStep],
     changelist: ChangeList,
-    run_config: RunConfig = None,
+    run_config: Optional[RunConfig] = None,
 ) -> None:
     current_changes = changelist
     next_changes = ChangeList()
     iteration = 0
 
     with tracer.start_as_current_span("Start pipeline for changelist"):
         while not current_changes.empty() and iteration < 100:
             with tracer.start_as_current_span("run_steps"):
                 for step in steps:
                     with tracer.start_as_current_span(
-                        f'{step.get_name()} '
-                        f'{[i.name for i in step.get_input_dts()]} -> {[i.name for i in step.get_output_dts()]}'
+                        f"{step.get_name()} "
+                        f"{[i.name for i in step.input_dts]} -> {[i.name for i in step.output_dts]}"
                     ):
                         logger.info(
-                            f'Running {step.get_name()} '
-                            f'{[i.name for i in step.get_input_dts()]} -> {[i.name for i in step.get_output_dts()]}'
+                            f"Running {step.get_name()} "
+                            f"{[i.name for i in step.input_dts]} -> {[i.name for i in step.output_dts]}"
                         )
 
-                        step_changes = step.run_changelist(ds, current_changes, run_config)
-                        next_changes.extend(step_changes)
+                        try:
+                            step_changes = step.run_changelist(ds, current_changes, run_config)
+                            next_changes.extend(step_changes)
+                        except NotImplementedError:
+                            # Some steps do not implement `.run_changelist`, that's ok
+                            pass
 
             current_changes = next_changes
             next_changes = ChangeList()
             iteration += 1
```

### Comparing `datapipe_core-0.11.9a6/datapipe/core_steps.py` & `datapipe_core-0.12.0a2/datapipe/core_steps.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,281 +1,325 @@
 import logging
 import time
+from dataclasses import dataclass
 from typing import (
-    Any, Dict, Iterable, Iterator, List, Optional, Tuple, Union, Callable)
+    Any,
+    Callable,
+    Dict,
+    Iterable,
+    Iterator,
+    List,
+    Optional,
+    Protocol,
+    Tuple,
+    cast,
+)
 
 import tqdm
 from opentelemetry import trace
 
-from datapipe.compute import (Catalog, ComputeStep, DatatableTransformStep,
-                              PipelineStep)
+from datapipe.compute import Catalog, ComputeStep, PipelineStep
 from datapipe.datatable import DataStore, DataTable
 from datapipe.run_config import RunConfig
-from datapipe.types import ChangeList, DataDF, IndexDF
+from datapipe.types import ChangeList, DataDF, IndexDF, Labels, TransformResult
 
-logger = logging.getLogger('datapipe.core_steps')
+logger = logging.getLogger("datapipe.core_steps")
 tracer = trace.get_tracer("datapipe.core_steps")
 
 
-BatchTransformFunc = Callable[..., Union[DataDF, List[DataDF], Tuple[DataDF, ...]]]
+class DatatableTransformFunc(Protocol):
+    __name__: str
 
+    def __call__(
+        self,
+        ds: DataStore,
+        input_dts: List[DataTable],
+        output_dts: List[DataTable],
+        run_config: Optional[RunConfig],
+        # Возможно, лучше передавать как переменную, а не  **
+        **kwargs,
+    ) -> None:
+        ...
 
-def do_batch_transform(
-    func: BatchTransformFunc,
-    ds: DataStore,
-    input_dts: List[DataTable],
-    output_dts: List[DataTable],
-    idx_gen: Iterable[IndexDF],
-    idx_count: int = None,
-    kwargs: Dict[str, Any] = None,
-    run_config: RunConfig = None,
-) -> Iterator[ChangeList]:
-    '''
-    Множественная инкрементальная обработка `input_dts' на основе изменяющихся индексов
-    '''
-
-    logger.info(f'Batches to process {idx_count}')
-
-    if idx_count is not None and idx_count == 0:
-        # Nothing to process
-        return [ChangeList()]
-
-    for idx in tqdm.tqdm(idx_gen, total=idx_count):
-        with tracer.start_as_current_span("process batch"):
-            logger.debug(f'Idx to process: {idx.to_records()}')
-
-            with tracer.start_as_current_span("get input data"):
-                try:
-                    input_dfs = [inp.get_data(idx) for inp in input_dts]
-                except Exception as e:
-                    logger.error(f"Get input data failed: {str(e)}")
-                    ds.event_logger.log_exception(
-                        e,
-                        run_config=RunConfig.add_labels(run_config, {'idx': idx.to_dict(orient="records")})
-                    )
-
-                    continue
-
-            changes = ChangeList()
-
-            if sum(len(j) for j in input_dfs) > 0:
-                with tracer.start_as_current_span("run transform"):
-                    try:
-                        chunks_df = func(*input_dfs, **kwargs or {})
-                    except Exception as e:
-                        logger.error(f"Transform failed ({func.__name__}): {str(e)}")
-                        ds.event_logger.log_exception(
-                            e,
-                            run_config=RunConfig.add_labels(run_config, {'idx': idx.to_dict(orient="records")})
-                        )
-
-                        continue
-
-                if isinstance(chunks_df, (list, tuple)):
-                    assert len(chunks_df) == len(output_dts)
-                else:
-                    assert len(output_dts) == 1
-                    chunks_df = [chunks_df]
-
-                with tracer.start_as_current_span("store output batch"):
-                    try:
-                        for k, res_dt in enumerate(output_dts):
-                            # Берем k-ое значение функции для k-ой таблички
-                            # Добавляем результат в результирующие чанки
-                            change_idx = res_dt.store_chunk(
-                                data_df=chunks_df[k],
-                                processed_idx=idx,
-                                run_config=run_config,
-                            )
-
-                            changes.append(res_dt.name, change_idx)
-                    except Exception as e:
-                        logger.error(f"Store output batch failed: {str(e)}")
-                        ds.event_logger.log_exception(
-                            e,
-                            run_config=RunConfig.add_labels(run_config, {'idx': idx.to_dict(orient="records")})
-                        )
-
-                        continue
 
-            else:
-                with tracer.start_as_current_span("delete missing data from output"):
-                    for k, res_dt in enumerate(output_dts):
-                        del_idx = res_dt.meta_table.get_existing_idx(idx)
+# TODO подумать, может быть мы хотим дать возможность возвращать итератор TransformResult
+class DatatableBatchTransformFunc(Protocol):
+    __name__: str
 
-                        res_dt.delete_by_idx(del_idx, run_config=run_config)
+    def __call__(
+        self,
+        ds: DataStore,
+        idx: IndexDF,
+        input_dts: List[DataTable],
+        run_config: Optional[RunConfig] = None,
+        kwargs: Optional[Dict[str, Any]] = None,
+    ) -> TransformResult:
+        ...
 
-                        changes.append(res_dt.name, del_idx)
 
-            yield changes
+# TODO подумать, может быть мы хотим дать возможность возвращать итератор TransformResult
+BatchTransformFunc = Callable[..., TransformResult]
 
+BatchGenerateFunc = Callable[..., Iterator[TransformResult]]
 
-def do_full_batch_transform(
-    func: BatchTransformFunc,
-    ds: DataStore,
-    input_dts: List[DataTable],
-    output_dts: List[DataTable],
-    kwargs: Optional[Dict] = None,
-    chunk_size: int = 1000,
-    run_config: RunConfig = None,
-) -> None:
-    with tracer.start_as_current_span("compute ids to process"):
-        idx_count, idx_gen = ds.get_full_process_ids(
-            inputs=input_dts,
-            outputs=output_dts,
-            chunk_size=chunk_size,
-            run_config=run_config
-        )
 
-    gen = do_batch_transform(
-        func,
-        kwargs=kwargs,
-        ds=ds,
-        idx_count=idx_count,
-        idx_gen=idx_gen,
-        input_dts=input_dts,
-        output_dts=output_dts,
-        run_config=run_config,
-    )
+@dataclass
+class DatatableTransform(PipelineStep):
+    func: DatatableTransformFunc
+    inputs: List[str]
+    outputs: List[str]
+    check_for_changes: bool = True
+    kwargs: Optional[Dict[str, Any]] = None
+    labels: Optional[Labels] = None
 
-    for changes in gen:
-        pass
+    def build_compute(self, ds: DataStore, catalog: Catalog) -> List["ComputeStep"]:
+        return [
+            DatatableTransformStep(
+                name=self.func.__name__,
+                input_dts=[catalog.get_datatable(ds, i) for i in self.inputs],
+                output_dts=[catalog.get_datatable(ds, i) for i in self.outputs],
+                func=self.func,
+                kwargs=self.kwargs,
+                check_for_changes=self.check_for_changes,
+                labels=self.labels,
+            )
+        ]
 
 
-class BatchTransform(PipelineStep):
+class DatatableTransformStep(ComputeStep):
     def __init__(
         self,
-        func: BatchTransformFunc,
-        inputs: List[str],
-        outputs: List[str],
-        chunk_size: int = 1000,
-        kwargs: Dict[str, Any] = None,
-    ):
+        name: str,
+        input_dts: List[DataTable],
+        output_dts: List[DataTable],
+        func: DatatableTransformFunc,
+        kwargs: Optional[Dict] = None,
+        check_for_changes: bool = True,
+        labels: Optional[Labels] = None,
+    ) -> None:
+        ComputeStep.__init__(self, name, input_dts, output_dts, labels)
+
         self.func = func
-        self.inputs = inputs
-        self.outputs = outputs
-        self.chunk_size = chunk_size
         self.kwargs = kwargs or {}
+        self.check_for_changes = check_for_changes
+
+    def run_full(self, ds: DataStore, run_config: Optional[RunConfig] = None) -> None:
+        logger.info(f"Running: {self.name}")
+
+        if len(self.input_dts) > 0 and self.check_for_changes:
+            with tracer.start_as_current_span("check for changes"):
+                changed_idx_count = ds.get_changed_idx_count(
+                    inputs=self.input_dts,
+                    outputs=self.output_dts,
+                    run_config=run_config,
+                )
+
+                if changed_idx_count == 0:
+                    logger.debug(f"Skipping {self.get_name()} execution - nothing to compute")
+
+                    return
+
+        run_config = RunConfig.add_labels(run_config, {"step_name": self.get_name()})
+
+        with tracer.start_as_current_span(f"Run {self.func}"):
+            try:
+                self.func(
+                    ds=ds,
+                    input_dts=self.input_dts,
+                    output_dts=self.output_dts,
+                    run_config=run_config,
+                    kwargs=self.kwargs,
+                )
+            except Exception as e:
+                logger.error(f"Datatable transform ({self.func}) run failed: {str(e)}")
+                ds.event_logger.log_exception(e, run_config=run_config)
+
+
+@dataclass
+class BatchTransform(PipelineStep):
+    func: BatchTransformFunc
+    inputs: List[str]
+    outputs: List[str]
+    chunk_size: int = 1000
+    kwargs: Optional[Dict[str, Any]] = None
+    labels: Optional[Labels] = None
 
     def build_compute(self, ds: DataStore, catalog: Catalog) -> List[ComputeStep]:
         input_dts = [catalog.get_datatable(ds, name) for name in self.inputs]
         output_dts = [catalog.get_datatable(ds, name) for name in self.outputs]
 
         return [
             BatchTransformStep(
-                f'{self.func.__name__}',  # type: ignore # mypy bug: https://github.com/python/mypy/issues/10976
+                f"{self.func.__name__}",  # type: ignore # mypy bug: https://github.com/python/mypy/issues/10976
                 input_dts=input_dts,
                 output_dts=output_dts,
                 func=self.func,
                 kwargs=self.kwargs,
                 chunk_size=self.chunk_size,
+                labels=self.labels,
             )
         ]
 
 
 class BatchTransformStep(ComputeStep):
     def __init__(
         self,
         name: str,
+        func: BatchTransformFunc,
         input_dts: List[DataTable],
         output_dts: List[DataTable],
-
-        func: BatchTransformFunc,
-        kwargs: Dict[str, Any] = None,
+        kwargs: Optional[Dict[str, Any]] = None,
         chunk_size: int = 1000,
+        labels: Optional[Labels] = None,
     ) -> None:
-        ComputeStep.__init__(self, name)
-
-        self.input_dts = input_dts
-        self.output_dts = output_dts
+        ComputeStep.__init__(self, name, input_dts, output_dts, labels)
 
         self.func = func
         self.kwargs = kwargs or {}
         self.chunk_size = chunk_size
 
-    def get_input_dts(self) -> List[DataTable]:
-        return self.input_dts
-
-    def get_output_dts(self) -> List[DataTable]:
-        return self.output_dts
-
-    def run_full(self, ds: DataStore, run_config: RunConfig = None) -> None:
-        run_config = RunConfig.add_labels(run_config, {'step_name': self.name})
+    def get_full_process_ids(
+        self,
+        ds: DataStore,
+        run_config: Optional[RunConfig] = None,
+    ) -> Tuple[int, Iterable[IndexDF]]:
+        with tracer.start_as_current_span("compute ids to process"):
+            return ds.get_full_process_ids(
+                inputs=self.input_dts,
+                outputs=self.output_dts,
+                chunk_size=self.chunk_size,
+                run_config=run_config,
+            )
 
-        with tracer.start_as_current_span("Get ids to process"):
-            idx_count, idx_gen = ds.get_full_process_ids(
+    def get_change_list_process_ids(
+        self,
+        ds: DataStore,
+        change_list: ChangeList,
+        run_config: Optional[RunConfig] = None,
+    ) -> Tuple[int, Iterable[IndexDF]]:
+        with tracer.start_as_current_span("compute ids to process"):
+            return ds.get_change_list_process_ids(
                 inputs=self.input_dts,
                 outputs=self.output_dts,
+                change_list=change_list,
                 chunk_size=self.chunk_size,
-                run_config=run_config
+                run_config=run_config,
             )
 
-        gen = do_batch_transform(
-            self.func,
-            ds=ds,
-            idx_count=idx_count,
-            idx_gen=idx_gen,
-            input_dts=self.input_dts,
-            output_dts=self.output_dts,
-            run_config=run_config,
-            kwargs=self.kwargs,
-        )
+    def process_batch_dfs(
+        self,
+        ds: DataStore,
+        idx: IndexDF,
+        input_dfs: List[DataDF],
+        run_config: Optional[RunConfig] = None,
+    ) -> TransformResult:
+        return self.func(*input_dfs, **self.kwargs or {})
+
+
+@dataclass
+class DatatableBatchTransform(PipelineStep):
+    func: DatatableBatchTransformFunc
+    inputs: List[str]
+    outputs: List[str]
+    chunk_size: int = 1000
+    kwargs: Optional[Dict] = None
+    labels: Optional[Labels] = None
 
-        for changes in gen:
-            pass
+    def build_compute(self, ds: DataStore, catalog: Catalog) -> List[ComputeStep]:
+        input_dts = [catalog.get_datatable(ds, name) for name in self.inputs]
+        output_dts = [catalog.get_datatable(ds, name) for name in self.outputs]
 
-    def run_changelist(self, ds: DataStore, change_list: ChangeList, run_config: RunConfig = None) -> ChangeList:
-        run_config = RunConfig.add_labels(run_config, {'step_name': self.name})
+        return [
+            DatatableBatchTransformStep(
+                f"{self.func.__name__}",
+                func=self.func,
+                input_dts=input_dts,
+                output_dts=output_dts,
+                kwargs=self.kwargs,
+                chunk_size=self.chunk_size,
+                labels=self.labels,
+            )
+        ]
 
-        idx_count, idx_gen = ds.get_change_list_process_ids(
-            inputs=self.input_dts,
-            outputs=self.output_dts,
-            change_list=change_list,
-            chunk_size=self.chunk_size,
-            run_config=run_config
-        )
 
-        gen = do_batch_transform(
-            self.func,
+class DatatableBatchTransformStep(ComputeStep):
+    def __init__(
+        self,
+        name: str,
+        func: DatatableBatchTransformFunc,
+        input_dts: List[DataTable],
+        output_dts: List[DataTable],
+        kwargs: Optional[Dict] = None,
+        chunk_size: int = 1000,
+        labels: Optional[Labels] = None,
+    ) -> None:
+        super().__init__(name, input_dts, output_dts, labels)
+
+        self.func = func
+        self.kwargs = kwargs
+        self.chunk_size = chunk_size
+
+    def get_full_process_ids(
+        self,
+        ds: DataStore,
+        run_config: Optional[RunConfig] = None,
+    ) -> Tuple[int, Iterable[IndexDF]]:
+        with tracer.start_as_current_span("compute ids to process"):
+            return ds.get_full_process_ids(
+                inputs=self.input_dts,
+                outputs=self.output_dts,
+                chunk_size=self.chunk_size,
+                run_config=run_config,
+            )
+
+    def get_change_list_process_ids(
+        self,
+        ds: DataStore,
+        change_list: ChangeList,
+        run_config: Optional[RunConfig] = None,
+    ) -> Tuple[int, Iterable[IndexDF]]:
+        with tracer.start_as_current_span("compute ids to process"):
+            return ds.get_change_list_process_ids(
+                inputs=self.input_dts,
+                outputs=self.output_dts,
+                change_list=change_list,
+                chunk_size=self.chunk_size,
+                run_config=run_config,
+            )
+
+    def process_batch_dts(
+        self,
+        ds: DataStore,
+        idx: IndexDF,
+        run_config: Optional[RunConfig] = None,
+    ) -> Optional[TransformResult]:
+        return self.func(
             ds=ds,
+            idx=idx,
             input_dts=self.input_dts,
-            output_dts=self.output_dts,
-            idx_count=idx_count,
-            idx_gen=idx_gen,
             run_config=run_config,
             kwargs=self.kwargs,
         )
 
-        res_changelist = ChangeList()
-
-        for changes in gen:
-            res_changelist.extend(changes)
-
-        return res_changelist
-
-
-BatchGenerateFunc = Callable[..., Iterator[Union[DataDF, Tuple[DataDF, ...]]]]
-
 
 def do_batch_generate(
     func: BatchGenerateFunc,
-
     ds: DataStore,
     output_dts: List[DataTable],
-    kwargs: Dict[str, Any] = None,
-    run_config: RunConfig = None,
+    run_config: Optional[RunConfig] = None,
+    kwargs: Optional[Dict] = None,
 ) -> None:
     import inspect
 
     import pandas as pd
 
-    '''
+    """
     Создание новой таблицы из результатов запуска `proc_func`.
     Функция может быть как обычной, так и генерирующейся
-    '''
+    """
 
     now = time.time()
     empty_generator = True
 
     assert inspect.isgeneratorfunction(func), "Starting v0.8.0 proc_func should be a generator"
 
     with tracer.start_as_current_span("init generator"):
@@ -322,63 +366,49 @@
                 dt_k.store_chunk(chunk_dfs[k], run_config=run_config)
 
     with tracer.start_as_current_span("delete stale rows"):
         for k, dt_k in enumerate(output_dts):
             dt_k.delete_stale_by_process_ts(now, run_config=run_config)
 
 
+@dataclass
 class BatchGenerate(PipelineStep):
-    def __init__(
-        self,
-        func: BatchGenerateFunc,
-        outputs: List[str],
-        kwargs: Optional[Dict] = None,
-    ):
-        self.func = func
-        self.outputs = outputs
-        self.kwargs = kwargs
+    func: BatchGenerateFunc
+    outputs: List[str]
+    kwargs: Optional[Dict] = None
+    labels: Optional[Labels] = None
 
     def build_compute(self, ds: DataStore, catalog: Catalog) -> List[ComputeStep]:
-        def transform_func(
-            ds: DataStore,
-            input_dts: List[DataTable],
-            output_dts: List[DataTable],
-            run_config: Optional[RunConfig],
-            **kwargs
-        ):
-            return do_batch_generate(
-                func=self.func,
-                kwargs=kwargs,
-                ds=ds,
-                output_dts=output_dts,
-                run_config=run_config,
-            )
-
         return [
             DatatableTransformStep(
-                name=self.func.__name__,  # type: ignore # mypy bug: https://github.com/python/mypy/issues/10976
-                func=transform_func,
+                name=self.func.__name__,
+                func=cast(
+                    DatatableTransformFunc,
+                    lambda ds, input_dts, output_dts, run_config, kwargs: do_batch_generate(
+                        func=self.func, ds=ds, output_dts=output_dts, run_config=run_config, kwargs=kwargs
+                    ),
+                ),
                 input_dts=[],
                 output_dts=[catalog.get_datatable(ds, name) for name in self.outputs],
                 check_for_changes=False,
                 kwargs=self.kwargs,
+                labels=self.labels,
             )
         ]
 
 
-def update_external_table(ds: DataStore, table: DataTable, run_config: RunConfig = None) -> None:
+def update_external_table(ds: DataStore, table: DataTable, run_config: Optional[RunConfig] = None) -> None:
     now = time.time()
 
     for ps_df in tqdm.tqdm(table.table_store.read_rows_meta_pseudo_df(run_config=run_config)):
-
         (
             new_df,
             changed_df,
             new_meta_df,
-            changed_meta_df
+            changed_meta_df,
         ) = table.meta_table.get_changes_for_store_chunk(ps_df, now=now)
 
         ds.event_logger.log_state(
             table.name,
             added_count=len(new_df),
             updated_count=len(changed_df),
             deleted_count=0,
@@ -388,42 +418,48 @@
 
         # TODO switch to iterative store_chunk and table.sync_meta_by_process_ts
 
         table.meta_table.insert_meta_for_store_chunk(new_meta_df)
         table.meta_table.update_meta_for_store_chunk(changed_meta_df)
 
     for stale_idx in table.meta_table.get_stale_idx(now, run_config=run_config):
-        logger.debug(f'Deleting {len(stale_idx.index)} rows from {table.name} data')
+        logger.debug(f"Deleting {len(stale_idx.index)} rows from {table.name} data")
         table.event_logger.log_state(
             table.name,
             added_count=0,
             updated_count=0,
             deleted_count=len(stale_idx),
             processed_count=len(stale_idx),
             run_config=run_config,
         )
 
         table.meta_table.mark_rows_deleted(stale_idx, now=now)
 
 
 class UpdateExternalTable(PipelineStep):
-    def __init__(self, output: str) -> None:
+    def __init__(
+        self,
+        output: str,
+        labels: Optional[Labels] = None,
+    ) -> None:
         self.output_table_name = output
+        self.labels = labels
 
     def build_compute(self, ds: DataStore, catalog: Catalog) -> List[ComputeStep]:
         def transform_func(
             ds: DataStore,
             input_dts: List[DataTable],
             output_dts: List[DataTable],
             run_config: Optional[RunConfig],
-            **kwargs
+            **kwargs,
         ):
             return update_external_table(ds, output_dts[0], run_config)
 
         return [
             DatatableTransformStep(
-                name=f'update_{self.output_table_name}',
-                func=transform_func,
+                name=f"update_{self.output_table_name}",
+                func=cast(DatatableTransformFunc, transform_func),
                 input_dts=[],
                 output_dts=[catalog.get_datatable(ds, self.output_table_name)],
+                labels=self.labels,
             )
         ]
```

### Comparing `datapipe_core-0.11.9a6/datapipe/datatable.py` & `datapipe_core-0.12.0a2/datapipe/datatable.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,18 +7,24 @@
 from sqlalchemy import alias, and_, func, or_, select, column
 
 from datapipe.event_logger import EventLogger
 from datapipe.metastore import MetaTable
 from datapipe.run_config import LabelDict, RunConfig
 from datapipe.store.database import DBConn, sql_apply_runconfig_filter
 from datapipe.store.table_store import TableStore
-from datapipe.types import (ChangeList, DataDF, IndexDF, MetadataDF,
-                            data_to_index, index_difference)
+from datapipe.types import (
+    ChangeList,
+    DataDF,
+    IndexDF,
+    MetadataDF,
+    data_to_index,
+    index_difference,
+)
 
-logger = logging.getLogger('datapipe.datatable')
+logger = logging.getLogger("datapipe.datatable")
 tracer = trace.get_tracer("datapipe.datatable")
 
 
 class DataTable:
     def __init__(
         self,
         name: str,
@@ -44,44 +50,51 @@
 
     def reset_metadata(self):
         self.meta_dbconn.con.execute(
             self.meta_table.sql_table.update().values(process_ts=0, update_ts=0)
         )
 
     def get_size(self) -> int:
-        '''
+        """
         Get the number of non-deleted rows in the DataTable
-        '''
+        """
         return self.meta_table.get_metadata_size(idx=None, include_deleted=False)
 
     def store_chunk(
         self,
         data_df: DataDF,
-        processed_idx: IndexDF = None,
-        now: float = None,
-        run_config: RunConfig = None,
+        processed_idx: Optional[IndexDF] = None,
+        now: Optional[float] = None,
+        run_config: Optional[RunConfig] = None,
     ) -> IndexDF:
-        '''
+        """
         Записать новые данные в таблицу.
 
         При указанном `processed_idx` удалить те строки, которые находятся
         внутри `processed_idx`, но отсутствуют в `data_df`.
-        '''
+        """
+
+        # Check that all index values in `data_df` is unique
+        if data_df.duplicated(self.primary_keys).any():
+            raise ValueError("`data_df` index values should be unique")
+
         changes = [IndexDF(pd.DataFrame(columns=self.primary_keys))]
 
         with tracer.start_as_current_span(f"{self.name} store_chunk"):
             if not data_df.empty:
-                logger.debug(f'Inserting chunk {len(data_df.index)} rows into {self.name}')
+                logger.debug(
+                    f"Inserting chunk {len(data_df.index)} rows into {self.name}"
+                )
 
                 with tracer.start_as_current_span("get_changes_for_store_chunk"):
                     (
                         new_df,
                         changed_df,
                         new_meta_df,
-                        changed_meta_df
+                        changed_meta_df,
                     ) = self.meta_table.get_changes_for_store_chunk(data_df, now)
 
                 self.event_logger.log_state(
                     self.name,
                     added_count=len(new_df),
                     updated_count=len(changed_df),
                     deleted_count=0,
@@ -115,19 +128,19 @@
                     changes.append(deleted_idx)
 
         return cast(IndexDF, pd.concat(changes))
 
     def delete_by_idx(
         self,
         idx: IndexDF,
-        now: float = None,
-        run_config: RunConfig = None,
+        now: Optional[float] = None,
+        run_config: Optional[RunConfig] = None,
     ) -> None:
         if len(idx) > 0:
-            logger.debug(f'Deleting {len(idx.index)} rows from {self.name} data')
+            logger.debug(f"Deleting {len(idx.index)} rows from {self.name} data")
             self.event_logger.log_state(
                 self.name,
                 added_count=0,
                 updated_count=0,
                 deleted_count=len(idx),
                 processed_count=len(idx),
                 run_config=run_config,
@@ -135,31 +148,35 @@
 
             self.table_store.delete_rows(idx)
             self.meta_table.mark_rows_deleted(idx, now=now)
 
     def delete_stale_by_process_ts(
         self,
         process_ts: float,
-        now: float = None,
-        run_config: RunConfig = None,
+        now: Optional[float] = None,
+        run_config: Optional[RunConfig] = None,
     ) -> None:
-        for deleted_df in self.meta_table.get_stale_idx(process_ts, run_config=run_config):
+        for deleted_df in self.meta_table.get_stale_idx(
+            process_ts, run_config=run_config
+        ):
             deleted_idx = data_to_index(deleted_df, self.primary_keys)
 
             self.delete_by_idx(deleted_idx, now=now, run_config=run_config)
 
 
 class DataStore:
     def __init__(
         self,
         meta_dbconn: DBConn,
         create_meta_table: bool = False,
     ) -> None:
         self.meta_dbconn = meta_dbconn
-        self.event_logger = EventLogger(self.meta_dbconn, create_table=create_meta_table)
+        self.event_logger = EventLogger(
+            self.meta_dbconn, create_table=create_meta_table
+        )
         self.tables: Dict[str, DataTable] = {}
         self.create_meta_table = create_meta_table
 
     def create_table(self, name: str, table_store: TableStore) -> DataTable:
         assert name not in self.tables
 
         primary_schema = table_store.get_primary_schema()
@@ -169,15 +186,15 @@
             name=name,
             meta_dbconn=self.meta_dbconn,
             meta_table=MetaTable(
                 dbconn=self.meta_dbconn,
                 name=name,
                 primary_schema=primary_schema,
                 meta_schema=meta_schema,
-                create_table=self.create_meta_table
+                create_table=self.create_meta_table,
             ),
             table_store=table_store,
             event_logger=self.event_logger,
         )
 
         self.tables[name] = res
 
@@ -185,149 +202,143 @@
 
     def get_or_create_table(self, name: str, table_store: TableStore) -> DataTable:
         if name in self.tables:
             return self.tables[name]
         else:
             return self.create_table(name, table_store)
 
-    def get_join_keys(self, inputs: List[DataTable], outputs: List[DataTable]) -> List[str]:
+    def get_join_keys(
+        self, inputs: List[DataTable], outputs: List[DataTable]
+    ) -> List[str]:
         inp_p_keys = [set(inp.primary_keys) for inp in inputs]
         out_p_keys = [set(out.primary_keys) for out in outputs]
 
         return list(set.intersection(*inp_p_keys, *out_p_keys))
 
     def get_table(self, name: str) -> DataTable:
         return self.tables[name]
 
     def _build_changed_idx_sql(
         self,
         inputs: List[DataTable],
         outputs: List[DataTable],
-        run_config: RunConfig = None,
+        run_config: Optional[RunConfig] = None,
     ) -> Tuple[Iterable[str], select]:
         inp_keys = [set(inp.primary_keys) for inp in inputs]
         out_keys = [set(out.primary_keys) for out in outputs]
         join_keys = list(set.intersection(*inp_keys, *out_keys))
 
+        if len(join_keys) == 0:
+            raise NotImplementedError()
+
         if self.meta_dbconn.con.driver in ("sqlite", "pysqlite"):
             greatest_func = func.max
         else:
             greatest_func = func.greatest
 
         def _make_agg_cte(dt: DataTable, agg_fun, agg_col: str):
             tbl = dt.meta_table.sql_table
 
             key_cols = [column(k) for k in join_keys]
 
-            sql = select(*key_cols + [agg_fun(tbl.c[agg_col]).label(agg_col)])\
-                .select_from(tbl).group_by(*key_cols)
+            sql = (
+                select(*key_cols + [agg_fun(tbl.c[agg_col]).label(agg_col)])
+                .select_from(tbl)
+                .group_by(*key_cols)
+            )
 
             sql = sql_apply_runconfig_filter(sql, tbl, dt.primary_keys, run_config)
 
             return sql.cte(name=f"{tbl.name}__{agg_col}")
 
         def _make_agg_of_agg(ctes, agg_col):
             assert len(ctes) > 0
 
             if len(ctes) == 1:
                 return ctes[0]
 
             if len(join_keys) > 1:
                 coalesce_keys = [
-                    func.coalesce(
-                        *[
-                            subq.c[key]
-                            for subq in ctes
-                        ]
-                    ).label(key)
+                    func.coalesce(*[subq.c[key] for subq in ctes]).label(key)
                     for key in join_keys
                 ]
             else:
                 coalesce_keys = [subq.c[join_keys[0]] for subq in ctes]
 
             agg = greatest_func(*[subq.c[agg_col] for subq in ctes]).label(agg_col)
 
             sql = select(*coalesce_keys + [agg]).select_from(ctes[0])
 
             for cte in ctes[1:]:
                 sql = sql.outerjoin(
                     cte,
-                    onclause=and_(
-                        *[
-                            ctes[0].c[key] == cte.c[key]
-                            for key in join_keys
-                        ]
-                    ),
+                    onclause=and_(*[ctes[0].c[key] == cte.c[key] for key in join_keys]),
                     full=True,
                 )
 
             return sql.cte(name=f"all__{agg_col}")
 
         inp_ctes = [_make_agg_cte(tbl, func.max, "update_ts") for tbl in inputs]
         out_ctes = [_make_agg_cte(tbl, func.min, "process_ts") for tbl in outputs]
 
         inp = _make_agg_of_agg(inp_ctes, "update_ts")
         out = _make_agg_of_agg(out_ctes, "process_ts")
 
-        sql = select(*[func.coalesce(inp.c[key], out.c[key]).label(key) for key in join_keys])\
-            .select_from(inp)\
+        sql = (
+            select(
+                *[func.coalesce(inp.c[key], out.c[key]).label(key) for key in join_keys]
+            )
+            .select_from(inp)
             .outerjoin(
-                out,
-                onclause=and_(
-                    *[
-                        inp.c[key] == out.c[key]
-                        for key in join_keys
-                    ]
-                )
-            ).where(
+                out, onclause=and_(*[inp.c[key] == out.c[key] for key in join_keys])
+            )
+            .where(
                 or_(
                     inp.c.update_ts > out.c.process_ts,
                     inp.c.update_ts == None,  # noqa
                     out.c.process_ts == None,  # noqa
                 )
             )
+        )
 
         return (join_keys, sql)
 
     def get_changed_idx_count(
         self,
         inputs: List[DataTable],
         outputs: List[DataTable],
-        run_config: RunConfig = None,
+        run_config: Optional[RunConfig] = None,
     ) -> int:
         _, sql = self._build_changed_idx_sql(
-            inputs=inputs,
-            outputs=outputs,
-            run_config=run_config
+            inputs=inputs, outputs=outputs, run_config=run_config
         )
 
         idx_count = self.meta_dbconn.con.execute(
-            select([func.count()])
-            .select_from(
-                alias(sql.subquery(), name='union_select')
+            select([func.count()]).select_from(
+                alias(sql.subquery(), name="union_select")
             )
         ).scalar()
 
         return idx_count
 
     def get_full_process_ids(
         self,
         inputs: List[DataTable],
         outputs: List[DataTable],
         chunk_size: int = 1000,
-        run_config: RunConfig = None,
+        run_config: Optional[RunConfig] = None,
     ) -> Tuple[int, Iterable[IndexDF]]:
-        '''
+        """
         Метод для получения перечня индексов для обработки.
 
         Returns: (idx_size, iterator<idx_df>)
 
         - idx_size - количество индексов требующих обработки
         - idx_df - датафрейм без колонок с данными, только индексная колонка
-        '''
+        """
 
         if len(inputs) == 0:
             return (0, iter([]))
 
         idx_count = self.get_changed_idx_count(
             inputs=inputs,
             outputs=outputs,
@@ -340,41 +351,37 @@
             run_config=run_config,
         )
 
         # Список ключей из фильтров, которые нужно добавить в результат
         extra_filters: LabelDict
         if run_config is not None:
             extra_filters = {
-                k: v
-                for k, v in run_config.filters.items()
-                if k not in join_keys
+                k: v for k, v in run_config.filters.items() if k not in join_keys
             }
         else:
             extra_filters = {}
 
         def alter_res_df():
             for df in pd.read_sql_query(
-                u1,
-                con=self.meta_dbconn.con,
-                chunksize=chunk_size
+                u1, con=self.meta_dbconn.con, chunksize=chunk_size
             ):
                 for k, v in extra_filters.items():
                     df[k] = v
 
                 yield df
 
         return math.ceil(idx_count / chunk_size), alter_res_df()
 
     def get_change_list_process_ids(
         self,
         inputs: List[DataTable],
         outputs: List[DataTable],
         change_list: ChangeList,
         chunk_size: int = 1000,
-        run_config: RunConfig = None,
+        run_config: Optional[RunConfig] = None,
     ) -> Tuple[int, Iterable[IndexDF]]:
         join_keys = self.get_join_keys(inputs, outputs)
         changes = [pd.DataFrame(columns=join_keys)]
 
         if not join_keys:
             raise ValueError("Primary keys intersection for ChangeList are empty")
 
@@ -384,10 +391,10 @@
 
                 changes.append(data_to_index(idx, join_keys))
 
         idx = IndexDF(pd.concat(changes).drop_duplicates(subset=join_keys))
 
         def gen():
             for i in range(math.ceil(len(idx) / chunk_size)):
-                yield idx[i * chunk_size: (i + 1) * chunk_size]
+                yield idx[i * chunk_size : (i + 1) * chunk_size]
 
         return len(idx), gen()
```

### Comparing `datapipe_core-0.11.9a6/datapipe/event_logger.py` & `datapipe_core-0.12.0a2/datapipe/event_logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,75 @@
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Optional
 from enum import Enum
 
 import logging
-import traceback
+from traceback_with_variables import format_exc
 
 from sqlalchemy.sql import func
 from sqlalchemy.sql.schema import Column, Table
 from sqlalchemy.sql.sqltypes import DateTime, Integer, String, JSON
 from sqlalchemy.dialects.postgresql import JSONB
 
 from datapipe.run_config import RunConfig
 
 
-logger = logging.getLogger('datapipe.event_logger')
+logger = logging.getLogger("datapipe.event_logger")
 
 if TYPE_CHECKING:
     from datapipe.metastore import DBConn
 
 
 class EventTypes(Enum):
     STATE = "state"
     ERROR = "error"
 
 
+class StepEventTypes(Enum):
+    RUN_FULL_COMPLETE = "run_full_complete"
+
+
 class EventLogger:
-    def __init__(self, dbconn: 'DBConn', create_table: bool = False):
+    def __init__(self, dbconn: "DBConn", create_table: bool = False):
         self.dbconn = dbconn
 
         self.events_table = Table(
-            'datapipe_events',
+            "datapipe_events",
+            dbconn.sqla_metadata,
+            Column("id", Integer, primary_key=True, autoincrement=True),
+            Column("event_ts", DateTime, server_default=func.now()),
+            Column("type", String(100)),
+            Column("event", JSON if dbconn.con.name == "sqlite" else JSONB),
+        )
+
+        self.step_events_table = Table(
+            "datapipe_step_events",
             dbconn.sqla_metadata,
-            *self._make_table_schema(dbconn),
+            Column("id", Integer, primary_key=True, autoincrement=True),
+            Column("step", String(100)),
+            Column("event_ts", DateTime, server_default=func.now()),
+            Column("event", String(100)),
+            Column("event_payload", JSON if dbconn.con.name == "sqlite" else JSONB),
         )
 
         if create_table:
             self.events_table.create(self.dbconn.con, checkfirst=True)
-
-    def _make_table_schema(self, dbconn: 'DBConn'):
-        return [
-            Column('id', Integer, primary_key=True, autoincrement=True),
-            Column('event_ts', DateTime, server_default=func.now()),
-            Column('type', String(100)),
-            Column('event', JSON if dbconn.con.name == 'sqlite' else JSONB)
-        ]
+            self.step_events_table.create(self.dbconn.con, checkfirst=True)
 
     def log_state(
         self,
         table_name,
         added_count,
         updated_count,
         deleted_count,
         processed_count,
-        run_config: RunConfig = None,
+        run_config: Optional[RunConfig] = None,
     ):
         logger.debug(
             f'Table "{table_name}": added = {added_count}; updated = {updated_count}; '
-            f'deleted = {deleted_count}, processed_count = {deleted_count}'
+            f"deleted = {deleted_count}, processed_count = {deleted_count}"
         )
 
         if run_config is not None:
             meta = {
                 "labels": run_config.labels,
                 "filters": run_config.filters,
             }
@@ -72,58 +82,73 @@
                 "meta": meta,
                 "data": {
                     "table_name": table_name,
                     "added_count": added_count,
                     "updated_count": updated_count,
                     "deleted_count": deleted_count,
                     "processed_count": processed_count,
-                }
-            }
+                },
+            },
         )
 
         self.dbconn.con.execute(ins)
 
     def log_error(
         self,
         type,
         message,
         description,
         params,
-        run_config: RunConfig = None,
+        run_config: Optional[RunConfig] = None,
     ) -> None:
         if run_config is not None:
-            logger.debug(f'Error in step {run_config.labels.get("step_name")}: {type} {message}')
+            logger.debug(
+                f'Error in step {run_config.labels.get("step_name")}: {type} {message}\n{description}'
+            )
             meta = {
                 "labels": run_config.labels,
                 "filters": run_config.filters,
             }
         else:
-            logger.debug(f'Error: {type} {message}')
+            logger.debug(f"Error: {type} {message}\n{description}")
             meta = {}
 
         ins = self.events_table.insert().values(
             type=EventTypes.ERROR.value,
             event={
                 "meta": meta,
                 "data": {
                     "type": type,
                     "message": message,
                     "description": description,
                     "params": params,
-                }
-            }
+                },
+            },
         )
 
         self.dbconn.con.execute(ins)
 
     def log_exception(
         self,
         exc: Exception,
-        run_config: RunConfig = None,
+        run_config: Optional[RunConfig] = None,
     ) -> None:
         self.log_error(
             type=type(exc).__name__,
             message=str(exc),
-            description=traceback.format_exc(),
-            params=exc.args,
+            description=format_exc(exc),
+            params=[],  # exc.args, # Not all args can be serialized to JSON, dont really need them
             run_config=run_config,
         )
+
+    def log_step_full_complete(
+        self,
+        step_name: str,
+    ) -> None:
+        logger.debug(f"Step {step_name} is marked complete")
+
+        ins = self.step_events_table.insert().values(
+            step=step_name,
+            event=StepEventTypes.RUN_FULL_COMPLETE.value,
+        )
+
+        self.dbconn.con.execute(ins)
```

### Comparing `datapipe_core-0.11.9a6/datapipe/metastore.py` & `datapipe_core-0.12.0a2/datapipe/metastore.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 import copy
 import logging
 import math
 import time
 from dataclasses import dataclass
-from typing import Iterator, List, Tuple, cast
+from typing import Iterator, List, Tuple, cast, Optional
 
 import pandas as pd
 from cityhash import CityHash32
 from sqlalchemy import Column, Float, Integer, Table, func
 from sqlalchemy.sql.expression import and_, delete, or_, select, text, tuple_
 
 from datapipe.run_config import RunConfig
-from datapipe.store.database import (DBConn, MetaKey,
-                                     sql_apply_runconfig_filter,
-                                     sql_schema_to_sqltype)
-from datapipe.types import (DataDF, DataSchema, IndexDF, MetadataDF,
-                            MetaSchema, TAnyDF, data_to_index)
+from datapipe.store.database import (
+    DBConn,
+    MetaKey,
+    sql_apply_runconfig_filter,
+    sql_schema_to_sqltype,
+)
+from datapipe.types import (
+    DataDF,
+    DataSchema,
+    IndexDF,
+    MetadataDF,
+    MetaSchema,
+    TAnyDF,
+    data_to_index,
+)
 
-logger = logging.getLogger('datapipe.metastore')
+logger = logging.getLogger("datapipe.metastore")
 
 METADATA_SQL_SCHEMA = [
-    Column('hash', Integer),
-    Column('create_ts', Float),   # Время создания строки
-    Column('update_ts', Float),   # Время последнего изменения
-    Column('process_ts', Float),  # Время последней успешной обработки
-    Column('delete_ts', Float),   # Время удаления
+    Column("hash", Integer),
+    Column("create_ts", Float),  # Время создания строки
+    Column("update_ts", Float),  # Время последнего изменения
+    Column("process_ts", Float),  # Время последней успешной обработки
+    Column("delete_ts", Float),  # Время удаления
 ]
 
 
 @dataclass
 class TableDebugInfo:
     name: str
     size: int
@@ -54,23 +64,27 @@
 
         self.meta_schema = meta_schema
         self.meta_keys = {}
 
         meta_key_prop = MetaKey.get_property_name()
 
         for column in meta_schema:
-            target_name = column.meta_key.target_name if hasattr(column, meta_key_prop) else column.name
+            target_name = (
+                column.meta_key.target_name
+                if hasattr(column, meta_key_prop)
+                else column.name
+            )
             self.meta_keys[target_name] = column.name
 
         sql_schema = primary_schema + meta_schema + METADATA_SQL_SCHEMA
 
         self.sql_schema = [copy.copy(i) for i in sql_schema]
 
         self.sql_table = Table(
-            f'{self.name}_meta',
+            f"{self.name}_meta",
             self.dbconn.sqla_metadata,
             *self.sql_schema,
         )
 
         if create_table:
             self.sql_table.create(self.dbconn.con, checkfirst=True)
 
@@ -78,63 +92,66 @@
         # Magic number derived empirically. See
         # https://github.com/epoch8/datapipe/issues/178 for details.
         #
         # TODO Investigate deeper how does stack in Postgres work
         return 5000 // len(self.primary_keys)
 
     def _chunk_idx_df(self, idx: TAnyDF) -> Iterator[TAnyDF]:
-        '''
+        """
         Split IndexDF to chunks acceptable for typical Postgres configuration.
         See `_chunk_size` for detatils.
-        '''
+        """
 
         CHUNK_SIZE = self._chunk_size()
 
         for chunk_no in range(int(math.ceil(len(idx) / CHUNK_SIZE))):
-            chunk_idx = idx.iloc[chunk_no*CHUNK_SIZE:(chunk_no+1)*CHUNK_SIZE, :]
+            chunk_idx = idx.iloc[chunk_no * CHUNK_SIZE : (chunk_no + 1) * CHUNK_SIZE, :]
 
             yield cast(TAnyDF, chunk_idx)
 
-    def _build_metadata_query(self, sql, idx: IndexDF = None, include_deleted: bool = False):
+    def _build_metadata_query(
+        self, sql, idx: Optional[IndexDF] = None, include_deleted: bool = False
+    ):
         if idx is not None:
             if len(self.primary_keys) == 0:
                 # Когда ключей нет - не делаем ничего
                 pass
 
             elif len(self.primary_keys) == 1:
                 # Когда ключ один - сравниваем напрямую
                 key = self.primary_keys[0]
-                sql = sql.where(
-                    self.sql_table.c[key].in_(idx[key].to_list())
-                )
+                sql = sql.where(self.sql_table.c[key].in_(idx[key].to_list()))
 
             else:
                 # Когда ключей много - сравниваем через tuple
-                keys = tuple_(*[
-                    self.sql_table.c[key]
-                    for key in self.primary_keys
-                ])
-
-                sql = sql.where(keys.in_([
-                    tuple([r[key] for key in self.primary_keys])  # type: ignore
-                    for r in idx.to_dict(orient='records')
-                ]))
+                keys = tuple_(*[self.sql_table.c[key] for key in self.primary_keys])
+
+                sql = sql.where(
+                    keys.in_(
+                        [
+                            tuple([r[key] for key in self.primary_keys])  # type: ignore
+                            for r in idx.to_dict(orient="records")
+                        ]
+                    )
+                )
 
         if not include_deleted:
             sql = sql.where(self.sql_table.c.delete_ts.is_(None))
 
         return sql
 
-    def get_metadata(self, idx: IndexDF = None, include_deleted: bool = False) -> MetadataDF:
-        '''
+    def get_metadata(
+        self, idx: Optional[IndexDF] = None, include_deleted: bool = False
+    ) -> MetadataDF:
+        """
         Получить датафрейм с метаданными.
 
         idx - опциональный фильтр по целевым строкам
         include_deleted - флаг, возвращать ли удаленные строки, по умолчанию = False
-        '''
+        """
 
         res = []
         sql = select(self.sql_schema)
 
         if idx is None:
             sql = self._build_metadata_query(sql, idx, include_deleted)
             return cast(MetadataDF, pd.read_sql_query(sql, con=self.dbconn.con))
@@ -142,23 +159,28 @@
         for chunk_idx in self._chunk_idx_df(idx):
             chunk_sql = self._build_metadata_query(sql, chunk_idx, include_deleted)
             res.append(pd.read_sql_query(chunk_sql, con=self.dbconn.con))
 
         if len(res) > 0:
             return cast(MetadataDF, pd.concat(res))
         else:
-            return cast(MetadataDF, pd.DataFrame(columns=[column.name for column in self.sql_schema]))
+            return cast(
+                MetadataDF,
+                pd.DataFrame(columns=[column.name for column in self.sql_schema]),
+            )
 
-    def get_metadata_size(self, idx: IndexDF = None, include_deleted: bool = False) -> int:
-        '''
+    def get_metadata_size(
+        self, idx: Optional[IndexDF] = None, include_deleted: bool = False
+    ) -> int:
+        """
         Получить количество строк метаданных.
 
         idx - опциональный фильтр по целевым строкам
         include_deleted - флаг, возвращать ли удаленные строки, по умолчанию = False
-        '''
+        """
 
         sql = select([func.count()]).select_from(self.sql_table)
         sql = self._build_metadata_query(sql, idx, include_deleted)
 
         res = self.dbconn.con.execute(sql).fetchone()
         return res[0]
 
@@ -167,49 +189,58 @@
         res_df = df[meta_keys]
 
         res_df = res_df.assign(
             hash=self._get_hash_for_df(df),
             create_ts=now,
             update_ts=now,
             process_ts=now,
-            delete_ts=None
+            delete_ts=None,
         )
 
         return cast(MetadataDF, res_df)
 
     def _get_meta_data_columns(self):
-        return self.primary_keys + list(self.meta_keys.values()) + [column.name for column in METADATA_SQL_SCHEMA]
+        return (
+            self.primary_keys
+            + list(self.meta_keys.values())
+            + [column.name for column in METADATA_SQL_SCHEMA]
+        )
 
     def _get_hash_for_df(self, df) -> pd.DataFrame:
-        return (
-            df
-            .apply(lambda x: str(list(x)), axis=1)
-            .apply(lambda x: int.from_bytes(CityHash32(x).to_bytes(4, 'little'), 'little', signed=True))
+        return df.apply(lambda x: str(list(x)), axis=1).apply(
+            lambda x: int.from_bytes(
+                CityHash32(x).to_bytes(4, "little"), "little", signed=True
+            )
         )
 
     # Fix numpy types in Index
     # FIXME разобраться, что это за грязный хак
     def _get_sql_param(self, param):
         return param.item() if hasattr(param, "item") else param
 
-    def get_existing_idx(self, idx: IndexDF = None) -> IndexDF:
+    def get_existing_idx(self, idx: Optional[IndexDF] = None) -> IndexDF:
         sql = select(self.sql_schema)
 
         if idx is not None:
-            idx_cols = list(set(idx.columns) & set(self.primary_keys))
+            if len(idx.index) == 0:
+                # Empty index -> empty result
+                return cast(IndexDF, pd.DataFrame(
+                    columns=[column.name for column in self.sql_schema]
+                ))
+            idx_cols = list(set(idx.columns.tolist()) & set(self.primary_keys))
 
             if not idx_cols:
                 raise ValueError("Index does not contain any primary key ")
 
             row_queries = []
 
             # FIXME поправить на сравнение кортежей
             for _, row in idx.iterrows():
                 and_params = [
-                    self.sql_table.c[key] == self._get_sql_param(row[key])
+                    self.sql_table.c[key] == self._get_sql_param(row[key])  # type: ignore
                     for key in idx_cols
                     if key in self.primary_keys
                 ]
                 and_query = and_(*and_params)
                 row_queries.append(and_query)
 
             sql = sql.where(or_(*row_queries))
@@ -222,101 +253,101 @@
         )
 
         return data_to_index(res_df, self.primary_keys)
 
     def get_table_debug_info(self) -> TableDebugInfo:
         return TableDebugInfo(
             name=self.name,
-            size=self.dbconn.con.execute(select([func.count()]).select_from(self.sql_table)).fetchone()[0]
+            size=self.dbconn.con.execute(
+                select([func.count()]).select_from(self.sql_table)
+            ).fetchone()[0],
         )
 
     # TODO Может быть переделать работу с метадатой на контекстный менеджер?
     # FIXME поправить возвращаемые структуры данных, _meta_df должны содержать только _meta колонки
     def get_changes_for_store_chunk(
-        self,
-        data_df: DataDF,
-        now: float = None
+        self, data_df: DataDF, now: Optional[float] = None
     ) -> Tuple[DataDF, DataDF, MetadataDF, MetadataDF]:
-        '''
+        """
         Анализирует блок данных data_df, выделяет строки new_ которые нужно добавить и строки changed_ которые нужно обновить
 
         Returns tuple:
             new_data_df     - строки данных, которые нужно добавить
             changed_data_df - строки данных, которые нужно изменить
             new_meta_df     - строки метаданных, которые нужно добавить
             changed_meta_df - строки метаданных, которые нужно изменить
-        '''
+        """
 
         if now is None:
             now = time.time()
 
         # получить meta по чанку
-        existing_meta_df = self.get_metadata(data_to_index(data_df, self.primary_keys), include_deleted=True)
+        existing_meta_df = self.get_metadata(
+            data_to_index(data_df, self.primary_keys), include_deleted=True
+        )
         data_cols = list(data_df.columns)
         meta_cols = self._get_meta_data_columns()
 
         # Дополняем данные методанными
         merged_df = pd.merge(
             data_df.assign(data_hash=self._get_hash_for_df(data_df)),
             existing_meta_df,
-            how='left',
+            how="left",
             left_on=self.primary_keys,
             right_on=self.primary_keys,
-            suffixes=('', '_exist')
+            suffixes=("", "_exist"),
         )
 
-        new_idx = (merged_df['hash'].isna() | merged_df['delete_ts'].notnull())
+        new_idx = merged_df["hash"].isna() | merged_df["delete_ts"].notnull()
 
         # Ищем новые записи
-        new_df = data_df.loc[new_idx.values, data_cols]
+        new_df = data_df.loc[new_idx.values, data_cols]  # type: ignore
 
         # Создаем мета данные для новых записей
-        new_meta_data_df = merged_df.loc[merged_df['hash'].isna().values, data_cols]
+        new_meta_data_df = merged_df.loc[merged_df["hash"].isna().values, data_cols]  # type: ignore
         new_meta_df = self._make_new_metadata_df(now, new_meta_data_df)
 
         # Ищем изменившиеся записи
         changed_idx = (
-            (merged_df['hash'].notna()) &
-            (merged_df['delete_ts'].isnull()) &
-            (merged_df['hash'] != merged_df['data_hash'])
+            (merged_df["hash"].notna())
+            & (merged_df["delete_ts"].isnull())
+            & (merged_df["hash"] != merged_df["data_hash"])
         )
-        changed_df = merged_df.loc[changed_idx.values, data_cols]
+        changed_df = merged_df.loc[changed_idx.values, data_cols]  # type: ignore
 
         # Меняем мета данные для существующих записей
-        changed_meta_idx = (
-            (merged_df['hash'].notna()) &
-            (merged_df['hash'] != merged_df['data_hash']) |
-            (merged_df['delete_ts'].notnull())
-        )
-        changed_meta_df = merged_df.loc[merged_df['hash'].notna(), :].copy()
-
-        changed_meta_df.loc[changed_meta_idx, 'update_ts'] = now
-        changed_meta_df['process_ts'] = now
-        changed_meta_df['delete_ts'] = None
-        changed_meta_df['hash'] = changed_meta_df['data_hash']
+        changed_meta_idx = (merged_df["hash"].notna()) & (
+            merged_df["hash"] != merged_df["data_hash"]
+        ) | (merged_df["delete_ts"].notnull())
+        changed_meta_df = merged_df.loc[merged_df["hash"].notna(), :].copy()
+
+        changed_meta_df.loc[changed_meta_idx, "update_ts"] = now
+        changed_meta_df["process_ts"] = now
+        changed_meta_df["delete_ts"] = None
+        changed_meta_df["hash"] = changed_meta_df["data_hash"]
 
         return (
             cast(DataDF, new_df),
             cast(DataDF, changed_df),
             cast(MetadataDF, new_meta_df),
             cast(MetadataDF, changed_meta_df[meta_cols]),
         )
 
     def _insert_rows(self, df: MetadataDF) -> None:
         if len(df) > 0:
-            logger.debug(f'Inserting {len(df)} rows into {self.name} data')
+            logger.debug(f"Inserting {len(df)} rows into {self.name} data")
 
             df.to_sql(
                 name=self.sql_table.name,
                 con=self.dbconn.con,
                 schema=self.dbconn.schema,
-                if_exists='append',
+                if_exists="append",
                 index=False,
                 chunksize=1000,
-                method='multi',
+                method="multi",
                 dtype=sql_schema_to_sqltype(self.sql_schema),
             )
 
     def _delete_rows(self, df: MetadataDF) -> None:
         if len(df) == 0:
             return
 
@@ -329,61 +360,73 @@
                 key = self.primary_keys[0]
                 chunk_sql = sql.where(
                     self.sql_table.c[key].in_(chunk_idx[key].to_list())
                 )
 
             else:
                 # Когда ключей много - сравниваем через tuple
-                keys = tuple_(*[
-                    self.sql_table.c[key]
-                    for key in self.primary_keys
-                ])
-
-                chunk_sql = sql.where(keys.in_([
-                    tuple([r[key] for key in self.primary_keys])  # type: ignore
-                    for r in chunk_idx.to_dict(orient='records')
-                ]))
+                keys = tuple_(*[self.sql_table.c[key] for key in self.primary_keys])
+
+                chunk_sql = sql.where(
+                    keys.in_(
+                        [
+                            tuple([r[key] for key in self.primary_keys])  # type: ignore
+                            for r in chunk_idx.to_dict(orient="records")
+                        ]
+                    )
+                )
 
             self.dbconn.con.execute(chunk_sql)
 
     def _update_existing_metadata_rows(self, df: MetadataDF) -> None:
         if len(df) == 0:
             return
 
-        table = f'{self.dbconn.schema}.{self.sql_table.name}' if self.dbconn.schema else self.sql_table.name
-        values_table = f'{self.sql_table.name}_values'
+        table = (
+            f"{self.dbconn.schema}.{self.sql_table.name}"
+            if self.dbconn.schema
+            else self.sql_table.name
+        )
+        values_table = f"{self.sql_table.name}_values"
         columns = [column.name for column in self.sql_schema]
         update_columns = set(columns) - set(self.primary_keys)
 
-        update_expression = ', '.join([f'{column}={values_table}.{column}'
-                                       for column in update_columns])
+        update_expression = ", ".join(
+            [f"{column}={values_table}.{column}" for column in update_columns]
+        )
 
-        where_expressiom = ' AND '.join([f'{table}.{key} = {values_table}.{key}'
-                                         for key in self.primary_keys])
+        where_expressiom = " AND ".join(
+            [f"{table}.{key} = {values_table}.{key}" for key in self.primary_keys]
+        )
 
         for chunk_df in self._chunk_idx_df(df):
             params_df = chunk_df.reset_index()[columns]
             values_params = []
             params = {}
 
             for index, row in params_df.iterrows():
-                row_values = [f'CAST(:{column.name}_{index} AS {column.type})' for column in self.sql_schema]
-                row_params = {f'{key}_{index}': row[key] for key in row.keys()}
+                row_values = [
+                    f"CAST(:{column.name}_{index} AS {column.type})"
+                    for column in self.sql_schema
+                ]
+                row_params = {f"{key}_{index}": row[key] for key in row.keys()}
 
                 values_params.append(f'({", ".join(row_values)})')
                 params.update(row_params)
 
-            stmt = text(f"""
+            stmt = text(
+                f"""
                 UPDATE {table}
                 SET {update_expression}
                 FROM (
                     VALUES {", ".join(values_params)}
                 ) AS {values_table} ({', '.join(columns)})
                 WHERE {where_expressiom}
-            """)
+            """
+            )
 
             self.dbconn.con.execution_options(compiled_cache=None).execute(stmt, params)
 
     # TODO объединить
     def insert_meta_for_store_chunk(self, new_meta_df: MetadataDF) -> None:
         if len(new_meta_df) > 0:
             self._insert_rows(new_meta_df)
@@ -395,52 +438,52 @@
             else:
                 self._delete_rows(changed_meta_df)
                 self._insert_rows(changed_meta_df)
 
     def mark_rows_deleted(
         self,
         deleted_idx: IndexDF,
-        now: float = None,
+        now: Optional[float] = None,
     ) -> None:
         if len(deleted_idx) > 0:
             if now is None:
                 now = time.time()
 
             meta_df = self.get_metadata(deleted_idx)
 
             meta_df["hash"] = 0
             meta_df["delete_ts"] = now
             meta_df["update_ts"] = now
             meta_df["process_ts"] = now
 
             self.update_meta_for_store_chunk(meta_df)
 
-    def get_stale_idx(self, process_ts: float, run_config: RunConfig = None) -> Iterator[IndexDF]:
+    def get_stale_idx(
+        self, process_ts: float, run_config: Optional[RunConfig] = None
+    ) -> Iterator[IndexDF]:
         idx_cols = [self.sql_table.c[key] for key in self.primary_keys]
         sql = select(idx_cols).where(
             and_(
                 self.sql_table.c.process_ts < process_ts,
-                self.sql_table.c.delete_ts.is_(None)
+                self.sql_table.c.delete_ts.is_(None),
             )
         )
 
-        sql = sql_apply_runconfig_filter(sql, self.sql_table, self.primary_keys, run_config)
+        sql = sql_apply_runconfig_filter(
+            sql, self.sql_table, self.primary_keys, run_config
+        )
 
         return cast(
             Iterator[IndexDF],
-            pd.read_sql_query(
-                sql,
-                con=self.dbconn.con,
-                chunksize=1000
-            )
+            pd.read_sql_query(sql, con=self.dbconn.con, chunksize=1000),
         )
 
 
 class MetaTableData:
-    def __init__(self, tbl: MetaTable, sql_prefix: str = '') -> None:
+    def __init__(self, tbl: MetaTable, sql_prefix: str = "") -> None:
         self.primary_keys = set(tbl.primary_keys)
         self.meta_keys = set(tbl.meta_keys.keys())
         self.meta_column_names = tbl.meta_keys
         self.sql_table = tbl.sql_table.alias(f"{sql_prefix}_{tbl.name}")
 
     def get_keys(self):
         return self.primary_keys | self.meta_keys
```

### Comparing `datapipe_core-0.11.9a6/datapipe/run_config.py` & `datapipe_core-0.12.0a2/datapipe/run_config.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     # если не пуст, то во время запуска обрабатываются только те строки,
     # которые строго соответствуют фильтру
     # (в случае, если у таблицы есть идентификатор с совпадающим именем).
     filters: LabelDict = field(default_factory=dict)
     labels: LabelDict = field(default_factory=dict)
 
     @classmethod
-    def add_labels(cls, rc: Optional['RunConfig'], labels: LabelDict) -> 'RunConfig':
+    def add_labels(cls, rc: Optional["RunConfig"], labels: LabelDict) -> "RunConfig":
         if rc is not None:
             return RunConfig(
                 filters=rc.filters,
                 labels={**rc.labels, **labels},
             )
         else:
             return RunConfig(labels=labels)
```

### Comparing `datapipe_core-0.11.9a6/datapipe/store/database.py` & `datapipe_core-0.12.0a2/datapipe/store/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,88 +10,90 @@
 from sqlalchemy.pool import SingletonThreadPool
 from sqlalchemy.schema import SchemaItem
 from sqlalchemy.sql.base import SchemaEventTarget
 from sqlalchemy.sql.expression import delete, select, tuple_
 
 from datapipe.run_config import RunConfig
 from datapipe.store.table_store import TableStore
-from datapipe.types import (DataDF, DataSchema, IndexDF, MetaSchema, TAnyDF,
-                            data_to_index)
+from datapipe.types import (
+    DataDF,
+    DataSchema,
+    IndexDF,
+    MetaSchema,
+    TAnyDF,
+    data_to_index,
+)
 
 logger = logging.getLogger("datapipe.store.database")
 tracer = trace.get_tracer("datapipe.store.database")
 
 
 SCHEMA_TO_DTYPE_LOOKUP = {
     String: str,
     Integer: int,
 }
 
 
 def sql_schema_to_dtype(schema: List[Column]) -> Dict[str, Any]:
-    return {
-        i.name: SCHEMA_TO_DTYPE_LOOKUP[i.type.__class__]
-        for i in schema
-    }
+    return {i.name: SCHEMA_TO_DTYPE_LOOKUP[i.type.__class__] for i in schema}
 
 
 def sql_schema_to_sqltype(schema: List[Column]) -> Dict[str, Any]:
-    return {
-        i.name: i.type for i in schema
-    }
+    return {i.name: i.type for i in schema}
 
 
 class DBConn:
-    def __init__(self, connstr: str, schema: str = None):
+    def __init__(self, connstr: str, schema: Optional[str] = None):
         self._init(connstr, schema)
 
     def _init(self, connstr: str, schema: Optional[str]) -> None:
         self.connstr = connstr
         self.schema = schema
 
-        if connstr.startswith('sqlite'):
+        if connstr.startswith("sqlite"):
             self.supports_update_from = False
         else:
             # Assume relatively new Postgres
             self.supports_update_from = True
 
         self.con = create_engine(
             connstr,
             poolclass=SingletonThreadPool,
         )
 
-        SQLAlchemyInstrumentor().instrument(
-            engine=self.con
-        )
+        SQLAlchemyInstrumentor().instrument(engine=self.con)
 
         self.sqla_metadata = MetaData(schema=schema)
 
     def __getstate__(self):
         return {
-            'connstr': self.connstr,
-            'schema': self.schema,
+            "connstr": self.connstr,
+            "schema": self.schema,
         }
 
     def __setstate__(self, state):
-        self._init(state['connstr'], state['schema'])
+        self._init(state["connstr"], state["schema"])
 
 
-def sql_apply_runconfig_filter(sql: select, table: Table, primary_keys: List[str], run_config: RunConfig = None) -> select:
+def sql_apply_runconfig_filter(
+    sql: select,
+    table: Table,
+    primary_keys: List[str],
+    run_config: Optional[RunConfig] = None,
+) -> select:
     if run_config is not None:
         for k, v in run_config.filters.items():
             if k in primary_keys:
-                sql = sql.where(
-                    table.c[k] == v
-                )
+                sql = sql.where(table.c[k] == v)
 
     return sql
 
 
 class MetaKey(SchemaItem):
-    def __init__(self, target_name: str = None) -> None:
+    def __init__(self, target_name: Optional[str] = None) -> None:
         self.target_name = target_name
 
     def _set_parent(self, parent: SchemaEventTarget, **kw: Any) -> None:
         self.parent = parent
         self.parent.meta_key = self
 
         if not self.target_name:
@@ -101,114 +103,116 @@
     def get_property_name(cls) -> str:
         return "meta_key"
 
 
 class TableStoreDB(TableStore):
     def __init__(
         self,
-        dbconn: Union['DBConn', str],
+        dbconn: Union["DBConn", str],
         name: str,
         data_sql_schema: List[Column],
         create_table: bool = False,
     ) -> None:
         if isinstance(dbconn, str):
             self.dbconn = DBConn(dbconn)
         else:
             self.dbconn = dbconn
         self.name = name
 
         self.data_sql_schema = data_sql_schema
 
         self.data_table = Table(
-            self.name, self.dbconn.sqla_metadata,
+            self.name,
+            self.dbconn.sqla_metadata,
             *[copy.copy(i) for i in self.data_sql_schema],
-            extend_existing=True
+            extend_existing=True,
         )
 
         if create_table:
             self.data_table.create(self.dbconn.con, checkfirst=True)
 
     def get_schema(self) -> DataSchema:
         return self.data_sql_schema
 
     def get_primary_schema(self) -> DataSchema:
         return [column for column in self.data_sql_schema if column.primary_key]
 
     def get_meta_schema(self) -> MetaSchema:
         meta_key_prop = MetaKey.get_property_name()
-        return [column for column in self.data_sql_schema if hasattr(column, meta_key_prop)]
+        return [
+            column for column in self.data_sql_schema if hasattr(column, meta_key_prop)
+        ]
 
     def _chunk_size(self):
         # Magic number derived empirically. See
         # https://github.com/epoch8/datapipe/issues/178 for details.
         #
         # TODO Investigate deeper how does stack in Postgres work
         return 5000 // len(self.primary_keys)
 
     def _chunk_idx_df(self, idx: TAnyDF) -> Iterator[TAnyDF]:
-        '''
+        """
         Split IndexDF to chunks acceptable for typical Postgres configuration.
         See `_chunk_size` for detatils.
-        '''
+        """
 
         CHUNK_SIZE = self._chunk_size()
 
         for chunk_no in range(int(math.ceil(len(idx) / CHUNK_SIZE))):
-            chunk_idx = idx.iloc[chunk_no*CHUNK_SIZE:(chunk_no+1)*CHUNK_SIZE, :]
+            chunk_idx = idx.iloc[chunk_no * CHUNK_SIZE : (chunk_no + 1) * CHUNK_SIZE, :]
 
             yield cast(TAnyDF, chunk_idx)
 
     def _apply_where_expression(self, sql, idx: IndexDF):
         if len(self.primary_keys) == 1:
             # Когда ключ один - сравниваем напрямую
             key = self.primary_keys[0]
-            sql = sql.where(
-                self.data_table.c[key].in_(idx[key].to_list())
-            )
+            sql = sql.where(self.data_table.c[key].in_(idx[key].to_list()))
 
         else:
             # Когда ключей много - сравниваем через tuple
-            keys = tuple_(*[
-                self.data_table.c[key]
-                for key in self.primary_keys
-            ])
-
-            sql = sql.where(keys.in_([
-                tuple([r[key] for key in self.primary_keys])  # type: ignore
-                for r in idx.to_dict(orient='records')
-            ]))
+            keys = tuple_(*[self.data_table.c[key] for key in self.primary_keys])
+
+            sql = sql.where(
+                keys.in_(
+                    [
+                        tuple([r[key] for key in self.primary_keys])  # type: ignore
+                        for r in idx.to_dict(orient="records")
+                    ]
+                )
+            )
 
         return sql
 
     def delete_rows(self, idx: IndexDF) -> None:
         if idx is None or len(idx.index) == 0:
             return
 
-        logger.debug(f'Deleting {len(idx.index)} rows from {self.name} data')
+        logger.debug(f"Deleting {len(idx.index)} rows from {self.name} data")
 
         for chunk_idx in self._chunk_idx_df(idx):
             sql = self._apply_where_expression(delete(self.data_table), chunk_idx)
             self.dbconn.con.execute(sql)
 
     def insert_rows(self, df: DataDF) -> None:
         if df.empty:
             return
 
         self.delete_rows(data_to_index(df, self.primary_keys))
-        logger.debug(f'Inserting {len(df)} rows into {self.name} data')
+        logger.debug(f"Inserting {len(df)} rows into {self.name} data")
 
         for chunk_df in self._chunk_idx_df(df):
             chunk_df.to_sql(
                 name=self.name,
                 con=self.dbconn.con,
                 schema=self.dbconn.schema,
-                if_exists='append',
+                if_exists="append",
                 index=False,
                 chunksize=1000,
-                method='multi',
+                method="multi",
                 dtype=sql_schema_to_sqltype(self.data_sql_schema),
             )
 
     def update_rows(self, df: DataDF) -> None:
         self.insert_rows(df)
 
     # Fix numpy types in IndexDF
@@ -217,35 +221,38 @@
 
     def read_rows(self, idx: Optional[IndexDF] = None) -> pd.DataFrame:
         sql = select(self.data_table.c)
 
         if idx is not None:
             if len(idx.index) == 0:
                 # Empty index -> empty result
-                return pd.DataFrame(columns=[column.name for column in self.data_sql_schema])
+                return pd.DataFrame(
+                    columns=[column.name for column in self.data_sql_schema]
+                )
 
             res = []
 
             for chunk_idx in self._chunk_idx_df(idx):
                 chunk_sql = self._apply_where_expression(sql, chunk_idx)
                 chunk_df = pd.read_sql_query(chunk_sql, con=self.dbconn.con)
 
                 res.append(chunk_df)
 
             return pd.concat(res, ignore_index=True)
 
         else:
-            return pd.read_sql_query(
-                sql,
-                con=self.dbconn.con
-            )
+            return pd.read_sql_query(sql, con=self.dbconn.con)
 
-    def read_rows_meta_pseudo_df(self, chunksize: int = 1000, run_config: RunConfig = None) -> Iterator[DataDF]:
+    def read_rows_meta_pseudo_df(
+        self, chunksize: int = 1000, run_config: Optional[RunConfig] = None
+    ) -> Iterator[DataDF]:
         sql = select(self.data_table.c)
 
-        sql = sql_apply_runconfig_filter(sql, self.data_table, self.primary_keys, run_config)
+        sql = sql_apply_runconfig_filter(
+            sql, self.data_table, self.primary_keys, run_config
+        )
 
         return pd.read_sql_query(
             sql,
             con=self.dbconn.con.execution_options(stream_results=True),
-            chunksize=chunksize
+            chunksize=chunksize,
         )
```

### Comparing `datapipe_core-0.11.9a6/datapipe/store/filedir.py` & `datapipe_core-0.12.0a2/datapipe/store/filedir.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,90 +24,84 @@
         raise NotImplementedError
 
     def dump(self, obj: Dict[str, Any], f: IO) -> None:
         raise NotImplementedError
 
 
 class JSONFile(ItemStoreFileAdapter):
-    '''
+    """
     Converts each JSON file into Pandas record
-    '''
+    """
 
-    mode = 't'
+    mode = "t"
 
     def __init__(self, **dump_params) -> None:
         self.dump_params = dump_params
 
     def load(self, f: IO) -> Dict[str, Any]:
         return json.load(f)
 
     def dump(self, obj: Dict[str, Any], f: IO) -> None:
         return json.dump(obj, f, **self.dump_params)
 
 
 class PILFile(ItemStoreFileAdapter):
-    '''
+    """
     Uses `image` column with PIL.Image for save/load
-    '''
+    """
 
-    mode = 'b'
+    mode = "b"
 
     def __init__(self, format: str, **dump_params) -> None:
         self.format = format
         self.dump_params = dump_params
 
     def load(self, f: IO) -> Dict[str, Any]:
         im = Image.open(f)
         im.load()
-        return {'image': im}
+        return {"image": im}
 
     def dump(self, obj: Dict[str, Any], f: IO) -> None:
-        im: Image.Image = obj['image']
+        im: Image.Image = obj["image"]
         im.save(f, format=self.format, **self.dump_params)
 
 
 def _pattern_to_attrnames(pat: str) -> List[str]:
-    attrnames = re.findall(r'\{([^/]+?)\}', pat)
+    attrnames = re.findall(r"\{([^/]+?)\}", pat)
 
     assert len(attrnames) > 0, "The scheme is not valid."
     if len(attrnames) >= 2:
         duplicates_attrnames = list(duplicates(attrnames))
         assert len(duplicates_attrnames) == 0, f"Some keys are repeated: {duplicates_attrnames}. Rename them."
 
     return attrnames
 
 
 def _pattern_to_patterns_or(pat) -> List[str]:
-    pattern_or = re.compile(r'(?P<or>\(([a-zA-Z0-9]+\|)+[a-zA-Z0-9]+\))')
+    pattern_or = re.compile(r"(?P<or>\(([a-zA-Z0-9]+\|)+[a-zA-Z0-9]+\))")
     # Ищем вхождения вида (aaa|bbb|ccc), в виду list of list [[aaa, bbb, ccc], [ddd, eee], ...]
-    values = [
-        list(dict.fromkeys(match.group('or')[1:-1].split('|')))
-        for match in pattern_or.finditer(pat)
-    ]
+    values = [list(dict.fromkeys(match.group("or")[1:-1].split("|"))) for match in pattern_or.finditer(pat)]
     # Всевозможные комбинации для замены [[aaa, ddd], [aaa, eee], [bbb, ddd], ...]
     possible_combinatios_values = [list(combination) for combination in itertools.product(*values)]
     # Получаем всевозможные списки шаблонов из комбинаций
-    filename_patterns = [
-        re.sub(pattern_or, Replacer(combination), pat)
-        for combination in possible_combinatios_values
-    ]
+    filename_patterns = [re.sub(pattern_or, Replacer(combination), pat) for combination in possible_combinatios_values]
     return filename_patterns
 
 
 def _pattern_to_glob(pat: str) -> str:
-    return re.sub(r'\{([^/]+?)\}', '*', pat)  # Меняем все вхождения {id1}_{id2} в звездочки *_*
+    return re.sub(r"\{([^/]+?)\}", "*", pat)  # Меняем все вхождения {id1}_{id2} в звездочки *_*
 
 
 def _pattern_to_match(pat: str) -> str:
     # TODO сделать трансформацию правильнее
     # * -> r'[^/]+'
     # ** -> r'([^/]+/)*?[^/]+'
 
-    pat = re.sub(r'\*\*?', r'([^/]+/)*[^/]+', pat)  # Меняем все вхождения * и ** в произвольные символы
-    pat = re.sub(r'\{([^/]+?)\}', r'(?P<\1>[^/]+?)', pat)  # Меняем все вхождения вида {id} на непустые послед. символов
+    pat = re.sub(r"\*\*?", r"([^/]+/)*[^/]+", pat)  # Меняем все вхождения * и ** в произвольные символы
+    pat = re.sub(r"\{([^/]+?)\}", r"(?P<\1>[^/]+?)", pat)  # Меняем все вхождения вида {id} на непустые послед. символов
     pat = f"{pat}\\Z"  # Учитываем конец строки
     return pat
 
 
 class Replacer:
     def __init__(self, values: List[str]):
         self.counter = -1
@@ -120,18 +114,18 @@
 
 class TableStoreFiledir(TableStore):
     def __init__(
         self,
         filename_pattern: Union[str, Path],
         adapter: ItemStoreFileAdapter,
         add_filepath_column: bool = False,
-        primary_schema: DataSchema = None,
+        primary_schema: Optional[DataSchema] = None,
         read_data: bool = True,
         readonly: Optional[bool] = None,
-        enable_rm: bool = False
+        enable_rm: bool = False,
     ):
         """
         При построении `TableStoreFiledir` есть два способа указать схему
         индексов:
 
         1. Явный - в конструктор передается `primary_schema`, которая должна
            содержать все поля, упоминаемые в `filename_pattern`
@@ -163,15 +157,15 @@
 
         enable_rm -- если True, включить удаление файлов
         """
 
         self.protocol, path = fsspec.core.split_protocol(filename_pattern)
         self.filesystem = fsspec.filesystem(self.protocol)
 
-        if self.protocol is None or self.protocol == 'file':
+        if self.protocol is None or self.protocol == "file":
             filename_pattern = str(Path(path).resolve())
             filename_pattern_for_match = filename_pattern
             self.protocol_str = "" if self.protocol is None else "file://"
         else:
             filename_pattern = str(filename_pattern)
             filename_pattern_for_match = path
             self.protocol_str = f"{self.protocol}://"
@@ -180,55 +174,42 @@
         self.attrnames = _pattern_to_attrnames(filename_pattern)
         self.filename_glob = [_pattern_to_glob(pat) for pat in self.filename_patterns]
         self.filename_match = _pattern_to_match(filename_pattern_for_match)
 
         # Multiply extensions check
         if len(self.filename_glob) >= 2:
             if readonly is not None and not readonly:
-                raise ValueError(
-                    "When `readonly=False`, in filename_pattern shouldn't be several extensions."
-                )
+                raise ValueError("When `readonly=False`, in filename_pattern shouldn't be several extensions.")
             elif readonly:
                 readonly = True
         # Any * and ** pattern check
-        if '*' in path:
+        if "*" in path:
             if readonly is not None and not readonly:
-                raise ValueError(
-                    "When `readonly=False`, in filename_pattern shouldn't be any `*` characters."
-                )
+                raise ValueError("When `readonly=False`, in filename_pattern shouldn't be any `*` characters.")
             elif readonly is None:
                 readonly = True
         elif readonly is None:
             readonly = False
 
         self.readonly = readonly
         self.enable_rm = enable_rm
 
         self.adapter = adapter
         self.add_filepath_column = add_filepath_column
         self.read_data = read_data
 
-        type_to_cls = {
-            String: str,
-            Integer: int
-        }
+        type_to_cls = {String: str, Integer: int}
 
         if primary_schema is not None:
             assert sorted(self.attrnames) == sorted(i.name for i in primary_schema)
             assert all([isinstance(column.type, (String, Integer)) for column in primary_schema])
             self.primary_schema = primary_schema
         else:
-            self.primary_schema = [
-                Column(attrname, String(100), primary_key=True)
-                for attrname in self.attrnames
-            ]
-        self.attrname_to_cls = {
-            column.name: type_to_cls[type(column.type)]
-            for column in self.primary_schema
-        }
+            self.primary_schema = [Column(attrname, String(100), primary_key=True) for attrname in self.attrnames]
+        self.attrname_to_cls = {column.name: type_to_cls[type(column.type)] for column in self.primary_schema}
 
     def get_primary_schema(self) -> DataSchema:
         return self.primary_schema
 
     def get_meta_schema(self) -> MetaSchema:
         return []
 
@@ -238,23 +219,21 @@
 
         assert not self.readonly
 
         for row_idx in idx.index:
             attrnames_series = idx.loc[row_idx, self.attrnames]
             assert isinstance(attrnames_series, pd.Series)
 
-            _, path = fsspec.core.split_protocol(
-                self._filenames_from_idxs_values(attrnames_series.tolist())[0]
-            )
+            attrnames = cast(List[str], attrnames_series.tolist())
+
+            _, path = fsspec.core.split_protocol(self._filenames_from_idxs_values(attrnames)[0])
             self.filesystem.rm(path)
 
     def _filenames_from_idxs_values(self, idxs_values: List[str]) -> List[str]:
-        return [
-            re.sub(r'\{([^/]+?)\}', Replacer(idxs_values), pat) for pat in self.filename_patterns
-        ]
+        return [re.sub(r"\{([^/]+?)\}", Replacer(idxs_values), pat) for pat in self.filename_patterns]
 
     def _idxs_values_from_filepath(self, filepath: str) -> Dict[str, Any]:
         _, filepath = fsspec.core.split_protocol(filepath)
         m = re.match(self.filename_match, filepath)
         assert m is not None, f"Filepath {filepath} does not match the pattern {self.filename_match}"
 
         data = {}
@@ -262,98 +241,95 @@
             data[attrname] = self.attrname_to_cls[attrname](m.group(attrname))
 
         return data
 
     def _assert_key_values(self, filepath: str, idxs_values: List[str]):
         idx_data = self._idxs_values_from_filepath(filepath)
         idxs_values_np = np.array(idxs_values)
-        idxs_values_parsed_from_filepath = np.array(
-            [idx_data[attrname] for attrname in self.attrnames]
-        )
+        idxs_values_parsed_from_filepath = np.array([idx_data[attrname] for attrname in self.attrnames])
 
-        assert (
-            len(idxs_values_np) == len(idxs_values_parsed_from_filepath) and
-
-            np.all(idxs_values_np == idxs_values_parsed_from_filepath)
+        assert len(idxs_values_np) == len(idxs_values_parsed_from_filepath) and np.all(
+            idxs_values_np == idxs_values_parsed_from_filepath
         ), (
             "Multiply indexes have complex contradictory values, so that it couldn't unambiguously name the files. "
             "This is most likely due to imperfect separators between {id} keys in the scheme or "
-            " idxs types differences. ", f"{idxs_values_np=} not equals {idxs_values_parsed_from_filepath=}"
+            " idxs types differences. ",
+            f"{idxs_values_np=} not equals {idxs_values_parsed_from_filepath=}",
         )
 
     def insert_rows(self, df: pd.DataFrame, adapter: Optional[ItemStoreFileAdapter] = None) -> None:
         if df.empty:
             return
         assert not self.readonly
         if adapter is None:
             adapter = self.adapter
 
         # WARNING: Здесь я поставил .drop(columns=self.attrnames), тк ключи будут хранится снаружи, в имени
         for row_idx, data in zip(
-            df.index, cast(List[Dict[str, Any]], df.drop(columns=self.attrnames).to_dict('records'))
+            df.index,
+            cast(List[Dict[str, Any]], df.drop(columns=self.attrnames).to_dict("records")),
         ):
             attrnames_series = df.loc[row_idx, self.attrnames]
             assert isinstance(attrnames_series, pd.Series)
 
             idxs_values = attrnames_series.tolist()
             filepath = self._filenames_from_idxs_values(idxs_values)[0]
 
             # Проверяем, что значения ключей не приведут к неоднозначному результату при парсинге регулярки
             self._assert_key_values(filepath, idxs_values)
 
-            with fsspec.open(filepath, f'w{self.adapter.mode}') as f:
+            with fsspec.open(filepath, f"w{self.adapter.mode}") as f:
                 self.adapter.dump(data, f)
 
     def _read_rows_fast(
         self,
         idx: IndexDF,
     ) -> DataDF:
         res = idx.copy()
         res["filepath"] = None
 
         for row_idx in idx.index:
             attrnames_series = idx.loc[row_idx, self.attrnames]
             assert isinstance(attrnames_series, pd.Series)
 
-            _, path = fsspec.core.split_protocol(
-                self._filenames_from_idxs_values(attrnames_series.tolist())[0]
-            )
+            attrnames = cast(List[str], attrnames_series.tolist())
+
+            _, path = fsspec.core.split_protocol(self._filenames_from_idxs_values(attrnames)[0])
 
             res.loc[row_idx, "filepath"] = f"{self.protocol_str}{path}"
 
         return res
 
     def read_rows(
         self,
-        idx: IndexDF = None,
+        idx: Optional[IndexDF] = None,
         read_data: Optional[bool] = None,
-        adapter: Optional[ItemStoreFileAdapter] = None
+        adapter: Optional[ItemStoreFileAdapter] = None,
     ) -> DataDF:
 
         if read_data is None:
             read_data = self.read_data
         if adapter is None:
             adapter = self.adapter
 
         if (not read_data) and (len(self.filename_patterns) == 1) and (idx is not None) and self.add_filepath_column:
             return self._read_rows_fast(idx)
 
         def _iterate_files():
             if idx is None:
-                for file_open in fsspec.open_files(self.filename_glob, f'r{adapter.mode}'):
+                for file_open in fsspec.open_files(self.filename_glob, f"r{adapter.mode}"):
                     yield file_open
             else:
                 filepaths_extenstions = [
-                    self._filenames_from_idxs_values(idx.loc[row_idx, self.attrnames])
-                    for row_idx in idx.index
+                    self._filenames_from_idxs_values(idx.loc[row_idx, self.attrnames]) for row_idx in idx.index
                 ]
                 for filepaths in filepaths_extenstions:
                     found_files = [
                         file_open
-                        for file_open in fsspec.open_files(filepaths, f'r{adapter.mode}')
+                        for file_open in fsspec.open_files(filepaths, f"r{adapter.mode}")
                         if self.filesystem.exists(file_open.path)
                     ]
                     if len(found_files) == 0:
                         raise FileNotFoundError(f"No such file: {' or '.join(filepaths)}")
                     elif len(found_files) > 1:
                         raise ValueError(
                             f"Some files are duplitcated as indexes in filepaths: {found_files}. "
@@ -377,71 +353,63 @@
                         f"Remove these keys from data."
                     )
 
                 idxs_values = self._idxs_values_from_filepath(file_open.path)
                 data.update(idxs_values)
 
                 if self.add_filepath_column:
-                    assert 'filepath' not in data, (
+                    assert "filepath" not in data, (
                         "The key 'filepath' is already exists in data. "
                         "Switch argument add_filepath_column to False or rename this key in input data."
                     )
-                    data['filepath'] = f"{self.protocol_str}{file_open.path}"
+                    data["filepath"] = f"{self.protocol_str}{file_open.path}"
 
                 df_records.append(data)
 
         df = pd.DataFrame(df_records)
 
         if df.empty:
             df = pd.DataFrame(columns=self.primary_keys)
 
         return df
 
-    def read_rows_meta_pseudo_df(self, chunksize: int = 1000, run_config: RunConfig = None) -> Iterator[DataDF]:
+    def read_rows_meta_pseudo_df(
+        self, chunksize: int = 1000, run_config: Optional[RunConfig] = None
+    ) -> Iterator[DataDF]:
         # FIXME реализовать чанкирование
 
         files = fsspec.open_files(self.filename_glob)
 
-        ids: Dict[str, List[str]] = {
-            attrname: []
-            for attrname in self.attrnames
-        }
+        ids: Dict[str, List[str]] = {attrname: [] for attrname in self.attrnames}
         ukeys = []
         filepaths = []
 
         for f in files:
             m = re.match(self.filename_match, f.path)
 
             assert m is not None
             for attrname in self.attrnames:
                 ids[attrname].append(m.group(attrname))
 
             ukeys.append(files.fs.ukey(f.path))
             filepaths.append(f"{self.protocol_str}{f.path}")
 
-        keys_values = [
-            (ids[attrname][i] for attrname in self.attrnames)
-            for i in range(len(ukeys))
-        ]
+        keys_values = [(ids[attrname][i] for attrname in self.attrnames) for i in range(len(ukeys))]
         duplicates_keys_values = list(duplicates(keys_values))
         assert len(duplicates_keys_values) == 0, (
             f"Some files are duplitcated as indexes in filepaths: {duplicates_keys_values}. "
             "Change the pattern or delete them."
         )
 
         if len(ids) > 0:
             pseudo_data_df = pd.DataFrame.from_records(
                 {
                     **ids,
-                    'ukey': ukeys,
-                    **({'filepath': filepaths} if self.add_filepath_column else {})
+                    "ukey": ukeys,
+                    **({"filepath": filepaths} if self.add_filepath_column else {}),
                 }
             )
-            yield pseudo_data_df.astype(object)
+
+            yield pseudo_data_df.astype(object)  # type: ignore # TODO fix typing issue
         else:
-            filepath_kw: Dict = {'filepath': []} if self.add_filepath_column else {}
-            yield pd.DataFrame(
-                {
-                    'ukey': [],
-                    **filepath_kw,
-                }
-            ).astype(object)
+            filepath_kw: Dict = {"filepath": []} if self.add_filepath_column else {}
+            yield pd.DataFrame({"ukey": [], **filepath_kw}).astype(object)  # type: ignore # TODO fix typing issue
```

### Comparing `datapipe_core-0.11.9a6/datapipe/store/milvus.py` & `datapipe_core-0.12.0a2/datapipe/store/milvus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 import pandas as pd
 
 from typing import Dict, List, Optional
-from pymilvus import connections, utility, CollectionSchema, Collection, FieldSchema, SearchResult
+from pymilvus import (
+    connections,
+    utility,
+    CollectionSchema,
+    Collection,
+    FieldSchema,
+    SearchResult,
+)
 
 from datapipe.types import DataSchema, MetaSchema, IndexDF, DataDF, data_to_index
 from datapipe.store.table_store import TableStore
 
 
 class MilvusStore(TableStore):
     def __init__(
         self,
         name: str,
         schema: List[FieldSchema],
         primary_db_schema: DataSchema,
         index_params: Dict,
         pk_field: str,
         embedding_field: str,
-        connection_details: Dict
+        connection_details: Dict,
     ):
         super().__init__()
         self.name = name
         self.schema = schema
         self.primary_db_schema = primary_db_schema
         self.index_params = index_params
         self.pk_field = pk_field
@@ -86,19 +93,15 @@
         names = [field.name for field in self.schema]
 
         result = self.query_search(f"{self.pk_field} in [{ids_joined}]", names)
 
         return pd.DataFrame.from_records(result)
 
     def vector_search(
-        self,
-        embeddings: List,
-        query_params: Dict,
-        expr: str,
-        limit: int
+        self, embeddings: List, query_params: Dict, expr: str, limit: int
     ) -> SearchResult:
         if not self._collection_loaded:
             self.collection.load()
             self._collection_loaded = True
 
         return self.collection.search(
             data=embeddings,
@@ -110,11 +113,8 @@
         )
 
     def query_search(self, expr: str, output_fields: List) -> List:
         if not self._collection_loaded:
             self.collection.load()
             self._collection_loaded = True
 
-        return self.collection.query(
-            expr=expr,
-            output_fields=output_fields
-        )
+        return self.collection.query(expr=expr, output_fields=output_fields)
```

### Comparing `datapipe_core-0.11.9a6/datapipe/store/pandas.py` & `datapipe_core-0.12.0a2/datapipe/store/pandas.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,33 +11,33 @@
 
 class TableStoreExcel(TableDataSingleFileStore, ABC):
     def load_file(self) -> Optional[pd.DataFrame]:
         of = fsspec.open(self.filename)
 
         if of.fs.exists(of.path):
             dtypes = sql_schema_to_dtype(self.primary_schema)
-            df = pd.read_excel(of.open(), engine='openpyxl', dtype=dtypes)
+            df = pd.read_excel(of.open(), engine="openpyxl", dtype=dtypes)
 
             return df
         else:
             return None
 
     def save_file(self, df: DataDF) -> None:
-        with fsspec.open(self.filename, 'wb+') as f:
-            df.to_excel(f, engine='openpyxl', index=False)
+        with fsspec.open(self.filename, "wb+") as f:
+            df.to_excel(f, engine="openpyxl", index=False)
 
 
 class TableStoreJsonLine(TableDataSingleFileStore):
     def load_file(self) -> Optional[pd.DataFrame]:
         of = fsspec.open(self.filename)
 
         if of.fs.exists(of.path):
             dtypes = sql_schema_to_dtype(self.primary_schema)
-            df = pd.read_json(of.open(), orient='records', lines=True, dtype=dtypes)
+            df = pd.read_json(of.open(), orient="records", lines=True, dtype=dtypes)
 
             return df
         else:
             return None
 
     def save_file(self, df: DataDF) -> None:
-        with fsspec.open(self.filename, 'w+') as f:
-            df.to_json(f, orient='records', lines=True, force_ascii=False)
+        with fsspec.open(self.filename, "w+") as f:
+            df.to_json(f, orient="records", lines=True, force_ascii=False)
```

### Comparing `datapipe_core-0.11.9a6/datapipe/store/redis.py` & `datapipe_core-0.12.0a2/datapipe/store/redis.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,46 +3,46 @@
 
 import pandas as pd
 from redis.client import Redis
 from sqlalchemy import Column
 
 from datapipe.store.database import MetaKey
 from datapipe.store.table_store import TableStore
-from datapipe.types import (DataDF, DataSchema, IndexDF, MetaSchema,
-                            data_to_index)
+from datapipe.types import DataDF, DataSchema, IndexDF, MetaSchema, data_to_index
 
 
 def _serialize(values):
     return json.dumps(values)
 
 
 def _deserialize(bytestring):
     return json.loads(bytestring)
 
 
 def _to_itertuples(df: DataDF, colnames):
-    return tuple(df[colnames].itertuples(index=False, name=None))
+    return list(df[colnames].itertuples(index=False, name=None))
 
 
 class RedisStore(TableStore):
     def __init__(
-        self,
-        connection: Union[Redis, str],
-        name: str,
-        data_sql_schema: List[Column]
+        self, connection: Union[Redis, str], name: str, data_sql_schema: List[Column]
     ) -> None:
 
         if isinstance(connection, str):
             self.redis_connection = Redis.from_url(connection, decode_responses=True)
         else:
             self.redis_connection = connection
         self.name = name
         self.data_sql_schema = data_sql_schema
-        self.prim_keys = [column.name for column in self.data_sql_schema if column.primary_key]
-        self.value_cols = [column.name for column in self.data_sql_schema if not column.primary_key]
+        self.prim_keys = [
+            column.name for column in self.data_sql_schema if column.primary_key
+        ]
+        self.value_cols = [
+            column.name for column in self.data_sql_schema if not column.primary_key
+        ]
 
     def insert_rows(self, df: DataDF) -> None:
         if df.empty:
             return
 
         # get rows as Iter[Tuple]
         key_rows = _to_itertuples(df, self.prim_keys)
@@ -56,42 +56,39 @@
         # удаляем существующие ключи
         if df.empty:
             df = pd.DataFrame(columns=[column.name for column in self.data_sql_schema])
         self.delete_rows(data_to_index(df, self.prim_keys))
         self.insert_rows(df)
 
     def read_rows(self, df_keys: Optional[IndexDF] = None) -> DataDF:
-        if df_keys is not None:
-            if df_keys.empty:
-                return pd.DataFrame(columns=[column.name for column in self.data_sql_schema])
-
-            keys = _to_itertuples(df_keys, self.prim_keys)
-            keys_json = [_serialize(key) for key in keys]
-            values = self.redis_connection.hmget(self.name, keys_json)
-            values = [_deserialize(val) for val in values if val]
-        else:
-            pairs = self.redis_connection.hgetall(self.name)
-            keys = [_deserialize(key) for key in pairs.keys()]
-            values = [_deserialize(val) for val in pairs.values()]
-
-        result_df = pd.concat([
-            pd.DataFrame.from_records(keys, columns=self.prim_keys),
-            pd.DataFrame.from_records(values, columns=self.value_cols)
-        ], axis=1)
-        if values:
-            return result_df
-        else:
-            return result_df.iloc[:0]
+        assert df_keys is not None
+
+        if df_keys.empty:
+            return pd.DataFrame(
+                columns=[column.name for column in self.data_sql_schema]
+            )
+
+        keys = _to_itertuples(df_keys, self.prim_keys)
+        keys_json = [_serialize(key) for key in keys]
+        values = self.redis_connection.hmget(self.name, keys_json)
+        data = [list(key) + _deserialize(val) for key, val in zip(keys, values) if val]
+
+        result_df = pd.DataFrame.from_records(
+            data, columns=self.prim_keys + self.value_cols
+        )
+        return result_df
 
     def delete_rows(self, df_keys: IndexDF) -> None:
         if df_keys.empty:
             return
         keys = _to_itertuples(df_keys, self.prim_keys)
         keys = [_serialize(key) for key in keys]
         self.redis_connection.hdel(self.name, *keys)
 
     def get_primary_schema(self) -> DataSchema:
         return [column for column in self.data_sql_schema if column.primary_key]
 
     def get_meta_schema(self) -> MetaSchema:
         meta_key_prop = MetaKey.get_property_name()
-        return [column for column in self.data_sql_schema if hasattr(column, meta_key_prop)]
+        return [
+            column for column in self.data_sql_schema if hasattr(column, meta_key_prop)
+        ]
```

### Comparing `datapipe_core-0.11.9a6/datapipe/store/table_store.py` & `datapipe_core-0.12.0a2/datapipe/store/table_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 from pathlib import Path
 from typing import Iterator, List, Optional, Union
 
 import pandas as pd
 from sqlalchemy import Column, String
 
 from datapipe.run_config import RunConfig
-from datapipe.types import (DataDF, DataSchema, IndexDF, MetaSchema,
-                            data_to_index)
+from datapipe.types import DataDF, DataSchema, IndexDF, MetaSchema, data_to_index
 
 
 class TableStore(ABC):
     def get_primary_schema(self) -> DataSchema:
         raise NotImplementedError
 
     def get_meta_schema(self) -> MetaSchema:
@@ -32,24 +31,30 @@
 
     def update_rows(self, df: DataDF) -> None:
         if df.empty:
             return
         self.delete_rows(data_to_index(df, self.primary_keys))
         self.insert_rows(df)
 
-    def read_rows(self, idx: IndexDF = None) -> DataDF:
+    def read_rows(self, idx: Optional[IndexDF] = None) -> DataDF:
         raise NotImplementedError
 
-    def read_rows_meta_pseudo_df(self, chunksize: int = 1000, run_config: RunConfig = None) -> Iterator[DataDF]:
+    def read_rows_meta_pseudo_df(
+        self, chunksize: int = 1000, run_config: Optional[RunConfig] = None
+    ) -> Iterator[DataDF]:
         # FIXME сделать честную чанкированную реализацию во всех сторах
         yield self.read_rows()
 
 
 class TableDataSingleFileStore(TableStore):
-    def __init__(self, filename: Union[Path, str] = None, primary_schema: DataSchema = None):
+    def __init__(
+        self,
+        filename: Union[Path, str, None] = None,
+        primary_schema: Optional[DataSchema] = None,
+    ):
         if primary_schema is None:
             primary_schema = [Column("id", String(), primary_key=True)]
 
         self.primary_schema = primary_schema
         self.filename = filename
 
     def get_primary_schema(self) -> DataSchema:
@@ -69,15 +74,17 @@
 
         if file_df is not None:
             if index_df is not None:
                 if len(index_df):
                     file_df = file_df.set_index(self.primary_keys)
                     idx = index_df.set_index(self.primary_keys)
 
-                    return file_df.loc[idx.index].reset_index()
+                    idx_to_read = file_df.index.intersection(idx.index)
+
+                    return file_df.loc[idx_to_read].reset_index()
                 else:
                     return pd.DataFrame(columns=self.primary_keys)
             else:
                 return file_df
         else:
             return pd.DataFrame(columns=self.primary_keys)
 
@@ -85,15 +92,15 @@
         if df.empty:
             return
 
         self.delete_rows(data_to_index(df, self.primary_keys))
 
         file_df = self.load_file()
 
-        if set(self.primary_keys) - set(df.columns):
+        if set(self.primary_keys) - set(df.columns.tolist()):
             raise ValueError("DataDf does not contains all primary keys")
 
         if file_df is None:
             new_df = df
         else:
             new_df = pd.concat([file_df, df], axis="index")
```

### Comparing `datapipe_core-0.11.9a6/datapipe/types.py` & `datapipe_core-0.12.0a2/datapipe/types.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 from __future__ import annotations  # NOQA
 
 from dataclasses import dataclass, field
-from typing import Dict, List, NewType, TypeVar, cast
+from typing import (
+    Dict,
+    List,
+    NewType,
+    Tuple,
+    TypeVar,
+    Union,
+    cast,
+)
 
 import pandas as pd
 from sqlalchemy import Column
 
 DataSchema = List[Column]
 MetaSchema = List[Column]
 
 # Dataframe with columns (<index_cols ...>)
-IndexDF = NewType('IndexDF', pd.DataFrame)
+IndexDF = NewType("IndexDF", pd.DataFrame)
 
 # Dataframe with columns (<index_cols ...>, hash, create_ts, update_ts, process_ts, delete_ts)
-MetadataDF = NewType('MetadataDF', pd.DataFrame)
+MetadataDF = NewType("MetadataDF", pd.DataFrame)
 
 # Dataframe with columns (<index_cols ...>, <data_cols ...>)
 # DataDF = NewType('DataDF', pd.DataFrame)
 DataDF = pd.DataFrame
 
 TAnyDF = TypeVar("TAnyDF", pd.DataFrame, IndexDF, MetadataDF)
 
+Labels = List[Tuple[str, str]]
+
+TransformResult = Union[DataDF, List[DataDF], Tuple[DataDF, ...]]
+
 
 @dataclass
 class ChangeList:
     changes: Dict[str, IndexDF] = field(default_factory=lambda: cast(Dict[str, IndexDF], {}))
 
     def append(self, table_name: str, idx: IndexDF) -> None:
         if table_name in self.changes:
             self_cols = set(self.changes[table_name].columns)
             other_cols = set(idx.columns)
 
             if self_cols != other_cols:
                 raise ValueError(f"Different IndexDF for table {table_name}")
 
-            self.changes[table_name] = cast(IndexDF, pd.concat([self.changes[table_name], idx], axis='index'))
+            self.changes[table_name] = cast(IndexDF, pd.concat([self.changes[table_name], idx], axis="index"))
         else:
             self.changes[table_name] = idx
 
     def extend(self, other: ChangeList):
         for key in other.changes.keys():
             self.append(key, other.changes[key])
 
@@ -58,25 +70,25 @@
 
 
 def meta_to_index(meta_df: MetadataDF, primary_keys: List[str]) -> IndexDF:
     return cast(IndexDF, meta_df[primary_keys])
 
 
 def index_difference(idx1_df: IndexDF, idx2_df: IndexDF) -> IndexDF:
-    assert(list(idx1_df.columns) == list(idx2_df.columns))
+    assert list(idx1_df.columns) == list(idx2_df.columns)
     cols = idx1_df.columns.to_list()
 
     idx1_idx = idx1_df.set_index(cols).index
     idx2_idx = idx2_df.set_index(cols).index
 
     return cast(IndexDF, idx1_idx.difference(idx2_idx).to_frame(index=False))
 
 
 def index_intersection(idx1_df: IndexDF, idx2_df: IndexDF) -> IndexDF:
-    assert(sorted(list(idx1_df.columns)) == sorted(list(idx2_df.columns)))
+    assert sorted(list(idx1_df.columns.tolist())) == sorted(list(idx2_df.columns.tolist()))
     cols = idx1_df.columns.to_list()
 
     idx1_idx = idx1_df.set_index(cols).index
     idx2_idx = idx2_df.set_index(cols).index
 
     return cast(IndexDF, idx1_idx.intersection(idx2_idx).to_frame(index=False))
```

### Comparing `datapipe_core-0.11.9a6/pyproject.toml` & `datapipe_core-0.12.0a2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datapipe-core"
-version = "0.11.9-alpha.6"
+version = "0.12.0-alpha.2"
 description = ""
 authors = ["Andrey Tatarinov <a@tatarinov.co>"]
 packages = [
     { include = "datapipe" }
 ]
 
 [tool.poetry.dependencies]
@@ -20,39 +20,61 @@
 psycopg2_binary = ">=2.8.4"
 cloudpickle = ">=1.6.0"
 PyYAML = ">=5.3.1"
 Pillow = "^9.0.0"
 tqdm = ">=4.60.0"
 iteration-utilities = ">=0.11.0"
 cityhash = "^0.4.2"
+traceback-with-variables = "^2.0.4"
 
 pymilvus = {version="^2.0.2", optional=true}
 
 opentelemetry-api = "^1.8.0"
 opentelemetry-sdk = "^1.8.0"
 opentelemetry-instrumentation-sqlalchemy = "0.35b0"
 
 xlrd = {version=">=2.0.1", optional=true}
 openpyxl = {version=">=3.0.7", optional=true}
 redis = {version="^4.3.4", optional=true}
 
+pysqlite3-binary = {version="^0.5.0", optional=true}
+sqlalchemy-pysqlite3-binary = {version="^0.0.4", optional=true}
+qdrant-client = {version="^1.1.7", optional=true}
+
+click = ">=7.1.2"
+rich = "^13.3.2"
+
+# Copypaste without thinking from https://github.com/meltano/sdk/blob/main/pyproject.toml
+sphinx = {version = ">=4.5,<6.0", optional = true}
+myst-parser = {version = ">=0.17.2,<1.1.0", optional = true}
+
 [tool.poetry.extras]
 
+sqlite = ["pysqlite3-binary", "sqlalchemy-pysqlite3-binary"]
 excel = ["xlrd", "openpyxl"]
 milvus = ["pymilvus"]
+qdrant = ["qdrant-client"]
 gcsfs = ["gcsfs"]
 s3fs = ["s3fs"]
 redis = ["redis"]
 
-[tool.poetry.dev-dependencies]
+docs = ["sphinx", "myst-parser"]
+
+[tool.poetry.group.dev.dependencies]
 pytest = "*"
 flake8 = "*"
-mypy = "<=0.990"
+mypy = "*"
 black = "*"
 pandas-stubs = "*"
 pytest-cases = "*"
 types-setuptools = "*"
 types-redis = "*"
+types-tqdm = "*"
+types-pillow = "*"
+types-PyYAML = "*"
+
+[tool.poetry.scripts]
+datapipe = 'datapipe.cli:main'
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `datapipe_core-0.11.9a6/PKG-INFO` & `datapipe_core-0.12.0a2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 Metadata-Version: 2.1
 Name: datapipe-core
-Version: 0.11.9a6
+Version: 0.12.0a2
 Summary: 
 Author: Andrey Tatarinov
 Author-email: a@tatarinov.co
 Requires-Python: >=3.8,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Provides-Extra: docs
 Provides-Extra: excel
 Provides-Extra: gcsfs
 Provides-Extra: milvus
+Provides-Extra: qdrant
 Provides-Extra: redis
 Provides-Extra: s3fs
+Provides-Extra: sqlite
 Requires-Dist: Pillow (>=9.0.0,<10.0.0)
 Requires-Dist: PyYAML (>=5.3.1)
 Requires-Dist: SQLAlchemy (>=1.4.25,<2.0.0)
 Requires-Dist: cityhash (>=0.4.2,<0.5.0)
+Requires-Dist: click (>=7.1.2)
 Requires-Dist: cloudpickle (>=1.6.0)
 Requires-Dist: fsspec (>=2021.11.1)
-Requires-Dist: gcsfs (>=2021.11.1); extra == "gcsfs"
+Requires-Dist: gcsfs (>=2021.11.1) ; extra == "gcsfs"
 Requires-Dist: iteration-utilities (>=0.11.0)
+Requires-Dist: myst-parser (>=0.17.2,<1.1.0) ; extra == "docs"
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
-Requires-Dist: openpyxl (>=3.0.7); extra == "excel"
+Requires-Dist: openpyxl (>=3.0.7) ; extra == "excel"
 Requires-Dist: opentelemetry-api (>=1.8.0,<2.0.0)
 Requires-Dist: opentelemetry-instrumentation-sqlalchemy (==0.35b0)
 Requires-Dist: opentelemetry-sdk (>=1.8.0,<2.0.0)
 Requires-Dist: pandas (>=1.2.0,<2.0.0)
 Requires-Dist: psycopg2_binary (>=2.8.4)
-Requires-Dist: pymilvus (>=2.0.2,<3.0.0); extra == "milvus"
-Requires-Dist: redis (>=4.3.4,<5.0.0); extra == "redis"
-Requires-Dist: s3fs (>=2021.11.1); extra == "s3fs"
+Requires-Dist: pymilvus (>=2.0.2,<3.0.0) ; extra == "milvus"
+Requires-Dist: pysqlite3-binary (>=0.5.0,<0.6.0) ; extra == "sqlite"
+Requires-Dist: qdrant-client (>=1.1.7,<2.0.0) ; extra == "qdrant"
+Requires-Dist: redis (>=4.3.4,<5.0.0) ; extra == "redis"
+Requires-Dist: rich (>=13.3.2,<14.0.0)
+Requires-Dist: s3fs (>=2021.11.1) ; extra == "s3fs"
+Requires-Dist: sphinx (>=4.5,<6.0) ; extra == "docs"
+Requires-Dist: sqlalchemy-pysqlite3-binary (>=0.0.4,<0.0.5) ; extra == "sqlite"
 Requires-Dist: tqdm (>=4.60.0)
-Requires-Dist: xlrd (>=2.0.1); extra == "excel"
+Requires-Dist: traceback-with-variables (>=2.0.4,<3.0.0)
+Requires-Dist: xlrd (>=2.0.1) ; extra == "excel"
```

