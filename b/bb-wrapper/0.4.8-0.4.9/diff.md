# Comparing `tmp/bb-wrapper-0.4.8.tar.gz` & `tmp/bb-wrapper-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bb-wrapper-0.4.8.tar", max compression
+gzip compressed data, was "bb-wrapper-0.4.9.tar", max compression
```

## Comparing `bb-wrapper-0.4.8.tar` & `bb-wrapper-0.4.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     2719 2022-09-12 21:25:45.647092 bb-wrapper-0.4.8/README.rst
--rw-r--r--   0        0        0      213 2022-09-12 21:26:25.305896 bb-wrapper-0.4.8/bb_wrapper/__init__.py
--rw-r--r--   0        0        0      748 2022-09-12 21:25:45.647092 bb-wrapper-0.4.8/bb_wrapper/constants.py
--rw-r--r--   0        0        0        0 2022-09-12 21:25:45.647092 bb-wrapper-0.4.8/bb_wrapper/models/__init__.py
--rw-r--r--   0        0        0     2819 2022-09-12 21:25:45.647092 bb-wrapper-0.4.8/bb_wrapper/models/barcode.py
--rw-r--r--   0        0        0     3072 2022-09-12 21:25:45.647092 bb-wrapper-0.4.8/bb_wrapper/models/boleto.py
--rw-r--r--   0        0        0    22579 2022-09-12 21:25:45.647092 bb-wrapper-0.4.8/bb_wrapper/models/pagamentos.py
--rw-r--r--   0        0        0      827 2022-09-12 21:25:45.647092 bb-wrapper-0.4.8/bb_wrapper/models/perfis.py
--rw-r--r--   0        0        0      657 2022-09-12 21:25:45.647092 bb-wrapper-0.4.8/bb_wrapper/models/pix_cob.py
--rw-r--r--   0        0        0      463 2022-09-12 21:25:45.647092 bb-wrapper-0.4.8/bb_wrapper/services/__init__.py
--rw-r--r--   0        0        0      469 2022-09-12 21:25:45.647092 bb-wrapper-0.4.8/bb_wrapper/services/b64.py
--rw-r--r--   0        0        0     2367 2022-09-12 21:25:45.647092 bb-wrapper-0.4.8/bb_wrapper/services/barcode.py
--rw-r--r--   0        0        0     5597 2022-09-12 21:25:45.647092 bb-wrapper-0.4.8/bb_wrapper/services/barcode_cobranca.py
--rw-r--r--   0        0        0     7909 2022-09-12 21:25:45.647092 bb-wrapper-0.4.8/bb_wrapper/services/barcode_tributo.py
--rw-r--r--   0        0        0     2098 2022-09-12 21:25:45.647092 bb-wrapper-0.4.8/bb_wrapper/services/brcode.py
--rw-r--r--   0        0        0      636 2022-09-12 21:25:45.647092 bb-wrapper-0.4.8/bb_wrapper/services/dac.py
--rw-r--r--   0        0        0      816 2022-09-12 21:25:45.651092 bb-wrapper-0.4.8/bb_wrapper/services/document.py
--rw-r--r--   0        0        0     2718 2022-09-12 21:25:45.651092 bb-wrapper-0.4.8/bb_wrapper/services/mod.py
--rw-r--r--   0        0        0     1313 2022-09-12 21:25:45.651092 bb-wrapper-0.4.8/bb_wrapper/services/pix.py
--rw-r--r--   0        0        0     2897 2022-09-12 21:25:45.651092 bb-wrapper-0.4.8/bb_wrapper/services/pixcode.py
--rw-r--r--   0        0        0      494 2022-09-12 21:25:45.651092 bb-wrapper-0.4.8/bb_wrapper/services/qrcode.py
--rw-r--r--   0        0        0      420 2022-09-12 21:25:45.651092 bb-wrapper-0.4.8/bb_wrapper/services/unicode.py
--rw-r--r--   0        0        0      238 2022-09-12 21:25:45.651092 bb-wrapper-0.4.8/bb_wrapper/utils.py
--rw-r--r--   0        0        0      154 2022-09-12 21:25:45.651092 bb-wrapper-0.4.8/bb_wrapper/wrapper/__init__.py
--rw-r--r--   0        0        0     7661 2022-09-12 21:25:45.651092 bb-wrapper-0.4.8/bb_wrapper/wrapper/bb.py
--rw-r--r--   0        0        0     5183 2022-09-12 21:25:45.651092 bb-wrapper-0.4.8/bb_wrapper/wrapper/cobrancas.py
--rw-r--r--   0        0        0    14751 2022-09-12 21:25:45.651092 bb-wrapper-0.4.8/bb_wrapper/wrapper/pagamento_lote.py
--rw-r--r--   0        0        0     6062 2022-09-12 21:25:45.651092 bb-wrapper-0.4.8/bb_wrapper/wrapper/pix_cob.py
--rw-r--r--   0        0        0     5386 2022-09-12 21:25:45.651092 bb-wrapper-0.4.8/bb_wrapper/wrapper/request.py
--rw-r--r--   0        0        0     2061 2022-09-12 21:26:25.257892 bb-wrapper-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     3715 2022-09-12 21:26:25.943139 bb-wrapper-0.4.8/setup.py
--rw-r--r--   0        0        0     4209 2022-09-12 21:26:25.944152 bb-wrapper-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     2719 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/README.rst
+-rw-r--r--   0        0        0      213 2022-09-26 15:47:56.729763 bb-wrapper-0.4.9/bb_wrapper/__init__.py
+-rw-r--r--   0        0        0      747 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/constants.py
+-rw-r--r--   0        0        0        0 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/models/__init__.py
+-rw-r--r--   0        0        0     2819 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/models/barcode.py
+-rw-r--r--   0        0        0     3072 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/models/boleto.py
+-rw-r--r--   0        0        0    22579 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/models/pagamentos.py
+-rw-r--r--   0        0        0      827 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/models/perfis.py
+-rw-r--r--   0        0        0      657 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/models/pix_cob.py
+-rw-r--r--   0        0        0      463 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/services/__init__.py
+-rw-r--r--   0        0        0      469 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/services/b64.py
+-rw-r--r--   0        0        0     2367 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/services/barcode.py
+-rw-r--r--   0        0        0     5597 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/services/barcode_cobranca.py
+-rw-r--r--   0        0        0     7909 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/services/barcode_tributo.py
+-rw-r--r--   0        0        0     2098 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/services/brcode.py
+-rw-r--r--   0        0        0      636 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/services/dac.py
+-rw-r--r--   0        0        0      816 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/services/document.py
+-rw-r--r--   0        0        0     2718 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/services/mod.py
+-rw-r--r--   0        0        0     1313 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/services/pix.py
+-rw-r--r--   0        0        0     2897 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/services/pixcode.py
+-rw-r--r--   0        0        0      494 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/services/qrcode.py
+-rw-r--r--   0        0        0      420 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/services/unicode.py
+-rw-r--r--   0        0        0      238 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/utils.py
+-rw-r--r--   0        0        0      154 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/wrapper/__init__.py
+-rw-r--r--   0        0        0     7794 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/wrapper/bb.py
+-rw-r--r--   0        0        0     5148 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/wrapper/cobrancas.py
+-rw-r--r--   0        0        0    14751 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/wrapper/pagamento_lote.py
+-rw-r--r--   0        0        0     6062 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/wrapper/pix_cob.py
+-rw-r--r--   0        0        0     5720 2022-09-26 15:47:19.885258 bb-wrapper-0.4.9/bb_wrapper/wrapper/request.py
+-rw-r--r--   0        0        0     2061 2022-09-26 15:47:56.685762 bb-wrapper-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     3715 2022-09-26 15:47:57.227913 bb-wrapper-0.4.9/setup.py
+-rw-r--r--   0        0        0     4209 2022-09-26 15:47:57.228700 bb-wrapper-0.4.9/PKG-INFO
```

### Comparing `bb-wrapper-0.4.8/README.rst` & `bb-wrapper-0.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `bb-wrapper-0.4.8/bb_wrapper/constants.py` & `bb-wrapper-0.4.9/bb_wrapper/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from decouple import config
 
-
 IS_SANDBOX = config("IMOBANCO_BB_IS_SANDBOX", default=True, cast=bool)
 """É ambiente de teste?"""
 
 BASIC_TOKEN = config("IMOBANCO_BB_BASIC_TOKEN", default="")
 """Token básico para autenticação"""
 
 GW_APP_KEY = config("IMOBANCO_BB_GW_APP_KEY", default="")
```

