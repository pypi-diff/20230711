# Comparing `tmp/pyxcp-0.20.4.tar.gz` & `tmp/pyxcp-0.21.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyxcp-0.20.4.tar", last modified: Wed Jul  5 14:18:31 2023, max compression
+gzip compressed data, was "pyxcp-0.21.1.tar", last modified: Tue Jul 11 13:05:46 2023, max compression
```

## Comparing `pyxcp-0.20.4.tar` & `pyxcp-0.21.1.tar`

### file list

```diff
@@ -1,142 +1,146 @@
--rw-r--r--   0        0        0     7652 2023-07-05 14:18:17.711047 pyxcp-0.20.4/LICENSE
--rw-r--r--   0        0        0     2484 2023-07-05 14:18:17.711047 pyxcp-0.20.4/README.md
--rw-r--r--   0        0        0     1285 2023-07-05 14:18:17.711047 pyxcp-0.20.4/build_ext.py
--rw-r--r--   0        0        0     3035 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyproject.toml
--rw-r--r--   0        0        0      699 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/__init__.py
--rw-r--r--   0        0        0     1557 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/aml/EtasCANMonitoring.a2l
--rw-r--r--   0        0        0     2338 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/aml/EtasCANMonitoring.aml
--rw-r--r--   0        0        0    15038 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/aml/XCP_Common.aml
--rw-r--r--   0        0        0     3771 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/aml/XCPonCAN.aml
--rw-r--r--   0        0        0     2214 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/aml/XCPonEth.aml
--rw-r--r--   0        0        0     4647 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/aml/XCPonFlx.aml
--rw-r--r--   0        0        0     3235 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/aml/XCPonSxI.aml
--rw-r--r--   0        0        0     4846 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/aml/XCPonUSB.aml
--rw-r--r--   0        0        0      593 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/aml/ifdata_CAN.a2l
--rw-r--r--   0        0        0      240 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/aml/ifdata_Eth.a2l
--rw-r--r--   0        0        0     1798 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/aml/ifdata_Flx.a2l
--rw-r--r--   0        0        0      304 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/aml/ifdata_SxI.a2l
--rw-r--r--   0        0        0     3576 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/aml/ifdata_USB.a2l
--rw-r--r--   0        0        0        0 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/asam/__init__.py
--rw-r--r--   0        0        0     2361 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/asam/types.py
--rw-r--r--   0        0        0     2836 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/asamkeydll.c
--rw-r--r--   0        0        0       57 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/asamkeydll.sh
--rw-r--r--   0        0        0    10837 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/checksum.py
--rw-r--r--   0        0        0     2089 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/cmdline.py
--rw-r--r--   0        0        0     1423 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/config.py
--rw-r--r--   0        0        0     1258 2023-07-05 14:18:17.711047 pyxcp-0.20.4/pyxcp/constants.py
--rw-r--r--   0        0        0      410 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/asynchiofactory.hpp
--rw-r--r--   0        0        0     1180 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/blocking_client.cpp
--rw-r--r--   0        0        0     1001 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/blocking_socket.cpp
--rw-r--r--   0        0        0    15549 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/blocking_socket.hpp
--rw-r--r--   0        0        0     1412 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/concurrent_queue.hpp
--rw-r--r--   0        0        0      921 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/eth.hpp
--rw-r--r--   0        0        0      678 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/exceptions.hpp
--rw-r--r--   0        0        0      624 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/iasyncioservice.hpp
--rw-r--r--   0        0        0      230 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/iresource.hpp
--rw-r--r--   0        0        0      613 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/isocket.hpp
--rw-r--r--   0        0        0     1857 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/linux/epoll.cpp
--rw-r--r--   0        0        0     2357 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/linux/epoll.hpp
--rw-r--r--   0        0        0      352 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/linux/lit_tester.cpp
--rw-r--r--   0        0        0     7123 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/linux/socket.hpp
--rw-r--r--   0        0        0     1600 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/linux/timeout.hpp
--rw-r--r--   0        0        0      652 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/memoryblock.hpp
--rw-r--r--   0        0        0     1755 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/pool.hpp
--rw-r--r--   0        0        0      111 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/poolmgr.cpp
--rw-r--r--   0        0        0      424 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/poolmgr.hpp
--rw-r--r--   0        0        0     1432 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/test_queue.cpp
--rw-r--r--   0        0        0     1928 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/timestamp.hpp
--rw-r--r--   0        0        0      627 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/utils.cpp
--rw-r--r--   0        0        0      802 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/utils.hpp
--rw-r--r--   0        0        0     7292 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/win/iocp.cpp
--rw-r--r--   0        0        0      879 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/win/iocp.hpp
--rw-r--r--   0        0        0      488 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/win/perhandledata.hpp
--rw-r--r--   0        0        0     1945 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/win/periodata.hpp
--rw-r--r--   0        0        0     5246 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/win/socket.hpp
--rw-r--r--   0        0        0     1856 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/cxx/win/timeout.hpp
--rw-r--r--   0        0        0     2459 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/dllif.py
--rw-r--r--   0        0        0    44403 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/errormatrix.py
--rw-r--r--   0        0        0      454 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/examples/conf_can.json
--rw-r--r--   0        0        0      322 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/examples/conf_can.toml
--rw-r--r--   0        0        0      298 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/examples/conf_can_user.toml
--rw-r--r--   0        0        0      256 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/examples/conf_can_vector.json
--rw-r--r--   0        0        0      199 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/examples/conf_can_vector.toml
--rw-r--r--   0        0        0      148 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/examples/conf_eth.json
--rw-r--r--   0        0        0      109 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/examples/conf_eth.toml
--rw-r--r--   0        0        0      460 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/examples/conf_nixnet.json
--rw-r--r--   0        0        0      257 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/examples/conf_socket_can.toml
--rw-r--r--   0        0        0      163 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/examples/conf_sxi.json
--rw-r--r--   0        0        0      118 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/examples/conf_sxi.toml
--rw-r--r--   0        0        0      839 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/examples/xcp_read_benchmark.py
--rw-r--r--   0        0        0     1160 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/examples/xcp_skel.py
--rw-r--r--   0        0        0      675 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/examples/xcp_unlock.py
--rw-r--r--   0        0        0     1046 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/examples/xcp_user_supplied_driver.py
--rw-r--r--   0        0        0     2479 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/examples/xcphello.py
--rw-r--r--   0        0        0     1924 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/logger.py
--rw-r--r--   0        0        0      319 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/master/__init__.py
--rw-r--r--   0        0        0    13219 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/master/errorhandler.py
--rw-r--r--   0        0        0    69088 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/master/master.py
--rw-r--r--   0        0        0     2185 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/recorder/__init__.py
--rw-r--r--   0        0        0      174 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/recorder/build_clang.cmd
--rwxr-xr-x   0        0        0      179 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/recorder/build_clang.sh
--rw-r--r--   0        0        0      237 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/recorder/build_gcc.cmd
--rwxr-xr-x   0        0        0      209 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/recorder/build_gcc.sh
--rwxr-xr-x   0        0        0      238 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/recorder/build_gcc_arm.sh
--rw-r--r--   0        0        0   105107 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/recorder/lz4.cpp
--rw-r--r--   0        0        0    40859 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/recorder/lz4.h
--rw-r--r--   0        0        0    59847 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/recorder/mio.hpp
--rw-r--r--   0        0        0     8541 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/recorder/reco.py
--rw-r--r--   0        0        0        0 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/recorder/recorder.rst
--rw-r--r--   0        0        0     1790 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/recorder/rekorder.cpp
--rw-r--r--   0        0        0    18556 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/recorder/rekorder.hpp
--rw-r--r--   0        0        0     1068 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/recorder/setup.py
--rw-r--r--   0        0        0     1031 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/recorder/test_reko.py
--rw-r--r--   0        0        0      813 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/recorder/wrap.cpp
--rw-r--r--   0        0        0        0 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/scripts/__init__.py
--rw-r--r--   0        0        0      597 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/scripts/pyxcp_probe_can_drivers.py
--rw-r--r--   0        0        0      897 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/scripts/xcp_fetch_a2l.py
--rw-r--r--   0        0        0      472 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/scripts/xcp_id_scanner.py
--rw-r--r--   0        0        0     2479 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/scripts/xcp_info.py
--rw-r--r--   0        0        0      563 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/tests/test_asam_types.py
--rw-r--r--   0        0        0     4886 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/tests/test_can.py
--rw-r--r--   0        0        0     1712 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/tests/test_checksum.py
--rw-r--r--   0        0        0     1317 2023-07-05 14:18:17.715047 pyxcp-0.20.4/pyxcp/tests/test_config.py
--rw-r--r--   0        0        0     3012 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/tests/test_frame_padding.py
--rw-r--r--   0        0        0    69219 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/tests/test_master.py
--rw-r--r--   0        0        0     1680 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/tests/test_transport.py
--rw-r--r--   0        0        0      941 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/tests/test_utils.py
--rw-r--r--   0        0        0     1670 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/timing.py
--rw-r--r--   0        0        0      140 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/__init__.py
--rw-r--r--   0        0        0    10504 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/base.py
--rw-r--r--   0        0        0    12209 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/can.py
--rw-r--r--   0        0        0       46 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/__init__.py
--rw-r--r--   0        0        0      713 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/pc_canalystii.py
--rw-r--r--   0        0        0      602 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/pc_etas.py
--rw-r--r--   0        0        0      563 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/pc_gsusb.py
--rw-r--r--   0        0        0      571 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/pc_iscan.py
--rw-r--r--   0        0        0      722 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/pc_ixxat.py
--rw-r--r--   0        0        0     1104 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/pc_kvaser.py
--rw-r--r--   0        0        0      893 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/pc_neovi.py
--rw-r--r--   0        0        0      557 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/pc_nican.py
--rw-r--r--   0        0        0      565 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/pc_nixnet.py
--rw-r--r--   0        0        0      570 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/pc_pcan.py
--rw-r--r--   0        0        0      732 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/pc_seeed.py
--rw-r--r--   0        0        0      689 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/pc_serial.py
--rw-r--r--   0        0        0      827 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/pc_slcan.py
--rw-r--r--   0        0        0      535 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/pc_socketcan.py
--rw-r--r--   0        0        0      812 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/pc_systec.py
--rw-r--r--   0        0        0      662 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/pc_usb2can.py
--rw-r--r--   0        0        0      972 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/pc_vector.py
--rw-r--r--   0        0        0     3027 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/candriver/python_can.py
--rw-r--r--   0        0        0     1179 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/cxx_ext/CMakeLists.txt
--rw-r--r--   0        0        0     1247 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/cxx_ext/setup.py
--rw-r--r--   0        0        0      871 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/cxx_ext/tests/test_basic_socket.cpp
--rw-r--r--   0        0        0      833 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/cxx_ext/tests/test_pool.cpp
--rw-r--r--   0        0        0      513 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/cxx_ext/tests/test_timestamp.cpp
--rw-r--r--   0        0        0     6975 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/eth.py
--rw-r--r--   0        0        0     2474 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/sxi.py
--rw-r--r--   0        0        0     6881 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/transport/usb_transport.py
--rw-r--r--   0        0        0    23338 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/types.py
--rw-r--r--   0        0        0     1604 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/utils.py
--rw-r--r--   0        0        0        0 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/vector/__init__.py
--rw-r--r--   0        0        0     2285 2023-07-05 14:18:17.719047 pyxcp-0.20.4/pyxcp/vector/map.py
--rw-r--r--   0        0        0     3371 1970-01-01 00:00:00.000000 pyxcp-0.20.4/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-07-11 13:05:31.020678 pyxcp-0.21.1/LICENSE
+-rw-r--r--   0        0        0     2484 2023-07-11 13:05:31.020678 pyxcp-0.21.1/README.md
+-rw-r--r--   0        0        0     1283 2023-07-11 13:05:31.020678 pyxcp-0.21.1/build_ext.py
+-rw-r--r--   0        0        0     3035 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyproject.toml
+-rw-r--r--   0        0        0      699 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/__init__.py
+-rw-r--r--   0        0        0     1557 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/aml/EtasCANMonitoring.a2l
+-rw-r--r--   0        0        0     2338 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/aml/EtasCANMonitoring.aml
+-rw-r--r--   0        0        0    15038 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/aml/XCP_Common.aml
+-rw-r--r--   0        0        0     3771 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/aml/XCPonCAN.aml
+-rw-r--r--   0        0        0     2214 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/aml/XCPonEth.aml
+-rw-r--r--   0        0        0     4647 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/aml/XCPonFlx.aml
+-rw-r--r--   0        0        0     3235 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/aml/XCPonSxI.aml
+-rw-r--r--   0        0        0     4846 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/aml/XCPonUSB.aml
+-rw-r--r--   0        0        0      593 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/aml/ifdata_CAN.a2l
+-rw-r--r--   0        0        0      240 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/aml/ifdata_Eth.a2l
+-rw-r--r--   0        0        0     1798 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/aml/ifdata_Flx.a2l
+-rw-r--r--   0        0        0      304 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/aml/ifdata_SxI.a2l
+-rw-r--r--   0        0        0     3576 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/aml/ifdata_USB.a2l
+-rw-r--r--   0        0        0        0 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/asam/__init__.py
+-rw-r--r--   0        0        0     2361 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/asam/types.py
+-rw-r--r--   0        0        0     2862 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/asamkeydll.c
+-rw-r--r--   0        0        0       57 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/asamkeydll.sh
+-rw-r--r--   0        0        0    10837 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/checksum.py
+-rw-r--r--   0        0        0     2117 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cmdline.py
+-rw-r--r--   0        0        0     1423 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/config.py
+-rw-r--r--   0        0        0     1258 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/constants.py
+-rw-r--r--   0        0        0      410 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/asynchiofactory.hpp
+-rw-r--r--   0        0        0     1180 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/blocking_client.cpp
+-rw-r--r--   0        0        0     1001 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/blocking_socket.cpp
+-rw-r--r--   0        0        0    15549 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/blocking_socket.hpp
+-rw-r--r--   0        0        0     1412 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/concurrent_queue.hpp
+-rw-r--r--   0        0        0      921 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/eth.hpp
+-rw-r--r--   0        0        0      678 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/exceptions.hpp
+-rw-r--r--   0        0        0      624 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/iasyncioservice.hpp
+-rw-r--r--   0        0        0      230 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/iresource.hpp
+-rw-r--r--   0        0        0      613 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/isocket.hpp
+-rw-r--r--   0        0        0     1857 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/linux/epoll.cpp
+-rw-r--r--   0        0        0     2357 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/linux/epoll.hpp
+-rw-r--r--   0        0        0      352 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/linux/lit_tester.cpp
+-rw-r--r--   0        0        0     7123 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/linux/socket.hpp
+-rw-r--r--   0        0        0     1600 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/linux/timeout.hpp
+-rw-r--r--   0        0        0      652 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/memoryblock.hpp
+-rw-r--r--   0        0        0     1755 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/pool.hpp
+-rw-r--r--   0        0        0      111 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/poolmgr.cpp
+-rw-r--r--   0        0        0      424 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/poolmgr.hpp
+-rw-r--r--   0        0        0     1432 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/test_queue.cpp
+-rw-r--r--   0        0        0     1928 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/timestamp.hpp
+-rw-r--r--   0        0        0      627 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/utils.cpp
+-rw-r--r--   0        0        0      802 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/utils.hpp
+-rw-r--r--   0        0        0     7292 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/win/iocp.cpp
+-rw-r--r--   0        0        0      879 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/win/iocp.hpp
+-rw-r--r--   0        0        0      488 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/win/perhandledata.hpp
+-rw-r--r--   0        0        0     1945 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/win/periodata.hpp
+-rw-r--r--   0        0        0     5246 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/win/socket.hpp
+-rw-r--r--   0        0        0     1856 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/cxx/win/timeout.hpp
+-rw-r--r--   0        0        0     3023 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/dllif.py
+-rw-r--r--   0        0        0    44403 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/errormatrix.py
+-rw-r--r--   0        0        0      454 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/conf_can.json
+-rw-r--r--   0        0        0      322 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/conf_can.toml
+-rw-r--r--   0        0        0      298 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/conf_can_user.toml
+-rw-r--r--   0        0        0      256 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/conf_can_vector.json
+-rw-r--r--   0        0        0      199 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/conf_can_vector.toml
+-rw-r--r--   0        0        0      148 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/conf_eth.json
+-rw-r--r--   0        0        0      109 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/conf_eth.toml
+-rw-r--r--   0        0        0      460 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/conf_nixnet.json
+-rw-r--r--   0        0        0      257 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/conf_socket_can.toml
+-rw-r--r--   0        0        0      163 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/conf_sxi.json
+-rw-r--r--   0        0        0      118 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/conf_sxi.toml
+-rw-r--r--   0        0        0     1881 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/xcp_policy.py
+-rw-r--r--   0        0        0      839 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/xcp_read_benchmark.py
+-rw-r--r--   0        0        0     1160 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/xcp_skel.py
+-rw-r--r--   0        0        0      675 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/xcp_unlock.py
+-rw-r--r--   0        0        0     1046 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/xcp_user_supplied_driver.py
+-rw-r--r--   0        0        0     2480 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/xcphello.py
+-rw-r--r--   0        0        0     3265 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/examples/xcphello_recorder.py
+-rw-r--r--   0        0        0     1924 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/logger.py
+-rw-r--r--   0        0        0      319 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/master/__init__.py
+-rw-r--r--   0        0        0    13219 2023-07-11 13:05:31.020678 pyxcp-0.21.1/pyxcp/master/errorhandler.py
+-rw-r--r--   0        0        0    69202 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/master/master.py
+-rw-r--r--   0        0        0     2260 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/__init__.py
+-rw-r--r--   0        0        0      174 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/build_clang.cmd
+-rwxr-xr-x   0        0        0      179 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/build_clang.sh
+-rw-r--r--   0        0        0      237 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/build_gcc.cmd
+-rwxr-xr-x   0        0        0      209 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/build_gcc.sh
+-rwxr-xr-x   0        0        0      238 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/build_gcc_arm.sh
+-rw-r--r--   0        0        0   114204 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/lz4.c
+-rw-r--r--   0        0        0    44421 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/lz4.h
+-rw-r--r--   0        0        0    70760 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/lz4hc.c
+-rw-r--r--   0        0        0    20179 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/lz4hc.h
+-rw-r--r--   0        0        0    59847 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/mio.hpp
+-rw-r--r--   0        0        0     8541 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/reco.py
+-rw-r--r--   0        0        0        0 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/recorder.rst
+-rw-r--r--   0        0        0     1794 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/rekorder.cpp
+-rw-r--r--   0        0        0    18964 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/rekorder.hpp
+-rw-r--r--   0        0        0     1068 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/setup.py
+-rw-r--r--   0        0        0     1031 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/test_reko.py
+-rw-r--r--   0        0        0      813 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/recorder/wrap.cpp
+-rw-r--r--   0        0        0        0 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/scripts/__init__.py
+-rw-r--r--   0        0        0      597 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/scripts/pyxcp_probe_can_drivers.py
+-rw-r--r--   0        0        0      897 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/scripts/xcp_fetch_a2l.py
+-rw-r--r--   0        0        0      472 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/scripts/xcp_id_scanner.py
+-rw-r--r--   0        0        0     2479 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/scripts/xcp_info.py
+-rw-r--r--   0        0        0      563 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/tests/test_asam_types.py
+-rw-r--r--   0        0        0     4886 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/tests/test_can.py
+-rw-r--r--   0        0        0     1712 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/tests/test_checksum.py
+-rw-r--r--   0        0        0     1317 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/tests/test_config.py
+-rw-r--r--   0        0        0     3012 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/tests/test_frame_padding.py
+-rw-r--r--   0        0        0    69219 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/tests/test_master.py
+-rw-r--r--   0        0        0     1680 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/tests/test_transport.py
+-rw-r--r--   0        0        0      941 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/tests/test_utils.py
+-rw-r--r--   0        0        0     1670 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/timing.py
+-rw-r--r--   0        0        0      297 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/__init__.py
+-rw-r--r--   0        0        0    14247 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/base.py
+-rw-r--r--   0        0        0    12231 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/can.py
+-rw-r--r--   0        0        0       46 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/__init__.py
+-rw-r--r--   0        0        0      713 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/pc_canalystii.py
+-rw-r--r--   0        0        0      602 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/pc_etas.py
+-rw-r--r--   0        0        0      563 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/pc_gsusb.py
+-rw-r--r--   0        0        0      571 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/pc_iscan.py
+-rw-r--r--   0        0        0      722 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/pc_ixxat.py
+-rw-r--r--   0        0        0     1104 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/pc_kvaser.py
+-rw-r--r--   0        0        0      893 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/pc_neovi.py
+-rw-r--r--   0        0        0      557 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/pc_nican.py
+-rw-r--r--   0        0        0      565 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/pc_nixnet.py
+-rw-r--r--   0        0        0      570 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/pc_pcan.py
+-rw-r--r--   0        0        0      732 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/pc_seeed.py
+-rw-r--r--   0        0        0      689 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/pc_serial.py
+-rw-r--r--   0        0        0      827 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/pc_slcan.py
+-rw-r--r--   0        0        0      535 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/pc_socketcan.py
+-rw-r--r--   0        0        0      812 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/pc_systec.py
+-rw-r--r--   0        0        0      662 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/pc_usb2can.py
+-rw-r--r--   0        0        0      972 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/pc_vector.py
+-rw-r--r--   0        0        0     3027 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/candriver/python_can.py
+-rw-r--r--   0        0        0     1179 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/cxx_ext/CMakeLists.txt
+-rw-r--r--   0        0        0     1247 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/cxx_ext/setup.py
+-rw-r--r--   0        0        0      871 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/cxx_ext/tests/test_basic_socket.cpp
+-rw-r--r--   0        0        0      833 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/cxx_ext/tests/test_pool.cpp
+-rw-r--r--   0        0        0      513 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/cxx_ext/tests/test_timestamp.cpp
+-rw-r--r--   0        0        0     7537 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/eth.py
+-rw-r--r--   0        0        0     2496 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/sxi.py
+-rw-r--r--   0        0        0     6903 2023-07-11 13:05:31.024679 pyxcp-0.21.1/pyxcp/transport/usb_transport.py
+-rw-r--r--   0        0        0    23520 2023-07-11 13:05:31.028679 pyxcp-0.21.1/pyxcp/types.py
+-rw-r--r--   0        0        0     1604 2023-07-11 13:05:31.028679 pyxcp-0.21.1/pyxcp/utils.py
+-rw-r--r--   0        0        0        0 2023-07-11 13:05:31.028679 pyxcp-0.21.1/pyxcp/vector/__init__.py
+-rw-r--r--   0        0        0     2285 2023-07-11 13:05:31.028679 pyxcp-0.21.1/pyxcp/vector/map.py
+-rw-r--r--   0        0        0     3371 1970-01-01 00:00:00.000000 pyxcp-0.21.1/PKG-INFO
```

### Comparing `pyxcp-0.20.4/LICENSE` & `pyxcp-0.21.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/README.md` & `pyxcp-0.21.1/README.md`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/build_ext.py` & `pyxcp-0.21.1/build_ext.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 ParallelCompile("NPY_NUM_BUILD_JOBS", needs_recompile=naive_recompile).install()
 
 ext_modules = [
     Pybind11Extension(
         EXT_NAMES[0],
         include_dirs=[PYB11_INCLUDE_DIRS, "pyxcp/recorder"],
-        sources=["pyxcp/recorder/lz4.cpp", "pyxcp/recorder/wrap.cpp"],
+        sources=["pyxcp/recorder/lz4.c", "pyxcp/recorder/wrap.cpp"],
         define_macros=[("EXTENSION_NAME", EXT_NAMES[0]), ("NDEBUG", 1)],
         optional=False,
         cxx_std=20,  # Extension will use C++20 generators/coroutines.
     ),
 ]
```

