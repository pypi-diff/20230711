# Comparing `tmp/ezQgd-1.0.0-py2.py3-none-any.whl.zip` & `tmp/ezQgd-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 17199 bytes, number of entries: 13
--rw-r--r--  2.0 unx    33043 b- defN 23-May-24 15:55 ezQgd.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-24 15:55 qasmtoqcis/__init__.py
--rw-r--r--  2.0 unx     3973 b- defN 23-May-24 15:55 qasmtoqcis/const.py
--rw-r--r--  2.0 unx     7400 b- defN 23-May-24 15:55 qasmtoqcis/qasm.py
--rw-r--r--  2.0 unx    11185 b- defN 23-May-24 15:55 qasmtoqcis/qasm_to_qcis.py
--rw-r--r--  2.0 unx        0 b- defN 23-May-24 15:55 qcistoqasm/__init__.py
--rw-r--r--  2.0 unx      409 b- defN 23-May-24 15:55 qcistoqasm/const.py
--rw-r--r--  2.0 unx     2612 b- defN 23-May-24 15:55 qcistoqasm/qcis.py
--rw-r--r--  2.0 unx     2216 b- defN 23-May-24 15:55 qcistoqasm/qcis_to_qasm.py
--rw-r--r--  2.0 unx      872 b- defN 23-May-24 16:02 ezQgd-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-May-24 16:02 ezQgd-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       28 b- defN 23-May-24 16:02 ezQgd-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      976 b- defN 23-May-24 16:02 ezQgd-1.0.0.dist-info/RECORD
-13 files, 62824 bytes uncompressed, 15593 bytes compressed:  75.2%
+Zip file size: 17672 bytes, number of entries: 13
+-rw-r--r--  2.0 unx    35259 b- defN 23-Jul-11 15:38 ezQgd.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 05:52 qasmtoqcis/__init__.py
+-rw-r--r--  2.0 unx     3973 b- defN 23-Jul-11 05:52 qasmtoqcis/const.py
+-rw-r--r--  2.0 unx     7400 b- defN 23-Jul-11 05:52 qasmtoqcis/qasm.py
+-rw-r--r--  2.0 unx    11185 b- defN 23-Jul-11 05:52 qasmtoqcis/qasm_to_qcis.py
+-rw-r--r--  2.0 unx        0 b- defN 23-Jul-11 05:52 qcistoqasm/__init__.py
+-rw-r--r--  2.0 unx      409 b- defN 23-Jul-11 05:52 qcistoqasm/const.py
+-rw-r--r--  2.0 unx     2612 b- defN 23-Jul-11 05:52 qcistoqasm/qcis.py
+-rw-r--r--  2.0 unx     2216 b- defN 23-Jul-11 05:52 qcistoqasm/qcis_to_qasm.py
+-rw-r--r--  2.0 unx      872 b- defN 23-Jul-11 15:42 ezQgd-1.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-11 15:42 ezQgd-1.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       28 b- defN 23-Jul-11 15:42 ezQgd-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      975 b- defN 23-Jul-11 15:42 ezQgd-1.0.2.dist-info/RECORD
+13 files, 65021 bytes uncompressed, 16066 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: qcistoqasm/qcis.py
 Comment: 
 
 Filename: qcistoqasm/qcis_to_qasm.py
 Comment: 
 
-Filename: ezQgd-1.0.0.dist-info/METADATA
+Filename: ezQgd-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: ezQgd-1.0.0.dist-info/WHEEL
+Filename: ezQgd-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: ezQgd-1.0.0.dist-info/top_level.txt
+Filename: ezQgd-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: ezQgd-1.0.0.dist-info/RECORD
+Filename: ezQgd-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ezQgd.py