### Comparing `bb-wrapper-0.4.8/bb_wrapper/models/barcode.py` & `bb-wrapper-0.4.9/bb_wrapper/models/barcode.py`

 * *Files identical despite different names*

### Comparing `bb-wrapper-0.4.8/bb_wrapper/models/boleto.py` & `bb-wrapper-0.4.9/bb_wrapper/models/boleto.py`

 * *Files identical despite different names*

### Comparing `bb-wrapper-0.4.8/bb_wrapper/models/pagamentos.py` & `bb-wrapper-0.4.9/bb_wrapper/models/pagamentos.py`

 * *Files identical despite different names*

### Comparing `bb-wrapper-0.4.8/bb_wrapper/models/perfis.py` & `bb-wrapper-0.4.9/bb_wrapper/models/perfis.py`

 * *Files identical despite different names*

### Comparing `bb-wrapper-0.4.8/bb_wrapper/models/pix_cob.py` & `bb-wrapper-0.4.9/bb_wrapper/models/pix_cob.py`

 * *Files identical despite different names*

### Comparing `bb-wrapper-0.4.8/bb_wrapper/services/barcode.py` & `bb-wrapper-0.4.9/bb_wrapper/services/barcode.py`

 * *Files identical despite different names*

### Comparing `bb-wrapper-0.4.8/bb_wrapper/services/barcode_cobranca.py` & `bb-wrapper-0.4.9/bb_wrapper/services/barcode_cobranca.py`

 * *Files identical despite different names*