### Comparing `pyxcp-0.20.4/pyproject.toml` & `pyxcp-0.21.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
     "pyserial<4.0,>=3.5",
     "pyusb<2.0.0,>=1.2.1",
     "toml<1.0.0,>=0.10.2",
     "python-can>=4.0.0",
     "uptime>=3.0.1",
 ]
 name = "pyxcp"
-version = "0.20.4"
+version = "0.21.1"
 readme = "README.md"
 description = "Universal Calibration Protocol for Python"
 keywords = [
     "automotive",
     "ecu",
     "xcp",
     "asam",
```

### Comparing `pyxcp-0.20.4/pyxcp/__init__.py` & `pyxcp-0.21.1/pyxcp/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,8 +21,8 @@
 from .master import Master
 from .transport import Can
 from .transport import Eth
 from .transport import SxI
 from .transport import Usb
 
 # if you update this manually, do not forget to update .bumpversion.cfg
-__version__ = "0.20.4"
+__version__ = "0.21.1"
```

### Comparing `pyxcp-0.20.4/pyxcp/aml/EtasCANMonitoring.a2l` & `pyxcp-0.21.1/pyxcp/aml/EtasCANMonitoring.a2l`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/aml/EtasCANMonitoring.aml` & `pyxcp-0.21.1/pyxcp/aml/EtasCANMonitoring.aml`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/aml/XCP_Common.aml` & `pyxcp-0.21.1/pyxcp/aml/XCP_Common.aml`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/aml/XCPonCAN.aml` & `pyxcp-0.21.1/pyxcp/aml/XCPonCAN.aml`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/aml/XCPonEth.aml` & `pyxcp-0.21.1/pyxcp/aml/XCPonEth.aml`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/aml/XCPonFlx.aml` & `pyxcp-0.21.1/pyxcp/aml/XCPonFlx.aml`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/aml/XCPonSxI.aml` & `pyxcp-0.21.1/pyxcp/aml/XCPonSxI.aml`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/aml/XCPonUSB.aml` & `pyxcp-0.21.1/pyxcp/aml/XCPonUSB.aml`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/aml/ifdata_CAN.a2l` & `pyxcp-0.21.1/pyxcp/aml/ifdata_CAN.a2l`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/aml/ifdata_Flx.a2l` & `pyxcp-0.21.1/pyxcp/aml/ifdata_Flx.a2l`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/aml/ifdata_USB.a2l` & `pyxcp-0.21.1/pyxcp/aml/ifdata_USB.a2l`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/asam/types.py` & `pyxcp-0.21.1/pyxcp/asam/types.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/asamkeydll.c` & `pyxcp-0.21.1/pyxcp/asamkeydll.c`

 * *Files 2% similar despite different names*

```diff
@@ -106,11 +106,12 @@
         cbuf[0] = nameBuffer[idx * 2];
         cbuf[1] = nameBuffer[(idx * 2) + 1 ];
         cbuf[2] = '\x00';
         seedBuffer[idx] = strtol(cbuf, 0, 16);
     }
 
     res = GetKey((char *)&dllname, privilege, seedlen, (BYTE *)&seedBuffer, &keylen, (BYTE *)&keyBuffer);
+    printf("%lu\n", res);
     if (res == 0) {
         hexlify(keyBuffer, keylen);
     }
 }
```

### Comparing `pyxcp-0.20.4/pyxcp/checksum.py` & `pyxcp-0.21.1/pyxcp/checksum.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cmdline.py` & `pyxcp-0.21.1/pyxcp/cmdline.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,26 +45,26 @@
         self._parser.epilog = "To get specific help on transport layers\nuse <layer> -h, e.g. {} eth -h".format(self._parser.prog)
         self._args = []
 
     @property
     def args(self):
         return self._args
 
-    def run(self):
+    def run(self, policy=None):
         """"""
         self._args = self.parser.parse_args()
         args = self.args
         if args.conf is None:
             raise RuntimeError("Configuration file must be specified! (option: -c <file>)")
         config = readConfiguration(args.conf)
         config["LOGLEVEL"] = args.loglevel
         if "TRANSPORT" not in config:
             raise AttributeError("TRANSPORT must be specified in config!")
         transport = config["TRANSPORT"].lower()
-        master = Master(transport, config=config)
+        master = Master(transport, config=config, policy=policy)
         if self.callout:
             self.callout(master, args)
         return master
 
     @property
     def parser(self):
         return self._parser
```

### Comparing `pyxcp-0.20.4/pyxcp/config.py` & `pyxcp-0.21.1/pyxcp/config.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/constants.py` & `pyxcp-0.21.1/pyxcp/constants.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/blocking_client.cpp` & `pyxcp-0.21.1/pyxcp/cxx/blocking_client.cpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/blocking_socket.cpp` & `pyxcp-0.21.1/pyxcp/cxx/blocking_socket.cpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/blocking_socket.hpp` & `pyxcp-0.21.1/pyxcp/cxx/blocking_socket.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/concurrent_queue.hpp` & `pyxcp-0.21.1/pyxcp/cxx/concurrent_queue.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/eth.hpp` & `pyxcp-0.21.1/pyxcp/cxx/eth.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/exceptions.hpp` & `pyxcp-0.21.1/pyxcp/cxx/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/iasyncioservice.hpp` & `pyxcp-0.21.1/pyxcp/cxx/iasyncioservice.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/isocket.hpp` & `pyxcp-0.21.1/pyxcp/cxx/isocket.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/linux/epoll.cpp` & `pyxcp-0.21.1/pyxcp/cxx/linux/epoll.cpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/linux/epoll.hpp` & `pyxcp-0.21.1/pyxcp/cxx/linux/epoll.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/linux/socket.hpp` & `pyxcp-0.21.1/pyxcp/cxx/linux/socket.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/linux/timeout.hpp` & `pyxcp-0.21.1/pyxcp/cxx/linux/timeout.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/memoryblock.hpp` & `pyxcp-0.21.1/pyxcp/cxx/memoryblock.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/pool.hpp` & `pyxcp-0.21.1/pyxcp/cxx/pool.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/test_queue.cpp` & `pyxcp-0.21.1/pyxcp/cxx/test_queue.cpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/timestamp.hpp` & `pyxcp-0.21.1/pyxcp/cxx/timestamp.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/utils.cpp` & `pyxcp-0.21.1/pyxcp/cxx/utils.cpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/utils.hpp` & `pyxcp-0.21.1/pyxcp/cxx/utils.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/win/iocp.cpp` & `pyxcp-0.21.1/pyxcp/cxx/win/iocp.cpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/win/iocp.hpp` & `pyxcp-0.21.1/pyxcp/cxx/win/iocp.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/win/periodata.hpp` & `pyxcp-0.21.1/pyxcp/cxx/win/periodata.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/win/socket.hpp` & `pyxcp-0.21.1/pyxcp/cxx/win/socket.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/cxx/win/timeout.hpp` & `pyxcp-0.21.1/pyxcp/cxx/win/timeout.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/dllif.py` & `pyxcp-0.21.1/pyxcp/dllif.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,15 @@
 import binascii
 import ctypes
 import enum
 import platform
 import re
 import subprocess
 import sys
-
-
-CMD_GET_KEY = 0x20
-CMD_QUIT = 0x30
+from pathlib import Path
 
 
 class SeedNKeyResult(enum.IntEnum):
     ACK = 0  # o.k.
     ERR_PRIVILEGE_NOT_AVAILABLE = 1  # the requested privilege can not be unlocked with this DLL
     ERR_INVALID_SEED_LENGTH = 2  # the seed length is wrong, key could not be computed
     ERR_UNSUFFICIENT_KEY_LENGTH = 3  # the space for the key is too small
@@ -23,33 +20,40 @@
     ERR_COULD_NOT_LOAD_FUNC = 17
 
 
 class SeedNKeyError(Exception):
     """"""
 
 
-LOADER = "asamkeydll"
+LOADER = Path(sys.modules["pyxcp"].__file__).parent / "asamkeydll"  # Absolute path to DLL loader.
 
 bwidth, _ = platform.architecture()
 
 if sys.platform in ("win32", "linux"):
     if bwidth == "64bit":
         use_ctypes = False
     elif bwidth == "32bit":
         use_ctypes = True
 else:
     raise RuntimeError("Platform '{}' currently not supported.".format(sys.platform))
 
 
-def getKey(dllName: str, privilege: int, seed: str, assume_same_bit_width: bool):
+def getKey(logger, dllName: str, privilege: int, seed: str, assume_same_bit_width: bool):
+
+    dllName = str(Path(dllName).absolute())  # Fix loader issues.
+
     use_ctypes = False
     if assume_same_bit_width:
         use_ctypes = True
     if use_ctypes:
-        lib = ctypes.cdll.LoadLibrary(dllName)
+        try:
+            lib = ctypes.cdll.LoadLibrary(dllName)
+        except OSError:
+            logger.error(f"Could not load DLL '{dllName}' -- Probably an 64bit vs 32bit issue?")
+            return (SeedNKeyResult.ERR_COULD_NOT_LOAD_DLL, None)
         func = lib.XCP_ComputeKeyFromSeed
         func.restype = ctypes.c_uint32
         func.argtypes = [
             ctypes.c_uint8,
             ctypes.c_uint8,
             ctypes.c_char_p,
             ctypes.POINTER(ctypes.c_uint8),
@@ -68,19 +72,21 @@
     else:
         try:
             p0 = subprocess.Popen(
                 [LOADER, dllName, str(privilege), binascii.hexlify(seed).decode("ascii")],
                 stdout=subprocess.PIPE,
                 shell=False,
             )
+        except FileNotFoundError as exc:
+            logger.error(f"Could not find executable '{LOADER}' -- {exc}")
+            return (SeedNKeyResult.ERR_COULD_NOT_LOAD_DLL, None)
         except OSError as exc:
-            print(f"Cannot execute {LOADER}: {exc}")
+            logger.error(f"Cannot execute {LOADER} -- {exc}")
             return (SeedNKeyResult.ERR_COULD_NOT_LOAD_DLL, None)
         key = p0.stdout.read()
         if not key:
+            logger.error(f"Something went wrong while calling seed-and-key-DLL '{dllName}'")
             return (SeedNKeyResult.ERR_COULD_NOT_LOAD_DLL, None)
         res = re.split(b"\r?\n", key)
         returnCode = int(res[0])
-        if len(res) < 2:
-            return (returnCode, None)
         key = binascii.unhexlify(res[1])
     return (returnCode, key)
```

### Comparing `pyxcp-0.20.4/pyxcp/errormatrix.py` & `pyxcp-0.21.1/pyxcp/errormatrix.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/examples/xcp_read_benchmark.py` & `pyxcp-0.21.1/pyxcp/examples/xcp_read_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/examples/xcp_skel.py` & `pyxcp-0.21.1/pyxcp/examples/xcp_skel.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/examples/xcp_unlock.py` & `pyxcp-0.21.1/pyxcp/examples/xcp_unlock.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/examples/xcp_user_supplied_driver.py` & `pyxcp-0.21.1/pyxcp/examples/xcp_user_supplied_driver.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/examples/xcphello.py` & `pyxcp-0.21.1/pyxcp/scripts/xcp_info.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/logger.py` & `pyxcp-0.21.1/pyxcp/logger.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/master/errorhandler.py` & `pyxcp-0.21.1/pyxcp/master/errorhandler.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/master/master.py` & `pyxcp-0.21.1/pyxcp/master/master.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,16 @@
 from pyxcp.constants import makeWordPacker
 from pyxcp.constants import makeWordUnpacker
 from pyxcp.constants import PackerType
 from pyxcp.constants import UnpackerType
 from pyxcp.master.errorhandler import disable_error_handling
 from pyxcp.master.errorhandler import wrapped
 from pyxcp.transport.base import createTransport
-from pyxcp.utils import delay, SHORT_SLEEP
+from pyxcp.utils import delay
+from pyxcp.utils import SHORT_SLEEP
 
 
 def broadcasted(func: Callable):
     """"""
     return func
 
 
@@ -81,23 +82,23 @@
             False,
         ),  # Bypass error-handling for performance reasons.
         "SEED_N_KEY_DLL": (str, False, ""),
         "SEED_N_KEY_DLL_SAME_BIT_WIDTH": (bool, False, False),
         "DISCONNECT_RESPONSE_OPTIONAL": (bool, False, False),
     }
 
-    def __init__(self, transportName, config=None):
+    def __init__(self, transportName, config=None, policy=None):
         self.ctr = 0
         self.succeeded = True
         self.config = Configuration(self.PARAMETER_MAP or {}, config or {})
         self.logger = logging.getLogger("pyXCP")
         self.logger.setLevel(self.config.get("LOGLEVEL"))
         disable_error_handling(self.config.get("DISABLE_ERROR_HANDLING"))
 
-        self.transport = createTransport(transportName, config)
+        self.transport = createTransport(transportName, config, policy)
         self.transport_name = transportName
 
         # In some cases the transport-layer needs to communicate with us.
         self.transport.parent = self
         self.service = None
 
         # (D)Word (un-)packers are byte-order dependent
@@ -152,14 +153,15 @@
         ----
         Internal Function, only to be used by transport-layer.
         """
         self.service = service
 
     def close(self):
         """Closes transport layer connection."""
+        self.transport.policy.finalize()
         self.transport.close()
 
     # Mandatory Commands.
     @wrapped
     def connect(self, mode=0x00):
         """Build up connection to an XCP slave.
 
@@ -1764,14 +1766,15 @@
             if length > MAX_PAYLOAD:
                 remaining = length - len(seed)
                 while remaining > 0:
                     result = self.getSeed(types.XcpGetSeedMode.REMAINING, resource_value)
                     seed.extend(list(result.seed))
                     remaining = result.length
             result, key = getKey(
+                self.logger,
                 self.seedNKeyDLL,
                 resource_value,
                 bytes(seed),
                 self.seedNKeyDLL_same_bit_width,
             )
             if result == SeedNKeyResult.ACK:
                 key = list(key)
```

### Comparing `pyxcp-0.20.4/pyxcp/recorder/__init__.py` & `pyxcp-0.21.1/pyxcp/recorder/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # -*- coding: utf-8 -*-
 """XCP Frame Recording Facility.
 """
 from dataclasses import dataclass
 from enum import IntEnum
 from typing import Union
 
+from pyxcp.types import FrameCategory
+
 try:
     import pandas as pd
 except ImportError:
     HAS_PANDAS = False
 else:
     HAS_PANDAS = True
 
@@ -23,27 +25,14 @@
     num_containers: int
     record_count: int
     size_uncompressed: int
     size_compressed: int
     compression_ratio: float
 
 
-class FrameCategory(IntEnum):
-    """ """
-
-    META = 0
-    CMD = 1
-    RES = 2
-    ERR = 3
-    EV = 4
-    SERV = 5
-    DAQ = 6
-    STIM = 7
-
-
 COUNTER_MAX = 0xFFFF
 
 
 class XcpLogFileReader:
     """ """
 
     def __init__(self, file_name):
@@ -54,33 +43,39 @@
 
     def __iter__(self):
         while True:
             frames = self._reader.next_block()
             if frames is None:
                 break
             for category, counter, timestamp, _, payload in frames:
-                yield (category, counter, timestamp, payload)
+                yield (FrameCategory(category), counter, timestamp, payload)
 
     def reset_iter(self):
         self._reader.reset()
 
     def as_dataframe(self):
         if HAS_PANDAS:
             df = pd.DataFrame((f for f in self), columns=["category", "counter", "timestamp", "payload"])
             df = df.set_index("timestamp")
+            df.counter = df.counter.astype("uint16")
             df.category = df.category.map({v: k for k, v in FrameCategory.__members__.items()}).astype("category")
             return df
         else:
             raise NotImplementedError("method as_dataframe() requires 'pandas' package")
 
 
 class XcpLogFileWriter:
     """ """
 
     def __init__(self, file_name: str, prealloc=10, chunk_size=1):
         self._writer = rec._PyXcpLogFileWriter(file_name, prealloc, chunk_size)
+        self._finalized = False
+
+    def __del__(self):
+        if not self._finalized:
+            self.finalize()
 
     def add_frame(self, category: FrameCategory, counter: int, timestamp: float, payload: Union[bytes, bytearray]):
         self._writer.add_frame(category, counter % (COUNTER_MAX + 1), timestamp, len(payload), payload)
 
     def finalize(self):
         self._writer.finalize()
