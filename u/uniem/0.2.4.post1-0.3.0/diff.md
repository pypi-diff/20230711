# Comparing `tmp/uniem-0.2.4.post1.tar.gz` & `tmp/uniem-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uniem-0.2.4.post1.tar", max compression
+gzip compressed data, was "uniem-0.3.0.tar", max compression
```

## Comparing `uniem-0.2.4.post1.tar` & `uniem-0.3.0.tar`

### file list

```diff
@@ -1,14 +1,17 @@
--rw-r--r--   0        0        0    11357 2023-07-03 08:22:19.445050 uniem-0.2.4.post1/LICENSE
--rw-r--r--   0        0        0     5876 2023-07-03 08:22:19.445050 uniem-0.2.4.post1/README.md
--rw-r--r--   0        0        0      799 2023-07-03 08:22:19.457049 uniem-0.2.4.post1/pyproject.toml
--rw-r--r--   0        0        0      104 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/__init__.py
--rw-r--r--   0        0        0     7166 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/criteria.py
--rw-r--r--   0        0        0    10992 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/data.py
--rw-r--r--   0        0        0     1109 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/data_structures.py
--rw-r--r--   0        0        0    14799 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/finetuner.py
--rw-r--r--   0        0        0    14611 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/model.py
--rw-r--r--   0        0        0     6025 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/trainer.py
--rw-r--r--   0        0        0      658 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/types.py
--rw-r--r--   0        0        0     4675 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/utils.py
--rw-r--r--   0        0        0       22 2023-07-03 08:22:19.553048 uniem-0.2.4.post1/uniem/version.py
--rw-r--r--   0        0        0     6517 1970-01-01 00:00:00.000000 uniem-0.2.4.post1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-07-11 11:08:20.264987 uniem-0.3.0/LICENSE
+-rw-r--r--   0        0        0     6213 2023-07-11 11:08:20.264987 uniem-0.3.0/README.md
+-rw-r--r--   0        0        0      813 2023-07-11 11:08:20.276987 uniem-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0       92 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/__init__.py
+-rw-r--r--   0        0        0     7166 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/criteria.py
+-rw-r--r--   0        0        0    12450 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/data.py
+-rw-r--r--   0        0        0     1109 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/data_structures.py
+-rw-r--r--   0        0        0    14276 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/finetuner.py
+-rw-r--r--   0        0        0        0 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/integration/__init__.py
+-rw-r--r--   0        0        0     1339 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/integration/sentence_transformers_wrapper.py
+-rw-r--r--   0        0        0    13360 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/model.py
+-rw-r--r--   0        0        0     6331 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/trainer.py
+-rw-r--r--   0        0        0     3678 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/training_strategy.py
+-rw-r--r--   0        0        0      658 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/types.py
+-rw-r--r--   0        0        0     6193 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/utils.py
+-rw-r--r--   0        0        0       22 2023-07-11 11:08:20.372987 uniem-0.3.0/uniem/version.py
+-rw-r--r--   0        0        0     6848 1970-01-01 00:00:00.000000 uniem-0.3.0/PKG-INFO
```

### Comparing `uniem-0.2.4.post1/LICENSE` & `uniem-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uniem-0.2.4.post1/README.md` & `uniem-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 
 uniem 项目的目标是创建中文最好的通用文本嵌入模型。
 
 本项目主要包括模型的训练，微调和评测代码，模型与数据集会在 [HuggingFace](https://huggingface.co/) 社区上进行开源。
 
 ## 🌟 重要更新
 
-- 🎉 **2023.06.08** , 发布 [M3E models](https://huggingface.co/moka-ai/m3e-base) ，在中文文本分类和文本检索上均优于 `openai text-embedding-ada-002`，详请请参考 [M3E models README](https://huggingface.co/moka-ai/m3e-base/blob/main/README.md)。
-- 📊 **2023.06.17** , 发布 [MTEB-zh](https://github.com/wangyuxinwhy/uniem/tree/main/mteb-zh) 正式版 ， 支持 6 大类 Embedding 模型 ，支持 4 大类任务 ，共 9 种数据集的自动化评测
+- ➿ **2023.07.11** , 发布 uniem 0.3.0， `FineTuner` 除 M3E 外，还支持 `sentence_transformers`, `text2vec` 等模型的微调，同时还支持 [SGPT](https://github.com/Muennighoff/sgpt) 的方式对 GPT 系列模型进行训练，以及 Prefix Tuning。 **FineTuner 初始化的 API 有小小的变化，无法兼容 0.2.0**
 - ➿ **2023.06.17** , 发布 uniem 0.2.1 ， 实现了 `FineTuner` 以原生支持模型微调，**几行代码，即刻适配**！
+- 📊 **2023.06.17** , 发布 [MTEB-zh](https://github.com/wangyuxinwhy/uniem/tree/main/mteb-zh) 正式版 ， 支持 6 大类 Embedding 模型 ，支持 4 大类任务 ，共 9 种数据集的自动化评测
+- 🎉 **2023.06.08** , 发布 [M3E models](https://huggingface.co/moka-ai/m3e-base) ，在中文文本分类和文本检索上均优于 `openai text-embedding-ada-002`，详请请参考 [M3E models README](https://huggingface.co/moka-ai/m3e-base/blob/main/README.md)。
 
 ## 🔧 使用 M3E
 
 M3E 系列模型完全兼容 [sentence-transformers](https://www.sbert.net/) ，你可以通过 **替换模型名称** 的方式在所有支持 sentence-transformers 的项目中无缝使用 M3E Models，比如 [chroma](https://docs.trychroma.com/getting-started), [guidance](https://github.com/microsoft/guidance), [semantic-kernel](https://github.com/microsoft/semantic-kernel) 。
 
 安装
```

### Comparing `uniem-0.2.4.post1/pyproject.toml` & `uniem-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uniem"
-version = "0.2.4.post1"
+version = "0.3.0"
 description = "unified embedding model"
 authors = ["wangyuxin <wangyuxin@mokahr.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -21,14 +21,15 @@
 isort = "^5.12.0"
 pyright = "^1.1.314"
 
 [tool.poetry.group.mteb.dependencies]
 mteb = "^1.0.2"
 openai = "^0.27.8"
 sentence-transformers = "^2.2.2"
+text2vec = "^1.2.1"
 
 [tool.ruff]
 line-length = 128
 select = [
     'E',
     'F',
     'I',
```

### Comparing `uniem-0.2.4.post1/uniem/criteria.py` & `uniem-0.3.0/uniem/criteria.py`

 * *Files identical despite different names*

### Comparing `uniem-0.2.4.post1/uniem/data.py` & `uniem-0.3.0/uniem/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import json
 from collections import defaultdict
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, Sequence, cast
+from typing import Any, Iterable, Sequence, cast
 
 import torch
 from datasets import Dataset as HfDataset
-from torch.utils.data import Dataset, RandomSampler
+from datasets import IterableDataset as HfIterableDataset
+from torch.utils.data import Dataset, IterableDataset, RandomSampler
 
 from uniem.data_structures import (
     PairRecord,
     RecordType,
     ScoredPairRecord,
     TripletRecord,
     infer_record_type,
@@ -147,14 +148,32 @@
         record = self.dataset[index]
         return self.record_cls(**record)
 
     def __len__(self):
         return len(self.dataset)
 
 
+class FinetuneIterableDataset(IterableDataset):
+    def __init__(
+        self,
+        dataset: HfIterableDataset | Iterable[dict],
+        record_type: RecordType | str | None = None,
+    ) -> None:
+        self.dataset = dataset
+        if record_type:
+            self.record_type = RecordType(record_type)
+        else:
+            self.record_type = infer_record_type(next(iter(dataset)))
+        self.record_cls = record_type_cls_map[self.record_type]
+
+    def __iter__(self):
+        for record in self.dataset:
+            yield self.record_cls(**record)
+
+
 class PrefixFinetuneDataset(FinetuneDataset):
     def __init__(
         self,
         dataset: HfDataset | Sequence[dict],
         prefix: str,
         record_type: RecordType | str | None = None,
     ) -> None:
@@ -169,14 +188,36 @@
             case RecordType.TRIPLET:
                 record['text'] = self.prefix + record['text']
             case RecordType.SCORED_PAIR:
                 record['sentence1'] = self.prefix + record['sentence1']
         return self.record_cls(**record)
 
 
+class PrefixFinetuneIterableDataset(FinetuneIterableDataset):
+    def __init__(
+        self,
+        dataset: HfIterableDataset | Iterable[dict],
+        prefix: str,
+        record_type: RecordType | str | None = None,
+    ) -> None:
+        super().__init__(dataset=dataset, record_type=record_type)
+        self.prefix = prefix
+
+    def __iter__(self):
+        for record in self.dataset:
+            match self.record_type:
+                case RecordType.PAIR:
+                    record['text'] = self.prefix + record['text']
+                case RecordType.TRIPLET:
+                    record['text'] = self.prefix + record['text']
+                case RecordType.SCORED_PAIR:
+                    record['sentence1'] = self.prefix + record['sentence1']
+            yield self.record_cls(**record)
+
+
 class MediDataset(Dataset):
     def __init__(
         self,
         medi_data_file: str | Path,
         batch_size: int = 32,
         pair_or_triplet: str = 'triplet',
         with_prompt: bool = True,
```

### Comparing `uniem-0.2.4.post1/uniem/data_structures.py` & `uniem-0.3.0/uniem/data_structures.py`

 * *Files identical despite different names*

### Comparing `uniem-0.2.4.post1/uniem/model.py` & `uniem-0.3.0/uniem/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,27 @@
-import importlib
 from enum import Enum
 from pathlib import Path
-from typing import ClassVar, Literal, Type, TypeVar, cast
+from typing import ClassVar, Literal, Protocol, Type, TypeVar, cast
 
 import numpy as np
 import torch
 import tqdm
-from transformers import AutoModel, AutoTokenizer, PreTrainedModel  # type: ignore
+from transformers import AutoConfig, AutoTokenizer, PreTrainedModel  # type: ignore
 
 from uniem.criteria import (
     CoSentLoss,
     PairInBatchNegCoSentLoss,
     PairInBatchNegSigmoidContrastLoss,
     PairInBatchNegSoftmaxContrastLoss,
     TripletInBatchNegCoSentLoss,
     TripletInBatchNegSigmoidContrastLoss,
     TripletInBatchNegSoftmaxContrastLoss,
 )
 from uniem.types import Tokenizer
-from uniem.utils import generate_batch
+from uniem.utils import create_attention_mask_from_input_ids, generate_batch, load_hf_pretrained_model
 
 T = TypeVar('T')
 
 
 class PoolingStrategy(str, Enum):
     cls = 'cls'
     last_mean = 'last_mean'
@@ -33,43 +32,30 @@
 
 class InBatchNegLossType(str, Enum):
     sigmoid = 'sigmoid'
     softmax = 'softmax'
     cosent = 'cosent'
 
 
-def creat_attention_mask_from_input_ids(input_ids: torch.Tensor, pad_token_id: int) -> torch.Tensor:
-    return input_ids != pad_token_id
-
-
 def mean_pooling(hidden_state: torch.Tensor, attention_mask: torch.Tensor | None = None) -> torch.Tensor:
     if attention_mask is None:
         return torch.mean(hidden_state, dim=1)
     attention_mask = attention_mask.float()
     return torch.sum(hidden_state * attention_mask.unsqueeze(-1), dim=1) / torch.sum(attention_mask, dim=-1, keepdim=True)
 
 
-def load_hf_pretrained_model(
-    model_name_or_path: str, model_class: str | None | Type[PreTrainedModel] | Type[AutoModel] = None
-) -> PreTrainedModel:
-    if model_class is None:
-        model_class = AutoModel
-    elif isinstance(model_class, str):
-        transformers_module = importlib.import_module('transformers')
-        model_class = getattr(transformers_module, model_class)
+StrategyEmbedderClsMap: dict[PoolingStrategy, Type['UniemEmbedder']] = {}
 
-    model = model_class.from_pretrained(model_name_or_path)  # type: ignore
-    model = cast(PreTrainedModel, model)
-    return model
 
+class Embedder(Protocol):
+    def __call__(self, input_ids: torch.Tensor, **kwargs) -> torch.Tensor:
+        ...
 
-StrategyEmbedderClsMap: dict[PoolingStrategy, Type['Embedder']] = {}
 
-
-class Embedder(torch.nn.Module):
+class UniemEmbedder(torch.nn.Module, Embedder):
     pooling_strategy: ClassVar[PoolingStrategy]
 
     def __init__(self, encoder: PreTrainedModel, pad_token_id: int | None = None):
         super().__init__()
         self.encoder = encoder
         self.encoder.config.uniem_pooling_strategy = str(self.pooling_strategy.value)
 
@@ -88,164 +74,162 @@
         raise NotImplementedError
 
     def save_pretrained(self, path: str | Path):
         self.encoder.save_pretrained(path)
 
     @classmethod
     def from_pretrained(cls, model_name_or_path: str):
-        encoder = load_hf_pretrained_model(model_name_or_path)
-        return cls(encoder)
+        config = AutoConfig.from_pretrained(str(model_name_or_path))
+        if hasattr(config, 'uniem_pooling_strategy'):
+            strategy_string = config.uniem_pooling_strategy
+        elif hasattr(config, 'uniem_embedding_strategy'):
+            strategy_string = config.uniem_embedding_strategy
+        else:
+            raise ValueError('Can not find uniem pooling strategy in config, Model is not trained by UniEmbedder.')
+        return create_uniem_embedder(str(model_name_or_path), pooling_strategy=strategy_string)
 
     @property
     def max_length(self):
         return self.encoder.config.max_position_embeddings
 
 
-class LastMeanEmbedder(Embedder):
+class LastMeanEmbedder(UniemEmbedder):
     pooling_strategy: ClassVar[PoolingStrategy] = PoolingStrategy.last_mean
 
     def forward(self, input_ids: torch.Tensor, attention_mask: torch.Tensor | None = None) -> torch.Tensor:
         if attention_mask is None:
-            attention_mask = creat_attention_mask_from_input_ids(input_ids, self.pad_token_id)
+            attention_mask = create_attention_mask_from_input_ids(input_ids, self.pad_token_id)
         embeddings = self.encoder(input_ids, attention_mask=attention_mask).last_hidden_state
         embeddings = mean_pooling(embeddings, attention_mask)
         return embeddings
 
 
-class ClsEmbedder(Embedder):
+class ClsEmbedder(UniemEmbedder):
     pooling_strategy: ClassVar[PoolingStrategy] = PoolingStrategy.cls
 
     def forward(self, input_ids: torch.Tensor, attention_mask: torch.Tensor | None = None) -> torch.Tensor:
         if attention_mask is None:
-            attention_mask = creat_attention_mask_from_input_ids(input_ids, self.pad_token_id)
+            attention_mask = create_attention_mask_from_input_ids(input_ids, self.pad_token_id)
         embeddings = self.encoder(input_ids, attention_mask=attention_mask).last_hidden_state[:, 0]
         return embeddings
 
 
-class FirstLastEmbedder(Embedder):
+class FirstLastEmbedder(UniemEmbedder):
     pooling_strategy: ClassVar[PoolingStrategy] = PoolingStrategy.first_last_mean
 
     def forward(self, input_ids: torch.Tensor, attention_mask: torch.Tensor | None = None) -> torch.Tensor:
         if attention_mask is None:
-            attention_mask = creat_attention_mask_from_input_ids(input_ids, self.pad_token_id)
+            attention_mask = create_attention_mask_from_input_ids(input_ids, self.pad_token_id)
         embeddings = self.encoder(input_ids, attention_mask=attention_mask, output_hidden_states=True).hidden_states
         first_embeddings = mean_pooling(embeddings[0], attention_mask)
         last_embeddings = mean_pooling(embeddings[-1], attention_mask)
         embeddings = (first_embeddings + last_embeddings) / 2
         return embeddings
 
 
-class EmbeddingLastEmbedder(Embedder):
+class EmbeddingLastEmbedder(UniemEmbedder):
     pooling_strategy: ClassVar[PoolingStrategy] = PoolingStrategy.embedding_last_mean
 
     def __init__(self, encoder: PreTrainedModel, pad_token_id: int | None = None):
         super().__init__(encoder, pad_token_id)
         self.embedding_layer = self.encoder.get_input_embeddings()
 
     def forward(self, input_ids: torch.Tensor, attention_mask: torch.Tensor | None = None) -> torch.Tensor:
         if attention_mask is None:
-            attention_mask = creat_attention_mask_from_input_ids(input_ids, self.pad_token_id)
+            attention_mask = create_attention_mask_from_input_ids(input_ids, self.pad_token_id)
         static_embeddings = self.embedding_layer(input_ids)
         mean_last_embeddings = mean_pooling(
             self.encoder(input_ids, attention_mask=attention_mask).last_hidden_state, attention_mask
         )
         mean_static_embeddings = mean_pooling(static_embeddings, attention_mask)
         return (mean_last_embeddings + mean_static_embeddings) / 2
 
 
-class LastWeightedEmbedder(Embedder):
+class LastWeightedEmbedder(UniemEmbedder):
     pooling_strategy: ClassVar[PoolingStrategy] = PoolingStrategy.last_weighted
 
     def __init__(self, encoder: PreTrainedModel, pad_token_id: int | None = None):
         super().__init__(encoder, pad_token_id)
         self.embedding_layer = self.encoder.get_input_embeddings()
 
     def forward(self, input_ids: torch.Tensor, attention_mask: torch.Tensor | None = None) -> torch.Tensor:
         if attention_mask is None:
-            attention_mask = creat_attention_mask_from_input_ids(input_ids, self.pad_token_id)
+            attention_mask = create_attention_mask_from_input_ids(input_ids, self.pad_token_id)
         weights = (torch.arange(input_ids.shape[1], device=input_ids.device) + 1).float()
         embeddings = self.encoder(input_ids).last_hidden_state
         embeddings = embeddings * attention_mask.unsqueeze(-1).float() * weights.unsqueeze(0).unsqueeze(-1)
         embeddings = torch.sum(embeddings, dim=1) / torch.sum(weights * attention_mask, dim=-1, keepdim=True)
         return embeddings
 
 
-class AutoEmbedder:
-    @classmethod
-    def from_pretrained(cls, model_name_or_path: str | Path):
-        encoder = load_hf_pretrained_model(str(model_name_or_path))
-        if hasattr(encoder.config, 'uniem_pooling_strategy'):
-            strategy_string = encoder.config.uniem_pooling_strategy
-        elif hasattr(encoder.config, 'uniem_embedding_strategy'):
-            strategy_string = encoder.config.uniem_embedding_strategy
-        else:
-            raise ValueError('Can not find uniem pooling strategy in config, Model is not trained by UniEmbedder.')
-        embedder_cls = StrategyEmbedderClsMap[PoolingStrategy(strategy_string)]
-        return embedder_cls(encoder)
+def create_uniem_embedder(
+    model_name_or_path: str,
+    model_class: str | None = None,
+    pooling_strategy: PoolingStrategy | str = PoolingStrategy.last_mean,
+):
+    pretrained_model = load_hf_pretrained_model(model_name_or_path, model_class=model_class)
+    embedder_cls = StrategyEmbedderClsMap[PoolingStrategy(pooling_strategy)]
+    embedder = embedder_cls(pretrained_model)
+    return embedder
 
 
 class EmbedderForTrain(torch.nn.Module):
     embedder: Embedder
 
-    def __init__(self, embedder: Embedder):
+    def __init__(
+        self,
+        embedder: Embedder,
+        criterion: torch.nn.Module,
+    ):
         super().__init__()
         self.embedder = embedder
+        self.criterion = criterion
 
 
 class EmbedderForPairInBatchNegTrain(EmbedderForTrain):
     def __init__(
         self,
-        model_name_or_path: str,
-        model_class: str | None = None,
-        temperature: float | None = None,
+        embedder: Embedder,
+        temperature: float = 0.05,
         loss_type: InBatchNegLossType | str = InBatchNegLossType.softmax,
-        embedding_strategy: PoolingStrategy | str = PoolingStrategy.last_mean,
     ):
-        pretrained_model = load_hf_pretrained_model(model_name_or_path, model_class=model_class)
-        embedder = StrategyEmbedderClsMap[PoolingStrategy(embedding_strategy)](pretrained_model)
-        super().__init__(embedder)
-        temperature = temperature or 0.05
         self.loss_type = InBatchNegLossType(loss_type)
         match self.loss_type:
             case InBatchNegLossType.sigmoid:
-                self.criterion = PairInBatchNegSigmoidContrastLoss(temperature)
+                criterion = PairInBatchNegSigmoidContrastLoss(temperature)
             case InBatchNegLossType.softmax:
-                self.criterion = PairInBatchNegSoftmaxContrastLoss(temperature)
+                criterion = PairInBatchNegSoftmaxContrastLoss(temperature)
             case InBatchNegLossType.cosent:
-                self.criterion = PairInBatchNegCoSentLoss(temperature)
+                criterion = PairInBatchNegCoSentLoss(temperature)
+        super().__init__(embedder, criterion)
 
     def forward(self, text_ids: torch.Tensor, text_pos_ids: torch.Tensor) -> dict[str, torch.Tensor]:
         text_embeddings = self.embedder(text_ids)
         text_pos_embeddings = self.embedder(text_pos_ids)
         loss = self.criterion(text_embeddings, text_pos_embeddings)
         return {'loss': loss}
 
 
 class EmbedderForTripletInBatchNegTrain(EmbedderForTrain):
     def __init__(
         self,
-        model_name_or_path: str,
-        model_class: str | None = None,
-        temperature: float | None = None,
+        embedder: Embedder,
+        temperature: float = 0.05,
         loss_type: InBatchNegLossType | str = InBatchNegLossType.softmax,
-        embedding_strategy: PoolingStrategy | str = PoolingStrategy.last_mean,
         add_swap_loss: bool = False,
     ):
-        pretrained_model = load_hf_pretrained_model(model_name_or_path, model_class=model_class)
-        embedder = StrategyEmbedderClsMap[PoolingStrategy(embedding_strategy)](pretrained_model)
-        super().__init__(embedder)
-        temperature = temperature or 0.05
         self.loss_type = InBatchNegLossType(loss_type)
         match self.loss_type:
             case InBatchNegLossType.sigmoid:
-                self.criterion = TripletInBatchNegSigmoidContrastLoss(temperature, add_swap_loss)
+                criterion = TripletInBatchNegSigmoidContrastLoss(temperature, add_swap_loss)
             case InBatchNegLossType.softmax:
-                self.criterion = TripletInBatchNegSoftmaxContrastLoss(temperature, add_swap_loss)
+                criterion = TripletInBatchNegSoftmaxContrastLoss(temperature, add_swap_loss)
             case InBatchNegLossType.cosent:
-                self.criterion = TripletInBatchNegCoSentLoss(temperature, add_swap_loss)
+                criterion = TripletInBatchNegCoSentLoss(temperature, add_swap_loss)
+        super().__init__(embedder, criterion)
 
     def forward(
         self,
         text_ids: torch.Tensor,
         text_pos_ids: torch.Tensor,
         text_neg_ids: torch.Tensor,
     ) -> dict[str, torch.Tensor]:
@@ -255,43 +239,38 @@
         loss = self.criterion(text_embeddings, text_pos_embeddings, text_neg_embeddings)
         return {'loss': loss}
 
 
 class EmbedderForScoredPairTrain(EmbedderForTrain):
     def __init__(
         self,
-        model_name_or_path: str,
-        temperature: float | None = None,
-        embedding_strategy: PoolingStrategy | str = PoolingStrategy.last_mean,
+        embedder: Embedder,
+        temperature: float = 0.05,
     ):
-        pretrained_model = load_hf_pretrained_model(model_name_or_path)
-        embedder = StrategyEmbedderClsMap[PoolingStrategy(embedding_strategy)](pretrained_model)
-        super().__init__(embedder)
-        temperature = temperature or 0.05
-        self.criterion = CoSentLoss(temperature)
+        super().__init__(embedder, CoSentLoss(temperature))
 
     def forward(
         self,
         text_ids: torch.Tensor,
         text_pair_ids: torch.Tensor,
         labels: torch.Tensor,
     ) -> dict[str, torch.Tensor]:
         text_embeddings = self.embedder(text_ids)
         text_pos_embeddings = self.embedder(text_pair_ids)
         predict_labels = torch.cosine_similarity(text_embeddings, text_pos_embeddings, dim=-1)
         loss = self.criterion(predict_labels, labels)
         return {'loss': loss, 'predict_labels': predict_labels}
 
 
-class UniEmbedder:
+class Uniem:
     PROGRESS_BAR_THRESHOLD = 1000
 
     def __init__(
         self,
-        embedder: Embedder,
+        embedder: UniemEmbedder,
         tokenizer: Tokenizer,
         normalize: bool = True,
         max_length: int | None = None,
         device: str | None = None,
     ):
         super().__init__()
         self.embedder = embedder.eval()
@@ -350,14 +329,14 @@
         return embeddings
 
     def encode_single(self, sentence: str):
         return self.encode([sentence])[0]
 
     @classmethod
     def from_pretrained(cls, model_name_or_path: str, **kwargs):
-        encoder = AutoEmbedder.from_pretrained(model_name_or_path)
+        embedder = UniemEmbedder.from_pretrained(model_name_or_path)
         tokenizer = AutoTokenizer.from_pretrained(model_name_or_path)
-        return cls(encoder, tokenizer, **kwargs)
+        return cls(embedder, tokenizer, **kwargs)
 
     def save_pretrained(self, ouptut_dir: str):
         self.embedder.save_pretrained(ouptut_dir)
         self.tokenizer.save_pretrained(ouptut_dir)
```

### Comparing `uniem-0.2.4.post1/uniem/trainer.py` & `uniem-0.3.0/uniem/trainer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Any
+from typing import Any, Sized
 
 import torch
 from accelerate import Accelerator
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import LRScheduler
 from torch.utils.data import DataLoader
 from tqdm.auto import tqdm
@@ -33,15 +33,19 @@
         self.accelerator = accelerator
         self.epochs = epochs
         self.log_interval = log_interval
         self.save_on_epoch_end = save_on_epoch_end
 
         self.train_loss_tracker = LossTracker()
         self.validation_loss_tracker = LossTracker()
-        self.progress_bar = DistributedTqdmProgressBar(self.epochs, len(self.train_dataloader))
+        if isinstance(self.train_dataloader.dataset, Sized):
+            num_steps_per_epoch = len(self.train_dataloader)
+        else:
+            num_steps_per_epoch = None
+        self.progress_bar = DistributedTqdmProgressBar(self.epochs, num_steps_per_epoch=num_steps_per_epoch)
         self.epoch_end_callbacks = epoch_end_callbacks or []
         self.current_step = 0
 
     def train(self):
         for current_epoch in range(1, self.epochs + 1):
             self.model.train()
             self.progress_bar.on_epoch_start()
@@ -73,14 +77,15 @@
             if self.validation_dataloader:
                 validation_loss = evaluate(
                     self.model,
                     self.validation_dataloader,
                     self.validation_loss_tracker,
                 )
                 validation_metrics = self.add_prefix({'loss': validation_loss}, 'validation')
+                self.accelerator.print(f'Epoch {current_epoch} Validation loss: {validation_loss:.4f}')
                 self.accelerator.log(validation_metrics, step=current_epoch)
 
             if self.save_on_epoch_end:
                 self.accelerator.save_state()
 
             if self.epoch_end_callbacks:
                 for callback in self.epoch_end_callbacks:
@@ -121,15 +126,15 @@
         pass
 
     def set_description(self, description: str) -> None:
         pass
 
 
 class DistributedTqdmProgressBar:
-    def __init__(self, epochs: int, num_steps_per_epoch: int, **kwargs) -> None:
+    def __init__(self, epochs: int, num_steps_per_epoch: int | None, **kwargs) -> None:
         self.accelerator = Accelerator()
         self.epochs = epochs
         self.current_epoch = 1
         self.num_steps_per_epoch = num_steps_per_epoch
         self.tqdm_kwargs = kwargs
 
     def on_epoch_start(self):
```

### Comparing `uniem-0.2.4.post1/uniem/types.py` & `uniem-0.3.0/uniem/types.py`

 * *Files identical despite different names*

### Comparing `uniem-0.2.4.post1/PKG-INFO` & `uniem-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniem
-Version: 0.2.4.post1
+Version: 0.3.0
 Summary: unified embedding model
 License: MIT
 Author: wangyuxin
 Author-email: wangyuxin@mokahr.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -25,17 +25,18 @@
 
 uniem 项目的目标是创建中文最好的通用文本嵌入模型。
 
 本项目主要包括模型的训练，微调和评测代码，模型与数据集会在 [HuggingFace](https://huggingface.co/) 社区上进行开源。
 
 ## 🌟 重要更新
 
-- 🎉 **2023.06.08** , 发布 [M3E models](https://huggingface.co/moka-ai/m3e-base) ，在中文文本分类和文本检索上均优于 `openai text-embedding-ada-002`，详请请参考 [M3E models README](https://huggingface.co/moka-ai/m3e-base/blob/main/README.md)。
-- 📊 **2023.06.17** , 发布 [MTEB-zh](https://github.com/wangyuxinwhy/uniem/tree/main/mteb-zh) 正式版 ， 支持 6 大类 Embedding 模型 ，支持 4 大类任务 ，共 9 种数据集的自动化评测
+- ➿ **2023.07.11** , 发布 uniem 0.3.0， `FineTuner` 除 M3E 外，还支持 `sentence_transformers`, `text2vec` 等模型的微调，同时还支持 [SGPT](https://github.com/Muennighoff/sgpt) 的方式对 GPT 系列模型进行训练，以及 Prefix Tuning。 **FineTuner 初始化的 API 有小小的变化，无法兼容 0.2.0**
 - ➿ **2023.06.17** , 发布 uniem 0.2.1 ， 实现了 `FineTuner` 以原生支持模型微调，**几行代码，即刻适配**！
+- 📊 **2023.06.17** , 发布 [MTEB-zh](https://github.com/wangyuxinwhy/uniem/tree/main/mteb-zh) 正式版 ， 支持 6 大类 Embedding 模型 ，支持 4 大类任务 ，共 9 种数据集的自动化评测
+- 🎉 **2023.06.08** , 发布 [M3E models](https://huggingface.co/moka-ai/m3e-base) ，在中文文本分类和文本检索上均优于 `openai text-embedding-ada-002`，详请请参考 [M3E models README](https://huggingface.co/moka-ai/m3e-base/blob/main/README.md)。
 
 ## 🔧 使用 M3E
 
 M3E 系列模型完全兼容 [sentence-transformers](https://www.sbert.net/) ，你可以通过 **替换模型名称** 的方式在所有支持 sentence-transformers 的项目中无缝使用 M3E Models，比如 [chroma](https://docs.trychroma.com/getting-started), [guidance](https://github.com/microsoft/guidance), [semantic-kernel](https://github.com/microsoft/semantic-kernel) 。
 
 安装
```