### Comparing `bb-wrapper-0.4.8/bb_wrapper/services/barcode_tributo.py` & `bb-wrapper-0.4.9/bb_wrapper/services/barcode_tributo.py`

 * *Files identical despite different names*

### Comparing `bb-wrapper-0.4.8/bb_wrapper/services/brcode.py` & `bb-wrapper-0.4.9/bb_wrapper/services/brcode.py`

 * *Files identical despite different names*

### Comparing `bb-wrapper-0.4.8/bb_wrapper/services/dac.py` & `bb-wrapper-0.4.9/bb_wrapper/services/dac.py`

 * *Files identical despite different names*

### Comparing `bb-wrapper-0.4.8/bb_wrapper/services/document.py` & `bb-wrapper-0.4.9/bb_wrapper/services/document.py`

 * *Files identical despite different names*

### Comparing `bb-wrapper-0.4.8/bb_wrapper/services/mod.py` & `bb-wrapper-0.4.9/bb_wrapper/services/mod.py`

 * *Files identical despite different names*

### Comparing `bb-wrapper-0.4.8/bb_wrapper/services/pix.py` & `bb-wrapper-0.4.9/bb_wrapper/services/pix.py`

 * *Files identical despite different names*

### Comparing `bb-wrapper-0.4.8/bb_wrapper/services/pixcode.py` & `bb-wrapper-0.4.9/bb_wrapper/services/pixcode.py`

 * *Files identical despite different names*