```

### Comparing `pyxcp-0.20.4/pyxcp/recorder/lz4.cpp` & `pyxcp-0.21.1/pyxcp/recorder/lz4.c`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 */
 
 /*-************************************
 *  Tuning parameters
 **************************************/
 /*
  * LZ4_HEAPMODE :
- * Select how default compression functions will allocate memory for their hash table,
+ * Select how stateless compression functions like `LZ4_compress_default()`
+ * allocate memory for their hash table,
  * in memory stack (0:default, fastest), or in memory heap (1:requires malloc()).
  */
 #ifndef LZ4_HEAPMODE
 #  define LZ4_HEAPMODE 0
 #endif
 
 /*
@@ -120,14 +121,15 @@
 
 /*-************************************
 *  Compiler Options
 **************************************/
 #if defined(_MSC_VER) && (_MSC_VER >= 1400)  /* Visual Studio 2005+ */
 #  include <intrin.h>               /* only present in VS2005+ */
 #  pragma warning(disable : 4127)   /* disable: C4127: conditional expression is constant */
+#  pragma warning(disable : 6237)   /* disable: C6237: conditional expression is always 0 */
 #endif  /* _MSC_VER */
 
 #ifndef LZ4_FORCE_INLINE
 #  ifdef _MSC_VER    /* Visual Studio */
 #    define LZ4_FORCE_INLINE static __forceinline
 #  else
 #    if defined (__cplusplus) || defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L   /* C99 */
@@ -183,15 +185,35 @@
 # define LZ4_ALIGN_TEST 1
 #endif
 
 
 /*-************************************
 *  Memory routines
 **************************************/
-#ifdef LZ4_USER_MEMORY_FUNCTIONS
+
+/*! LZ4_STATIC_LINKING_ONLY_DISABLE_MEMORY_ALLOCATION :
+ *  Disable relatively high-level LZ4/HC functions that use dynamic memory
+ *  allocation functions (malloc(), calloc(), free()).
+ *
+ *  Note that this is a compile-time switch. And since it disables
+ *  public/stable LZ4 v1 API functions, we don't recommend using this
+ *  symbol to generate a library for distribution.
+ *
+ *  The following public functions are removed when this symbol is defined.
+ *  - lz4   : LZ4_createStream, LZ4_freeStream,
+ *            LZ4_createStreamDecode, LZ4_freeStreamDecode, LZ4_create (deprecated)
+ *  - lz4hc : LZ4_createStreamHC, LZ4_freeStreamHC,
+ *            LZ4_createHC (deprecated), LZ4_freeHC  (deprecated)
+ *  - lz4frame, lz4file : All LZ4F_* functions
+ */
+#if defined(LZ4_STATIC_LINKING_ONLY_DISABLE_MEMORY_ALLOCATION)
+#  define ALLOC(s)          lz4_error_memory_allocation_is_disabled
+#  define ALLOC_AND_ZERO(s) lz4_error_memory_allocation_is_disabled
+#  define FREEMEM(p)        lz4_error_memory_allocation_is_disabled
+#elif defined(LZ4_USER_MEMORY_FUNCTIONS)
 /* memory management functions can be customized by user project.
  * Below functions must exist somewhere in the Project
  * and be available at link time */
 void* LZ4_malloc(size_t s);
 void* LZ4_calloc(size_t n, size_t s);
 void  LZ4_free(void* p);
 # define ALLOC(s)          LZ4_malloc(s)
@@ -200,16 +222,21 @@
 #else
 # include <stdlib.h>   /* malloc, calloc, free */
 # define ALLOC(s)          malloc(s)
 # define ALLOC_AND_ZERO(s) calloc(1,s)
 # define FREEMEM(p)        free(p)
 #endif
 
-#include <string.h>   /* memset, memcpy */
-#define MEM_INIT(p,v,s)   memset((p),(v),(s))
+#if ! LZ4_FREESTANDING
+#  include <string.h>   /* memset, memcpy */
+#endif
+#if !defined(LZ4_memset)
+#  define LZ4_memset(p,v,s) memset((p),(v),(s))
+#endif
+#define MEM_INIT(p,v,s)   LZ4_memset((p),(v),(s))
 
 
 /*-************************************
 *  Common Constants
 **************************************/
 #define MINMATCH 4
 
@@ -249,15 +276,15 @@
 #define LZ4_STATIC_ASSERT(c)   { enum { LZ4_static_assert = 1/(int)(!!(c)) }; }   /* use after variable declarations */
 
 #if defined(LZ4_DEBUG) && (LZ4_DEBUG>=2)
 #  include <stdio.h>
    static int g_debuglog_enable = 1;
 #  define DEBUGLOG(l, ...) {                          \
         if ((g_debuglog_enable) && (l<=LZ4_DEBUG)) {  \
-            fprintf(stderr, __FILE__ ": ");           \
+            fprintf(stderr, __FILE__  " %i: ", __LINE__); \
             fprintf(stderr, __VA_ARGS__);             \
             fprintf(stderr, " \n");                   \
     }   }
 #else
 #  define DEBUGLOG(l, ...) {}    /* disabled */
 #endif
 
@@ -312,18 +339,28 @@
  * LZ4 relies on memcpy with a constant size being inlined. In freestanding
  * environments, the compiler can't assume the implementation of memcpy() is
  * standard compliant, so it can't apply its specialized memcpy() inlining
  * logic. When possible, use __builtin_memcpy() to tell the compiler to analyze
  * memcpy() as if it were standard compliant, so it can inline it in freestanding
  * environments. This is needed when decompressing the Linux Kernel, for example.
  */
-#if defined(__GNUC__) && (__GNUC__ >= 4)
-#define LZ4_memcpy(dst, src, size) __builtin_memcpy(dst, src, size)
-#else
-#define LZ4_memcpy(dst, src, size) memcpy(dst, src, size)
+#if !defined(LZ4_memcpy)
+#  if defined(__GNUC__) && (__GNUC__ >= 4)
+#    define LZ4_memcpy(dst, src, size) __builtin_memcpy(dst, src, size)
+#  else
+#    define LZ4_memcpy(dst, src, size) memcpy(dst, src, size)
+#  endif
+#endif
+
+#if !defined(LZ4_memmove)
+#  if defined(__GNUC__) && (__GNUC__ >= 4)
+#    define LZ4_memmove __builtin_memmove
+#  else
+#    define LZ4_memmove memmove
+#  endif
 #endif
 
 static unsigned LZ4_isLittleEndian(void)
 {
     const union { U32 u; BYTE c[4]; } one = { 1 };   /* don't use static : performance detrimental */
     return one.c[0];
 }
@@ -339,22 +376,24 @@
 static void LZ4_write16(void* memPtr, U16 value) { *(U16*)memPtr = value; }
 static void LZ4_write32(void* memPtr, U32 value) { *(U32*)memPtr = value; }
 
 #elif defined(LZ4_FORCE_MEMORY_ACCESS) && (LZ4_FORCE_MEMORY_ACCESS==1)
 
 /* __pack instructions are safer, but compiler specific, hence potentially problematic for some compilers */
 /* currently only defined for gcc and icc */
-typedef union { U16 u16; U32 u32; reg_t uArch; } __attribute__((packed)) unalign;
-
-static U16 LZ4_read16(const void* ptr) { return ((const unalign*)ptr)->u16; }
-static U32 LZ4_read32(const void* ptr) { return ((const unalign*)ptr)->u32; }
-static reg_t LZ4_read_ARCH(const void* ptr) { return ((const unalign*)ptr)->uArch; }
+typedef struct { U16 u16; } __attribute__((packed)) LZ4_unalign16;
+typedef struct { U32 u32; } __attribute__((packed)) LZ4_unalign32;
+typedef struct { reg_t uArch; } __attribute__((packed)) LZ4_unalignST;
+
+static U16 LZ4_read16(const void* ptr) { return ((const LZ4_unalign16*)ptr)->u16; }
+static U32 LZ4_read32(const void* ptr) { return ((const LZ4_unalign32*)ptr)->u32; }
+static reg_t LZ4_read_ARCH(const void* ptr) { return ((const LZ4_unalignST*)ptr)->uArch; }
 
-static void LZ4_write16(void* memPtr, U16 value) { ((unalign*)memPtr)->u16 = value; }
-static void LZ4_write32(void* memPtr, U32 value) { ((unalign*)memPtr)->u32 = value; }
+static void LZ4_write16(void* memPtr, U16 value) { ((LZ4_unalign16*)memPtr)->u16 = value; }
+static void LZ4_write32(void* memPtr, U32 value) { ((LZ4_unalign32*)memPtr)->u32 = value; }
 
 #else  /* safe and portable access using memcpy() */
 
 static U16 LZ4_read16(const void* memPtr)
 {
     U16 val; LZ4_memcpy(&val, memPtr, sizeof(val)); return val;
 }
@@ -417,18 +456,20 @@
 static const unsigned inc32table[8] = {0, 1, 2,  1,  0,  4, 4, 4};
 static const int      dec64table[8] = {0, 0, 0, -1, -4,  1, 2, 3};
 
 
 #ifndef LZ4_FAST_DEC_LOOP
 #  if defined __i386__ || defined _M_IX86 || defined __x86_64__ || defined _M_X64
 #    define LZ4_FAST_DEC_LOOP 1
+#  elif defined(__aarch64__) && defined(__APPLE__)
+#    define LZ4_FAST_DEC_LOOP 1
 #  elif defined(__aarch64__) && !defined(__clang__)
-     /* On aarch64, we disable this optimization for clang because on certain
-      * mobile chipsets, performance is reduced with clang. For information
-      * refer to https://github.com/lz4/lz4/pull/707 */
+     /* On non-Apple aarch64, we disable this optimization for clang because
+      * on certain mobile chipsets, performance is reduced with clang. For
+      * more information refer to https://github.com/lz4/lz4/pull/707 */
 #    define LZ4_FAST_DEC_LOOP 1
 #  else
 #    define LZ4_FAST_DEC_LOOP 0
 #  endif
 #endif
 
 #if LZ4_FAST_DEC_LOOP
@@ -482,15 +523,22 @@
     switch(offset) {
     case 1:
         MEM_INIT(v, *srcPtr, 8);
         break;
     case 2:
         LZ4_memcpy(v, srcPtr, 2);
         LZ4_memcpy(&v[2], srcPtr, 2);
+#if defined(_MSC_VER) && (_MSC_VER <= 1936) /* MSVC 2022 ver 17.6 or earlier */
+#  pragma warning(push)
+#  pragma warning(disable : 6385) /* warning C6385: Reading invalid data from 'v'. */
+#endif
         LZ4_memcpy(&v[4], v, 4);
+#if defined(_MSC_VER) && (_MSC_VER <= 1936) /* MSVC 2022 ver 17.6 or earlier */
+#  pragma warning(pop)
+#endif
         break;
     case 4:
         LZ4_memcpy(v, srcPtr, 4);
         LZ4_memcpy(&v[4], srcPtr, 4);
         break;
     default:
         LZ4_memcpy_using_offset_base(dstPtr, srcPtr, dstEnd, offset);
@@ -511,17 +559,28 @@
 *  Common functions
 **************************************/
 static unsigned LZ4_NbCommonBytes (reg_t val)
 {
     assert(val != 0);
     if (LZ4_isLittleEndian()) {
         if (sizeof(val) == 8) {
-#       if defined(_MSC_VER) && (_MSC_VER >= 1800) && defined(_M_AMD64) && !defined(LZ4_FORCE_SW_BITCOUNT)
+#       if defined(_MSC_VER) && (_MSC_VER >= 1800) && (defined(_M_AMD64) && !defined(_M_ARM64EC)) && !defined(LZ4_FORCE_SW_BITCOUNT)
+/*-*************************************************************************************************
+* ARM64EC is a Microsoft-designed ARM64 ABI compatible with AMD64 applications on ARM64 Windows 11.
+* The ARM64EC ABI does not support AVX/AVX2/AVX512 instructions, nor their relevant intrinsics
+* including _tzcnt_u64. Therefore, we need to neuter the _tzcnt_u64 code path for ARM64EC.
+****************************************************************************************************/
+#         if defined(__clang__) && (__clang_major__ < 10)
+            /* Avoid undefined clang-cl intrinsics issue.
+             * See https://github.com/lz4/lz4/pull/1017 for details. */
+            return (unsigned)__builtin_ia32_tzcnt_u64(val) >> 3;
+#         else
             /* x64 CPUS without BMI support interpret `TZCNT` as `REP BSF` */
             return (unsigned)_tzcnt_u64(val) >> 3;
+#         endif
 #       elif defined(_MSC_VER) && defined(_WIN64) && !defined(LZ4_FORCE_SW_BITCOUNT)
             unsigned long r = 0;
             _BitScanForward64(&r, (U64)val);
             return (unsigned)r >> 3;
 #       elif (defined(__clang__) || (defined(__GNUC__) && ((__GNUC__ > 3) || \
                             ((__GNUC__ == 3) && (__GNUC_MINOR__ >= 4))))) && \
                                         !defined(LZ4_FORCE_SW_BITCOUNT)
@@ -648,18 +707,18 @@
  *                   blob being compressed are valid and refer to the preceding
  *                   content (of length ctx->dictSize), which is available
  *                   contiguously preceding in memory the content currently
  *                   being compressed.
  * - usingExtDict  : Like withPrefix64k, but the preceding content is somewhere
  *                   else in memory, starting at ctx->dictionary with length
  *                   ctx->dictSize.
- * - usingDictCtx  : Like usingExtDict, but everything concerning the preceding
- *                   content is in a separate context, pointed to by
- *                   ctx->dictCtx. ctx->dictionary, ctx->dictSize, and table
- *                   entries in the current context that refer to positions
+ * - usingDictCtx  : Everything concerning the preceding content is
+ *                   in a separate context, pointed to by ctx->dictCtx.
+ *                   ctx->dictionary, ctx->dictSize, and table entries
+ *                   in the current context that refer to positions
  *                   preceding the beginning of the current compression are
  *                   ignored. Instead, ctx->dictCtx->dictionary and ctx->dictCtx
  *                   ->dictSize describe the location and size of the preceding
  *                   content, and matches are found by looking in the ctx
  *                   ->dictCtx->hashTable.
  */
 typedef enum { noDict = 0, withPrefix64k, usingExtDict, usingDictCtx } dict_directive;
@@ -668,30 +727,32 @@
 
 /*-************************************
 *  Local Utils
 **************************************/
 int LZ4_versionNumber (void) { return LZ4_VERSION_NUMBER; }
 const char* LZ4_versionString(void) { return LZ4_VERSION_STRING; }
 int LZ4_compressBound(int isize)  { return LZ4_COMPRESSBOUND(isize); }
-int LZ4_sizeofState(void) { return LZ4_STREAMSIZE; }
+int LZ4_sizeofState(void) { return sizeof(LZ4_stream_t); }
 
 
-/*-************************************
-*  Internal Definitions used in Tests
-**************************************/
+/*-****************************************
+*  Internal Definitions, used only in Tests
+*******************************************/
 #if defined (__cplusplus)
 extern "C" {
 #endif
 
 int LZ4_compress_forceExtDict (LZ4_stream_t* LZ4_dict, const char* source, char* dest, int srcSize);
 
 int LZ4_decompress_safe_forceExtDict(const char* source, char* dest,
                                      int compressedSize, int maxOutputSize,
                                      const void* dictStart, size_t dictSize);
-
+int LZ4_decompress_safe_partial_forceExtDict(const char* source, char* dest,
+                                     int compressedSize, int targetOutputSize, int dstCapacity,
+                                     const void* dictStart, size_t dictSize);
 #if defined (__cplusplus)
 }
 #endif
 
 /*-******************************
 *  Compression functions
 ********************************/
@@ -741,31 +802,27 @@
     case clearedTable: /* fallthrough */
     case byPtr: { /* illegal! */ assert(0); return; }
     case byU32: { U32* hashTable = (U32*) tableBase; hashTable[h] = idx; return; }
     case byU16: { U16* hashTable = (U16*) tableBase; assert(idx < 65536); hashTable[h] = (U16)idx; return; }
     }
 }
 
+/* LZ4_putPosition*() : only used in byPtr mode */
 LZ4_FORCE_INLINE void LZ4_putPositionOnHash(const BYTE* p, U32 h,
-                                  void* tableBase, tableType_t const tableType,
-                            const BYTE* srcBase)
+                                  void* tableBase, tableType_t const tableType)
 {
-    switch (tableType)
-    {
-    case clearedTable: { /* illegal! */ assert(0); return; }
-    case byPtr: { const BYTE** hashTable = (const BYTE**)tableBase; hashTable[h] = p; return; }
-    case byU32: { U32* hashTable = (U32*) tableBase; hashTable[h] = (U32)(p-srcBase); return; }
-    case byU16: { U16* hashTable = (U16*) tableBase; hashTable[h] = (U16)(p-srcBase); return; }
-    }
+    const BYTE** const hashTable = (const BYTE**)tableBase;
+    assert(tableType == byPtr); (void)tableType;
+    hashTable[h] = p;
 }
 
-LZ4_FORCE_INLINE void LZ4_putPosition(const BYTE* p, void* tableBase, tableType_t tableType, const BYTE* srcBase)
+LZ4_FORCE_INLINE void LZ4_putPosition(const BYTE* p, void* tableBase, tableType_t tableType)
 {
     U32 const h = LZ4_hashPosition(p, tableType);
-    LZ4_putPositionOnHash(p, h, tableBase, tableType, srcBase);
+    LZ4_putPositionOnHash(p, h, tableBase, tableType);
 }
 
 /* LZ4_getIndexOnHash() :
  * Index of match position registered in hash table.
  * hash position must be calculated by using base+index, or dictBase+index.
  * Assumption 1 : only valid if tableType == byU32 or byU16.
  * Assumption 2 : h is presumed valid (within limits of hash table)
@@ -782,28 +839,26 @@
         const U16* const hashTable = (const U16*) tableBase;
         assert(h < (1U << (LZ4_MEMORY_USAGE-1)));
         return hashTable[h];
     }
     assert(0); return 0;  /* forbidden case */
 }
 
-static const BYTE* LZ4_getPositionOnHash(U32 h, const void* tableBase, tableType_t tableType, const BYTE* srcBase)
+static const BYTE* LZ4_getPositionOnHash(U32 h, const void* tableBase, tableType_t tableType)
 {
-    if (tableType == byPtr) { const BYTE* const* hashTable = (const BYTE* const*) tableBase; return hashTable[h]; }
-    if (tableType == byU32) { const U32* const hashTable = (const U32*) tableBase; return hashTable[h] + srcBase; }
-    { const U16* const hashTable = (const U16*) tableBase; return hashTable[h] + srcBase; }   /* default, to ensure a return */
+    assert(tableType == byPtr); (void)tableType;
+    { const BYTE* const* hashTable = (const BYTE* const*) tableBase; return hashTable[h]; }
 }
 
 LZ4_FORCE_INLINE const BYTE*
 LZ4_getPosition(const BYTE* p,
-                const void* tableBase, tableType_t tableType,
-                const BYTE* srcBase)
+                const void* tableBase, tableType_t tableType)
 {
     U32 const h = LZ4_hashPosition(p, tableType);
-    return LZ4_getPositionOnHash(h, tableBase, tableType, srcBase);
+    return LZ4_getPositionOnHash(h, tableBase, tableType);
 }
 
 LZ4_FORCE_INLINE void
 LZ4_prepareTable(LZ4_stream_t_internal* const cctx,
            const int inputSize,
            const tableType_t tableType) {
     /* If the table hasn't been used, it's guaranteed to be zeroed out, and is
@@ -823,89 +878,92 @@
             cctx->currentOffset = 0;
             cctx->tableType = (U32)clearedTable;
         } else {
             DEBUGLOG(4, "LZ4_prepareTable: Re-use hash table (no reset)");
         }
     }
 
-    /* Adding a gap, so all previous entries are > LZ4_DISTANCE_MAX back, is faster
-     * than compressing without a gap. However, compressing with
-     * currentOffset == 0 is faster still, so we preserve that case.
+    /* Adding a gap, so all previous entries are > LZ4_DISTANCE_MAX back,
+     * is faster than compressing without a gap.
+     * However, compressing with currentOffset == 0 is faster still,
+     * so we preserve that case.
      */
     if (cctx->currentOffset != 0 && tableType == byU32) {
         DEBUGLOG(5, "LZ4_prepareTable: adding 64KB to currentOffset");
         cctx->currentOffset += 64 KB;
     }
 
     /* Finally, clear history */
     cctx->dictCtx = NULL;
     cctx->dictionary = NULL;
     cctx->dictSize = 0;
 }
 
 /** LZ4_compress_generic() :
  *  inlined, to ensure branches are decided at compilation time.
- *  Presumed already validated at this stage:
+ *  The following conditions are presumed already validated:
  *  - source != NULL
  *  - inputSize > 0
  */
 LZ4_FORCE_INLINE int LZ4_compress_generic_validated(
                  LZ4_stream_t_internal* const cctx,
                  const char* const source,
                  char* const dest,
                  const int inputSize,
-                 int *inputConsumed, /* only written when outputDirective == fillOutput */
+                 int*  inputConsumed, /* only written when outputDirective == fillOutput */
                  const int maxOutputSize,
                  const limitedOutput_directive outputDirective,
                  const tableType_t tableType,
                  const dict_directive dictDirective,
                  const dictIssue_directive dictIssue,
                  const int acceleration)
 {
     int result;
-    const BYTE* ip = (const BYTE*) source;
+    const BYTE* ip = (const BYTE*)source;
 
     U32 const startIndex = cctx->currentOffset;
-    const BYTE* base = (const BYTE*) source - startIndex;
+    const BYTE* base = (const BYTE*)source - startIndex;
     const BYTE* lowLimit;
 
     const LZ4_stream_t_internal* dictCtx = (const LZ4_stream_t_internal*) cctx->dictCtx;
     const BYTE* const dictionary =
         dictDirective == usingDictCtx ? dictCtx->dictionary : cctx->dictionary;
     const U32 dictSize =
         dictDirective == usingDictCtx ? dictCtx->dictSize : cctx->dictSize;
-    const U32 dictDelta = (dictDirective == usingDictCtx) ? startIndex - dictCtx->currentOffset : 0;   /* make indexes in dictCtx comparable with index in current context */
+    const U32 dictDelta =
+        (dictDirective == usingDictCtx) ? startIndex - dictCtx->currentOffset : 0;   /* make indexes in dictCtx comparable with indexes in current context */
 
     int const maybe_extMem = (dictDirective == usingExtDict) || (dictDirective == usingDictCtx);
     U32 const prefixIdxLimit = startIndex - dictSize;   /* used when dictDirective == dictSmall */
     const BYTE* const dictEnd = dictionary ? dictionary + dictSize : dictionary;
     const BYTE* anchor = (const BYTE*) source;
     const BYTE* const iend = ip + inputSize;
     const BYTE* const mflimitPlusOne = iend - MFLIMIT + 1;
     const BYTE* const matchlimit = iend - LASTLITERALS;
 
     /* the dictCtx currentOffset is indexed on the start of the dictionary,
      * while a dictionary in the current context precedes the currentOffset */
-    const BYTE* dictBase = !dictionary ? NULL : (dictDirective == usingDictCtx) ?
+    const BYTE* dictBase = (dictionary == NULL) ? NULL :
+                           (dictDirective == usingDictCtx) ?
                             dictionary + dictSize - dictCtx->currentOffset :
                             dictionary + dictSize - startIndex;
 
     BYTE* op = (BYTE*) dest;
     BYTE* const olimit = op + maxOutputSize;
 
     U32 offset = 0;
     U32 forwardH;
 
     DEBUGLOG(5, "LZ4_compress_generic_validated: srcSize=%i, tableType=%u", inputSize, tableType);
     assert(ip != NULL);
+    if (tableType == byU16) assert(inputSize<LZ4_64Klimit);  /* Size too large (not within 64K limit) */
+    if (tableType == byPtr) assert(dictDirective==noDict);   /* only supported use case with byPtr */
     /* If init conditions are not met, we don't have to mark stream
      * as having dirty context, since no action was taken yet */
     if (outputDirective == fillOutput && maxOutputSize < 1) { return 0; } /* Impossible to store anything */
-    if ((tableType == byU16) && (inputSize>=LZ4_64Klimit)) { return 0; }  /* Size too large (not within 64K limit) */
-    if (tableType==byPtr) assert(dictDirective==noDict);      /* only supported use case with byPtr */
     assert(acceleration >= 1);
 
     lowLimit = (const BYTE*)source - (dictDirective == withPrefix64k ? dictSize : 0);
 
     /* Update context state */
     if (dictDirective == usingDictCtx) {
         /* Subsequent linked blocks can't use the dictionary. */
@@ -917,15 +975,20 @@
     }
     cctx->currentOffset += (U32)inputSize;
     cctx->tableType = (U32)tableType;
 
     if (inputSize<LZ4_minLength) goto _last_literals;        /* Input too small, no compression (all literals) */
 
     /* First Byte */
-    LZ4_putPosition(ip, cctx->hashTable, tableType, base);
+    {   U32 const h = LZ4_hashPosition(ip, tableType);
+        if (tableType == byPtr) {
+            LZ4_putPositionOnHash(ip, h, cctx->hashTable, byPtr);
+        } else {
+            LZ4_putIndexOnHash(startIndex, h, cctx->hashTable, tableType);
+    }   }
     ip++; forwardH = LZ4_hashPosition(ip, tableType);
 
     /* Main Loop */
     for ( ; ; ) {
         const BYTE* match;
         BYTE* token;
         const BYTE* filledIp;
@@ -940,17 +1003,17 @@
                 ip = forwardIp;
                 forwardIp += step;
                 step = (searchMatchNb++ >> LZ4_skipTrigger);
 
                 if (unlikely(forwardIp > mflimitPlusOne)) goto _last_literals;
                 assert(ip < mflimitPlusOne);
 
-                match = LZ4_getPositionOnHash(h, cctx->hashTable, tableType, base);
+                match = LZ4_getPositionOnHash(h, cctx->hashTable, tableType);
                 forwardH = LZ4_hashPosition(forwardIp, tableType);
-                LZ4_putPositionOnHash(ip, h, cctx->hashTable, tableType, base);
+                LZ4_putPositionOnHash(ip, h, cctx->hashTable, tableType);
 
             } while ( (match+LZ4_DISTANCE_MAX < ip)
                    || (LZ4_read32(match) != LZ4_read32(ip)) );
 
         } else {   /* byU32, byU16 */
 
             const BYTE* forwardIp = ip;
@@ -977,18 +1040,19 @@
                         match = dictBase + matchIndex;
                         matchIndex += dictDelta;   /* make dictCtx index comparable with current context */
                         lowLimit = dictionary;
                     } else {
                         match = base + matchIndex;
                         lowLimit = (const BYTE*)source;
                     }
-                } else if (dictDirective==usingExtDict) {
+                } else if (dictDirective == usingExtDict) {
                     if (matchIndex < startIndex) {
                         DEBUGLOG(7, "extDict candidate: matchIndex=%5u  <  startIndex=%5u", matchIndex, startIndex);
                         assert(startIndex - matchIndex >= MINMATCH);
+                        assert(dictBase);
                         match = dictBase + matchIndex;
                         lowLimit = dictionary;
                     } else {
                         match = base + matchIndex;
                         lowLimit = (const BYTE*)source;
                     }
                 } else {   /* single continuous memory segment */
@@ -1139,44 +1203,52 @@
 
         anchor = ip;
 
         /* Test end of chunk */
         if (ip >= mflimitPlusOne) break;
 
         /* Fill table */
-        LZ4_putPosition(ip-2, cctx->hashTable, tableType, base);
+        {   U32 const h = LZ4_hashPosition(ip-2, tableType);
+            if (tableType == byPtr) {
+                LZ4_putPositionOnHash(ip-2, h, cctx->hashTable, byPtr);
+            } else {
+                U32 const idx = (U32)((ip-2) - base);
+                LZ4_putIndexOnHash(idx, h, cctx->hashTable, tableType);
+        }   }
 
         /* Test next position */
         if (tableType == byPtr) {
 
-            match = LZ4_getPosition(ip, cctx->hashTable, tableType, base);
-            LZ4_putPosition(ip, cctx->hashTable, tableType, base);
+            match = LZ4_getPosition(ip, cctx->hashTable, tableType);
+            LZ4_putPosition(ip, cctx->hashTable, tableType);
             if ( (match+LZ4_DISTANCE_MAX >= ip)
               && (LZ4_read32(match) == LZ4_read32(ip)) )
             { token=op++; *token=0; goto _next_match; }
 
         } else {   /* byU32, byU16 */
 
             U32 const h = LZ4_hashPosition(ip, tableType);
             U32 const current = (U32)(ip-base);
             U32 matchIndex = LZ4_getIndexOnHash(h, cctx->hashTable, tableType);
             assert(matchIndex < current);
             if (dictDirective == usingDictCtx) {
                 if (matchIndex < startIndex) {
                     /* there was no match, try the dictionary */
+                    assert(tableType == byU32);
                     matchIndex = LZ4_getIndexOnHash(h, dictCtx->hashTable, byU32);
                     match = dictBase + matchIndex;
                     lowLimit = dictionary;   /* required for match length counter */
                     matchIndex += dictDelta;
                 } else {
                     match = base + matchIndex;
                     lowLimit = (const BYTE*)source;  /* required for match length counter */
                 }
             } else if (dictDirective==usingExtDict) {
                 if (matchIndex < startIndex) {
+                    assert(dictBase);
                     match = dictBase + matchIndex;
                     lowLimit = dictionary;   /* required for match length counter */
                 } else {
                     match = base + matchIndex;
                     lowLimit = (const BYTE*)source;   /* required for match length counter */
                 }
             } else {   /* single memory segment */
@@ -1311,17 +1383,18 @@
  * Using this variant avoids an expensive initialization step. It is only safe
  * to call if the state buffer is known to be correctly initialized already
  * (see comment in lz4.h on LZ4_resetStream_fast() for a definition of
  * "correctly initialized").
  */
 int LZ4_compress_fast_extState_fastReset(void* state, const char* src, char* dst, int srcSize, int dstCapacity, int acceleration)
 {
-    LZ4_stream_t_internal* ctx = &((LZ4_stream_t*)state)->internal_donotuse;
+    LZ4_stream_t_internal* const ctx = &((LZ4_stream_t*)state)->internal_donotuse;
     if (acceleration < 1) acceleration = LZ4_ACCELERATION_DEFAULT;
     if (acceleration > LZ4_ACCELERATION_MAX) acceleration = LZ4_ACCELERATION_MAX;
+    assert(ctx != NULL);
 
     if (dstCapacity >= LZ4_compressBound(srcSize)) {
         if (srcSize < LZ4_64Klimit) {
             const tableType_t tableType = byU16;
             LZ4_prepareTable(ctx, srcSize, tableType);
             if (ctx->currentOffset) {
                 return LZ4_compress_generic(ctx, src, dst, srcSize, NULL, 0, notLimited, tableType, noDict, dictSmall, acceleration);
@@ -1347,36 +1420,36 @@
             LZ4_prepareTable(ctx, srcSize, tableType);
             return LZ4_compress_generic(ctx, src, dst, srcSize, NULL, dstCapacity, limitedOutput, tableType, noDict, noDictIssue, acceleration);
         }
     }
 }
 
 
-int LZ4_compress_fast(const char* source, char* dest, int inputSize, int maxOutputSize, int acceleration)
+int LZ4_compress_fast(const char* src, char* dest, int srcSize, int dstCapacity, int acceleration)
 {
     int result;
 #if (LZ4_HEAPMODE)
-    LZ4_stream_t* ctxPtr = ALLOC(sizeof(LZ4_stream_t));   /* malloc-calloc always properly aligned */
+    LZ4_stream_t* const ctxPtr = (LZ4_stream_t*)ALLOC(sizeof(LZ4_stream_t));   /* malloc-calloc always properly aligned */
     if (ctxPtr == NULL) return 0;
 #else
     LZ4_stream_t ctx;
     LZ4_stream_t* const ctxPtr = &ctx;
 #endif
-    result = LZ4_compress_fast_extState(ctxPtr, source, dest, inputSize, maxOutputSize, acceleration);
+    result = LZ4_compress_fast_extState(ctxPtr, src, dest, srcSize, dstCapacity, acceleration);
 
 #if (LZ4_HEAPMODE)
     FREEMEM(ctxPtr);
 #endif
     return result;
 }
 
 
-int LZ4_compress_default(const char* src, char* dst, int srcSize, int maxOutputSize)
+int LZ4_compress_default(const char* src, char* dst, int srcSize, int dstCapacity)
 {
-    return LZ4_compress_fast(src, dst, srcSize, maxOutputSize, 1);
+    return LZ4_compress_fast(src, dst, srcSize, dstCapacity, 1);
 }
 
 
 /* Note!: This function leaves the stream in an unclean/broken state!
  * It is not safe to subsequently use the same state with a _fastReset() or
  * _continue() call without resetting it. */
 static int LZ4_compress_destSize_extState (LZ4_stream_t* state, const char* src, char* dst, int* srcSizePtr, int targetDstSize)
@@ -1395,19 +1468,19 @@
     }   }
 }
 
 
 int LZ4_compress_destSize(const char* src, char* dst, int* srcSizePtr, int targetDstSize)
 {
 #if (LZ4_HEAPMODE)
-    LZ4_stream_t* ctx = (LZ4_stream_t*)ALLOC(sizeof(LZ4_stream_t));   /* malloc-calloc always properly aligned */
+    LZ4_stream_t* const ctx = (LZ4_stream_t*)ALLOC(sizeof(LZ4_stream_t));   /* malloc-calloc always properly aligned */
     if (ctx == NULL) return 0;
 #else
     LZ4_stream_t ctxBody;
-    LZ4_stream_t* ctx = &ctxBody;
+    LZ4_stream_t* const ctx = &ctxBody;
 #endif
 
     int result = LZ4_compress_destSize_extState(ctx, src, dst, srcSizePtr, targetDstSize);
 
 #if (LZ4_HEAPMODE)
     FREEMEM(ctx);
 #endif
@@ -1416,23 +1489,25 @@
 
 
 
 /*-******************************
 *  Streaming functions
 ********************************/
 
+#if !defined(LZ4_STATIC_LINKING_ONLY_DISABLE_MEMORY_ALLOCATION)
 LZ4_stream_t* LZ4_createStream(void)
 {
     LZ4_stream_t* const lz4s = (LZ4_stream_t*)ALLOC(sizeof(LZ4_stream_t));
-    LZ4_STATIC_ASSERT(LZ4_STREAMSIZE >= sizeof(LZ4_stream_t_internal));    /* A compilation error here means LZ4_STREAMSIZE is not large enough */
+    LZ4_STATIC_ASSERT(sizeof(LZ4_stream_t) >= sizeof(LZ4_stream_t_internal));
     DEBUGLOG(4, "LZ4_createStream %p", lz4s);
     if (lz4s == NULL) return NULL;
     LZ4_initStream(lz4s, sizeof(*lz4s));
     return lz4s;
 }
+#endif
 
 static size_t LZ4_stream_t_alignment(void)
 {
 #if LZ4_ALIGN_TEST
     typedef struct { char c; LZ4_stream_t t; } t_a;
     return sizeof(t_a) - sizeof(LZ4_stream_t);
 #else
@@ -1458,31 +1533,33 @@
     MEM_INIT(LZ4_stream, 0, sizeof(LZ4_stream_t_internal));
 }
 
 void LZ4_resetStream_fast(LZ4_stream_t* ctx) {
     LZ4_prepareTable(&(ctx->internal_donotuse), 0, byU32);
 }
 
+#if !defined(LZ4_STATIC_LINKING_ONLY_DISABLE_MEMORY_ALLOCATION)
 int LZ4_freeStream (LZ4_stream_t* LZ4_stream)
 {
     if (!LZ4_stream) return 0;   /* support free on NULL */
     DEBUGLOG(5, "LZ4_freeStream %p", LZ4_stream);
     FREEMEM(LZ4_stream);
     return (0);
 }
+#endif
 
 
 #define HASH_UNIT sizeof(reg_t)
 int LZ4_loadDict (LZ4_stream_t* LZ4_dict, const char* dictionary, int dictSize)
 {
-    LZ4_stream_t_internal* dict = &LZ4_dict->internal_donotuse;
+    LZ4_stream_t_internal* const dict = &LZ4_dict->internal_donotuse;
     const tableType_t tableType = byU32;
     const BYTE* p = (const BYTE*)dictionary;
     const BYTE* const dictEnd = p + dictSize;
-    const BYTE* base;
+    U32 idx32;
 
     DEBUGLOG(4, "LZ4_loadDict (%i bytes from %p into %p)", dictSize, dictionary, LZ4_dict);
 
     /* It's necessary to reset the context,
      * and not just continue it with prepareTable()
      * to avoid any risk of generating overflowing matchIndex
      * when compressing using this dictionary */
@@ -1497,29 +1574,31 @@
     dict->currentOffset += 64 KB;
 
     if (dictSize < (int)HASH_UNIT) {
         return 0;
     }
 
     if ((dictEnd - p) > 64 KB) p = dictEnd - 64 KB;
-    base = dictEnd - dict->currentOffset;
     dict->dictionary = p;
     dict->dictSize = (U32)(dictEnd - p);
     dict->tableType = (U32)tableType;
+    idx32 = dict->currentOffset - dict->dictSize;
 
     while (p <= dictEnd-HASH_UNIT) {
-        LZ4_putPosition(p, dict->hashTable, tableType, base);
-        p+=3;
+        U32 const h = LZ4_hashPosition(p, tableType);
+        LZ4_putIndexOnHash(idx32, h, dict->hashTable, tableType);
+        p+=3; idx32+=3;
     }
 
     return (int)dict->dictSize;
 }
 
-void LZ4_attach_dictionary(LZ4_stream_t* workingStream, const LZ4_stream_t* dictionaryStream) {
-    const LZ4_stream_t_internal* dictCtx = dictionaryStream == NULL ? NULL :
+void LZ4_attach_dictionary(LZ4_stream_t* workingStream, const LZ4_stream_t* dictionaryStream)
+{
+    const LZ4_stream_t_internal* dictCtx = (dictionaryStream == NULL) ? NULL :
         &(dictionaryStream->internal_donotuse);
 
     DEBUGLOG(4, "LZ4_attach_dictionary (%p, %p, size %u)",
              workingStream, dictionaryStream,
              dictCtx != NULL ? dictCtx->dictSize : 0);
 
     if (dictCtx != NULL) {
@@ -1564,44 +1643,48 @@
 
 int LZ4_compress_fast_continue (LZ4_stream_t* LZ4_stream,
                                 const char* source, char* dest,
                                 int inputSize, int maxOutputSize,
                                 int acceleration)
 {
     const tableType_t tableType = byU32;
-    LZ4_stream_t_internal* streamPtr = &LZ4_stream->internal_donotuse;
-    const BYTE* dictEnd = streamPtr->dictionary + streamPtr->dictSize;
+    LZ4_stream_t_internal* const streamPtr = &LZ4_stream->internal_donotuse;
+    const char* dictEnd = streamPtr->dictSize ? (const char*)streamPtr->dictionary + streamPtr->dictSize : NULL;
 
-    DEBUGLOG(5, "LZ4_compress_fast_continue (inputSize=%i)", inputSize);
+    DEBUGLOG(5, "LZ4_compress_fast_continue (inputSize=%i, dictSize=%u)", inputSize, streamPtr->dictSize);
 
-    LZ4_renormDictT(streamPtr, inputSize);   /* avoid index overflow */
+    LZ4_renormDictT(streamPtr, inputSize);   /* fix index overflow */
     if (acceleration < 1) acceleration = LZ4_ACCELERATION_DEFAULT;
     if (acceleration > LZ4_ACCELERATION_MAX) acceleration = LZ4_ACCELERATION_MAX;
 
     /* invalidate tiny dictionaries */
-    if ( (streamPtr->dictSize-1 < 4-1)   /* intentional underflow */
-      && (dictEnd != (const BYTE*)source) ) {
+    if ( (streamPtr->dictSize < 4)     /* tiny dictionary : not enough for a hash */
+      && (dictEnd != source)           /* prefix mode */
+      && (inputSize > 0)               /* tolerance : don't lose history, in case next invocation would use prefix mode */
+      && (streamPtr->dictCtx == NULL)  /* usingDictCtx */
+      ) {
         DEBUGLOG(5, "LZ4_compress_fast_continue: dictSize(%u) at addr:%p is too small", streamPtr->dictSize, streamPtr->dictionary);
+        /* remove dictionary existence from history, to employ faster prefix mode */
         streamPtr->dictSize = 0;
         streamPtr->dictionary = (const BYTE*)source;
-        dictEnd = (const BYTE*)source;
+        dictEnd = source;
     }
 
     /* Check overlapping input/dictionary space */
-    {   const BYTE* sourceEnd = (const BYTE*) source + inputSize;
-        if ((sourceEnd > streamPtr->dictionary) && (sourceEnd < dictEnd)) {
+    {   const char* const sourceEnd = source + inputSize;
+        if ((sourceEnd > (const char*)streamPtr->dictionary) && (sourceEnd < dictEnd)) {
             streamPtr->dictSize = (U32)(dictEnd - sourceEnd);
             if (streamPtr->dictSize > 64 KB) streamPtr->dictSize = 64 KB;
             if (streamPtr->dictSize < 4) streamPtr->dictSize = 0;
-            streamPtr->dictionary = dictEnd - streamPtr->dictSize;
+            streamPtr->dictionary = (const BYTE*)dictEnd - streamPtr->dictSize;
         }
     }
 
     /* prefix mode : source data follows dictionary */
-    if (dictEnd == (const BYTE*)source) {
+    if (dictEnd == source) {
         if ((streamPtr->dictSize < 64 KB) && (streamPtr->dictSize < streamPtr->currentOffset))
             return LZ4_compress_generic(streamPtr, source, dest, inputSize, NULL, maxOutputSize, limitedOutput, tableType, withPrefix64k, dictSmall, acceleration);
         else
             return LZ4_compress_generic(streamPtr, source, dest, inputSize, NULL, maxOutputSize, limitedOutput, tableType, withPrefix64k, noDictIssue, acceleration);
     }
 
     /* external dictionary mode */
@@ -1619,15 +1702,15 @@
                  * so that the compression loop is only looking into one table.
                  */
                 LZ4_memcpy(streamPtr, streamPtr->dictCtx, sizeof(*streamPtr));
                 result = LZ4_compress_generic(streamPtr, source, dest, inputSize, NULL, maxOutputSize, limitedOutput, tableType, usingExtDict, noDictIssue, acceleration);
             } else {
                 result = LZ4_compress_generic(streamPtr, source, dest, inputSize, NULL, maxOutputSize, limitedOutput, tableType, usingDictCtx, noDictIssue, acceleration);
             }
-        } else {
+        } else {  /* small data <= 4 KB */
             if ((streamPtr->dictSize < 64 KB) && (streamPtr->dictSize < streamPtr->currentOffset)) {
                 result = LZ4_compress_generic(streamPtr, source, dest, inputSize, NULL, maxOutputSize, limitedOutput, tableType, usingExtDict, dictSmall, acceleration);
             } else {
                 result = LZ4_compress_generic(streamPtr, source, dest, inputSize, NULL, maxOutputSize, limitedOutput, tableType, usingExtDict, noDictIssue, acceleration);
             }
         }
         streamPtr->dictionary = (const BYTE*)source;
@@ -1636,15 +1719,15 @@
     }
 }
 
 
 /* Hidden debug function, to force-test external dictionary mode */
 int LZ4_compress_forceExtDict (LZ4_stream_t* LZ4_dict, const char* source, char* dest, int srcSize)
 {
-    LZ4_stream_t_internal* streamPtr = &LZ4_dict->internal_donotuse;
+    LZ4_stream_t_internal* const streamPtr = &LZ4_dict->internal_donotuse;
     int result;
 
     LZ4_renormDictT(streamPtr, srcSize);
 
     if ((streamPtr->dictSize < 64 KB) && (streamPtr->dictSize < streamPtr->currentOffset)) {
         result = LZ4_compress_generic(streamPtr, source, dest, srcSize, NULL, 0, notLimited, byU32, usingExtDict, dictSmall, 1);
     } else {
@@ -1657,75 +1740,203 @@
     return result;
 }
 
 
 /*! LZ4_saveDict() :
  *  If previously compressed data block is not guaranteed to remain available at its memory location,
  *  save it into a safer place (char* safeBuffer).
- *  Note : you don't need to call LZ4_loadDict() afterwards,
- *         dictionary is immediately usable, you can therefore call LZ4_compress_fast_continue().
- *  Return : saved dictionary size in bytes (necessarily <= dictSize), or 0 if error.
+ *  Note : no need to call LZ4_loadDict() afterwards, dictionary is immediately usable,
+ *         one can therefore call LZ4_compress_fast_continue() right after.
+ * @return : saved dictionary size in bytes (necessarily <= dictSize), or 0 if error.
  */
 int LZ4_saveDict (LZ4_stream_t* LZ4_dict, char* safeBuffer, int dictSize)
 {
     LZ4_stream_t_internal* const dict = &LZ4_dict->internal_donotuse;
-    const BYTE* const previousDictEnd = dict->dictionary + dict->dictSize;
+
+    DEBUGLOG(5, "LZ4_saveDict : dictSize=%i, safeBuffer=%p", dictSize, safeBuffer);
 
     if ((U32)dictSize > 64 KB) { dictSize = 64 KB; } /* useless to define a dictionary > 64 KB */
     if ((U32)dictSize > dict->dictSize) { dictSize = (int)dict->dictSize; }
 
     if (safeBuffer == NULL) assert(dictSize == 0);
-    if (dictSize > 0)
-        memmove(safeBuffer, previousDictEnd - dictSize, dictSize);
+    if (dictSize > 0) {
+        const BYTE* const previousDictEnd = dict->dictionary + dict->dictSize;
+        assert(dict->dictionary);
+        LZ4_memmove(safeBuffer, previousDictEnd - dictSize, (size_t)dictSize);
+    }
 
     dict->dictionary = (const BYTE*)safeBuffer;
     dict->dictSize = (U32)dictSize;
 
     return dictSize;
 }
 
 
 
 /*-*******************************
  *  Decompression functions
  ********************************/
 
-typedef enum { endOnOutputSize = 0, endOnInputSize = 1 } endCondition_directive;
 typedef enum { decode_full_block = 0, partial_decode = 1 } earlyEnd_directive;
 
 #undef MIN
 #define MIN(a,b)    ( (a) < (b) ? (a) : (b) )
 
+
+/* variant for decompress_unsafe()
+ * does not know end of input
+ * presumes input is well formed
+ * note : will consume at least one byte */
+static size_t read_long_length_no_check(const BYTE** pp)
+{
+    size_t b, l = 0;
+    do { b = **pp; (*pp)++; l += b; } while (b==255);
+    DEBUGLOG(6, "read_long_length_no_check: +length=%zu using %zu input bytes", l, l/255 + 1)
+    return l;
+}
+
+/* core decoder variant for LZ4_decompress_fast*()
+ * for legacy support only : these entry points are deprecated.
+ * - Presumes input is correctly formed (no defense vs malformed inputs)
+ * - Does not know input size (presume input buffer is "large enough")
+ * - Decompress a full block (only)
+ * @return : nb of bytes read from input.
+ * Note : this variant is not optimized for speed, just for maintenance.
+ *        the goal is to remove support of decompress_fast*() variants by v2.0
+**/
+LZ4_FORCE_INLINE int
+LZ4_decompress_unsafe_generic(
+                 const BYTE* const istart,
+                 BYTE* const ostart,
+                 int decompressedSize,
+
+                 size_t prefixSize,
+                 const BYTE* const dictStart,  /* only if dict==usingExtDict */
+                 const size_t dictSize         /* note: =0 if dictStart==NULL */
+                 )
+{
+    const BYTE* ip = istart;
+    BYTE* op = (BYTE*)ostart;
+    BYTE* const oend = ostart + decompressedSize;
+    const BYTE* const prefixStart = ostart - prefixSize;
+
+    DEBUGLOG(5, "LZ4_decompress_unsafe_generic");
+    if (dictStart == NULL) assert(dictSize == 0);
+
+    while (1) {
+        /* start new sequence */
+        unsigned token = *ip++;
+
+        /* literals */
+        {   size_t ll = token >> ML_BITS;
+            if (ll==15) {
+                /* long literal length */
+                ll += read_long_length_no_check(&ip);
+            }
+            if ((size_t)(oend-op) < ll) return -1; /* output buffer overflow */
+            LZ4_memmove(op, ip, ll); /* support in-place decompression */
+            op += ll;
+            ip += ll;
+            if ((size_t)(oend-op) < MFLIMIT) {
+                if (op==oend) break;  /* end of block */
+                DEBUGLOG(5, "invalid: literals end at distance %zi from end of block", oend-op);
+                /* incorrect end of block :
+                 * last match must start at least MFLIMIT==12 bytes before end of output block */
+                return -1;
+        }   }
+
+        /* match */
+        {   size_t ml = token & 15;
+            size_t const offset = LZ4_readLE16(ip);
+            ip+=2;
+
+            if (ml==15) {
+                /* long literal length */
+                ml += read_long_length_no_check(&ip);
+            }
+            ml += MINMATCH;
+
+            if ((size_t)(oend-op) < ml) return -1; /* output buffer overflow */
+
+            {   const BYTE* match = op - offset;
+
+                /* out of range */
+                if (offset > (size_t)(op - prefixStart) + dictSize) {
+                    DEBUGLOG(6, "offset out of range");
+                    return -1;
+                }
+
+                /* check special case : extDict */
+                if (offset > (size_t)(op - prefixStart)) {
+                    /* extDict scenario */
+                    const BYTE* const dictEnd = dictStart + dictSize;
+                    const BYTE* extMatch = dictEnd - (offset - (size_t)(op-prefixStart));
+                    size_t const extml = (size_t)(dictEnd - extMatch);
+                    if (extml > ml) {
+                        /* match entirely within extDict */
+                        LZ4_memmove(op, extMatch, ml);
+                        op += ml;
+                        ml = 0;
+                    } else {
+                        /* match split between extDict & prefix */
+                        LZ4_memmove(op, extMatch, extml);
+                        op += extml;
+                        ml -= extml;
+                    }
+                    match = prefixStart;
+                }
+
+                /* match copy - slow variant, supporting overlap copy */
+                {   size_t u;
+                    for (u=0; u<ml; u++) {
+                        op[u] = match[u];
+            }   }   }
+            op += ml;
+            if ((size_t)(oend-op) < LASTLITERALS) {
+                DEBUGLOG(5, "invalid: match ends at distance %zi from end of block", oend-op);
+                /* incorrect end of block :
+                 * last match must stop at least LASTLITERALS==5 bytes before end of output block */
+                return -1;
+            }
+        } /* match */
+    } /* main loop */
+    return (int)(ip - istart);
+}
+
+
 /* Read the variable-length literal or match length.
  *
- * ip - pointer to use as input.
- * lencheck - end ip.  Return an error if ip advances >= lencheck.
- * loop_check - check ip >= lencheck in body of loop.  Returns loop_error if so.
- * initial_check - check ip >= lencheck before start of loop.  Returns initial_error if so.
- * error (output) - error code.  Should be set to 0 before call.
- */
-typedef enum { loop_error = -2, initial_error = -1, ok = 0 } variable_length_error;
-LZ4_FORCE_INLINE unsigned
-read_variable_length(const BYTE**ip, const BYTE* lencheck,
-                     int loop_check, int initial_check,
-                     variable_length_error* error)
-{
-    U32 length = 0;
-    U32 s;
-    if (initial_check && unlikely((*ip) >= lencheck)) {    /* overflow detection */
-        *error = initial_error;
-        return length;
+ * @ip : input pointer
+ * @ilimit : position after which if length is not decoded, the input is necessarily corrupted.
+ * @initial_check - check ip >= ipmax before start of loop.  Returns initial_error if so.
+ * @error (output) - error code.  Must be set to 0 before call.
+**/
+typedef size_t Rvl_t;
+static const Rvl_t rvl_error = (Rvl_t)(-1);
+LZ4_FORCE_INLINE Rvl_t
+read_variable_length(const BYTE** ip, const BYTE* ilimit,
+                     int initial_check)
+{
+    Rvl_t s, length = 0;
+    assert(ip != NULL);
+    assert(*ip !=  NULL);
+    assert(ilimit != NULL);
+    if (initial_check && unlikely((*ip) >= ilimit)) {    /* read limit reached */
+        return rvl_error;
     }
     do {
         s = **ip;
         (*ip)++;
         length += s;
-        if (loop_check && unlikely((*ip) >= lencheck)) {    /* overflow detection */
-            *error = loop_error;
-            return length;
+        if (unlikely((*ip) > ilimit)) {    /* read limit reached */
+            return rvl_error;
+        }
+        /* accumulator overflow detection (32-bit mode only) */
+        if ((sizeof(length)<8) && unlikely(length > ((Rvl_t)(-1)/2)) ) {
+            return rvl_error;
         }
     } while (s==255);
 
     return length;
 }
 
 /*! LZ4_decompress_generic() :
@@ -1737,15 +1948,14 @@
 LZ4_FORCE_INLINE int
 LZ4_decompress_generic(
                  const char* const src,
                  char* const dst,
                  int srcSize,
                  int outputSize,         /* If endOnInput==endOnInputSize, this value is `dstCapacity` */
 
-                 endCondition_directive endOnInput,   /* endOnOutputSize, endOnInputSize */
                  earlyEnd_directive partialDecoding,  /* full, partial */
                  dict_directive dict,                 /* noDict, withPrefix64k, usingExtDict */
                  const BYTE* const lowPrefix,  /* always <= dst, == dst when no prefix */
                  const BYTE* const dictStart,  /* only if dict==usingExtDict */
                  const size_t dictSize         /* note : = 0 if noDict */
                  )
 {
@@ -1756,146 +1966,148 @@
 
         BYTE* op = (BYTE*) dst;
         BYTE* const oend = op + outputSize;
         BYTE* cpy;
 
         const BYTE* const dictEnd = (dictStart == NULL) ? NULL : dictStart + dictSize;
 
-        const int safeDecode = (endOnInput==endOnInputSize);
-        const int checkOffset = ((safeDecode) && (dictSize < (int)(64 KB)));
+        const int checkOffset = (dictSize < (int)(64 KB));
 
 
         /* Set up the "end" pointers for the shortcut. */
-        const BYTE* const shortiend = iend - (endOnInput ? 14 : 8) /*maxLL*/ - 2 /*offset*/;
-        const BYTE* const shortoend = oend - (endOnInput ? 14 : 8) /*maxLL*/ - 18 /*maxML*/;
+        const BYTE* const shortiend = iend - 14 /*maxLL*/ - 2 /*offset*/;
+        const BYTE* const shortoend = oend - 14 /*maxLL*/ - 18 /*maxML*/;
 
         const BYTE* match;
         size_t offset;
         unsigned token;
         size_t length;
 
 
         DEBUGLOG(5, "LZ4_decompress_generic (srcSize:%i, dstSize:%i)", srcSize, outputSize);
 
         /* Special cases */
         assert(lowPrefix <= op);
-        if ((endOnInput) && (unlikely(outputSize==0))) {
+        if (unlikely(outputSize==0)) {
             /* Empty output buffer */
             if (partialDecoding) return 0;
             return ((srcSize==1) && (*ip==0)) ? 0 : -1;
         }
-        if ((!endOnInput) && (unlikely(outputSize==0))) { return (*ip==0 ? 1 : -1); }
-        if ((endOnInput) && unlikely(srcSize==0)) { return -1; }
+        if (unlikely(srcSize==0)) { return -1; }
 
-	/* Currently the fast loop shows a regression on qualcomm arm chips. */
+    /* LZ4_FAST_DEC_LOOP:
+     * designed for modern OoO performance cpus,
+     * where copying reliably 32-bytes is preferable to an unpredictable branch.
+     * note : fast loop may show a regression for some client arm chips. */
 #if LZ4_FAST_DEC_LOOP
         if ((oend - op) < FASTLOOP_SAFE_DISTANCE) {
             DEBUGLOG(6, "skip fast decode loop");
             goto safe_decode;
         }
 
-        /* Fast loop : decode sequences as long as output < iend-FASTLOOP_SAFE_DISTANCE */
+        /* Fast loop : decode sequences as long as output < oend-FASTLOOP_SAFE_DISTANCE */
+        DEBUGLOG(6, "using fast decode loop");
         while (1) {
             /* Main fastloop assertion: We can always wildcopy FASTLOOP_SAFE_DISTANCE */
             assert(oend - op >= FASTLOOP_SAFE_DISTANCE);
-            if (endOnInput) { assert(ip < iend); }
+            assert(ip < iend);
             token = *ip++;
             length = token >> ML_BITS;  /* literal length */
 
-            assert(!endOnInput || ip <= iend); /* ip < iend before the increment */
-
             /* decode literal length */
             if (length == RUN_MASK) {
-                variable_length_error error = ok;
-                length += read_variable_length(&ip, iend-RUN_MASK, (int)endOnInput, (int)endOnInput, &error);
-                if (error == initial_error) { goto _output_error; }
-                if ((safeDecode) && unlikely((uptrval)(op)+length<(uptrval)(op))) { goto _output_error; } /* overflow detection */
-                if ((safeDecode) && unlikely((uptrval)(ip)+length<(uptrval)(ip))) { goto _output_error; } /* overflow detection */
+                size_t const addl = read_variable_length(&ip, iend-RUN_MASK, 1);
+                if (addl == rvl_error) {
+                    DEBUGLOG(6, "error reading long literal length");
+                    goto _output_error;
+                }
+                length += addl;
+                if (unlikely((uptrval)(op)+length<(uptrval)(op))) { goto _output_error; } /* overflow detection */
+                if (unlikely((uptrval)(ip)+length<(uptrval)(ip))) { goto _output_error; } /* overflow detection */
 
                 /* copy literals */
                 cpy = op+length;
                 LZ4_STATIC_ASSERT(MFLIMIT >= WILDCOPYLENGTH);
-                if (endOnInput) {  /* LZ4_decompress_safe() */
-                    if ((cpy>oend-32) || (ip+length>iend-32)) { goto safe_literal_copy; }
-                    LZ4_wildCopy32(op, ip, cpy);
-                } else {   /* LZ4_decompress_fast() */
-                    if (cpy>oend-8) { goto safe_literal_copy; }
-                    LZ4_wildCopy8(op, ip, cpy); /* LZ4_decompress_fast() cannot copy more than 8 bytes at a time :
-                                                 * it doesn't know input length, and only relies on end-of-block properties */
-                }
+                if ((cpy>oend-32) || (ip+length>iend-32)) { goto safe_literal_copy; }
+                LZ4_wildCopy32(op, ip, cpy);
                 ip += length; op = cpy;
             } else {
                 cpy = op+length;
-                if (endOnInput) {  /* LZ4_decompress_safe() */
-                    DEBUGLOG(7, "copy %u bytes in a 16-bytes stripe", (unsigned)length);
-                    /* We don't need to check oend, since we check it once for each loop below */
-                    if (ip > iend-(16 + 1/*max lit + offset + nextToken*/)) { goto safe_literal_copy; }
-                    /* Literals can only be 14, but hope compilers optimize if we copy by a register size */
-                    LZ4_memcpy(op, ip, 16);
-                } else {  /* LZ4_decompress_fast() */
-                    /* LZ4_decompress_fast() cannot copy more than 8 bytes at a time :
-                     * it doesn't know input length, and relies on end-of-block properties */
-                    LZ4_memcpy(op, ip, 8);
-                    if (length > 8) { LZ4_memcpy(op+8, ip+8, 8); }
-                }
+                DEBUGLOG(7, "copy %u bytes in a 16-bytes stripe", (unsigned)length);
+                /* We don't need to check oend, since we check it once for each loop below */
+                if (ip > iend-(16 + 1/*max lit + offset + nextToken*/)) { goto safe_literal_copy; }
+                /* Literals can only be <= 14, but hope compilers optimize better when copy by a register size */
+                LZ4_memcpy(op, ip, 16);
                 ip += length; op = cpy;
             }
 
             /* get offset */
             offset = LZ4_readLE16(ip); ip+=2;
+            DEBUGLOG(6, " offset = %zu", offset);
             match = op - offset;
-            assert(match <= op);
+            assert(match <= op);  /* overflow check */
 
             /* get matchlength */
             length = token & ML_MASK;
 
             if (length == ML_MASK) {
-                variable_length_error error = ok;
-                if ((checkOffset) && (unlikely(match + dictSize < lowPrefix))) { goto _output_error; } /* Error : offset outside buffers */
-                length += read_variable_length(&ip, iend - LASTLITERALS + 1, (int)endOnInput, 0, &error);
-                if (error != ok) { goto _output_error; }
-                if ((safeDecode) && unlikely((uptrval)(op)+length<(uptrval)op)) { goto _output_error; } /* overflow detection */
+                size_t const addl = read_variable_length(&ip, iend - LASTLITERALS + 1, 0);
+                if (addl == rvl_error) {
+                    DEBUGLOG(6, "error reading long match length");
+                    goto _output_error;
+                }
+                length += addl;
                 length += MINMATCH;
+                if (unlikely((uptrval)(op)+length<(uptrval)op)) { goto _output_error; } /* overflow detection */
+                if ((checkOffset) && (unlikely(match + dictSize < lowPrefix))) {
+                    DEBUGLOG(6, "Error : offset outside buffers");
+                    goto _output_error;
+                }
                 if (op + length >= oend - FASTLOOP_SAFE_DISTANCE) {
                     goto safe_match_copy;
                 }
             } else {
                 length += MINMATCH;
                 if (op + length >= oend - FASTLOOP_SAFE_DISTANCE) {
                     goto safe_match_copy;
                 }
 
-                /* Fastpath check: Avoids a branch in LZ4_wildCopy32 if true */
+                /* Fastpath check: skip LZ4_wildCopy32 when true */
                 if ((dict == withPrefix64k) || (match >= lowPrefix)) {
                     if (offset >= 8) {
                         assert(match >= lowPrefix);
                         assert(match <= op);
                         assert(op + 18 <= oend);
 
                         LZ4_memcpy(op, match, 8);
                         LZ4_memcpy(op+8, match+8, 8);
                         LZ4_memcpy(op+16, match+16, 2);
                         op += length;
                         continue;
             }   }   }
 
-            if (checkOffset && (unlikely(match + dictSize < lowPrefix))) { goto _output_error; } /* Error : offset outside buffers */
+            if ( checkOffset && (unlikely(match + dictSize < lowPrefix)) ) {
+                DEBUGLOG(6, "Error : pos=%zi, offset=%zi => outside buffers", op-lowPrefix, op-match);
+                goto _output_error;
+            }
             /* match starting within external dictionary */
             if ((dict==usingExtDict) && (match < lowPrefix)) {
+                assert(dictEnd != NULL);
                 if (unlikely(op+length > oend-LASTLITERALS)) {
                     if (partialDecoding) {
                         DEBUGLOG(7, "partialDecoding: dictionary match, close to dstEnd");
                         length = MIN(length, (size_t)(oend-op));
                     } else {
-                        goto _output_error;  /* end-of-block condition violated */
+                        DEBUGLOG(6, "end-of-block condition violated")
+                        goto _output_error;
                 }   }
 
                 if (length <= (size_t)(lowPrefix-match)) {
                     /* match fits entirely within external dictionary : just copy */
-                    memmove(op, dictEnd - (lowPrefix-match), length);
+                    LZ4_memmove(op, dictEnd - (lowPrefix-match), length);
                     op += length;
                 } else {
                     /* match stretches into both external dictionary and current block */
                     size_t const copySize = (size_t)(lowPrefix - match);
                     size_t const restSize = length - copySize;
                     LZ4_memcpy(op, dictEnd - copySize, copySize);
                     op += copySize;
@@ -1922,34 +2134,34 @@
 
             op = cpy;   /* wildcopy correction */
         }
     safe_decode:
 #endif
 
         /* Main Loop : decode remaining sequences where output < FASTLOOP_SAFE_DISTANCE */
+        DEBUGLOG(6, "using safe decode loop");
         while (1) {
+            assert(ip < iend);
             token = *ip++;
             length = token >> ML_BITS;  /* literal length */
 
-            assert(!endOnInput || ip <= iend); /* ip < iend before the increment */
-
             /* A two-stage shortcut for the most common case:
              * 1) If the literal length is 0..14, and there is enough space,
              * enter the shortcut and copy 16 bytes on behalf of the literals
              * (in the fast mode, only 8 bytes can be safely copied this way).
              * 2) Further if the match length is 4..18, copy 18 bytes in a similar
              * manner; but we ensure that there's enough space in the output for
              * those 18 bytes earlier, upon entering the shortcut (in other words,
              * there is a combined check for both stages).
              */
-            if ( (endOnInput ? length != RUN_MASK : length <= 8)
+            if ( (length != RUN_MASK)
                 /* strictly "less than" on input, to re-enter the loop with at least one byte */
-              && likely((endOnInput ? ip < shortiend : 1) & (op <= shortoend)) ) {
+              && likely((ip < shortiend) & (op <= shortoend)) ) {
                 /* Copy the literals */
-                LZ4_memcpy(op, ip, endOnInput ? 16 : 8);
+                LZ4_memcpy(op, ip, 16);
                 op += length; ip += length;
 
                 /* The second stage: prepare for match copying, decode full info.
                  * If it doesn't work out, the info won't be wasted. */
                 length = token & ML_MASK; /* match length */
                 offset = LZ4_readLE16(ip); ip += 2;
                 match = op - offset;
@@ -1971,40 +2183,37 @@
                 /* The second stage didn't work out, but the info is ready.
                  * Propel it right to the point of match copying. */
                 goto _copy_match;
             }
 
             /* decode literal length */
             if (length == RUN_MASK) {
-                variable_length_error error = ok;
-                length += read_variable_length(&ip, iend-RUN_MASK, (int)endOnInput, (int)endOnInput, &error);
-                if (error == initial_error) { goto _output_error; }
-                if ((safeDecode) && unlikely((uptrval)(op)+length<(uptrval)(op))) { goto _output_error; } /* overflow detection */
-                if ((safeDecode) && unlikely((uptrval)(ip)+length<(uptrval)(ip))) { goto _output_error; } /* overflow detection */
+                size_t const addl = read_variable_length(&ip, iend-RUN_MASK, 1);
+                if (addl == rvl_error) { goto _output_error; }
+                length += addl;
+                if (unlikely((uptrval)(op)+length<(uptrval)(op))) { goto _output_error; } /* overflow detection */
+                if (unlikely((uptrval)(ip)+length<(uptrval)(ip))) { goto _output_error; } /* overflow detection */
             }
 
             /* copy literals */
             cpy = op+length;
 #if LZ4_FAST_DEC_LOOP
         safe_literal_copy:
 #endif
             LZ4_STATIC_ASSERT(MFLIMIT >= WILDCOPYLENGTH);
-            if ( ((endOnInput) && ((cpy>oend-MFLIMIT) || (ip+length>iend-(2+1+LASTLITERALS))) )
-              || ((!endOnInput) && (cpy>oend-WILDCOPYLENGTH)) )
-            {
+            if ((cpy>oend-MFLIMIT) || (ip+length>iend-(2+1+LASTLITERALS))) {
                 /* We've either hit the input parsing restriction or the output parsing restriction.
                  * In the normal scenario, decoding a full block, it must be the last sequence,
                  * otherwise it's an error (invalid input or dimensions).
                  * In partialDecoding scenario, it's necessary to ensure there is no buffer overflow.
                  */
                 if (partialDecoding) {
                     /* Since we are partial decoding we may be in this block because of the output parsing
                      * restriction, which is not valid since the output buffer is allowed to be undersized.
                      */
-                    assert(endOnInput);
                     DEBUGLOG(7, "partialDecoding: copying literals, close to input or output end")
                     DEBUGLOG(7, "partialDecoding: literal length = %u", (unsigned)length);
                     DEBUGLOG(7, "partialDecoding: remaining space in dstBuffer : %i", (int)(oend - op));
                     DEBUGLOG(7, "partialDecoding: remaining space in srcBuffer : %i", (int)(iend - ip));
                     /* Finishing in the middle of a literals segment,
                      * due to lack of input.
                      */
@@ -2017,74 +2226,71 @@
                      */
                     if (cpy > oend) {
                         cpy = oend;
                         assert(op<=oend);
                         length = (size_t)(oend-op);
                     }
                 } else {
-                    /* We must be on the last sequence because of the parsing limitations so check
-                     * that we exactly regenerate the original size (must be exact when !endOnInput).
-                     */
-                    if ((!endOnInput) && (cpy != oend)) { goto _output_error; }
                      /* We must be on the last sequence (or invalid) because of the parsing limitations
                       * so check that we exactly consume the input and don't overrun the output buffer.
                       */
-                    if ((endOnInput) && ((ip+length != iend) || (cpy > oend))) {
+                    if ((ip+length != iend) || (cpy > oend)) {
                         DEBUGLOG(6, "should have been last run of literals")
                         DEBUGLOG(6, "ip(%p) + length(%i) = %p != iend (%p)", ip, (int)length, ip+length, iend);
                         DEBUGLOG(6, "or cpy(%p) > oend(%p)", cpy, oend);
                         goto _output_error;
                     }
                 }
-                memmove(op, ip, length);  /* supports overlapping memory regions; only matters for in-place decompression scenarios */
+                LZ4_memmove(op, ip, length);  /* supports overlapping memory regions, for in-place decompression scenarios */
                 ip += length;
                 op += length;
                 /* Necessarily EOF when !partialDecoding.
                  * When partialDecoding, it is EOF if we've either
                  * filled the output buffer or
                  * can't proceed with reading an offset for following match.
                  */
                 if (!partialDecoding || (cpy == oend) || (ip >= (iend-2))) {
                     break;
                 }
             } else {
-                LZ4_wildCopy8(op, ip, cpy);   /* may overwrite up to WILDCOPYLENGTH beyond cpy */
+                LZ4_wildCopy8(op, ip, cpy);   /* can overwrite up to 8 bytes beyond cpy */
                 ip += length; op = cpy;
             }
 
             /* get offset */
             offset = LZ4_readLE16(ip); ip+=2;
             match = op - offset;
 
             /* get matchlength */
             length = token & ML_MASK;
 
     _copy_match:
             if (length == ML_MASK) {
-              variable_length_error error = ok;
-              length += read_variable_length(&ip, iend - LASTLITERALS + 1, (int)endOnInput, 0, &error);
-              if (error != ok) goto _output_error;
-                if ((safeDecode) && unlikely((uptrval)(op)+length<(uptrval)op)) goto _output_error;   /* overflow detection */
+                size_t const addl = read_variable_length(&ip, iend - LASTLITERALS + 1, 0);
+                if (addl == rvl_error) { goto _output_error; }
+                length += addl;
+                if (unlikely((uptrval)(op)+length<(uptrval)op)) goto _output_error;   /* overflow detection */
             }
             length += MINMATCH;
 
 #if LZ4_FAST_DEC_LOOP
         safe_match_copy:
 #endif
             if ((checkOffset) && (unlikely(match + dictSize < lowPrefix))) goto _output_error;   /* Error : offset outside buffers */
             /* match starting within external dictionary */
             if ((dict==usingExtDict) && (match < lowPrefix)) {
+                assert(dictEnd != NULL);
                 if (unlikely(op+length > oend-LASTLITERALS)) {
                     if (partialDecoding) length = MIN(length, (size_t)(oend-op));
                     else goto _output_error;   /* doesn't respect parsing restriction */
                 }
 
                 if (length <= (size_t)(lowPrefix-match)) {
                     /* match fits entirely within external dictionary : just copy */
-                    memmove(op, dictEnd - (lowPrefix-match), length);
+                    LZ4_memmove(op, dictEnd - (lowPrefix-match), length);
                     op += length;
                 } else {
                     /* match stretches into both external dictionary and current block */
                     size_t const copySize = (size_t)(lowPrefix - match);
                     size_t const restSize = length - copySize;
                     LZ4_memcpy(op, dictEnd - copySize, copySize);
                     op += copySize;
@@ -2147,150 +2353,175 @@
                 LZ4_memcpy(op, match, 8);
                 if (length > 16)  { LZ4_wildCopy8(op+8, match+8, cpy); }
             }
             op = cpy;   /* wildcopy correction */
         }
 
         /* end of decoding */
-        if (endOnInput) {
-            DEBUGLOG(5, "decoded %i bytes", (int) (((char*)op)-dst));
-           return (int) (((char*)op)-dst);     /* Nb of output bytes decoded */
-       } else {
-           return (int) (((const char*)ip)-src);   /* Nb of input bytes read */
-       }
+        DEBUGLOG(5, "decoded %i bytes", (int) (((char*)op)-dst));
+        return (int) (((char*)op)-dst);     /* Nb of output bytes decoded */
 
         /* Overflow error detected */
     _output_error:
         return (int) (-(((const char*)ip)-src))-1;
     }
 }
 
 
 /*===== Instantiate the API decoding functions. =====*/
 
 LZ4_FORCE_O2
 int LZ4_decompress_safe(const char* source, char* dest, int compressedSize, int maxDecompressedSize)
 {
     return LZ4_decompress_generic(source, dest, compressedSize, maxDecompressedSize,
-                                  endOnInputSize, decode_full_block, noDict,
+                                  decode_full_block, noDict,
                                   (BYTE*)dest, NULL, 0);
 }
 
 LZ4_FORCE_O2
 int LZ4_decompress_safe_partial(const char* src, char* dst, int compressedSize, int targetOutputSize, int dstCapacity)
 {
     dstCapacity = MIN(targetOutputSize, dstCapacity);
     return LZ4_decompress_generic(src, dst, compressedSize, dstCapacity,
-                                  endOnInputSize, partial_decode,
+                                  partial_decode,
                                   noDict, (BYTE*)dst, NULL, 0);
 }
 
 LZ4_FORCE_O2
 int LZ4_decompress_fast(const char* source, char* dest, int originalSize)
 {
-    return LZ4_decompress_generic(source, dest, 0, originalSize,
-                                  endOnOutputSize, decode_full_block, withPrefix64k,
-                                  (BYTE*)dest - 64 KB, NULL, 0);
+    DEBUGLOG(5, "LZ4_decompress_fast");
+    return LZ4_decompress_unsafe_generic(
+                (const BYTE*)source, (BYTE*)dest, originalSize,
+                0, NULL, 0);
 }
 
 /*===== Instantiate a few more decoding cases, used more than once. =====*/
 
 LZ4_FORCE_O2 /* Exported, an obsolete API function. */
 int LZ4_decompress_safe_withPrefix64k(const char* source, char* dest, int compressedSize, int maxOutputSize)
 {
     return LZ4_decompress_generic(source, dest, compressedSize, maxOutputSize,
-                                  endOnInputSize, decode_full_block, withPrefix64k,
+                                  decode_full_block, withPrefix64k,
+                                  (BYTE*)dest - 64 KB, NULL, 0);
+}
+
+LZ4_FORCE_O2
+static int LZ4_decompress_safe_partial_withPrefix64k(const char* source, char* dest, int compressedSize, int targetOutputSize, int dstCapacity)
+{
+    dstCapacity = MIN(targetOutputSize, dstCapacity);
+    return LZ4_decompress_generic(source, dest, compressedSize, dstCapacity,
+                                  partial_decode, withPrefix64k,
                                   (BYTE*)dest - 64 KB, NULL, 0);
 }
 
 /* Another obsolete API function, paired with the previous one. */
 int LZ4_decompress_fast_withPrefix64k(const char* source, char* dest, int originalSize)
 {
-    /* LZ4_decompress_fast doesn't validate match offsets,
-     * and thus serves well with any prefixed dictionary. */
-    return LZ4_decompress_fast(source, dest, originalSize);
+    return LZ4_decompress_unsafe_generic(
+                (const BYTE*)source, (BYTE*)dest, originalSize,
+                64 KB, NULL, 0);
 }
 
 LZ4_FORCE_O2
 static int LZ4_decompress_safe_withSmallPrefix(const char* source, char* dest, int compressedSize, int maxOutputSize,
                                                size_t prefixSize)
 {
     return LZ4_decompress_generic(source, dest, compressedSize, maxOutputSize,
-                                  endOnInputSize, decode_full_block, noDict,
+                                  decode_full_block, noDict,
+                                  (BYTE*)dest-prefixSize, NULL, 0);
+}
+
+LZ4_FORCE_O2
+static int LZ4_decompress_safe_partial_withSmallPrefix(const char* source, char* dest, int compressedSize, int targetOutputSize, int dstCapacity,
+                                               size_t prefixSize)
+{
+    dstCapacity = MIN(targetOutputSize, dstCapacity);
+    return LZ4_decompress_generic(source, dest, compressedSize, dstCapacity,
+                                  partial_decode, noDict,
                                   (BYTE*)dest-prefixSize, NULL, 0);
 }
 
 LZ4_FORCE_O2
 int LZ4_decompress_safe_forceExtDict(const char* source, char* dest,
                                      int compressedSize, int maxOutputSize,
                                      const void* dictStart, size_t dictSize)
 {
+    DEBUGLOG(5, "LZ4_decompress_safe_forceExtDict");
     return LZ4_decompress_generic(source, dest, compressedSize, maxOutputSize,
-                                  endOnInputSize, decode_full_block, usingExtDict,
+                                  decode_full_block, usingExtDict,
+                                  (BYTE*)dest, (const BYTE*)dictStart, dictSize);
+}
+
+LZ4_FORCE_O2
+int LZ4_decompress_safe_partial_forceExtDict(const char* source, char* dest,
+                                     int compressedSize, int targetOutputSize, int dstCapacity,
+                                     const void* dictStart, size_t dictSize)
+{
+    dstCapacity = MIN(targetOutputSize, dstCapacity);
+    return LZ4_decompress_generic(source, dest, compressedSize, dstCapacity,
+                                  partial_decode, usingExtDict,
                                   (BYTE*)dest, (const BYTE*)dictStart, dictSize);
 }
 
 LZ4_FORCE_O2
 static int LZ4_decompress_fast_extDict(const char* source, char* dest, int originalSize,
                                        const void* dictStart, size_t dictSize)
 {
-    return LZ4_decompress_generic(source, dest, 0, originalSize,
-                                  endOnOutputSize, decode_full_block, usingExtDict,
-                                  (BYTE*)dest, (const BYTE*)dictStart, dictSize);
+    return LZ4_decompress_unsafe_generic(
+                (const BYTE*)source, (BYTE*)dest, originalSize,
+                0, (const BYTE*)dictStart, dictSize);
 }
 
 /* The "double dictionary" mode, for use with e.g. ring buffers: the first part
  * of the dictionary is passed as prefix, and the second via dictStart + dictSize.
  * These routines are used only once, in LZ4_decompress_*_continue().
  */
 LZ4_FORCE_INLINE
 int LZ4_decompress_safe_doubleDict(const char* source, char* dest, int compressedSize, int maxOutputSize,
                                    size_t prefixSize, const void* dictStart, size_t dictSize)
 {
     return LZ4_decompress_generic(source, dest, compressedSize, maxOutputSize,
-                                  endOnInputSize, decode_full_block, usingExtDict,
-                                  (BYTE*)dest-prefixSize, (const BYTE*)dictStart, dictSize);
-}
-
-LZ4_FORCE_INLINE
-int LZ4_decompress_fast_doubleDict(const char* source, char* dest, int originalSize,
-                                   size_t prefixSize, const void* dictStart, size_t dictSize)
-{
-    return LZ4_decompress_generic(source, dest, 0, originalSize,
-                                  endOnOutputSize, decode_full_block, usingExtDict,
+                                  decode_full_block, usingExtDict,
                                   (BYTE*)dest-prefixSize, (const BYTE*)dictStart, dictSize);
 }
 
 /*===== streaming decompression functions =====*/
 
+#if !defined(LZ4_STATIC_LINKING_ONLY_DISABLE_MEMORY_ALLOCATION)
 LZ4_streamDecode_t* LZ4_createStreamDecode(void)
 {
-    LZ4_streamDecode_t* lz4s = (LZ4_streamDecode_t*) ALLOC_AND_ZERO(sizeof(LZ4_streamDecode_t));
-    LZ4_STATIC_ASSERT(LZ4_STREAMDECODESIZE >= sizeof(LZ4_streamDecode_t_internal));    /* A compilation error here means LZ4_STREAMDECODESIZE is not large enough */
-    return lz4s;
+    LZ4_STATIC_ASSERT(sizeof(LZ4_streamDecode_t) >= sizeof(LZ4_streamDecode_t_internal));
+    return (LZ4_streamDecode_t*) ALLOC_AND_ZERO(sizeof(LZ4_streamDecode_t));
 }
 
 int LZ4_freeStreamDecode (LZ4_streamDecode_t* LZ4_stream)
 {
     if (LZ4_stream == NULL) { return 0; }  /* support free on NULL */
     FREEMEM(LZ4_stream);
     return 0;
 }
+#endif
 
 /*! LZ4_setStreamDecode() :
  *  Use this function to instruct where to find the dictionary.
  *  This function is not necessary if previous data is still available where it was decoded.
  *  Loading a size of 0 is allowed (same effect as no dictionary).
  * @return : 1 if OK, 0 if error
  */
 int LZ4_setStreamDecode (LZ4_streamDecode_t* LZ4_streamDecode, const char* dictionary, int dictSize)
 {
     LZ4_streamDecode_t_internal* lz4sd = &LZ4_streamDecode->internal_donotuse;
-    lz4sd->prefixSize = (size_t) dictSize;
-    lz4sd->prefixEnd = (const BYTE*) dictionary + dictSize;
+    lz4sd->prefixSize = (size_t)dictSize;
+    if (dictSize) {
+        assert(dictionary != NULL);
+        lz4sd->prefixEnd = (const BYTE*) dictionary + dictSize;
+    } else {
+        lz4sd->prefixEnd = (const BYTE*) dictionary;
+    }
     lz4sd->externalDict = NULL;
     lz4sd->extDictSize  = 0;
     return 1;
 }
 
 /*! LZ4_decoderRingBufferSize() :
  *  when setting a ring buffer for streaming decompression (optional scenario),
@@ -2354,37 +2585,43 @@
         lz4sd->prefixSize = (size_t)result;
         lz4sd->prefixEnd  = (BYTE*)dest + result;
     }
 
     return result;
 }
 
-LZ4_FORCE_O2
-int LZ4_decompress_fast_continue (LZ4_streamDecode_t* LZ4_streamDecode, const char* source, char* dest, int originalSize)
+LZ4_FORCE_O2 int
+LZ4_decompress_fast_continue (LZ4_streamDecode_t* LZ4_streamDecode,
+                        const char* source, char* dest, int originalSize)
 {
-    LZ4_streamDecode_t_internal* lz4sd = &LZ4_streamDecode->internal_donotuse;
+    LZ4_streamDecode_t_internal* const lz4sd =
+        (assert(LZ4_streamDecode!=NULL), &LZ4_streamDecode->internal_donotuse);
     int result;
+
+    DEBUGLOG(5, "LZ4_decompress_fast_continue (toDecodeSize=%i)", originalSize);
     assert(originalSize >= 0);
 
     if (lz4sd->prefixSize == 0) {
+        DEBUGLOG(5, "first invocation : no prefix nor extDict");
         assert(lz4sd->extDictSize == 0);
         result = LZ4_decompress_fast(source, dest, originalSize);
         if (result <= 0) return result;
         lz4sd->prefixSize = (size_t)originalSize;
         lz4sd->prefixEnd = (BYTE*)dest + originalSize;
     } else if (lz4sd->prefixEnd == (BYTE*)dest) {
-        if (lz4sd->prefixSize >= 64 KB - 1 || lz4sd->extDictSize == 0)
-            result = LZ4_decompress_fast(source, dest, originalSize);
-        else
-            result = LZ4_decompress_fast_doubleDict(source, dest, originalSize,
-                                                    lz4sd->prefixSize, lz4sd->externalDict, lz4sd->extDictSize);
+        DEBUGLOG(5, "continue using existing prefix");
+        result = LZ4_decompress_unsafe_generic(
+                        (const BYTE*)source, (BYTE*)dest, originalSize,
+                        lz4sd->prefixSize,
+                        lz4sd->externalDict, lz4sd->extDictSize);
         if (result <= 0) return result;
         lz4sd->prefixSize += (size_t)originalSize;
         lz4sd->prefixEnd  += originalSize;
     } else {
+        DEBUGLOG(5, "prefix becomes extDict");
         lz4sd->extDictSize = lz4sd->prefixSize;
         lz4sd->externalDict = lz4sd->prefixEnd - lz4sd->extDictSize;
         result = LZ4_decompress_fast_extDict(source, dest, originalSize,
                                              lz4sd->externalDict, lz4sd->extDictSize);
         if (result <= 0) return result;
         lz4sd->prefixSize = (size_t)originalSize;
         lz4sd->prefixEnd  = (BYTE*)dest + originalSize;
@@ -2412,18 +2649,35 @@
         assert(dictSize >= 0);
         return LZ4_decompress_safe_withSmallPrefix(source, dest, compressedSize, maxOutputSize, (size_t)dictSize);
     }
     assert(dictSize >= 0);
     return LZ4_decompress_safe_forceExtDict(source, dest, compressedSize, maxOutputSize, dictStart, (size_t)dictSize);
 }
 
+int LZ4_decompress_safe_partial_usingDict(const char* source, char* dest, int compressedSize, int targetOutputSize, int dstCapacity, const char* dictStart, int dictSize)
+{
+    if (dictSize==0)
+        return LZ4_decompress_safe_partial(source, dest, compressedSize, targetOutputSize, dstCapacity);
+    if (dictStart+dictSize == dest) {
+        if (dictSize >= 64 KB - 1) {
+            return LZ4_decompress_safe_partial_withPrefix64k(source, dest, compressedSize, targetOutputSize, dstCapacity);
+        }
+        assert(dictSize >= 0);
+        return LZ4_decompress_safe_partial_withSmallPrefix(source, dest, compressedSize, targetOutputSize, dstCapacity, (size_t)dictSize);
+    }
+    assert(dictSize >= 0);
+    return LZ4_decompress_safe_partial_forceExtDict(source, dest, compressedSize, targetOutputSize, dstCapacity, dictStart, (size_t)dictSize);
+}
+
 int LZ4_decompress_fast_usingDict(const char* source, char* dest, int originalSize, const char* dictStart, int dictSize)
 {
     if (dictSize==0 || dictStart+dictSize == dest)
-        return LZ4_decompress_fast(source, dest, originalSize);
+        return LZ4_decompress_unsafe_generic(
+                        (const BYTE*)source, (BYTE*)dest, originalSize,
+                        (size_t)dictSize, NULL, 0);
     assert(dictSize >= 0);
     return LZ4_decompress_fast_extDict(source, dest, originalSize, dictStart, (size_t)dictSize);
 }
 
 
 /*=*************************************************
 *  Obsolete Functions
@@ -2467,28 +2721,30 @@
 int LZ4_uncompress_unknownOutputSize (const char* source, char* dest, int isize, int maxOutputSize)
 {
     return LZ4_decompress_safe(source, dest, isize, maxOutputSize);
 }
 
 /* Obsolete Streaming functions */
 
-int LZ4_sizeofStreamState(void) { return LZ4_STREAMSIZE; }
+int LZ4_sizeofStreamState(void) { return sizeof(LZ4_stream_t); }
 
 int LZ4_resetStreamState(void* state, char* inputBuffer)
 {
     (void)inputBuffer;
     LZ4_resetStream((LZ4_stream_t*)state);
     return 0;
 }
 
+#if !defined(LZ4_STATIC_LINKING_ONLY_DISABLE_MEMORY_ALLOCATION)
 void* LZ4_create (char* inputBuffer)
 {
     (void)inputBuffer;
     return LZ4_createStream();
 }
+#endif
 
 char* LZ4_slideInputBuffer (void* state)
 {
     /* avoid const char * -> char * conversion warning */
     return (char *)(uptrval)((LZ4_stream_t*)state)->internal_donotuse.dictionary;
 }
```

