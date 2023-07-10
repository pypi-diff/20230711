# Comparing `tmp/bus_station-6.1.2.tar.gz` & `tmp/bus_station-6.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bus_station-6.1.2.tar", max compression
+gzip compressed data, was "bus_station-6.1.3.tar", max compression
```

## Comparing `bus_station-6.1.2.tar` & `bus_station-6.1.3.tar`

### file list

```diff
@@ -1,162 +1,162 @@
--rw-r--r--   0        0        0       48 2023-07-07 08:30:00.373248 bus_station-6.1.2/README.md
--rw-r--r--   0        0        0      985 2023-07-07 08:31:33.988417 bus_station-6.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/__init__.py
--rw-r--r--   0        0        0      143 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/bus_stop.py
--rw-r--r--   0        0        0      185 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/bus_stop_not_found.py
--rw-r--r--   0        0        0      692 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/environment.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/address/__init__.py
--rw-r--r--   0        0        0      199 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/address/address_not_found_for_bus_stop.py
--rw-r--r--   0        0        0      407 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/address/bus_stop_address_registry.py
--rw-r--r--   0        0        0      673 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/address/redis_bus_stop_address_registry.py
--rw-r--r--   0        0        0     3774 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/bus_stop_registry.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/supervisor/__init__.py
--rw-r--r--   0        0        0     1180 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/supervisor/bus_stop_address_registration_supervisor.py
--rw-r--r--   0        0        0      255 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/supervisor/bus_stop_registration_supervisor.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/resolvers/__init__.py
--rw-r--r--   0        0        0      250 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/resolvers/bus_stop_resolver.py
--rw-r--r--   0        0        0      587 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/resolvers/in_memory_bus_stop_resolver.py
--rw-r--r--   0        0        0      772 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/resolvers/pypendency_bus_stop_resolver.py
--rw-r--r--   0        0        0     1107 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/resolvers/yandil_bus_stop_resolver.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/asynchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/asynchronous/distributed/__init__.py
--rw-r--r--   0        0        0     1352 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py
--rw-r--r--   0        0        0      889 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py
--rw-r--r--   0        0        0     1237 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py
--rw-r--r--   0        0        0      258 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/command_bus.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/synchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/synchronous/distributed/__init__.py
--rw-r--r--   0        0        0     2315 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py
--rw-r--r--   0        0        0     2188 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py
--rw-r--r--   0        0        0     1128 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/__init__.py
--rw-r--r--   0        0        0     1326 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py
--rw-r--r--   0        0        0     2747 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py
--rw-r--r--   0        0        0     1856 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py
--rw-r--r--   0        0        0     1266 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py
--rw-r--r--   0        0        0      253 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/command.py
--rw-r--r--   0        0        0      292 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/command_execution_failed.py
--rw-r--r--   0        0        0      457 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/command_handler.py
--rw-r--r--   0        0        0      227 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/command_handler_not_found.py
--rw-r--r--   0        0        0     1795 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/command_handler_registry.py
--rw-r--r--   0        0        0      233 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/handler_not_found_for_command.py
--rw-r--r--   0        0        0      725 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/json_rpc_command_server.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/middleware/__init__.py
--rw-r--r--   0        0        0      607 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/middleware/command_middleware.py
--rw-r--r--   0        0        0     1078 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/middleware/command_middleware_receiver.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/middleware/implementations/__init__.py
--rw-r--r--   0        0        0     1070 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py
--rw-r--r--   0        0        0     1039 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py
--rw-r--r--   0        0        0      890 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py
--rw-r--r--   0        0        0      712 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/rpyc_command_server.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/asynchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/asynchronous/distributed/__init__.py
--rw-r--r--   0        0        0     1247 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py
--rw-r--r--   0        0        0     1212 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py
--rw-r--r--   0        0        0      984 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py
--rw-r--r--   0        0        0      246 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/event_bus.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/synchronous/__init__.py
--rw-r--r--   0        0        0      872 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus_engine/__init__.py
--rw-r--r--   0        0        0     3196 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py
--rw-r--r--   0        0        0     1625 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py
--rw-r--r--   0        0        0      249 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/event.py
--rw-r--r--   0        0        0      446 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/event_consumer.py
--rw-r--r--   0        0        0      221 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/event_consumer_not_found.py
--rw-r--r--   0        0        0     1439 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/event_consumer_registry.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/middleware/__init__.py
--rw-r--r--   0        0        0      590 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/middleware/event_middleware.py
--rw-r--r--   0        0        0     1049 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/middleware/event_middleware_receiver.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/middleware/implementations/__init__.py
--rw-r--r--   0        0        0     1038 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py
--rw-r--r--   0        0        0     1012 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py
--rw-r--r--   0        0        0      864 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/__init__.py
--rw-r--r--   0        0        0     1440 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/memory_queue_passenger_worker.py
--rw-r--r--   0        0        0     2319 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/passenger.py
--rw-r--r--   0        0        0     2042 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/passenger_kombu_consumer.py
--rw-r--r--   0        0        0     2294 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/passenger_mapper.py
--rw-r--r--   0        0        0       76 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/passenger_middleware.py
--rw-r--r--   0        0        0      637 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/passenger_registry.py
--rw-r--r--   0        0        0      641 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/passenger_resolvers.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/reception/__init__.py
--rw-r--r--   0        0        0     1386 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/reception/passenger_middleware_receiver.py
--rw-r--r--   0        0        0      792 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/reception/passenger_receiver.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/serialization/__init__.py
--rw-r--r--   0        0        0      347 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/serialization/passenger_deserialization_error.py
--rw-r--r--   0        0        0      321 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/serialization/passenger_deserializer.py
--rw-r--r--   0        0        0     1016 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/serialization/passenger_json_deserializer.py
--rw-r--r--   0        0        0      822 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/serialization/passenger_json_serializer.py
--rw-r--r--   0        0        0      241 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/serialization/passenger_serializer.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus/__init__.py
--rw-r--r--   0        0        0      323 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus/query_bus.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus/synchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus/synchronous/distributed/__init__.py
--rw-r--r--   0        0        0     2671 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py
--rw-r--r--   0        0        0     2580 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py
--rw-r--r--   0        0        0     1127 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus_engine/__init__.py
--rw-r--r--   0        0        0     1242 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py
--rw-r--r--   0        0        0     1218 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py
--rw-r--r--   0        0        0      219 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/handler_not_found_for_query.py
--rw-r--r--   0        0        0     1483 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/json_rpc_query_server.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/middleware/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/middleware/implementations/__init__.py
--rw-r--r--   0        0        0     1261 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py
--rw-r--r--   0        0        0     1178 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py
--rw-r--r--   0        0        0     1227 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py
--rw-r--r--   0        0        0      726 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/middleware/query_middleware.py
--rw-r--r--   0        0        0     1286 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/middleware/query_middleware_receiver.py
--rw-r--r--   0        0        0      249 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/query.py
--rw-r--r--   0        0        0      273 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/query_execution_failed.py
--rw-r--r--   0        0        0      520 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/query_handler.py
--rw-r--r--   0        0        0      215 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/query_handler_not_found.py
--rw-r--r--   0        0        0     1747 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/query_handler_registry.py
--rw-r--r--   0        0        0      138 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/query_response.py
--rw-r--r--   0        0        0     1442 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/rpyc_query_server.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/serialization/__init__.py
--rw-r--r--   0        0        0      282 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/serialization/query_response_deserializer.py
--rw-r--r--   0        0        0      465 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/serialization/query_response_json_deserializer.py
--rw-r--r--   0        0        0      390 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/serialization/query_response_json_serializer.py
--rw-r--r--   0        0        0      267 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/serialization/query_response_serializer.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/broker_connection/__init__.py
--rw-r--r--   0        0        0      352 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/broker_connection/broker_connection_type.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/broker_connection/connection_parameters/__init__.py
--rw-r--r--   0        0        0      176 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/broker_connection/connection_parameters/connection_parameters.py
--rw-r--r--   0        0        0     1249 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py
--rw-r--r--   0        0        0      695 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/bus.py
--rw-r--r--   0        0        0      438 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/context.py
--rw-r--r--   0        0        0      118 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/dataclass_type.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/engine/__init__.py
--rw-r--r--   0        0        0      181 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/engine/engine.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/engine/runner/__init__.py
--rw-r--r--   0        0        0      436 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/engine/runner/engine_runner.py
--rw-r--r--   0        0        0      805 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py
--rw-r--r--   0        0        0      241 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/engine/runner/self_process_engine_runner.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/factories/__init__.py
--rw-r--r--   0        0        0      381 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/factories/kombu_connection_factory.py
--rw-r--r--   0        0        0      545 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/factories/memory_queue_factory.py
--rw-r--r--   0        0        0      305 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/fqn.py
--rw-r--r--   0        0        0     2493 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/json_rpc_server.py
--rw-r--r--   0        0        0      956 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/kafka_topic_creator.py
--rw-r--r--   0        0        0     2037 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/rpyc_server.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/models/__init__.py
--rw-r--r--   0        0        0      185 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/models/command_tracking.py
--rw-r--r--   0        0        0      183 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/models/event_tracking.py
--rw-r--r--   0        0        0      950 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py
--rw-r--r--   0        0        0      347 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/models/passenger_tracking.py
--rw-r--r--   0        0        0      744 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py
--rw-r--r--   0        0        0      297 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/models/passenger_tracking_serializer.py
--rw-r--r--   0        0        0      281 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/models/query_tracking.py
--rw-r--r--   0        0        0        0 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/trackers/__init__.py
--rw-r--r--   0        0        0     1400 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py
--rw-r--r--   0        0        0     2483 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/trackers/passenger_tracker.py
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 bus_station-6.1.2/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-07-10 22:28:28.364446 bus_station-6.1.3/README.md
+-rw-r--r--   0        0        0      985 2023-07-10 22:30:19.186889 bus_station-6.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/__init__.py
+-rw-r--r--   0        0        0      143 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/bus_stop.py
+-rw-r--r--   0        0        0      185 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/bus_stop_not_found.py
+-rw-r--r--   0        0        0      690 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/environment.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/address/__init__.py
+-rw-r--r--   0        0        0      199 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/address/address_not_found_for_bus_stop.py
+-rw-r--r--   0        0        0      407 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/address/bus_stop_address_registry.py
+-rw-r--r--   0        0        0      673 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/address/redis_bus_stop_address_registry.py
+-rw-r--r--   0        0        0     3774 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/bus_stop_registry.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/supervisor/__init__.py
+-rw-r--r--   0        0        0     1180 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/supervisor/bus_stop_address_registration_supervisor.py
+-rw-r--r--   0        0        0      255 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/registration/supervisor/bus_stop_registration_supervisor.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/resolvers/__init__.py
+-rw-r--r--   0        0        0      250 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/resolvers/bus_stop_resolver.py
+-rw-r--r--   0        0        0      587 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/resolvers/in_memory_bus_stop_resolver.py
+-rw-r--r--   0        0        0      772 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/resolvers/pypendency_bus_stop_resolver.py
+-rw-r--r--   0        0        0     1107 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/bus_stop/resolvers/yandil_bus_stop_resolver.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/asynchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/asynchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     1352 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py
+-rw-r--r--   0        0        0      889 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py
+-rw-r--r--   0        0        0     1237 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py
+-rw-r--r--   0        0        0      258 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/command_bus.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/synchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/synchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     2315 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py
+-rw-r--r--   0        0        0     2188 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py
+-rw-r--r--   0        0        0     1128 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/__init__.py
+-rw-r--r--   0        0        0     1326 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py
+-rw-r--r--   0        0        0     2747 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py
+-rw-r--r--   0        0        0     1856 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py
+-rw-r--r--   0        0        0     1266 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py
+-rw-r--r--   0        0        0      253 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/command.py
+-rw-r--r--   0        0        0      292 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/command_execution_failed.py
+-rw-r--r--   0        0        0      457 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/command_handler.py
+-rw-r--r--   0        0        0      227 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/command_handler_not_found.py
+-rw-r--r--   0        0        0     1795 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/command_handler_registry.py
+-rw-r--r--   0        0        0      233 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/handler_not_found_for_command.py
+-rw-r--r--   0        0        0      725 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/json_rpc_command_server.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/middleware/__init__.py
+-rw-r--r--   0        0        0      607 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/middleware/command_middleware.py
+-rw-r--r--   0        0        0     1078 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/middleware/command_middleware_receiver.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/middleware/implementations/__init__.py
+-rw-r--r--   0        0        0     1070 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py
+-rw-r--r--   0        0        0     1039 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py
+-rw-r--r--   0        0        0      890 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py
+-rw-r--r--   0        0        0      712 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/command_terminal/rpyc_command_server.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/asynchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/asynchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     1247 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py
+-rw-r--r--   0        0        0     1212 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py
+-rw-r--r--   0        0        0      984 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py
+-rw-r--r--   0        0        0      246 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/event_bus.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/synchronous/__init__.py
+-rw-r--r--   0        0        0      872 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus_engine/__init__.py
+-rw-r--r--   0        0        0     3196 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py
+-rw-r--r--   0        0        0     1625 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py
+-rw-r--r--   0        0        0      249 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/event.py
+-rw-r--r--   0        0        0      446 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/event_consumer.py
+-rw-r--r--   0        0        0      221 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/event_consumer_not_found.py
+-rw-r--r--   0        0        0     1439 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/event_consumer_registry.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/middleware/__init__.py
+-rw-r--r--   0        0        0      590 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/middleware/event_middleware.py
+-rw-r--r--   0        0        0     1049 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/middleware/event_middleware_receiver.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/middleware/implementations/__init__.py
+-rw-r--r--   0        0        0     1038 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py
+-rw-r--r--   0        0        0     1012 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py
+-rw-r--r--   0        0        0      864 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/__init__.py
+-rw-r--r--   0        0        0     1440 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/memory_queue_passenger_worker.py
+-rw-r--r--   0        0        0     2319 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/passenger.py
+-rw-r--r--   0        0        0     2042 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/passenger_kombu_consumer.py
+-rw-r--r--   0        0        0     2294 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/passenger_mapper.py
+-rw-r--r--   0        0        0       76 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/passenger_middleware.py
+-rw-r--r--   0        0        0      637 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/passenger_registry.py
+-rw-r--r--   0        0        0      641 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/passenger_resolvers.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/reception/__init__.py
+-rw-r--r--   0        0        0     1386 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/reception/passenger_middleware_receiver.py
+-rw-r--r--   0        0        0      792 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/reception/passenger_receiver.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/serialization/__init__.py
+-rw-r--r--   0        0        0      347 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/serialization/passenger_deserialization_error.py
+-rw-r--r--   0        0        0      321 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/serialization/passenger_deserializer.py
+-rw-r--r--   0        0        0     1016 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/serialization/passenger_json_deserializer.py
+-rw-r--r--   0        0        0      822 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/serialization/passenger_json_serializer.py
+-rw-r--r--   0        0        0      241 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/passengers/serialization/passenger_serializer.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/query_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/query_terminal/bus/__init__.py
+-rw-r--r--   0        0        0      323 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/query_terminal/bus/query_bus.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/query_terminal/bus/synchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.368446 bus_station-6.1.3/src/bus_station/query_terminal/bus/synchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     2671 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py
+-rw-r--r--   0        0        0     2580 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py
+-rw-r--r--   0        0        0     1127 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/bus_engine/__init__.py
+-rw-r--r--   0        0        0     1242 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py
+-rw-r--r--   0        0        0     1218 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py
+-rw-r--r--   0        0        0      219 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/handler_not_found_for_query.py
+-rw-r--r--   0        0        0     1483 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/json_rpc_query_server.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/middleware/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/middleware/implementations/__init__.py
+-rw-r--r--   0        0        0     1261 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py
+-rw-r--r--   0        0        0     1178 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py
+-rw-r--r--   0        0        0     1227 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py
+-rw-r--r--   0        0        0      726 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/middleware/query_middleware.py
+-rw-r--r--   0        0        0     1286 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/middleware/query_middleware_receiver.py
+-rw-r--r--   0        0        0      249 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/query.py
+-rw-r--r--   0        0        0      273 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/query_execution_failed.py
+-rw-r--r--   0        0        0      520 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/query_handler.py
+-rw-r--r--   0        0        0      215 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/query_handler_not_found.py
+-rw-r--r--   0        0        0     1747 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/query_handler_registry.py
+-rw-r--r--   0        0        0      138 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/query_response.py
+-rw-r--r--   0        0        0     1442 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/rpyc_query_server.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/serialization/__init__.py
+-rw-r--r--   0        0        0      282 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/serialization/query_response_deserializer.py
+-rw-r--r--   0        0        0      465 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/serialization/query_response_json_deserializer.py
+-rw-r--r--   0        0        0      390 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/serialization/query_response_json_serializer.py
+-rw-r--r--   0        0        0      267 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/query_terminal/serialization/query_response_serializer.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/broker_connection/__init__.py
+-rw-r--r--   0        0        0      352 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/broker_connection/broker_connection_type.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/broker_connection/connection_parameters/__init__.py
+-rw-r--r--   0        0        0      176 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/broker_connection/connection_parameters/connection_parameters.py
+-rw-r--r--   0        0        0     1249 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py
+-rw-r--r--   0        0        0      695 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/bus.py
+-rw-r--r--   0        0        0      438 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/context.py
+-rw-r--r--   0        0        0      118 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/dataclass_type.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/engine/__init__.py
+-rw-r--r--   0        0        0      181 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/engine/engine.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/engine/runner/__init__.py
+-rw-r--r--   0        0        0      436 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/engine/runner/engine_runner.py
+-rw-r--r--   0        0        0      805 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py
+-rw-r--r--   0        0        0      241 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/engine/runner/self_process_engine_runner.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/factories/__init__.py
+-rw-r--r--   0        0        0      381 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/factories/kombu_connection_factory.py
+-rw-r--r--   0        0        0      545 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/factories/memory_queue_factory.py
+-rw-r--r--   0        0        0      305 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/fqn.py
+-rw-r--r--   0        0        0     2493 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/json_rpc_server.py
+-rw-r--r--   0        0        0      956 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/kafka_topic_creator.py
+-rw-r--r--   0        0        0     2037 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/shared_terminal/rpyc_server.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/models/__init__.py
+-rw-r--r--   0        0        0      185 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/models/command_tracking.py
+-rw-r--r--   0        0        0      183 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/models/event_tracking.py
+-rw-r--r--   0        0        0      950 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py
+-rw-r--r--   0        0        0      347 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/models/passenger_tracking.py
+-rw-r--r--   0        0        0      744 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py
+-rw-r--r--   0        0        0      297 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/models/passenger_tracking_serializer.py
+-rw-r--r--   0        0        0      281 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/models/query_tracking.py
+-rw-r--r--   0        0        0        0 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/trackers/__init__.py
+-rw-r--r--   0        0        0     1400 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py
+-rw-r--r--   0        0        0     2483 2023-07-10 22:28:28.372446 bus_station-6.1.3/src/bus_station/tracking_terminal/trackers/passenger_tracker.py
+-rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 bus_station-6.1.3/PKG-INFO
```

### Comparing `bus_station-6.1.2/pyproject.toml` & `bus_station-6.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bus-station"
-version = "6.1.2"
+version = "6.1.3"
 description = "A python bus station"
 readme = "README.md"
 authors = ["DeejayRevok <seryi_one@hotmail.com>"]
 
 [tool.poetry.dependencies]
 python = "~=3.10.0"
 kombu = "5.2.2"