### Comparing `bb-wrapper-0.4.8/bb_wrapper/wrapper/bb.py` & `bb-wrapper-0.4.9/bb_wrapper/wrapper/bb.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,21 @@
     SCOPE = ""
 
     TOKEN_EXPIRE_TIME = (10 * 60) - 30  # 9:30 minutos
     AUTH_MAX_RETRY_ATTEMPTS = 5
 
     def __init__(
         self,
+        *args,
         basic_token=None,
         is_sandbox=None,
         gw_app_key=None,
-        verify_https=False,
+        verify_https=True,
         cert=None,
+        **kwargs,
     ):
         if is_sandbox is None:
             is_sandbox = IS_SANDBOX
 
         if basic_token is None:
             basic_token = BASIC_TOKEN
 
@@ -44,15 +46,21 @@
         self._is_sandbox = is_sandbox
 
         if self.__basic_token == "" or self.__gw_app_key == "":
             raise ValueError("Configure o basic_token/gw_app_key do BB!")
 
         base_url = self._construct_base_url()
 
-        super().__init__(base_url=base_url, verify_https=verify_https, cert=cert)
+        super().__init__(
+            *args,
+            base_url=base_url,
+            verify_https=verify_https,
+            cert=cert,
+            **kwargs,
+        )
 
     def __new__(cls, *args, **kwargs):
         """
         Quando se fala de múltiplas classes com herança fazer:
             >>> getattr(self, f"_{self.__class__.__name__}__data", None)
 
         tem comportamento diferente de
@@ -203,15 +211,15 @@
         url = self.__oauth_url()
         header = {"Authorization": f"Basic {self.__basic_token}"}
 
         data = {
             "grant_type": "client_credentials",
             "scope": self.SCOPE,
         }
-        kwargs = dict(headers=header, verify=False, data=data)
+        kwargs = dict(headers=header, verify=self._verify_https, data=data)
 
         if self.__should_authenticate():
             session = requests.Session()
             retry_strategy = Retry(
                 total=self.AUTH_MAX_RETRY_ATTEMPTS,
                 backoff_factor=0.1,
                 status_forcelist=[401, 429, 500, 502, 503, 504],
```

### Comparing `bb-wrapper-0.4.8/bb_wrapper/wrapper/cobrancas.py` & `bb-wrapper-0.4.9/bb_wrapper/wrapper/cobrancas.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,31 +7,31 @@
 class CobrancasBBWrapper(BaseBBWrapper):
     SCOPE = "cobrancas.boletos-info cobrancas.boletos-requisicao"
 
     BASE_DOMAIN = ".bb.com.br/cobrancas/v2/boletos"
 
     def __init__(
         self,
+        *args,
         convenio=None,
         carteira=None,
         variacao_carteira=None,
         agencia=None,
         conta=None,
         basic_token=None,
         is_sandbox=None,
         gw_app_key=None,
-        verify_https=False,
-        cert=None,
+        **kwargs,
     ):
         super().__init__(
+            *args,
             basic_token=basic_token,
             is_sandbox=is_sandbox,
             gw_app_key=gw_app_key,
-            verify_https=verify_https,
-            cert=cert,
+            **kwargs,
         )
 
         if convenio is None:
             convenio = CONVENIO
 
         if carteira is None:
             carteira = CARTEIRA
```

### Comparing `bb-wrapper-0.4.8/bb_wrapper/wrapper/pagamento_lote.py` & `bb-wrapper-0.4.9/bb_wrapper/wrapper/pagamento_lote.py`

 * *Files identical despite different names*

### Comparing `bb-wrapper-0.4.8/bb_wrapper/wrapper/pix_cob.py` & `bb-wrapper-0.4.9/bb_wrapper/wrapper/pix_cob.py`

 * *Files identical despite different names*

### Comparing `bb-wrapper-0.4.8/bb_wrapper/wrapper/request.py` & `bb-wrapper-0.4.9/bb_wrapper/wrapper/request.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,20 +10,24 @@
 
 class RequestsWrapper:
     """
     wrapper da lib requests
 
     Attributes:
         __base_url: Url base para construir os requests