### Comparing `pyxcp-0.20.4/pyxcp/recorder/lz4.h` & `pyxcp-0.21.1/pyxcp/recorder/lz4.h`

 * *Files 7% similar despite different names*

```diff
@@ -93,44 +93,85 @@
 #  define LZ4LIB_API __declspec(dllexport) LZ4LIB_VISIBILITY
 #elif defined(LZ4_DLL_IMPORT) && (LZ4_DLL_IMPORT==1)
 #  define LZ4LIB_API __declspec(dllimport) LZ4LIB_VISIBILITY /* It isn't required but allows to generate better code, saving a function pointer load from the IAT and an indirect jump.*/
 #else
 #  define LZ4LIB_API LZ4LIB_VISIBILITY
 #endif
 
+/*! LZ4_FREESTANDING :
+ *  When this macro is set to 1, it enables "freestanding mode" that is
+ *  suitable for typical freestanding environment which doesn't support
+ *  standard C library.
+ *
+ *  - LZ4_FREESTANDING is a compile-time switch.
+ *  - It requires the following macros to be defined:
+ *    LZ4_memcpy, LZ4_memmove, LZ4_memset.
+ *  - It only enables LZ4/HC functions which don't use heap.
+ *    All LZ4F_* functions are not supported.
+ *  - See tests/freestanding.c to check its basic setup.
+ */
+#if defined(LZ4_FREESTANDING) && (LZ4_FREESTANDING == 1)
+#  define LZ4_HEAPMODE 0
+#  define LZ4HC_HEAPMODE 0
+#  define LZ4_STATIC_LINKING_ONLY_DISABLE_MEMORY_ALLOCATION 1
+#  if !defined(LZ4_memcpy)
+#    error "LZ4_FREESTANDING requires macro 'LZ4_memcpy'."
+#  endif
+#  if !defined(LZ4_memset)
+#    error "LZ4_FREESTANDING requires macro 'LZ4_memset'."
+#  endif
+#  if !defined(LZ4_memmove)
+#    error "LZ4_FREESTANDING requires macro 'LZ4_memmove'."
+#  endif
+#elif ! defined(LZ4_FREESTANDING)
+#  define LZ4_FREESTANDING 0
+#endif
+
+
 /*------   Version   ------*/
 #define LZ4_VERSION_MAJOR    1    /* for breaking interface changes  */
 #define LZ4_VERSION_MINOR    9    /* for new (non-breaking) interface capabilities */
-#define LZ4_VERSION_RELEASE  3    /* for tweaks, bug-fixes, or development */
+#define LZ4_VERSION_RELEASE  4    /* for tweaks, bug-fixes, or development */
 
 #define LZ4_VERSION_NUMBER (LZ4_VERSION_MAJOR *100*100 + LZ4_VERSION_MINOR *100 + LZ4_VERSION_RELEASE)
 
 #define LZ4_LIB_VERSION LZ4_VERSION_MAJOR.LZ4_VERSION_MINOR.LZ4_VERSION_RELEASE
 #define LZ4_QUOTE(str) #str
 #define LZ4_EXPAND_AND_QUOTE(str) LZ4_QUOTE(str)
-#define LZ4_VERSION_STRING LZ4_EXPAND_AND_QUOTE(LZ4_LIB_VERSION)
+#define LZ4_VERSION_STRING LZ4_EXPAND_AND_QUOTE(LZ4_LIB_VERSION)  /* requires v1.7.3+ */
 
-LZ4LIB_API int LZ4_versionNumber (void);  /**< library version number; useful to check dll version */
-LZ4LIB_API const char* LZ4_versionString (void);   /**< library version string; useful to check dll version */
+LZ4LIB_API int LZ4_versionNumber (void);  /**< library version number; useful to check dll version; requires v1.3.0+ */
+LZ4LIB_API const char* LZ4_versionString (void);   /**< library version string; useful to check dll version; requires v1.7.5+ */
 
 
 /*-************************************
 *  Tuning parameter
 **************************************/
+#define LZ4_MEMORY_USAGE_MIN 10
+#define LZ4_MEMORY_USAGE_DEFAULT 14
+#define LZ4_MEMORY_USAGE_MAX 20
+
 /*!
  * LZ4_MEMORY_USAGE :
- * Memory usage formula : N->2^N Bytes (examples : 10 -> 1KB; 12 -> 4KB ; 16 -> 64KB; 20 -> 1MB; etc.)
- * Increasing memory usage improves compression ratio.
- * Reduced memory usage may improve speed, thanks to better cache locality.
+ * Memory usage formula : N->2^N Bytes (examples : 10 -> 1KB; 12 -> 4KB ; 16 -> 64KB; 20 -> 1MB; )
+ * Increasing memory usage improves compression ratio, at the cost of speed.
+ * Reduced memory usage may improve speed at the cost of ratio, thanks to better cache locality.
  * Default value is 14, for 16KB, which nicely fits into Intel x86 L1 cache
  */
 #ifndef LZ4_MEMORY_USAGE
-# define LZ4_MEMORY_USAGE 14
+# define LZ4_MEMORY_USAGE LZ4_MEMORY_USAGE_DEFAULT
 #endif
 
+#if (LZ4_MEMORY_USAGE < LZ4_MEMORY_USAGE_MIN)
+#  error "LZ4_MEMORY_USAGE is too small !"
+#endif
+
+#if (LZ4_MEMORY_USAGE > LZ4_MEMORY_USAGE_MAX)
+#  error "LZ4_MEMORY_USAGE is too large !"
+#endif
 
 /*-************************************
 *  Simple Functions
 **************************************/
 /*! LZ4_compress_default() :
  *  Compresses 'srcSize' bytes from buffer 'src'
  *  into already allocated 'dst' buffer of size 'dstCapacity'.
@@ -144,16 +185,17 @@
  *     @return  : the number of bytes written into buffer 'dst' (necessarily <= dstCapacity)
  *                or 0 if compression fails
  * Note : This function is protected against buffer overflow scenarios (never writes outside 'dst' buffer, nor read outside 'source' buffer).
  */
 LZ4LIB_API int LZ4_compress_default(const char* src, char* dst, int srcSize, int dstCapacity);
 
 /*! LZ4_decompress_safe() :
- *  compressedSize : is the exact complete size of the compressed block.
- *  dstCapacity : is the size of destination buffer (which must be already allocated), presumed an upper bound of decompressed size.
+ * @compressedSize : is the exact complete size of the compressed block.
+ * @dstCapacity : is the size of destination buffer (which must be already allocated),
+ *                is an upper bound of decompressed size.
  * @return : the number of bytes decompressed into destination buffer (necessarily <= dstCapacity)
  *           If destination buffer is not large enough, decoding will stop and output an error code (negative value).
  *           If the source stream is detected malformed, the function will stop decoding and return a negative result.
  * Note 1 : This function is protected against malicious data packets :
  *          it will never writes outside 'dst' buffer, nor read outside 'source' buffer,
  *          even if the compressed block is maliciously modified to order the decoder to do these actions.
  *          In such case, the decoder stops immediately, and considers the compressed block malformed.
@@ -210,15 +252,15 @@
  *  note: acceleration parameter is fixed to "default".
  *
  * *srcSizePtr : will be modified to indicate how many bytes where read from 'src' to fill 'dst'.
  *               New value is necessarily <= input value.
  * @return : Nb bytes written into 'dst' (necessarily <= targetDestSize)
  *           or 0 if compression fails.
  *
- * Note : from v1.8.2 to v1.9.1, this function had a bug (fixed un v1.9.2+):
+ * Note : from v1.8.2 to v1.9.1, this function had a bug (fixed in v1.9.2+):
  *        the produced compressed content could, in specific circumstances,
  *        require to be decompressed into a destination buffer larger
  *        by at least 1 byte than the content to decompress.
  *        If an application uses `LZ4_compress_destSize()`,
  *        it's highly recommended to update liblz4 to v1.9.2 or better.
  *        If this can't be done or ensured,
  *        the receiving decompression function should provide
@@ -266,16 +308,33 @@
 
 
 /*-*********************************************
 *  Streaming Compression Functions
 ***********************************************/
 typedef union LZ4_stream_u LZ4_stream_t;  /* incomplete type (defined later) */
 
+/**
+ Note about RC_INVOKED
+
+ - RC_INVOKED is predefined symbol of rc.exe (the resource compiler which is part of MSVC/Visual Studio).
+   https://docs.microsoft.com/en-us/windows/win32/menurc/predefined-macros
+
+ - Since rc.exe is a legacy compiler, it truncates long symbol (> 30 chars)
+   and reports warning "RC4011: identifier truncated".
+
+ - To eliminate the warning, we surround long preprocessor symbol with
+   "#if !defined(RC_INVOKED) ... #endif" block that means
+   "skip this block when rc.exe is trying to read it".
+*/
+#if !defined(RC_INVOKED) /* https://docs.microsoft.com/en-us/windows/win32/menurc/predefined-macros */
+#if !defined(LZ4_STATIC_LINKING_ONLY_DISABLE_MEMORY_ALLOCATION)
 LZ4LIB_API LZ4_stream_t* LZ4_createStream(void);
 LZ4LIB_API int           LZ4_freeStream (LZ4_stream_t* streamPtr);
+#endif /* !defined(LZ4_STATIC_LINKING_ONLY_DISABLE_MEMORY_ALLOCATION) */
+#endif
 
 /*! LZ4_resetStream_fast() : v1.9.0+
  *  Use this to prepare an LZ4_stream_t for a new chain of dependent blocks
  *  (e.g., LZ4_compress_fast_continue()).
  *
  *  An LZ4_stream_t must be initialized once before usage.
  *  This is automatically done when created by LZ4_createStream().
@@ -351,16 +410,20 @@
 ************************************************/
 typedef union LZ4_streamDecode_u LZ4_streamDecode_t;   /* tracking context */
 
 /*! LZ4_createStreamDecode() and LZ4_freeStreamDecode() :
  *  creation / destruction of streaming decompression tracking context.
  *  A tracking context can be re-used multiple times.
  */
+#if !defined(RC_INVOKED) /* https://docs.microsoft.com/en-us/windows/win32/menurc/predefined-macros */
+#if !defined(LZ4_STATIC_LINKING_ONLY_DISABLE_MEMORY_ALLOCATION)
 LZ4LIB_API LZ4_streamDecode_t* LZ4_createStreamDecode(void);
 LZ4LIB_API int                 LZ4_freeStreamDecode (LZ4_streamDecode_t* LZ4_stream);
+#endif /* !defined(LZ4_STATIC_LINKING_ONLY_DISABLE_MEMORY_ALLOCATION) */
+#endif
 
 /*! LZ4_setStreamDecode() :
  *  An LZ4_streamDecode_t context can be allocated once and re-used multiple times.
  *  Use this function to start decompression of a new stream of blocks.
  *  A dictionary can optionally be set. Use NULL or size 0 for a reset order.
  *  Dictionary is presumed stable : it must remain accessible and unmodified during next decompression.
  * @return : 1 if OK, 0 if error
@@ -377,19 +440,32 @@
  *  to be compatible with any source respecting maxBlockSize condition.
  * @return : minimum ring buffer size,
  *           or 0 if there is an error (invalid maxBlockSize).
  */
 LZ4LIB_API int LZ4_decoderRingBufferSize(int maxBlockSize);
 #define LZ4_DECODER_RING_BUFFER_SIZE(maxBlockSize) (65536 + 14 + (maxBlockSize))  /* for static allocation; maxBlockSize presumed valid */
 
-/*! LZ4_decompress_*_continue() :
- *  These decoding functions allow decompression of consecutive blocks in "streaming" mode.
- *  A block is an unsplittable entity, it must be presented entirely to a decompression function.
- *  Decompression functions only accepts one block at a time.
- *  The last 64KB of previously decoded data *must* remain available and unmodified at the memory position where they were decoded.
+/*! LZ4_decompress_safe_continue() :
+ *  This decoding function allows decompression of consecutive blocks in "streaming" mode.
+ *  The difference with the usual independent blocks is that
+ *  new blocks are allowed to find references into former blocks.
+ *  A block is an unsplittable entity, and must be presented entirely to the decompression function.
+ *  LZ4_decompress_safe_continue() only accepts one block at a time.
+ *  It's modeled after `LZ4_decompress_safe()` and behaves similarly.
+ *
+ * @LZ4_streamDecode : decompression state, tracking the position in memory of past data
+ * @compressedSize : exact complete size of one compressed block.
+ * @dstCapacity : size of destination buffer (which must be already allocated),
+ *                must be an upper bound of decompressed size.
+ * @return : number of bytes decompressed into destination buffer (necessarily <= dstCapacity)
+ *           If destination buffer is not large enough, decoding will stop and output an error code (negative value).
+ *           If the source stream is detected malformed, the function will stop decoding and return a negative result.
+ *
+ *  The last 64KB of previously decoded data *must* remain available and unmodified
+ *  at the memory position where they were previously decoded.
  *  If less than 64KB of data has been decoded, all the data must be present.
  *
  *  Special : if decompression side sets a ring buffer, it must respect one of the following conditions :
  *  - Decompression buffer size is _at least_ LZ4_decoderRingBufferSize(maxBlockSize).
  *    maxBlockSize is the maximum size of any single block. It can have any value > 16 bytes.
  *    In which case, encoding and decoding buffers do not need to be synchronized.
  *    Actually, data can be produced by any source compliant with LZ4 format specification, and respecting maxBlockSize.
@@ -402,26 +478,44 @@
  *    In which case, encoding and decoding buffers do not need to be synchronized,
  *    and encoding ring buffer can have any size, including small ones ( < 64 KB).
  *
  *  Whenever these conditions are not possible,
  *  save the last 64KB of decoded data into a safe buffer where it can't be modified during decompression,
  *  then indicate where this data is saved using LZ4_setStreamDecode(), before decompressing next block.
 */
-LZ4LIB_API int LZ4_decompress_safe_continue (LZ4_streamDecode_t* LZ4_streamDecode, const char* src, char* dst, int srcSize, int dstCapacity);
+LZ4LIB_API int
+LZ4_decompress_safe_continue (LZ4_streamDecode_t* LZ4_streamDecode,
+                        const char* src, char* dst,
+                        int srcSize, int dstCapacity);
 
 
-/*! LZ4_decompress_*_usingDict() :
- *  These decoding functions work the same as
- *  a combination of LZ4_setStreamDecode() followed by LZ4_decompress_*_continue()
- *  They are stand-alone, and don't need an LZ4_streamDecode_t structure.
+/*! LZ4_decompress_safe_usingDict() :
+ *  Works the same as
+ *  a combination of LZ4_setStreamDecode() followed by LZ4_decompress_safe_continue()
+ *  However, it's stateless: it doesn't need any LZ4_streamDecode_t state.
  *  Dictionary is presumed stable : it must remain accessible and unmodified during decompression.
  *  Performance tip : Decompression speed can be substantially increased
  *                    when dst == dictStart + dictSize.
  */
-LZ4LIB_API int LZ4_decompress_safe_usingDict (const char* src, char* dst, int srcSize, int dstCapcity, const char* dictStart, int dictSize);
+LZ4LIB_API int
+LZ4_decompress_safe_usingDict(const char* src, char* dst,
+                              int srcSize, int dstCapacity,
+                              const char* dictStart, int dictSize);
+
+/*! LZ4_decompress_safe_partial_usingDict() :
+ *  Behaves the same as LZ4_decompress_safe_partial()
+ *  with the added ability to specify a memory segment for past data.
+ *  Performance tip : Decompression speed can be substantially increased
+ *                    when dst == dictStart + dictSize.
+ */
+LZ4LIB_API int
+LZ4_decompress_safe_partial_usingDict(const char* src, char* dst,
+                                      int compressedSize,
+                                      int targetOutputSize, int maxOutputSize,
+                                      const char* dictStart, int dictSize);
 
 #endif /* LZ4_H_2983827168210 */
 
 
 /*^*************************************
  * !!!!!!   STATIC LINKING ONLY   !!!!!!
  ***************************************/
@@ -492,15 +586,17 @@
  *  compression call.
  *
  *  The dictionary will only remain attached to the working stream through the
  *  first compression call, at the end of which it is cleared. The dictionary
  *  stream (and source buffer) must remain in-place / accessible / unchanged
  *  through the completion of the first compression call on the stream.
  */
-LZ4LIB_STATIC_API void LZ4_attach_dictionary(LZ4_stream_t* workingStream, const LZ4_stream_t* dictionaryStream);
+LZ4LIB_STATIC_API void
+LZ4_attach_dictionary(LZ4_stream_t* workingStream,
+                const LZ4_stream_t* dictionaryStream);
 
 
 /*! In-place compression and decompression
  *
  * It's possible to have input and output sharing the same buffer,
  * for highly constrained memory environments.
  * In both cases, it requires input to lay at the end of the buffer,
@@ -588,46 +684,34 @@
 #else
   typedef   signed char  LZ4_i8;
   typedef unsigned char  LZ4_byte;
   typedef unsigned short LZ4_u16;
   typedef unsigned int   LZ4_u32;
 #endif
 
+/*! LZ4_stream_t :
+ *  Never ever use below internal definitions directly !
+ *  These definitions are not API/ABI safe, and may change in future versions.
+ *  If you need static allocation, declare or allocate an LZ4_stream_t object.
+**/
+
 typedef struct LZ4_stream_t_internal LZ4_stream_t_internal;
 struct LZ4_stream_t_internal {
     LZ4_u32 hashTable[LZ4_HASH_SIZE_U32];
-    LZ4_u32 currentOffset;
-    LZ4_u32 tableType;
     const LZ4_byte* dictionary;
     const LZ4_stream_t_internal* dictCtx;
+    LZ4_u32 currentOffset;
+    LZ4_u32 tableType;
     LZ4_u32 dictSize;
+    /* Implicit padding to ensure structure is aligned */
 };
 
-typedef struct {
-    const LZ4_byte* externalDict;
-    size_t extDictSize;
-    const LZ4_byte* prefixEnd;
-    size_t prefixSize;
-} LZ4_streamDecode_t_internal;
-
-
-/*! LZ4_stream_t :
- *  Do not use below internal definitions directly !
- *  Declare or allocate an LZ4_stream_t instead.
- *  LZ4_stream_t can also be created using LZ4_createStream(), which is recommended.
- *  The structure definition can be convenient for static allocation
- *  (on stack, or as part of larger structure).
- *  Init this structure with LZ4_initStream() before first use.
- *  note : only use this definition in association with static linking !
- *  this definition is not API/ABI safe, and may change in future versions.
- */
-#define LZ4_STREAMSIZE       16416  /* static size, for inter-version compatibility */
-#define LZ4_STREAMSIZE_VOIDP (LZ4_STREAMSIZE / sizeof(void*))
+#define LZ4_STREAM_MINSIZE  ((1UL << LZ4_MEMORY_USAGE) + 32)  /* static size, for inter-version compatibility */
 union LZ4_stream_u {
-    void* table[LZ4_STREAMSIZE_VOIDP];
+    char minStateSize[LZ4_STREAM_MINSIZE];
     LZ4_stream_t_internal internal_donotuse;
 }; /* previously typedef'd to LZ4_stream_t */
 
 
 /*! LZ4_initStream() : v1.9.0+
  *  An LZ4_stream_t structure must be initialized at least once.
  *  This is automatically done when invoking LZ4_createStream(),
@@ -637,29 +721,33 @@
  *  It can also initialize any arbitrary buffer of sufficient size,
  *  and will @return a pointer of proper type upon initialization.
  *
  *  Note : initialization fails if size and alignment conditions are not respected.
  *         In which case, the function will @return NULL.
  *  Note2: An LZ4_stream_t structure guarantees correct alignment and size.
  *  Note3: Before v1.9.0, use LZ4_resetStream() instead
- */
+**/
 LZ4LIB_API LZ4_stream_t* LZ4_initStream (void* buffer, size_t size);
 
 
 /*! LZ4_streamDecode_t :
- *  information structure to track an LZ4 stream during decompression.
- *  init this structure  using LZ4_setStreamDecode() before first use.
- *  note : only use in association with static linking !
- *         this definition is not API/ABI safe,
- *         and may change in a future version !
- */
-#define LZ4_STREAMDECODESIZE_U64 (4 + ((sizeof(void*)==16) ? 2 : 0) /*AS-400*/ )
-#define LZ4_STREAMDECODESIZE     (LZ4_STREAMDECODESIZE_U64 * sizeof(unsigned long long))
+ *  Never ever use below internal definitions directly !
+ *  These definitions are not API/ABI safe, and may change in future versions.
+ *  If you need static allocation, declare or allocate an LZ4_streamDecode_t object.
+**/
+typedef struct {
+    const LZ4_byte* externalDict;
+    const LZ4_byte* prefixEnd;
+    size_t extDictSize;
+    size_t prefixSize;
+} LZ4_streamDecode_t_internal;
+
+#define LZ4_STREAMDECODE_MINSIZE 32
 union LZ4_streamDecode_u {
-    unsigned long long table[LZ4_STREAMDECODESIZE_U64];
+    char minStateSize[LZ4_STREAMDECODE_MINSIZE];
     LZ4_streamDecode_t_internal internal_donotuse;
 } ;   /* previously typedef'd to LZ4_streamDecode_t */
 
 
 
 /*-************************************
 *  Obsolete Functions
```