@@ -41,15 +41,15 @@
 [tool.isort]
 profile = "black"
 py_version=310
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "6.1.2"
+version = "6.1.3"
 tag_format = "$version"
 version_files = [
   "pyproject.toml:version"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `bus_station-6.1.2/src/bus_station/bus_stop/environment.py` & `bus_station-6.1.3/src/bus_station/bus_stop/environment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from os import environ
 from re import sub
 from typing import Optional
 
 __SEPARATOR = "_"
 __BUS_STOP_ADDRESS_ENV_VARIABLE_NAME_PATTERN = f"BUS_STATION{__SEPARATOR}{{formatted_bus_stop_id}}{__SEPARATOR}ADDRESS"
-__SYMBOLS_REGEX = r"[^a-zA-Z0-9 \n\.]"
+__SYMBOLS_REGEX = r"[^a-zA-Z0-9 \n]"
 
 
 def get_bus_stop_address_from_environment(bus_stop_id: str) -> Optional[str]:
     bus_stop_env_var = get_bus_stop_address_env_variable(bus_stop_id)
     return environ.get(bus_stop_env_var)
```

### Comparing `bus_station-6.1.2/src/bus_station/bus_stop/registration/address/redis_bus_stop_address_registry.py` & `bus_station-6.1.3/src/bus_station/bus_stop/registration/address/redis_bus_stop_address_registry.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/bus_stop/registration/bus_stop_registry.py` & `bus_station-6.1.3/src/bus_station/bus_stop/registration/bus_stop_registry.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/bus_stop/registration/supervisor/bus_stop_address_registration_supervisor.py` & `bus_station-6.1.3/src/bus_station/bus_stop/registration/supervisor/bus_stop_address_registration_supervisor.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/bus_stop/resolvers/in_memory_bus_stop_resolver.py` & `bus_station-6.1.3/src/bus_station/bus_stop/resolvers/in_memory_bus_stop_resolver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/bus_stop/resolvers/pypendency_bus_stop_resolver.py` & `bus_station-6.1.3/src/bus_station/bus_stop/resolvers/pypendency_bus_stop_resolver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/bus_stop/resolvers/yandil_bus_stop_resolver.py` & `bus_station-6.1.3/src/bus_station/bus_stop/resolvers/yandil_bus_stop_resolver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py` & `bus_station-6.1.3/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py` & `bus_station-6.1.3/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py` & `bus_station-6.1.3/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py` & `bus_station-6.1.3/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py` & `bus_station-6.1.3/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py` & `bus_station-6.1.3/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py` & `bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py` & `bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py` & `bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py` & `bus_station-6.1.3/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/command_handler_registry.py` & `bus_station-6.1.3/src/bus_station/command_terminal/command_handler_registry.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/json_rpc_command_server.py` & `bus_station-6.1.3/src/bus_station/command_terminal/json_rpc_command_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/middleware/command_middleware.py` & `bus_station-6.1.3/src/bus_station/command_terminal/middleware/command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/middleware/command_middleware_receiver.py` & `bus_station-6.1.3/src/bus_station/command_terminal/middleware/command_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py` & `bus_station-6.1.3/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py` & `bus_station-6.1.3/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py` & `bus_station-6.1.3/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/command_terminal/rpyc_command_server.py` & `bus_station-6.1.3/src/bus_station/command_terminal/rpyc_command_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py` & `bus_station-6.1.3/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py` & `bus_station-6.1.3/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py` & `bus_station-6.1.3/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py` & `bus_station-6.1.3/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py` & `bus_station-6.1.3/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py` & `bus_station-6.1.3/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/event_terminal/event_consumer_registry.py` & `bus_station-6.1.3/src/bus_station/event_terminal/event_consumer_registry.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/event_terminal/middleware/event_middleware.py` & `bus_station-6.1.3/src/bus_station/event_terminal/middleware/event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/event_terminal/middleware/event_middleware_receiver.py` & `bus_station-6.1.3/src/bus_station/event_terminal/middleware/event_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py` & `bus_station-6.1.3/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py` & `bus_station-6.1.3/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py` & `bus_station-6.1.3/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/passengers/memory_queue_passenger_worker.py` & `bus_station-6.1.3/src/bus_station/passengers/memory_queue_passenger_worker.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/passengers/passenger.py` & `bus_station-6.1.3/src/bus_station/passengers/passenger.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/passengers/passenger_kombu_consumer.py` & `bus_station-6.1.3/src/bus_station/passengers/passenger_kombu_consumer.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/passengers/passenger_mapper.py` & `bus_station-6.1.3/src/bus_station/passengers/passenger_mapper.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/passengers/passenger_registry.py` & `bus_station-6.1.3/src/bus_station/passengers/passenger_registry.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/passengers/passenger_resolvers.py` & `bus_station-6.1.3/src/bus_station/passengers/passenger_resolvers.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/passengers/reception/passenger_middleware_receiver.py` & `bus_station-6.1.3/src/bus_station/passengers/reception/passenger_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/passengers/reception/passenger_receiver.py` & `bus_station-6.1.3/src/bus_station/passengers/reception/passenger_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/passengers/serialization/passenger_json_deserializer.py` & `bus_station-6.1.3/src/bus_station/passengers/serialization/passenger_json_deserializer.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/passengers/serialization/passenger_json_serializer.py` & `bus_station-6.1.3/src/bus_station/passengers/serialization/passenger_json_serializer.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py` & `bus_station-6.1.3/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py` & `bus_station-6.1.3/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py` & `bus_station-6.1.3/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py` & `bus_station-6.1.3/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py` & `bus_station-6.1.3/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/query_terminal/json_rpc_query_server.py` & `bus_station-6.1.3/src/bus_station/query_terminal/json_rpc_query_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py` & `bus_station-6.1.3/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py` & `bus_station-6.1.3/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py` & `bus_station-6.1.3/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/query_terminal/middleware/query_middleware.py` & `bus_station-6.1.3/src/bus_station/query_terminal/middleware/query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/query_terminal/middleware/query_middleware_receiver.py` & `bus_station-6.1.3/src/bus_station/query_terminal/middleware/query_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/query_terminal/query_handler.py` & `bus_station-6.1.3/src/bus_station/query_terminal/query_handler.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/query_terminal/query_handler_registry.py` & `bus_station-6.1.3/src/bus_station/query_terminal/query_handler_registry.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/query_terminal/rpyc_query_server.py` & `bus_station-6.1.3/src/bus_station/query_terminal/rpyc_query_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py` & `bus_station-6.1.3/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/shared_terminal/bus.py` & `bus_station-6.1.3/src/bus_station/shared_terminal/bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py` & `bus_station-6.1.3/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/shared_terminal/factories/memory_queue_factory.py` & `bus_station-6.1.3/src/bus_station/shared_terminal/factories/memory_queue_factory.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/shared_terminal/json_rpc_server.py` & `bus_station-6.1.3/src/bus_station/shared_terminal/json_rpc_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/shared_terminal/kafka_topic_creator.py` & `bus_station-6.1.3/src/bus_station/shared_terminal/kafka_topic_creator.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/shared_terminal/rpyc_server.py` & `bus_station-6.1.3/src/bus_station/shared_terminal/rpyc_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py` & `bus_station-6.1.3/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py` & `bus_station-6.1.3/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py` & `bus_station-6.1.3/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/src/bus_station/tracking_terminal/trackers/passenger_tracker.py` & `bus_station-6.1.3/src/bus_station/tracking_terminal/trackers/passenger_tracker.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.2/PKG-INFO` & `bus_station-6.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus-station
-Version: 6.1.2
+Version: 6.1.3
 Summary: A python bus station
 Author: DeejayRevok
 Author-email: seryi_one@hotmail.com
 Requires-Python: >=3.10.0,<3.11.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: confluent-kafka (>=2.1.1,<3.0.0)
```