+        __timeout: Tempo máximo de espera de requests
+        __verity_https: flag que ativa verificação https
+        __cert: certificado http
     """
 
-    def __init__(self, base_url, verify_https=False, cert=None):
+    def __init__(self, *args, base_url, verify_https=True, cert=None, **kwargs):
         self.__base_url = base_url
+        self._verify_https = verify_https
         self.__cert = cert
-        self.__verify_https = verify_https
+        self.__timeout = kwargs.get("timeout", None)
 
     @staticmethod
     def _process_response(response) -> requests.Response:
         """
         Processa a resposta.
 
         Adiciona o :attr:`.data` carregado do :meth:`requests.Response.json`.
@@ -105,45 +109,45 @@
         if not headers:
             headers = self._authorization_header_data
 
         headers["Content-type"] = "application/json"
 
         return dict(
             headers=headers,
-            verify=self.__verify_https,
+            verify=self._verify_https,
             cert=self.__cert,
         )
 
     def _delete(self, url, headers=None) -> requests.Response:
         """
         http delete
 
         Args:
             url: url de requisição
 
         Returns:
             (:class:`.requests.Response`)
         """
         request_info = self._get_request_info(headers)
-        response = requests.delete(url, **request_info)
+        response = requests.delete(url, timeout=self.__timeout, **request_info)
         response = self._process_response(response)
         return response
 
     def _get(self, url, headers=None) -> requests.Response:
         """
         http get
 
         Args:
             url: url de requisição
 
         Returns:
             (:class:`.requests.Response`)
         """
         request_info = self._get_request_info(headers)
-        response = requests.get(url, **request_info)
+        response = requests.get(url, timeout=self.__timeout, **request_info)
         response = self._process_response(response)
         return response
 
     def _post(self, url, data, headers=None, use_json=True) -> requests.Response:
         """
         http post
 
@@ -157,15 +161,15 @@
             (:class:`.requests.Response`)
         """
         request_info = self._get_request_info(headers)
         if use_json:
             request_info["json"] = data
         else:
             request_info["data"] = data
-        response = requests.post(url, **request_info)
+        response = requests.post(url, timeout=self.__timeout, **request_info)
         response = self._process_response(response)
         return response
 
     def _put(self, url, data, headers=None, use_json=True) -> requests.Response:
         """
         http put
 
@@ -177,20 +181,20 @@
             (:class:`.requests.Response`)
         """
         request_info = self._get_request_info(headers)
         if use_json:
             request_info["json"] = data
         else:
             request_info["data"] = data
-        response = requests.put(url, **request_info)
+        response = requests.put(url, timeout=self.__timeout, **request_info)
         response = self._process_response(response)
         return response
 
     def _patch(self, url, data, headers=None, use_json=True) -> requests.Response:
         request_info = self._get_request_info(headers)
         if use_json:
             request_info["json"] = data
         else:
             request_info["data"] = data
-        response = requests.patch(url, **request_info)
+        response = requests.patch(url, timeout=self.__timeout, **request_info)
         response = self._process_response(response)
         return response
```

### Comparing `bb-wrapper-0.4.8/pyproject.toml` & `bb-wrapper-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 	"*/tests/*",
 	"*/examples/*",
 	"*/__init__.py"
 ]
 
 [tool.poetry]
 name = "bb-wrapper"
-version = "0.4.8"
+version = "0.4.9"
 description = "Cliente não oficial da API do Banco do Brasil"
 authors = ["Imobanco"]
 readme = "README.rst"
 packages = [{include = "bb_wrapper/**/*.py"}]
 homepage = "https://github.com/imobanco/bb-wrapper"
 repository = "https://github.com/imobanco/bb-wrapper"
 license = "GPLv3"
```

### Comparing `bb-wrapper-0.4.8/setup.py` & `bb-wrapper-0.4.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'python-barcode>=0.13.1,<0.14.0',
  'python-decouple>=3.4,<4.0',
  'qrcode>=7.3,<8.0',
  'requests>=2.26.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'bb-wrapper',