### Comparing `pyxcp-0.20.4/pyxcp/recorder/mio.hpp` & `pyxcp-0.21.1/pyxcp/recorder/mio.hpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/recorder/reco.py` & `pyxcp-0.21.1/pyxcp/recorder/reco.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/recorder/rekorder.cpp` & `pyxcp-0.21.1/pyxcp/recorder/rekorder.cpp`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         auto fr = frame_header_t{};
         fr.category = 1;
         fr.counter = idx;
         fr.timestamp = std::clock();
         fr.length = 10 + (rand() % 240);
         filler = (filler + 1) % 16;
         memset(buffer, filler, fr.length);
-        writer.add_frame(fr.category, fr.counter, fr.timestamp, fr.length, reinterpret_cast<char const*>(&buffer));
+        writer.add_frame(fr.category, fr.counter, fr.timestamp, fr.length, std::bit_cast<char const*>(&buffer));
     }
 }
 
 
 int main()
 {
     srand(42);
@@ -51,13 +51,13 @@
 
 	while (true) {
 		const auto& frames = reader.next_block();
 	    if (!frames) {
 	        break;
 	    }
         for (const auto& frame: frames.value()) {
-            auto [category, counter, timestamp, length, payload] = frame;
+            auto const& [category, counter, timestamp, length, payload] = frame;
         }
 	}
     printf("---\n");
     printf("Finished.\n");
 }