```diff
@@ -1,22 +1,23 @@
 # -*- coding: utf-8 -*-
 import json
 import requests
 import re
 import os
+import shutil
 import traceback
 from time import time, sleep
 import random
 import datetime
 import numpy as np
 from qasmtoqcis.qasm_to_qcis import QasmToQcis
 from qcistoqasm.qcis_to_qasm import QcisToQasm
 from isqmap import transpile
 from sabreMapper.sabre_mapper import SabreMapper
-from typing import List, Optional, Dict
+from typing import List, Optional, Dict, Union
 
 
 class Account():
 
     def __init__(
             self, 
             login_key: Optional[str]=None, 
@@ -151,28 +152,31 @@
             return 0
         save_result = result.get('data').get('exp_id')
         return save_result
 
     def run_experiment(
             self,
             exp_id: str, 
-            num_shots: Optional[int]=12000
+            num_shots: Optional[int]=12000,
+            is_verify: Optional[bool]=True
         ):
         """running the experiment returns the query result id.
 
         Args:
             exp_id: 
                 the result returned by the save_experiment interface, experimental id
             num_shots: 
                 number of repetitions per experiment. Defaults to 12000.
+            is_verify:
+                Is the circuit verified.True verify, False do not verify. Defaults to True.
 
         Returns:
             Union[int, str]: 0 failed, not 0 successful, success returns the query id
         """
-        data = {"exp_id": exp_id, "shots": num_shots}
+        data = {"exp_id": exp_id, "shots": num_shots, "is_verify": is_verify}
         return self.handler_run_experiment_result(data)
 
     def handler_run_experiment_result(
             self, 
             data
         ):
         url = self.base_url + '/service/sdk/api/experiment/temporary/save'
@@ -184,27 +188,28 @@
             return 0
         result = json.loads(res.text)
         code = result.get('code', -1)
         msg = result.get('message', '运行实验失败')
         if code != 0:
             print(f'运行实验失败：{msg}')
             return 0
-        run_result = result.get('data').get('query_id')
+        run_result = result.get('data').get('query_ids')
         return run_result
 
     def submit_job(
             self,
-            circuit: Optional[str]=None, 
+            circuit: Optional[Union[List, str]]=None, 
             exp_name: Optional[str]="exp0",
-            parameters: Optional[List]=None, 
-            values: Optional[List]=None,
+            parameters: Optional[List[List]]=None, 
+            values: Optional[List[List]]=None,
             num_shots: Optional[int]=12000,
             lab_id: Optional[str]=None, 
             exp_id: Optional[str]=None, 
-            version: Optional[str]="version01"
+            version: Optional[str]="version01",
+            is_verify: Optional[bool]=True
         ):
         """submit experimental tasks
 
         Args:
             circuit: 
                 experimental content, qics. Defaults to None.
             exp_name:
@@ -217,85 +222,110 @@
                 number of repetitions per experiment. Defaults to 12000.
             lab_id: 
                 the result returned by the create_experiment interface, experimental set id. Defaults to None.
             exp_id: 
                 the result returned by the save_experiment interface, experimental id. Defaults to None.
             version: 
                 version description. Defaults to 'version01'.
+            is_verify:
+                Is the circuit verified.True verify, False do not verify. Defaults to True.
+
+            There are some parameter range limitations when using batch submission circiuts.
+                1. circuits length less than 50
+                   numshots maximum 100000
+                   the number of measurement qubits is less than 15
+                2. circuits length greater than 50 but less than 100
+                   numshots maximum 50000
+                   the number of measurement qubits is less than 30
+                3. circuits length greater than 100 but less than 300
+                   numshots maximum 10000
+                   the number of measurement bits is less than the number of all available qubits
 
         Returns:
             Union[int, str]: 0 failed, not 0 successful, success returns the query id.
         """
-        if circuit:
-            circuit = self.assign_parameters(
-                circuit.upper(), parameters, values)
-            if not circuit:
+        if isinstance(circuit, str):
+            circuit = [circuit]
+        if len(circuit) > 1:
+            version = None
+        if circuit and parameters and values and len(parameters) == len(circuit) == len(values):
+            new_circuit = self.assign_parameters(circuit, parameters, values)
+            if not new_circuit:
                 print('无法为线路赋值，请检查线路，参数和参数值之后重试')
                 return 0
+        else:
+            new_circuit = circuit
         data = {
             "exp_id": exp_id,
             "lab_id": lab_id,
-            "inputCode": circuit,
+            "inputCode": new_circuit,
             "languageCode": "qcis",
             "name": exp_name,
             "shots": num_shots,
             "source": "SDK",
             "computerCode": self.machine_name,
-            "experimentDetailName": version
+            "experimentDetailName": version,
+            "is_verify": is_verify
         }
         return self.handler_run_experiment_result(data)
 
     def query_experiment(
             self,
-            query_id: str,
+            query_id: Union[str, List[str]],
             max_wait_time: Optional[int]=60
         ):
         """query experimental results
 
         Args:
             query_id: 
                 the result returned by the run_experiment interface, experimental set id
             max_wait_time: 
                 maximum waiting time for querying experiments. Defaults to 60.
 
+            The maximum number of experimental result queries supported by the server is 50.
+            If there are more than 50, an error message will be displayed.
+
         Returns:
             Union[int, str]: 0 failed, not 0 successful, success returns the experimental result
         """
+        if isinstance(query_id, str):
+            query_id = [query_id]
         t0 = time()
         while time()-t0 < max_wait_time:
             try:
-                url = f'{self.base_url}/service/sdk/api/experiment/result/find/{query_id}'
+                url = f'{self.base_url}/service/sdk/api/experiment/result/find/results'
                 headers = {"basicToken": self.token, "Authorization": f'Bearer {self.token}'}
-                res = requests.get(url, headers=headers)
+                data = {"query_ids": query_id}
+                res = requests.post(url, json=data, headers=headers)
                 status_code = res.status_code
                 if status_code != 200:
                     print('查询接口请求失败')
                     return 0
                 result = json.loads(res.text)
                 code = result.get('code', -1)
                 msg = result.get('message', '查询实验失败')
                 if code != 0:
                     print(f'查询实验失败：{msg}')
-                query_exp = result.get('data')
+                query_exp = result.get('data').get('experimentResultModelList')
                 if query_exp:
                     return query_exp
             except:
                 continue
             sleep_time = random.randint(
                 0, 15)*0.3+round(random.uniform(0, 1.5), 2)
             print(f'查询实验结果请等待: {{:.2f}}秒'.format(sleep_time))
             sleep(sleep_time)
         print(f'查询实验结果失败')
         return 0
 
     def assign_parameters(
             self,
-            circuit: str, 
-            parameters: List, 
-            values: List
+            circuits: List[str], 
+            parameters: List[List], 
+            values: List[List]
         ):
         """Check if the number of parameters, values match the circuit definition
 
         Args:
             circuit: 
                 string, QCIS circuit definition with or without parameter place holder
             parameters: 
@@ -303,63 +333,65 @@
             values: 
                 list or ndarray of floats, values to be assigned
 
         Returns:
             circuit: circuit with parameters replaced by values or empty string
             empty string occurs when errors prevents parameters to be assigned
         """
-        circuit = circuit.upper()
-        p = re.compile(r'\{(\w+)\}')
-        circuit_parameters = p.findall(circuit)
-        if circuit_parameters:
-
-            # 如果values为整数或浮点数，改为列表格式##########################################################
-            if isinstance(values, (float, int)):
-                values = [values]
-            # 如果parameters为字符格式，改为列表格式#########################################################
-            if isinstance(parameters, str):
-                parameters = [parameters]
-            # 将所有parameter变为大写， 否则set(parameters) != set(circuit_parameters) 不通过 ###############
-            parameters = [p.upper() for p in parameters]
-
-            if not values:
-                error_message = f'线路含有参数{circuit_parameters}, 请提供相应的参数值'
-                print(error_message)
-                return ''
+        new_circuit = []
+        for circuit, parameter, value in zip(circuits, parameters, values):
+            circuit = circuit.upper()
+            p = re.compile(r'\{(\w+)\}')
+            circuit_parameters = p.findall(circuit)
+            if circuit_parameters:
+                # # 如果values为整数或浮点数，改为列表格式##########################################################
+                # if isinstance(values, (float, int)):
+                #     values = [values]
+                # # 如果parameters为字符格式，改为列表格式#########################################################
+                # if isinstance(parameters, str):
+                #     parameters = [parameters]
+                
+                # 将所有parameter变为大写， 否则set(parameters) != set(circuit_parameters) 不通过 ###############
+                parameters = [p.upper() for p in parameter]
 
-            else:
-                if len(circuit_parameters) != len(values):
-                    error_message = f'线路含有{len(circuit_parameters)}个参数, 您提供了{len(values)}个参数值'
+                if not value:
+                    error_message = f'线路含有参数{circuit_parameters}, 请提供相应的参数值'
                     print(error_message)
                     return ''
 
-                elif parameters and len(circuit_parameters) != len(parameters):
-                    error_message = f'线路含有{len(circuit_parameters)}个参数, 您提供了{len(parameters)}个参数'
-                    print(error_message)
-                    return ''
-                
-                elif set(parameters) != set(circuit_parameters):
-                    error_message = '线路中的参数与您输入的参数名称不符'
-                    print(error_message)
                 else:
-                    param_dic = {}
-                    ############################# 这个转化可以删了 #########################################
-                    #parameters_upper = [p.upper() for p in parameters]
-                    for p, v in zip(parameters, values):
-                        param_dic[p] = v
-                    expData = circuit.format(**param_dic)
-                    return expData
-
-        elif parameters or values:
-            error_message = '线路定义中不含有参数，无法接受您输入的参数或参数值'
-            print(error_message)
-            return ''
-        else:
-            expData = circuit
-            return expData
+                    if len(circuit_parameters) != len(value):
+                        error_message = f'线路含有{len(circuit_parameters)}个参数, 您提供了{len(value)}个参数值'
+                        print(error_message)
+                        return ''
+
+                    elif parameter and len(circuit_parameters) != len(parameter):
+                        error_message = f'线路含有{len(circuit_parameters)}个参数, 您提供了{len(parameter)}个参数'
+                        print(error_message)
+                        return ''
+                    
+                    elif set(parameter) != set(circuit_parameters):
+                        error_message = '线路中的参数与您输入的参数名称不符'
+                        print(error_message)
+                    else:
+                        param_dic = {}
+                        ############################# 这个转化可以删了 #########################################
+                        #parameters_upper = [p.upper() for p in parameters]
+                        for p, v in zip(parameter, value):
+                            param_dic[p] = v
+                        expData = circuit.format(**param_dic)
+                        new_circuit.append(expData)
+            elif parameter or value:
+                error_message = '线路定义中不含有参数，无法接受您输入的参数或参数值'
+                print(error_message)
+                return ''
+            else:
+                expData = circuit
+                new_circuit.append(expData)
+        return new_circuit
 
     def get_experiment_data(
             self, 
             circuit: str
         ):
         """Parse circuit description and generate 
            experiment script and extract number of measured qubits.
@@ -766,19 +798,21 @@
             qasm_transpiled, _, _, _ = transpile(qasm_circuit,
                                                 qpu_file, 
                                                 initial_layout=initial_layout,
                                                 objective=objective,
                                                 seed=seed,
                                                 use_post_opt=use_post_opt)
             simplity_qcis = self.convert_qasm_to_qcis(qasm_transpiled)
+            os.remove(qpu_file)
             return simplity_qcis
         except Exception as e:
             print(e)
             print(traceback.format_exc())
             print('circuit mapping error, will submit using the original route')
+            os.remove(qpu_file)
             return qcis_circuit
     
     def qcis_mapping_sabre(
             self, 
             qcis_circuit: str):
         """The script transpiles qcis string by searching for a mapping from virtual to physical qubit 
            and a swap strategy such that the circuit described by qcis can be fitted into a hardware 
@@ -790,17 +824,18 @@
         Returns:
             str : qcis after mapping
         """       
         config_json = self.download_config(down_file=False)
         try:
             # qcis转换成qasm并写入qasm_file中
             qasm_circuit = self.qcistoqasm.convert_qcis_to_qasm(qcis_circuit)
-            if not os.path.exists('temp'):
-                os.makedirs('temp')
-            qasm_file = 'temp/qasm.qasm'
+            folder_path = 'temp'
+            if not os.path.exists(folder_path):
+                os.makedirs(folder_path)
+            qasm_file = f'{folder_path}/qasm.qasm'
             with open(qasm_file, 'w') as f:
                 f.write(qasm_circuit)
             sabre = SabreMapper()
             # 组装chip_info_fn映射信息
             chip_info_fn = {}
             couplings = []
             coupler_maps = config_json.get('overview').get('coupler_map')
@@ -816,33 +851,34 @@
             qubit_fidelity = {}
             for qubit, error in zip(qubit_used, qubit_gate_error):
                 qubit_fidelity[qubit] = 1 - error
             chip_info_fn['fidelity'] = qubit_fidelity
             chip_info_fn['has multiple chips'] = False
             chip_info_fn['qubits'] = qubit_used
 
-            chip_info_fn_file = "temp/chip_info_fn.json"
-            mapped_qasm_fn_file = "temp/mapped_qasm_fn.qasm"
-            qubit_mapping_fn_file = "temp/qubit_mapping_fn.json"
+            chip_info_fn_file = f'{folder_path}/chip_info_fn.json'
+            mapped_qasm_fn_file = f'{folder_path}/mapped_qasm_fn.qasm'
+            qubit_mapping_fn_file = f'{folder_path}/qubit_mapping_fn.json'
             with open(chip_info_fn_file, 'w') as f:
                 json.dump(chip_info_fn, f)
             # 调用quMapper做mapping操作
             success = sabre.map_schedule(qasm_file, chip_info_fn_file, mapped_qasm_fn_file, qubit_mapping_fn_file)
             if success:
                 with open(qubit_mapping_fn_file, 'r') as f:
                     qubit_mapping_fn = json.load(f)
                 qubit_map = qubit_mapping_fn.get('physical qubits idx')
                 # mapping成功，将转换后的qasm转为qcis，其中编号根据physical qubits idx做映射
                 simplity_qcis = self.convert_qasm_to_qcis_from_file(mapped_qasm_fn_file, qubit_map)
+                shutil.rmtree(folder_path)
                 return simplity_qcis
         except Exception as e:
             print(e)
-            import traceback
             print(traceback.format_exc())
             print('circuit mapping error, will submit using the original route')
+            shutil.rmtree(folder_path)
             return qcis_circuit
 
     def get_experiment_circuit(
             self,
             exp_id: str):
         """according to the exp_id obtained experimental circuit
```