-    'version': '0.4.8',
+    'version': '0.4.9',
     'description': 'Cliente não oficial da API do Banco do Brasil',
     'long_description': "Cliente não oficial feito em Python, para realizar integração com as API's do Banco do Brasil.\n\n`Documentação oficial do BB <https://developers.bb.com.br/>`_\n\nInstalando\n===========\n\nNosso pacote está hospedado no `PyPI <https://pypi.org/project/bb-wrapper/>`_\n\n.. code-block:: bash\n\n    pip install bb-wrapper\n\n\n\nConfiguração\n==================\nPara utilizar o `bb-wrapper` é necessário ter algumas constantes/variáveis. sendo elas:\n\n.. code-block:: python\n\n    IMOBANCO_BB_IS_SANDBOX='flag True ou False para indicar utilização de sandbox ou não'\n    IMOBANCO_BB_BASIC_TOKEN='chave de autenticação gerada para a aplicação no site developers.bb'\n    IMOBANCO_BB_GW_APP_KEY='chave de desenvolvimento gerada para a aplicação no site developers.bb'\n\n\nPara geração de boletos é necessário:\n\n.. code-block:: python\n\n    IMOBANCO_BB_CONVENIO='convênio do contrato para geração de boletos'\n    IMOBANCO_BB_CARTEIRA='carteira do contrato para geração de boletos'\n    IMOBANCO_BB_VARIACAO_CARTEIRA='variação da carteira do contrato para geração de boletos\n    IMOBANCO_BB_AGENCIA='agência da conta berço do contrato para geração de boletos'\n    IMOBANCO_BB_CONTA='nº da conta berço do contrato para geração de boletos'\n\n\nRecomendamos criar um arquivo `.env` contendo essas varíaveis de ambiente.\n\n::\n\n    Podem ser criadas diretamente no terminal (não recomendado).\n\n    Podem ser criadas também diretamente no `arquivo.py` (não recomendado).\n\nRecursos disponíveis\n=====================\n\nAPI's\n---------------------\n\n- ☑ API de Cobrança (geração de boletos)\n- ☑ API PIX (recebimento PIX) {essa API ainda está instável e incompleta no BB}\n- ☐ API Arrecadação PIX {sem previsão de implementação}\n- ☑ API Lotes de Pagamentos {essa API ainda está instável e incompleta no BB}\n\n  - ☐ Transferência PIX\n  - ☑ Transferência Bancária\n  - ☐ Pagamento GPS\n  - ☐ Pagamento GRU\n  - ☐ Pagamento DARF Preto\n  - ☑ Pagamento Tributos\n  - ☑ Pagamento Boletos\n\nRecursos auxiliares\n-------------------\n\n- ☑ Geração de imagem b64\n- ☑ Geração, validação e conversão de código de barras de boleto\n- ☑ Geração, validação e conversão de código de barras de tributos\n- ☑ Geração de QR Code PIX\n- ☑ Validação e limpeza de CPF/CNPJ\n\nExemplos disponíveis\n=====================\nExistem exemplos de utilização da biblioteca na pasta `examples`.\n\nPreparando ambiente de desenvolvimento\n=======================================\n\n> O Nix é utilizado para gerenciar os pacotes necessários, por exemplo como a versão correta do python.\n\nCertifique-se que o ambiente está ativado, se não estiver execute:\n\n.. code-block:: bash\n\n    nix develop\n\n",
     'author': 'Imobanco',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/imobanco/bb-wrapper',
```

### Comparing `bb-wrapper-0.4.8/PKG-INFO` & `bb-wrapper-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bb-wrapper
-Version: 0.4.8
+Version: 0.4.9
 Summary: Cliente não oficial da API do Banco do Brasil
 Home-page: https://github.com/imobanco/bb-wrapper
 License: GPLv3
 Keywords: API,Banco,Brasil,BB,client,wrapper
 Author: Imobanco
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