```

### Comparing `pyxcp-0.20.4/pyxcp/recorder/rekorder.hpp` & `pyxcp-0.21.1/pyxcp/recorder/rekorder.hpp`

 * *Files 10% similar despite different names*

```diff
@@ -56,20 +56,20 @@
 #endif
 
 
 #define __ALIGNMENT_REQUIREMENT     __BIGGEST_ALIGNMENT__
 #define __ALIGN                     alignas(__ALIGNMENT_REQUIREMENT)
 
 
-constexpr auto kilobytes(std::size_t value) -> std::size_t
+constexpr auto kilobytes(std::uint32_t value) -> std::uint32_t
 {
     return value * 1024;
 }
 
-constexpr auto megabytes(std::size_t value) -> std::size_t
+constexpr auto megabytes(std::uint32_t value) -> std::uint32_t
 {
     return kilobytes(value) * 1024;
 }
 
 constexpr uint16_t XCP_PAYLOAD_MAX = 0xFFFF;
 
 /*
@@ -115,18 +115,16 @@
     double timestamp {0.0};
     uint16_t length {0};
 };
 #pragma pack(pop)
 
 using FrameTuple = std::tuple<std::uint8_t, std::uint16_t, double, std::uint16_t, payload_t>;
 using FrameVector = std::vector<FrameTuple>;
-
 using FrameTupleWriter = std::tuple<std::uint8_t, std::uint16_t, double, std::uint16_t, char *>;
 
-
 enum class FrameCategory : std::uint8_t {
     META,
     CMD,
     RES,
     ERR,
     EV,
     SERV,
@@ -141,130 +139,128 @@
     constexpr auto MAGIC_SIZE = 16;
     constexpr auto VERSION = 0x0100;
     constexpr auto FILE_HEADER_SIZE = sizeof(FileHeaderType);
     constexpr auto CONTAINER_SIZE = sizeof(ContainerHeaderType);
 }
 
 
-inline auto file_header_size() -> std::size_t {
+constexpr auto file_header_size() -> std::uint32_t {
     return (detail::FILE_HEADER_SIZE + detail::MAGIC_SIZE);
 }
 
-using rounding_func_t = std::function<std::size_t(std::size_t)>;
+using rounding_func_t = std::function<std::uint32_t(std::uint32_t)>;
 
-inline const rounding_func_t create_rounding_func(std::size_t multiple) {
-    return [=](std::size_t value) -> std::size_t {
+inline rounding_func_t create_rounding_func(std::uint32_t multiple)  {
+    return [multiple](std::uint32_t value) {
         return (value + (multiple - 1)) & ~(multiple -1 );
     };
 }
 
 const auto round_to_alignment = create_rounding_func(__ALIGNMENT_REQUIREMENT);
 
 
-inline void _fcopy(char * dest, char const * src, std::size_t n)
+inline void _fcopy(char * dest, char const * src, std::uint32_t n) noexcept
 {
-    for (std::size_t i = 0; i < n; ++i) {
+    for (std::uint32_t i = 0; i < n; ++i) {
         dest[i] = src[i];
     }
 }
 
 #if STANDALONE_REKORDER == 1
-    inline blob_t * get_payload_ptr(const payload_t& payload) {
+    inline blob_t * get_payload_ptr(const payload_t& payload) noexcept {
         return payload.get();
     }
 
-    inline payload_t create_payload(std::size_t size, blob_t const * data) {
-        //auto pl = std::make_unique<char[]>(size);
+    inline payload_t create_payload(std::uint32_t size, blob_t const * data) noexcept {
         auto pl = std::make_shared<blob_t[]>(size);
         _fcopy(reinterpret_cast<char*>(pl.get()), reinterpret_cast<char const*>(data), size);
         return pl;
     }
 #else
-	inline payload_t create_payload(std::size_t size, blob_t const * data) {
+	inline payload_t create_payload(std::uint32_t size, blob_t const * data) {
         return py::array_t<blob_t>(size, data);
     }
 
-    inline blob_t * get_payload_ptr(const payload_t& payload) {
+    inline blob_t * get_payload_ptr(const payload_t& payload) noexcept {
         py::buffer_info buf = payload.request();
 
         return  static_cast<blob_t *>(buf.ptr);
     }
 #endif /* STANDALONE_REKORDER */
 