## Comparing `ezQgd-1.0.0.dist-info/METADATA` & `ezQgd-1.0.2.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezQgd
-Version: 1.0.0
+Version: 1.0.2
 Summary: A SDK to use Quantum Computer @ quantumctek-cloud.com with QCIS.
 Home-page: https://quantumctek-cloud.com
 Author: Code42
 Author-email: support@quantumctek-cloud.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `ezQgd-1.0.0.dist-info/RECORD` & `ezQgd-1.0.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-ezQgd.py,sha256=5yqx39Gd64sNI4eA2cA88W79BaCca7VnKVC0TlfJiIU,33043
+ezQgd.py,sha256=7tZIDx1T0urunx-g77MUgWI3jXf2cW3QRMGUJaHFGnE,35259
 qasmtoqcis/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qasmtoqcis/const.py,sha256=AZTrt8AjrREnIHsK_VQrd_fEcB3TNBJqR1TiatsIurY,3973
 qasmtoqcis/qasm.py,sha256=Uu8zrTXpDCQok2lAeMCSChzjY6oE1xoV8LulgpAJSYc,7400
 qasmtoqcis/qasm_to_qcis.py,sha256=MSCwpWKtqcc5kY9tUgqg_0x30yi7J9v98_p89ikcKgI,11185
 qcistoqasm/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 qcistoqasm/const.py,sha256=jeuG0MbtqK3MxFlCC_eGwlsUO1nYp6B20KGztuJgmoc,409
 qcistoqasm/qcis.py,sha256=r5ae12O9ZFkCl3Bgw3ldyt2l451rESfZUC7P-qEaTL8,2612
 qcistoqasm/qcis_to_qasm.py,sha256=458xj6Z6rYhCD8918bc7TZZXLKcHhdJgPwQYCqOKIfM,2216
-ezQgd-1.0.0.dist-info/METADATA,sha256=WK3IaUl31d_zCL1M4Xp2fIkBJ2UJjg10STRcdJz_OxM,872
-ezQgd-1.0.0.dist-info/WHEEL,sha256=WzZ8cwjh8l0jtULNjYq1Hpr-WCqCRgPr--TX4P5I1Wo,110
-ezQgd-1.0.0.dist-info/top_level.txt,sha256=5SxS9D4ntYSuP5DotvN8wGdQVSZzRN2_NfaD7QO5U8o,28
-ezQgd-1.0.0.dist-info/RECORD,,
+ezQgd-1.0.2.dist-info/METADATA,sha256=_HtIoP6vfJH1pTt5q-mcYaA2ppfi7L7r0Z2AP82LDy4,872
+ezQgd-1.0.2.dist-info/WHEEL,sha256=ewwEueio1C2XeHTvT17n8dZUJgOvyCWCt0WVNLClP9o,92
+ezQgd-1.0.2.dist-info/top_level.txt,sha256=5SxS9D4ntYSuP5DotvN8wGdQVSZzRN2_NfaD7QO5U8o,28
+ezQgd-1.0.2.dist-info/RECORD,,
```