-inline void hexdump(blob_t const * buf, std::uint16_t sz)
-{
-    std::uint16_t idx;
-
-    for (idx = 0; idx < sz; ++idx)
+inline void hexdump(blob_t const * buf, std::uint16_t sz) {
+    for (std::uint16_t idx = 0; idx < sz; ++idx)
     {
         printf("%02X ", buf[idx]);
     }
     printf("\n\r");
 }
 
 
 template <typename T>
 class TsQueue {
 public:
-    explicit  TsQueue() {}
+    TsQueue() = default;
 
-    TsQueue(const TsQueue& other) : m_mtx{}, m_cond{} {
-        std::lock_guard<std::mutex> lock(other.m_mtx);
+    TsQueue(const TsQueue& other) noexcept {
+        std::scoped_lock lock(other.m_mtx);
         m_queue = other.m_queue;
     }
 
-    void put(T value) {
-        std::lock_guard<std::mutex> lock(m_mtx);
+    void put(T value) noexcept {
+        std::scoped_lock lock(m_mtx);
         m_queue.push(value);
         m_cond.notify_one();
     }
 
-    std::shared_ptr<T> get() {
-        std::unique_lock<std::mutex> lock(m_mtx);
+    std::shared_ptr<T> get() noexcept {
+        std::unique_lock lock(m_mtx);
         m_cond.wait(lock, [this]{return !m_queue.empty();});
         std::shared_ptr<T> result(std::make_shared<T>(m_queue.front()));
         m_queue.pop();
         return result;
     }
 
-    bool empty() const {
-        std::lock_guard<std::mutex> lock(m_mtx);
+    bool empty() const noexcept {
+        std::scoped_lock lock(m_mtx);
         return m_queue.empty();
     }
 
 private:
     mutable std::mutex m_mtx;
     std::queue<T> m_queue;
     std::condition_variable m_cond;
 };
 
 
 class Event {
 public:
-    explicit Event() {}
 
-    Event(const Event& other) {
-        std::lock_guard<std::mutex> lock(other.m_mtx);
+    Event(const Event& other) noexcept {
+        std::scoped_lock lock(other.m_mtx);
         m_flag = other.m_flag;
     }
 
-    void signal() {
-        std::lock_guard<std::mutex> lock(m_mtx);
+    ~Event() = default;
+    Event() = default;
+
+    void signal() noexcept {
+        std::scoped_lock lock(m_mtx);
         m_flag = true;
         m_cond.notify_one();
     }
 
-    void wait() {
-        std::unique_lock<std::mutex> lock(m_mtx);
+    void wait() noexcept {
+        std::unique_lock lock(m_mtx);
         m_cond.wait(lock, [this]{return m_flag;});
         m_flag = false;
     }
 
-    bool state() const {
-        std::lock_guard<std::mutex> lock(m_mtx);
+    bool state() const noexcept {
+        std::scoped_lock lock(m_mtx);
         return m_flag;
     }
 
 private:
     mutable std::mutex m_mtx {};
     bool m_flag {false};
     std::condition_variable m_cond {};
@@ -277,88 +273,98 @@
  *
  */
 template <typename T, int _IS, int _NB>
 class BlockMemory {
 
 public:
 
-    using mem_block_t = T[_IS];
+    using mem_block_t = std::array<T, _IS>;
 
-    explicit BlockMemory() : m_memory{nullptr}, m_allocation_count{0} {
-        m_memory = new T[_IS * _NB];	// Ts to allocate: itemsize * number of items.
-        //printf("mem-base  : %p\n", m_memory);
+    explicit BlockMemory() noexcept : m_memory{nullptr}, m_allocation_count{0} {
+        m_memory = new T[_IS * _NB];
     }
 
-    ~BlockMemory() {
+    ~BlockMemory() noexcept {
         if (m_memory) {
             delete[] m_memory;
         }
     }
 
     T * acquire() noexcept {
-        const std::lock_guard<std::mutex> lock(m_mtx);
+        const std::scoped_lock lock(m_mtx);
 
         if (m_allocation_count >= _NB) {
             return nullptr;
         }
-        T * ptr = reinterpret_cast<T *>((m_memory + (m_allocation_count * _IS)));
-        //printf("acquire() %p\n", ptr);
+        T * ptr = reinterpret_cast<T *>(m_memory + (m_allocation_count * _IS));
         m_allocation_count++;
         return ptr;
     }
 
     void release() noexcept {
-        const std::lock_guard<std::mutex> lock(m_mtx);
-        //printf("release() %u\n", m_allocation_count);
+        const std::scoped_lock lock(m_mtx);
         if (m_allocation_count == 0) {
             return;
         }
         m_allocation_count--;
     }
 
 private:
 
     T * m_memory;
-    std::size_t m_allocation_count;
+    std::uint32_t m_allocation_count;
     std::mutex m_mtx;
+
+public:
+
+    BlockMemory(T* m_memory, const std::uint32_t& m_allocation_count, const std::mutex& m_mtx)
+        : m_memory(m_memory), m_allocation_count(m_allocation_count), m_mtx(m_mtx)
+    {
+    }
+
+    bool operator==(const BlockMemory& other) const = default;
 };
 
 
 /**
  */
 class XcpLogFileWriter
 {
 public:
-    explicit XcpLogFileWriter(const std::string& file_name, uint32_t prealloc = 10UL, uint32_t chunk_size = 1)
+    explicit XcpLogFileWriter(const std::string& file_name, uint32_t prealloc = 10UL, uint32_t chunk_size = 1) noexcept
     {
-        m_file_name = file_name + detail::FILE_EXTENSION;
+        if (!file_name.ends_with(detail::FILE_EXTENSION)) {
+            m_file_name = file_name + detail::FILE_EXTENSION;
+        } else {
+            m_file_name = file_name;
+        }
+
 #if defined(_WIN32)
         m_fd = CreateFileA(
             m_file_name.c_str(),
             GENERIC_READ | GENERIC_WRITE,
             0,
             (LPSECURITY_ATTRIBUTES)nullptr,
             CREATE_ALWAYS,
             FILE_ATTRIBUTE_NORMAL | FILE_FLAG_RANDOM_ACCESS,
             nullptr
         );
-        //printf("CreateFile returned: %u\n", GetLastError());
 #else
         m_fd = open(m_file_name.c_str(), O_CREAT | O_RDWR | O_TRUNC, 0666);
 #endif
         truncate(megabytes(prealloc));
         m_mmap = new mio::mmap_sink(m_fd);
         m_chunk_size = megabytes(chunk_size);
         m_intermediate_storage = new blob_t[m_chunk_size + megabytes(1)];
         m_offset = detail::FILE_HEADER_SIZE + detail::MAGIC_SIZE;
 
         start_thread();
     }
 
-    ~XcpLogFileWriter() {
+    ~XcpLogFileWriter() noexcept {
         finalize();
     }
 
     void finalize() {
         if (!m_finalized) {
             m_finalized = true;
             stop_thread();
@@ -374,48 +380,47 @@
             close(m_fd);
 #endif
             delete m_mmap;
             delete[] m_intermediate_storage;
         }
     }
 
-    void add_frame(uint8_t category, uint16_t counter, double timestamp, uint16_t length, char const * data) {
+    void add_frame(uint8_t category, uint16_t counter, double timestamp, uint16_t length, char const * data) noexcept {
         auto payload= new char[length];
         //auto payload = mem.acquire();
 
     	_fcopy(payload, data, length);
     	my_queue.put(
             std::make_tuple(category, counter, timestamp, length, payload)
         );
     }
 
 protected:
-    void truncate(off_t size) const
+    void truncate(off_t size) const noexcept
     {
-        //printf("truncating to: %lldKBytes.\n", kilobytes(size));
 #if defined(_WIN32)
-
-        DWORD result;
-
-        result = SetFilePointer(m_fd, size, nullptr, FILE_BEGIN);
-
-        result = SetEndOfFile(m_fd);
-
+        if (SetFilePointer(m_fd, size, nullptr, FILE_BEGIN) == INVALID_SET_FILE_POINTER) {
+            // TODO: Errorhandling.
+        }
+        if (SetEndOfFile(m_fd) == 0) {
+            // TODO: Errorhandling.
+        }
 #else
         ftruncate(m_fd, size);
 #endif
     }
 
-    blob_t * ptr(std::size_t pos = 0) const
+    blob_t * ptr(std::uint32_t pos = 0) const noexcept
     {
         return (blob_t *)(m_mmap->data() + pos);
     }
 
-    void store_im(void const * data, std::size_t length) {
-        _fcopy(reinterpret_cast<char *>(m_intermediate_storage + m_intermediate_storage_offset), reinterpret_cast<char const*>(data), length);
+    template<typename T>
+    void store_im(T const * data, std::uint32_t length) noexcept {
+        _fcopy(reinterpret_cast<char*>(m_intermediate_storage + m_intermediate_storage_offset), reinterpret_cast<char const*>(data), length);
         m_intermediate_storage_offset += length;
     }
 
     void compress_frames() {
         auto container = ContainerHeaderType{};
         //printf("Compressing %u frames... [%d]\n", m_container_record_count, m_intermediate_storage_offset);
         const int cp_size = ::LZ4_compress_default(
@@ -437,49 +442,49 @@
         m_container_size_uncompressed = 0;
         m_container_size_compressed = 0;
         m_container_record_count = 0;
         m_intermediate_storage_offset = 0;
         m_num_containers += 1;
     }
 
-    void write_bytes(std::size_t pos, std::size_t count, char const * buf) const
+    void write_bytes(std::uint32_t pos, std::uint32_t count, char const * buf) const noexcept
     {
         auto addr = reinterpret_cast<char *>(ptr(pos));
 
         _fcopy(addr, buf, count);
     }
 
     void write_header(uint16_t version, uint16_t options, uint32_t num_containers,
-                      uint32_t record_count, uint32_t size_compressed, uint32_t size_uncompressed) {
+                      uint32_t record_count, uint32_t size_compressed, uint32_t size_uncompressed) noexcept {
         auto header = FileHeaderType{};
         write_bytes(0x00000000UL, detail::MAGIC_SIZE, detail::MAGIC.c_str());
         header.hdr_size = detail::FILE_HEADER_SIZE + detail::MAGIC_SIZE;
         header.version = version;
         header.options = options;
         header.num_containers = num_containers;
         header.record_count = record_count;
         header.size_compressed = size_compressed;
         header.size_uncompressed = size_uncompressed;
         write_bytes(0x00000000UL + detail::MAGIC_SIZE, detail::FILE_HEADER_SIZE, reinterpret_cast<char const*>(&header));
     }
 
-    bool start_thread() {
+    bool start_thread() noexcept {
         if (collector_thread.joinable()) {
             return false;
         }
         stop_collector_thread_flag = false;
-        collector_thread = std::thread([this]() {
+        collector_thread = std::jthread([this]() {
             while (!stop_collector_thread_flag) {
                 auto item = my_queue.get();
                 const auto content = item.get();
                 if (stop_collector_thread_flag == true)
                 {
                     break;
                 }
-                auto [category, counter, timestamp, length, payload] = content->value();
+                auto const& [category, counter, timestamp, length, payload] = content->value();
                 const frame_header_t frame{ category, counter, timestamp, length };
 
                 store_im(&frame, sizeof(frame));
                 store_im(payload, length);
                 delete[] payload;
                 //mem.release();
                 m_container_record_count += 1;
@@ -488,60 +493,65 @@
                     compress_frames();
                 }
             }
         });
         return true;
     }
 
-    bool stop_thread() {
+    bool stop_thread() noexcept {
         if (!collector_thread.joinable()) {
             return false;
         }
         stop_collector_thread_flag = true;
         my_queue.put(std::nullopt);
         collector_thread.join();
         return true;
     }
 
 private:
     std::string m_file_name;
-    std::size_t m_offset{0};
+    std::uint32_t m_offset{0};
     std::uint32_t m_chunk_size{0};
     std::uint32_t m_num_containers{0};
     std::uint32_t m_record_count{0UL};
     std::uint32_t m_container_record_count{0UL};
     std::uint32_t m_total_size_uncompressed{0UL};
     std::uint32_t m_total_size_compressed{0UL};
     std::uint32_t m_container_size_uncompressed{0UL};
     std::uint32_t m_container_size_compressed{0UL};
     __ALIGN blob_t * m_intermediate_storage{nullptr};
     std::uint32_t m_intermediate_storage_offset{0};
     mio::file_handle_type m_fd{INVALID_HANDLE_VALUE};
     mio::mmap_sink * m_mmap{nullptr};
     bool m_finalized{false};
-    std::thread collector_thread{};
+    std::jthread collector_thread{};
     std::mutex mtx;
     TsQueue<std::optional<FrameTupleWriter>> my_queue;
     BlockMemory<char, XCP_PAYLOAD_MAX, 16> mem{};
     std::atomic_bool stop_collector_thread_flag{false};
 };
 
 
 /**
  */
 class XcpLogFileReader
 {
 public:
     explicit XcpLogFileReader(const std::string& file_name)
     {
-        m_file_name = file_name + detail::FILE_EXTENSION;
+        if (!file_name.ends_with(detail::FILE_EXTENSION)) {
+            m_file_name = file_name + detail::FILE_EXTENSION;
+        } else {
+            m_file_name = file_name;
+        }
+
         m_mmap = new mio::mmap_source(m_file_name);
         blob_t magic[detail::MAGIC_SIZE + 1];
 
-        read_bytes(0ul, detail::MAGIC_SIZE, magic);
+        read_bytes(0UL, detail::MAGIC_SIZE, magic);
         if (memcmp(detail::MAGIC.c_str(), magic, detail::MAGIC_SIZE) != 0) {
             throw std::runtime_error("Invalid file magic.");
         }
         m_offset = detail::MAGIC_SIZE;
 
         read_bytes(m_offset, detail::FILE_HEADER_SIZE, reinterpret_cast<blob_t*>(&m_header));
         //printf("Sizes: %u %u %.3f\n", m_header.size_uncompressed,
@@ -565,37 +575,36 @@
 
     [[nodiscard]]
     FileHeaderType get_header()  const noexcept  {
         return m_header;
     }
 
     [[nodiscard]]
-    auto get_header_as_tuple() const -> HeaderTuple {
+    auto get_header_as_tuple() const noexcept -> HeaderTuple {
         auto hdr = get_header();
 
         return std::make_tuple(
             hdr.num_containers,
             hdr.record_count,
             hdr.size_uncompressed,
             hdr.size_compressed,
-            ((std::uint64_t)(((double)hdr.size_uncompressed / (double)hdr.size_compressed * (double)100.0) + (double)0.5)) / 100.0
+            (double)((std::uint64_t)(((double)hdr.size_uncompressed / (double)hdr.size_compressed * 100.0) + 0.5)) / 100.0
         );
     }
 
-    void reset() {
+    void reset() noexcept {
         m_current_container = 0;
         m_offset = file_header_size();
     }
 
-
-    std::optional<FrameVector> next_block() /*noexcept*/ {
+    std::optional<FrameVector> next_block() {
         auto container = ContainerHeaderType{};
         auto total = 0;
         auto frame = frame_header_t{};
-        size_t boffs = 0;
+        std::uint32_t boffs = 0;
         auto result = FrameVector{};
         payload_t payload;
 
         if (m_current_container >= m_header.num_containers) {
             return std::nullopt;
         }
         read_bytes(m_offset, detail::CONTAINER_SIZE, reinterpret_cast<blob_t*>(&container));
@@ -607,44 +616,44 @@
         if (uc_size < 0) {
             throw std::runtime_error("LZ4 decompression failed.");
         }
         boffs = 0;
         for (std::uint32_t idx = 0; idx < container.record_count; ++idx) {
             _fcopy(reinterpret_cast<char *>(&frame), reinterpret_cast<char const*>(&(buffer[boffs])), sizeof(frame_header_t));
             boffs += sizeof(frame_header_t);
-            result.emplace_back(std::make_tuple(frame.category, frame.counter, frame.timestamp, frame.length, create_payload(frame.length, &buffer[boffs])));
+            result.emplace_back(frame.category, frame.counter, frame.timestamp, frame.length, create_payload(frame.length, &buffer[boffs]));
             boffs += frame.length;
         }
         m_offset += container.size_compressed;
         m_current_container += 1;
         delete[] buffer;
 
         return std::optional<FrameVector>{result};
     }
 
-    ~XcpLogFileReader()
+    ~XcpLogFileReader() noexcept
     {
         delete m_mmap;
     }
 
 protected:
     [[nodiscard]]
-    blob_t const *ptr(std::size_t pos = 0) const
+    blob_t const *ptr(std::uint32_t pos = 0) const
     {
         return reinterpret_cast<blob_t const*>(m_mmap->data() + pos);
     }
 
-    void read_bytes(std::size_t pos, std::size_t count, blob_t * buf) const
+    void read_bytes(std::uint32_t pos, std::uint32_t count, blob_t * buf) const
     {
         auto addr = reinterpret_cast<char const*>(ptr(pos));
         _fcopy(reinterpret_cast<char *>(buf), addr, count);
     }
 
 private:
     std::string m_file_name;
-    std::size_t m_offset{0};
-    std::size_t m_current_container{0};
+    std::uint32_t m_offset{0};
+    std::uint32_t m_current_container{0};
     mio::mmap_source * m_mmap{nullptr};
     FileHeaderType m_header;
 };
 
 #endif // __REKORDER_HPP
```

### Comparing `pyxcp-0.20.4/pyxcp/recorder/setup.py` & `pyxcp-0.21.1/pyxcp/recorder/setup.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/recorder/test_reko.py` & `pyxcp-0.21.1/pyxcp/recorder/test_reko.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/recorder/wrap.cpp` & `pyxcp-0.21.1/pyxcp/recorder/wrap.cpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/scripts/pyxcp_probe_can_drivers.py` & `pyxcp-0.21.1/pyxcp/scripts/pyxcp_probe_can_drivers.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/scripts/xcp_fetch_a2l.py` & `pyxcp-0.21.1/pyxcp/scripts/xcp_fetch_a2l.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/scripts/xcp_info.py` & `pyxcp-0.21.1/pyxcp/examples/xcphello.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     "-d",
     "--daq-info",
     dest="daq_info",
     help="Display DAQ-info",
     default=False,
     action="store_true",
 )
+
 with ap.run() as x:
     x.connect()
     if x.slaveProperties.optionalCommMode:
         x.getCommModeInfo()
     identifier = x.identifier(0x01)
     print("\nSlave Properties:")
     print("=================")
```

### Comparing `pyxcp-0.20.4/pyxcp/tests/test_asam_types.py` & `pyxcp-0.21.1/pyxcp/tests/test_asam_types.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/tests/test_can.py` & `pyxcp-0.21.1/pyxcp/tests/test_can.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/tests/test_checksum.py` & `pyxcp-0.21.1/pyxcp/tests/test_checksum.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/tests/test_config.py` & `pyxcp-0.21.1/pyxcp/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/tests/test_frame_padding.py` & `pyxcp-0.21.1/pyxcp/tests/test_frame_padding.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/tests/test_master.py` & `pyxcp-0.21.1/pyxcp/tests/test_master.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/tests/test_transport.py` & `pyxcp-0.21.1/pyxcp/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/tests/test_utils.py` & `pyxcp-0.21.1/pyxcp/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/timing.py` & `pyxcp-0.21.1/pyxcp/timing.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/can.py` & `pyxcp-0.21.1/pyxcp/transport/can.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,20 @@
 """
 """
 import abc
 import functools
 import operator
 from bisect import bisect_left
 from collections import OrderedDict
-from pyxcp.config import Configuration
-from pyxcp.transport.base import BaseTransport
 from time import perf_counter
 from time import time
 
+from pyxcp.config import Configuration
+from pyxcp.transport.base import BaseTransport
+
 
 CAN_EXTENDED_ID = 0x80000000
 MAX_11_BIT_IDENTIFIER = (1 << 11) - 1
 MAX_29_BIT_IDENTIFIER = (1 << 29) - 1
 MAX_DLC_CLASSIC = 8
 CAN_FD_DLCS = (12, 16, 20, 24, 32, 48, 64)  # Discrete CAN-FD DLCs in case DLC > 8.
 
@@ -287,19 +288,19 @@
         "BITRATE": "bitrate",
     }
 
     MAX_DATAGRAM_SIZE = 7
     HEADER = EmptyHeader()
     HEADER_SIZE = 0
 
-    def __init__(self, config=None):
+    def __init__(self, config=None, policy=None):
         """init for CAN transport
         :param config: configuration
         """
-        super().__init__(config)
+        super().__init__(config, policy)
         self.loadConfig(config)
         drivers = registered_drivers()
         interfaceName = self.config.get("CAN_DRIVER")
         if interfaceName not in drivers:
             raise ValueError("{} is an invalid driver name -- choose from {}".format(interfaceName, [x for x in drivers.keys()]))
         canInterfaceClass = drivers[interfaceName]
         self.canInterface = canInterfaceClass()
```

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/pc_canalystii.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/pc_canalystii.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/pc_etas.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/pc_etas.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/pc_gsusb.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/pc_gsusb.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/pc_iscan.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/pc_iscan.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/pc_ixxat.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/pc_ixxat.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/pc_kvaser.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/pc_kvaser.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/pc_neovi.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/pc_neovi.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/pc_nican.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/pc_nican.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/pc_nixnet.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/pc_nixnet.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/pc_pcan.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/pc_pcan.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/pc_seeed.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/pc_seeed.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/pc_serial.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/pc_serial.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/pc_slcan.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/pc_slcan.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/pc_socketcan.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/pc_socketcan.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/pc_systec.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/pc_systec.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/pc_usb2can.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/pc_usb2can.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/pc_vector.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/pc_vector.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/candriver/python_can.py` & `pyxcp-0.21.1/pyxcp/transport/candriver/python_can.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/cxx_ext/CMakeLists.txt` & `pyxcp-0.21.1/pyxcp/transport/cxx_ext/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/cxx_ext/setup.py` & `pyxcp-0.21.1/pyxcp/transport/cxx_ext/setup.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/cxx_ext/tests/test_basic_socket.cpp` & `pyxcp-0.21.1/pyxcp/transport/cxx_ext/tests/test_basic_socket.cpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/cxx_ext/tests/test_pool.cpp` & `pyxcp-0.21.1/pyxcp/transport/cxx_ext/tests/test_pool.cpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/cxx_ext/tests/test_timestamp.cpp` & `pyxcp-0.21.1/pyxcp/transport/cxx_ext/tests/test_timestamp.cpp`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/transport/eth.py` & `pyxcp-0.21.1/pyxcp/transport/eth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,54 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import selectors
 import socket
 import struct
 import threading
 from collections import deque
-from pyxcp.transport.base import BaseTransport
-from pyxcp.utils import SHORT_SLEEP
 from time import perf_counter
 from time import sleep
 from time import time
 
+from pyxcp.transport.base import BaseTransport
+from pyxcp.utils import SHORT_SLEEP
+
 DEFAULT_XCP_PORT = 5555
 RECV_SIZE = 8196
 
 
 class Eth(BaseTransport):
     """"""
 
     PARAMETER_MAP = {
         #                  Type    Req'd   Default
         "HOST": (str, False, "localhost"),
         "PORT": (int, False, 5555),
+        "BIND_TO_ADDRESS": (str, False, ""),
+        "BIND_TO_PORT": (int, False, 5555),
         "PROTOCOL": (str, False, "TCP"),
         "IPV6": (bool, False, False),
         "TCP_NODELAY": (bool, False, False),
     }
 
     MAX_DATAGRAM_SIZE = 512
     HEADER = struct.Struct("<HH")
     HEADER_SIZE = HEADER.size
 
-    def __init__(self, config=None):
-        super(Eth, self).__init__(config)
+    def __init__(self, config=None, policy=None):
+        super(Eth, self).__init__(config, policy)
         self.loadConfig(config)
         self.host = self.config.get("HOST")
         self.port = self.config.get("PORT")
         self.protocol = self.config.get("PROTOCOL")
         self.ipv6 = self.config.get("IPV6")
         self.use_tcp_no_delay = self.config.get("TCP_NODELAY")
-
+        address_to_bind = self.config.get("BIND_TO_ADDRESS")
+        port_to_bind = self.config.get("BIND_TO_PORT")
+        self._local_address = (address_to_bind, port_to_bind) if address_to_bind else None
         if self.ipv6 and not socket.has_ipv6:
             raise RuntimeError("IPv6 not supported by your platform.")
         else:
             address_family = socket.AF_INET6 if self.ipv6 else socket.AF_INET
         proto = socket.SOCK_STREAM if self.protocol == "TCP" else socket.SOCK_DGRAM
         if self.host.lower() == "localhost":
             self.host = "::1" if self.ipv6 else "localhost"
@@ -62,15 +67,19 @@
         self.use_tcp = self.protocol == "TCP"
         self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         if self.use_tcp and self.use_tcp_no_delay:
             self.sock.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
         if hasattr(socket, "SO_REUSEPORT"):
             self.sock.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEPORT, 1)
         self.sock.settimeout(0.5)
-
+        if self._local_address:
+            try:
+                self.sock.bind(self._local_address)
+            except BaseException as ex:
+                raise Exception(f"Failed to bind socket to given address {self._local_address}") from ex
         self._packet_listener = threading.Thread(
             target=self._packet_listen,
             args=(),
             kwargs={},
         )
         self._packets = deque()
```

### Comparing `pyxcp-0.20.4/pyxcp/transport/sxi.py` & `pyxcp-0.21.1/pyxcp/transport/sxi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
-import pyxcp.types as types
 import struct
-from pyxcp.transport.base import BaseTransport
 from time import perf_counter
 from time import time
 
 import serial
 
+import pyxcp.types as types
+from pyxcp.transport.base import BaseTransport
+
 
 class SxI(BaseTransport):
     """"""
 
     PARAMETER_MAP = {
         #                        Type    Req'd   Default
         "PORT": (str, False, "COM1"),
@@ -22,16 +23,16 @@
     }
 
     MAX_DATAGRAM_SIZE = 512
     TIMEOUT = 0.75
     HEADER = struct.Struct("<HH")
     HEADER_SIZE = HEADER.size
 
-    def __init__(self, config=None):
-        super(SxI, self).__init__(config)
+    def __init__(self, config=None, policy=None):
+        super(SxI, self).__init__(config, policy)
         self.loadConfig(config)
         self.portName = self.config.get("PORT")
         self.baudrate = self.config.get("BITRATE")
 
     def __del__(self):
         self.closeConnection()
```

### Comparing `pyxcp-0.20.4/pyxcp/transport/usb_transport.py` & `pyxcp-0.21.1/pyxcp/transport/usb_transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 import struct
 import threading
 from array import array
 from collections import deque
-from pyxcp.transport.base import BaseTransport
-from pyxcp.utils import SHORT_SLEEP
 from time import perf_counter
 from time import sleep
 from time import time
 
 import usb.core
 import usb.util
 
+from pyxcp.transport.base import BaseTransport
+from pyxcp.utils import SHORT_SLEEP
+
 RECV_SIZE = 16384
 
 
 class Usb(BaseTransport):
     """"""
 
     PARAMETER_MAP = {
@@ -28,16 +29,16 @@
         "reply_endpoint_number": (int, True, 1),
         "vendor_id": (int, False, 0),
         "product_id": (int, False, 0),
     }
     HEADER = struct.Struct("<2H")
     HEADER_SIZE = HEADER.size
 
-    def __init__(self, config=None):
-        super(Usb, self).__init__(config)
+    def __init__(self, config=None, policy=None):
+        super(Usb, self).__init__(config, policy)
         self.loadConfig(config)
         self.serial_number = self.config.get("serial_number").strip()
         self.vendor_id = self.config.get("vendor_id")
         self.product_id = self.config.get("product_id")
         self.configuration_number = self.config.get("configuration_number")
         self.interface_number = self.config.get("interface_number")
         self.command_endpoint_number = self.config.get("command_endpoint_number")
```

### Comparing `pyxcp-0.20.4/pyxcp/types.py` & `pyxcp-0.21.1/pyxcp/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -896,7 +896,20 @@
     "DAQ_TIMESTAMP_UNIT_1S": 0,
 }
 
 
 class XcpGetSeedMode(enum.IntEnum):
     FIRST_PART = 0
     REMAINING = 1
+
+
+class FrameCategory(enum.IntEnum):
+    """XCP frame categories."""
+
+    METADATA = 0
+    CMD = 1
+    RESPONSE = 2
+    ERROR = 3
+    EVENT = 4
+    SERV = 5
+    DAQ = 6
+    STIM = 7
```

### Comparing `pyxcp-0.20.4/pyxcp/utils.py` & `pyxcp-0.21.1/pyxcp/utils.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/pyxcp/vector/map.py` & `pyxcp-0.21.1/pyxcp/vector/map.py`

 * *Files identical despite different names*

### Comparing `pyxcp-0.20.4/PKG-INFO` & `pyxcp-0.21.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyxcp
-Version: 0.20.4
+Version: 0.21.1
 Summary: Universal Calibration Protocol for Python
 Keywords: automotive,ecu,xcp,asam,autosar
 Author: Christoph Schueler
 Author-email: cpu12.gems@googlemail.com
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

