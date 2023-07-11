# Comparing `tmp/openworld-sdk-python-fraudpreventionv2-1.1.0.tar.gz` & `tmp/openworld-sdk-python-fraudpreventionv2-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openworld-sdk-python-fraudpreventionv2-1.1.0.tar", last modified: Tue Jul  4 14:18:44 2023, max compression
+gzip compressed data, was "openworld-sdk-python-fraudpreventionv2-1.2.0.tar", last modified: Tue Jul 11 14:09:49 2023, max compression
```

## Comparing `openworld-sdk-python-fraudpreventionv2-1.1.0.tar` & `openworld-sdk-python-fraudpreventionv2-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:18:44.371976 openworld-sdk-python-fraudpreventionv2-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-04 14:18:44.371976 openworld-sdk-python-fraudpreventionv2-1.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:18:44.367976 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:18:44.367976 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/sdk/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:18:44.367976 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/sdk/fraudpreventionv2/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-04 14:18:35.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/sdk/fraudpreventionv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-07-04 14:18:35.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/sdk/fraudpreventionv2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    89421 2023-07-04 14:18:35.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/sdk/fraudpreventionv2/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-04 14:18:44.371976 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld_sdk_python_fraudpreventionv2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-04 14:18:44.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-04 14:18:44.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld_sdk_python_fraudpreventionv2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-04 14:18:44.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld_sdk_python_fraudpreventionv2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-04 14:18:44.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld_sdk_python_fraudpreventionv2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-04 14:18:44.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/openworld_sdk_python_fraudpreventionv2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-04 14:18:44.371976 openworld-sdk-python-fraudpreventionv2-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-04 14:18:20.000000 openworld-sdk-python-fraudpreventionv2-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:09:49.596207 openworld-sdk-python-fraudpreventionv2-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-11 14:09:49.596207 openworld-sdk-python-fraudpreventionv2-1.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:09:49.596207 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:09:49.596207 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/sdk/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:09:49.596207 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/sdk/fraudpreventionv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-11 14:09:42.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/sdk/fraudpreventionv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5410 2023-07-11 14:09:42.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/sdk/fraudpreventionv2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99892 2023-07-11 14:09:42.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/sdk/fraudpreventionv2/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 14:09:49.596207 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld_sdk_python_fraudpreventionv2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-11 14:09:49.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-07-11 14:09:49.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld_sdk_python_fraudpreventionv2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 14:09:49.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld_sdk_python_fraudpreventionv2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-11 14:09:49.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld_sdk_python_fraudpreventionv2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-11 14:09:49.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/openworld_sdk_python_fraudpreventionv2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 14:09:49.596207 openworld-sdk-python-fraudpreventionv2-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-07-11 14:09:31.000000 openworld-sdk-python-fraudpreventionv2-1.2.0/setup.py
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.1.0/PKG-INFO` & `openworld-sdk-python-fraudpreventionv2-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openworld-sdk-python-fraudpreventionv2
-Version: 1.1.0
+Version: 1.2.0
 Summary: Open World fraudPreventionV2 SDK for Python
 Home-page: https://github.com/ExpediaGroup/openworld-sdk-python
 Author: Expedia Group
 Author-email: oss@expediagroup.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/sdk/fraudpreventionv2/__init__.py` & `openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/sdk/fraudpreventionv2/__init__.py`

 * *Files identical despite different names*

### Comparing `openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/sdk/fraudpreventionv2/client.py` & `openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/sdk/fraudpreventionv2/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         r"""fraudPreventionV2 API Client.
 
         Args:
             client_config(ClientConfig): SDK Client Configurations Holder.
         """
         python_version = platform.python_version()
         os_name, os_version, *_ = platform.platform().split('-')
-        sdk_metadata = f'open-world-sdk-python-fraudpreventionv2/1.1.0'
+        sdk_metadata = f'open-world-sdk-python-fraudpreventionv2/1.2.0'
 
         self.__api_client = ApiClient(client_config, _OpenWorldAuthClient)
 
         self.__user_agent = f'{sdk_metadata} (Python {python_version}; {os_name} {os_version})'
 
     def screen(
         self, transaction_id: UUID = uuid4(), body: OrderPurchaseScreenRequest = None
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.1.0/openworld/sdk/fraudpreventionv2/model.py` & `openworld-sdk-python-fraudpreventionv2-1.2.0/openworld/sdk/fraudpreventionv2/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -559,14 +559,126 @@
     Attributes:
         __root__(constr(max_length=50)): --
 
     """
     __root__: constr(max_length=50) = None
 
 
+class RouteType(
+    Enum,
+):
+    r"""pydantic model RouteType: The type of route or itinerary for the Rail product, indicating the travel arrangement and pattern. Possible values are:
+    - `MULTIPLE_DESTINATIONS` - The Rail product includes multiple destinations in its itinerary.
+    - `ONE_WAY` - The Rail product represents a one-way journey.
+    - `ROUNDTRIP` - The Rail product represents a roundtrip journey.
+
+    Attributes:
+        MULTIPLE_DESTINATIONS(Any): --
+        ONE_WAY(Any): --
+        ROUND_TRIP(Any): --
+
+    """
+    MULTIPLE_DESTINATIONS: Any = 'MULTIPLE_DESTINATIONS'
+    ONE_WAY: Any = 'ONE_WAY'
+    ROUND_TRIP: Any = 'ROUND_TRIP'
+
+
+class TransportationMethod(
+    Enum,
+):
+    r"""pydantic model TransportationMethod: This attribute represents the specific transportation method by which the passenger is traveling. It captures the mode of transportation used during the Rail product journey, Possible values are:
+        - `BUS` - The Rail product includes bus transportation for certain segments of the itinerary.
+        - `FERRY` - The Rail product involves ferry transportation as part of the journey.
+        - `PUBLIC_TRANSPORT` - The Rail product represents the use of public transportation modes for the journey.
+        - `TRAM` - The Rail product includes tram transportation as part of the journey.
+        - `RAIL` - The Rail product specifically utilizes train transportation for the journey.
+        - `TRANSFER` - The Rail product involves transfers between different modes of transportation.
+        - `OTHER` - The Rail product utilizes transportation methods not covered by the aforementioned categories.
+
+    Attributes:
+        BUS(Any): --
+        FERRY(Any): --
+        PUBLIC_TRANSPORT(Any): --
+        RAIL(Any): --
+        TRAM(Any): --
+        TRANSFER(Any): --
+        OTHERS(Any): --
+
+    """
+    BUS: Any = 'BUS'
+    FERRY: Any = 'FERRY'
+    PUBLIC_TRANSPORT: Any = 'PUBLIC_TRANSPORT'
+    RAIL: Any = 'RAIL'
+    TRAM: Any = 'TRAM'
+    TRANSFER: Any = 'TRANSFER'
+    OTHERS: Any = 'OTHERS'
+
+
+class OperatingCompany(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model OperatingCompany: This attribute captures the name or identifier of the company responsible for operating the Rail product. It represents the specific operating entity, such as Amtrak, British Railways, or a bus company.
+    Attributes:
+        marketing_name(Optional[constr(max_length=200)], optional): The name used by the transportation carrier for marketing purposes in the travel segment. Example: ARX, AMTRAC, ARRIVA
+
+    """
+    marketing_name: Optional[constr(max_length=200)] = None
+    """
+    The name used by the transportation carrier for marketing purposes in the travel segment. Example: ARX, AMTRAC, ARRIVA
+    """
+
+
+class Type(
+    Enum,
+):
+    r"""pydantic model Type: This attribute provides information about the specific classification assigned to the rail station. It helps differentiate between different types of stations, such as major stations (STATION) or stations located within a city (city).
+    Attributes:
+        STATION(Any): --
+        CITY(Any): --
+
+    """
+    STATION: Any = 'STATION'
+    CITY: Any = 'CITY'
+
+
+class RailwayStationDetails(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model RailwayStationDetails
+    Attributes:
+        name(constr(max_length=200)): The popularly known name or title by which the railway station is identified.
+        type(Optional[Type], optional): This attribute provides information about the specific classification assigned to the rail station. It helps differentiate between different types of stations, such as major stations (STATION) or stations located within a city (city).
+        station_code(constr(max_length=200)): The unique identifier or code assigned to an individual rail station or a pseudo-station representing all the stations within a specific city, from which rail travel originates.
+        address(Address): --
+        timezone(Optional[constr(max_length=200)], optional): The timezone associated with the location of the station, specifying the local time offset from Coordinated Universal Time (UTC).
+
+    """
+    name: constr(max_length=200) = Field(..., example='Grand Central Terminal')
+    """
+    The popularly known name or title by which the railway station is identified.
+    """
+    type: Optional[Type] = Field(None, example='STATION')
+    """
+    This attribute provides information about the specific classification assigned to the rail station. It helps differentiate between different types of stations, such as major stations (STATION) or stations located within a city (city).
+    """
+    station_code: constr(max_length=200) = Field(..., example='GCT')
+    """
+    The unique identifier or code assigned to an individual rail station or a pseudo-station representing all the stations within a specific city, from which rail travel originates.
+    """
+    address: Address = None
+    timezone: Optional[constr(max_length=200)] = Field(None, example='America/New_York')
+    """
+    The timezone associated with the location of the station, specifying the local time offset from Coordinated Universal Time (UTC).
+    """
+
+
 class FlightType(
     Enum,
 ):
     r"""pydantic model FlightType: Identifies the type of air trip based on the air destinations.
     Attributes:
         ROUNDTRIP(Any): --
         ONEWAY(Any): --
@@ -793,21 +905,23 @@
     r"""pydantic model TravelProductType: Type of product.
     Attributes:
         CRUISE(Any): --
         AIR(Any): --
         CAR(Any): --
         INSURANCE(Any): --
         HOTEL(Any): --
+        RAIL(Any): --
 
     """
     CRUISE: Any = 'CRUISE'
     AIR: Any = 'AIR'
     CAR: Any = 'CAR'
     INSURANCE: Any = 'INSURANCE'
     HOTEL: Any = 'HOTEL'
+    RAIL: Any = 'RAIL'
 
 
 class CardType(
     Enum,
 ):
     r"""pydantic model CardType: The 'card_type' field value is an enum value which is associated with the payment method of the specific payment instrument.
     For credit card payment method ensure attributes mentioned in dictionary below are set to corresponding values only.
@@ -1190,21 +1304,22 @@
 ):
     r"""pydantic model TravelProduct: The `type` field value is used as a discriminator, with the following mapping:
     * `CRUISE`: `Cruise`
     * `AIR`: `Air`
     * `CAR`: `Car`
     * `INSURANCE`: `Insurance`
     * `HOTEL`: `Hotel`
+    * `RAIL`: `Rail`
 
     Attributes:
         price(Amount): --
         type(TravelProductType): --
-        inventory_type(constr(max_length=30)): Type of inventory. Ensure attributes mentioned in dictionary below are set to corresponding values only. `inventory_type` has the following mapping with TravelProduct `type` attribute: *       inventory_type            :      type * ------------------------------------------------------ *  `Cruise`                       : `CRUISE` *  `Air`                          : `AIR` *  `Car`                          : `CAR` *  `Insurance`                    : `INSURANCE` *  `Hotel`                        : `HOTEL`
+        inventory_type(constr(max_length=30)): Type of inventory. Ensure attributes mentioned in dictionary below are set to corresponding values only. `inventory_type` has the following mapping with TravelProduct `type` attribute: *       inventory_type            :      type * ------------------------------------------------------ *  `Cruise`                       : `CRUISE` *  `Air`                          : `AIR` *  `Car`                          : `CAR` *  `Insurance`                    : `INSURANCE` *  `Hotel`                        : `HOTEL` *  `Rail`                         :  `RAIL`
         inventory_source(InventorySource): Identifies the business model through which the supply is being sold. Merchant/Agency. * `MERCHANT` is used when Partner is the merchant of record for this order. * `AGENCY` is used when this order is through an agency booking.
-        travelers_references(List[constr(max_length=50)]): List of travelerGuids who are part of the traveling party on the order for the product. Information for each product and its required travelers should be provided in the API request. If the product booking does not require accompanying quest information then that does not need to be provided in the API request. Example: * For Air products, all travelers' details are required to complete the booking. * For Hotel products, typically the details on the person checking-in is required. * For Car products, typically only the primary driver information is required. If multiple traveler details are in the itinerary, this structure allows to fill up traveler details once in the `travelers` section, and then associate individual products to the respective travelers. This association is made using `traveler_id` field. A GUID can be generated for each object in the `travelers` section. The same GUID can be provided in the `traveler_references` below. The `travelers` array should have at least one `traveler` object, and each `traveler` object should have a `traveler_id` which is not necessarily an account id. Example: *   Travelers * ------------ *  A - GUID1 *  B - GUID2 *  C - GUID3 * *   Products * ------------ * Air *   [GUID1, GUID2, GUID3] * Hotel *   [GUID1] * Car *   [GUID3] * * Above example shows all three travelers will be associated with the Air product, however only Traveler A will be associated with the Hotel product and only Traveler C will be associated with the Car product.
+        travelers_references(List[constr(max_length=50)]): List of travelerGuids who are part of the traveling party on the order for the product. Information for each product and its required travelers should be provided in the API request. If the product booking does not require accompanying quest information then that does not need to be provided in the API request. Example: * For Air products, all travelers' details are required to complete the booking. * For Hotel products, typically the details on the person checking-in is required. * For Car products, typically only the primary driver information is required. If multiple traveler details are in the itinerary, this structure allows to fill up traveler details once in the `travelers` section, and then associate individual products to the respective travelers. This association is made using `traveler_id` field. A GUID can be generated for each object in the `travelers` section. The same GUID can be provided in the `traveler_references` below. The `travelers` array should have at least one `traveler` object, and each `traveler` object should have a `traveler_id` which is not necessarily an account id. Example: *   Travelers * ------------ *  A - GUID1 *  B - GUID2 *  C - GUID3 * *   Products * ------------ * Air *   [GUID1, GUID2, GUID3] * Hotel *   [GUID1] * Car *   [GUID3] * Rail *   [GUID2] * Above example shows all three travelers will be associated with the Air product, * however, only Traveler A will be associated with the Hotel product, * and only Traveler C will be associated with the Car product. * Traveler B will be associated with the Rail product.
 
     """
     price: Amount = None
     type: TravelProductType = None
     inventory_type: constr(max_length=30) = None
     """
     Type of inventory.
@@ -1213,14 +1328,15 @@
     *       inventory_type            :      type
     * ------------------------------------------------------
     *  `Cruise`                       : `CRUISE`
     *  `Air`                          : `AIR`
     *  `Car`                          : `CAR`
     *  `Insurance`                    : `INSURANCE`
     *  `Hotel`                        : `HOTEL`
+    *  `Rail`                         :  `RAIL`
 
     """
     inventory_source: InventorySource = None
     """
     Identifies the business model through which the supply is being sold. Merchant/Agency.
     * `MERCHANT` is used when Partner is the merchant of record for this order.
     * `AGENCY` is used when this order is through an agency booking.
@@ -1249,18 +1365,65 @@
     * ------------
     * Air
     *   [GUID1, GUID2, GUID3]
     * Hotel
     *   [GUID1]
     * Car
     *   [GUID3]
-    *
-    * Above example shows all three travelers will be associated with the Air product, however only Traveler A will be associated with the Hotel product and only Traveler C will be associated with the Car product.
+    * Rail
+    *   [GUID2]
+    * Above example shows all three travelers will be associated with the Air product,
+    * however, only Traveler A will be associated with the Hotel product,
+    * and only Traveler C will be associated with the Car product.
+    * Traveler B will be associated with the Rail product.
+
+    """
+
+
+class RailSegments(
+    BaseModel,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model RailSegments
+    Attributes:
+        departure_time(datetime): The local date and time of the scheduled departure from the departure station, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+        arrival_time(datetime): The local date and time of the scheduled arrival at the destination station, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+        departure_station(RailwayStationDetails): --
+        arrival_station(RailwayStationDetails): --
+        transportation_method(TransportationMethod): This attribute represents the specific transportation method by which the passenger is traveling. It captures the mode of transportation used during the Rail product journey, Possible values are:     - `BUS` - The Rail product includes bus transportation for certain segments of the itinerary.     - `FERRY` - The Rail product involves ferry transportation as part of the journey.     - `PUBLIC_TRANSPORT` - The Rail product represents the use of public transportation modes for the journey.     - `TRAM` - The Rail product includes tram transportation as part of the journey.     - `RAIL` - The Rail product specifically utilizes train transportation for the journey.     - `TRANSFER` - The Rail product involves transfers between different modes of transportation.     - `OTHER` - The Rail product utilizes transportation methods not covered by the aforementioned categories.
+        operating_company(Optional[OperatingCompany], optional): This attribute captures the name or identifier of the company responsible for operating the Rail product. It represents the specific operating entity, such as Amtrak, British Railways, or a bus company.
+
+    """
+    departure_time: datetime = None
+    """
+    The local date and time of the scheduled departure from the departure station, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+    """
+    arrival_time: datetime = None
+    """
+    The local date and time of the scheduled arrival at the destination station, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
+    """
+    departure_station: RailwayStationDetails = None
+    arrival_station: RailwayStationDetails = None
+    transportation_method: TransportationMethod = None
+    """
+    This attribute represents the specific transportation method by which the passenger is traveling. It captures the mode of transportation used during the Rail product journey, Possible values are:
+        - `BUS` - The Rail product includes bus transportation for certain segments of the itinerary.
+        - `FERRY` - The Rail product involves ferry transportation as part of the journey.
+        - `PUBLIC_TRANSPORT` - The Rail product represents the use of public transportation modes for the journey.
+        - `TRAM` - The Rail product includes tram transportation as part of the journey.
+        - `RAIL` - The Rail product specifically utilizes train transportation for the journey.
+        - `TRANSFER` - The Rail product involves transfers between different modes of transportation.
+        - `OTHER` - The Rail product utilizes transportation methods not covered by the aforementioned categories.
 
     """
+    operating_company: Optional[OperatingCompany] = None
+    """
+    This attribute captures the name or identifier of the company responsible for operating the Rail product. It represents the specific operating entity, such as Amtrak, British Railways, or a bus company.
+    """
 
 
 class Air(
     TravelProductGeneric,
     smart_union=True,
     extra=Extra.forbid,
 ):
@@ -1644,14 +1807,38 @@
     """
     traveler_id: Optional[constr(max_length=100)] = None
     """
     A unique identifier for travelers in the transaction.
     """
 
 
+class Rail(
+    TravelProductGeneric,
+    smart_union=True,
+    extra=Extra.forbid,
+):
+    r"""pydantic model Rail
+    Attributes:
+        route_type(RouteType): The type of route or itinerary for the Rail product, indicating the travel arrangement and pattern. Possible values are: - `MULTIPLE_DESTINATIONS` - The Rail product includes multiple destinations in its itinerary. - `ONE_WAY` - The Rail product represents a one-way journey. - `ROUNDTRIP` - The Rail product represents a roundtrip journey.
+        rail_segments(List[RailSegments]): --
+        type(Literal['RAIL']): --
+
+    """
+    route_type: RouteType = None
+    """
+    The type of route or itinerary for the Rail product, indicating the travel arrangement and pattern. Possible values are:
+    - `MULTIPLE_DESTINATIONS` - The Rail product includes multiple destinations in its itinerary.
+    - `ONE_WAY` - The Rail product represents a one-way journey.
+    - `ROUNDTRIP` - The Rail product represents a roundtrip journey.
+
+    """
+    rail_segments: List[RailSegments] = Field(..., maxItems=20, minItems=1)
+    type: Literal['RAIL'] = 'RAIL'
+
+
 class PaymentOperation(
     BaseModel,
     smart_union=True,
     extra=Extra.forbid,
 ):
     r"""pydantic model PaymentOperation
     Attributes:
@@ -1826,17 +2013,17 @@
     Attributes:
         card_type(CardType): The 'card_type' field value is an enum value which is associated with the payment method of the specific payment instrument. For credit card payment method ensure attributes mentioned in dictionary below are set to corresponding values only. Ensure to comply with the naming standards provided in below dictionary. For example, some Payment processors use “Japan Credit Bureau” but “JCB” should be used when calling Fraud API. Incorrect `card_type` - `brand` combination will result in data quality issues and result in degraded risk recommendation. 'card_type' is an enum value with the following mapping with Payment `brand` attribute: *       card_type            :          brand * -------------------------------------------------------- * `AMERICAN_EXPRESS`         : `AMERICAN_EXPRESS` * `DINERS_CLUB`              : `DINERS_CLUB_INTERNATIONAL` * `DINERS_CLUB`              : `BC_CARD` * `DISCOVER`                 : `DISCOVER` * `DISCOVER`                 : `BC_CARD` * `DISCOVER`                 : `DINERS_CLUB_INTERNATIONAL` * `DISCOVER`                 : `JCB` * `JCB`                      : `JCB` * `MASTER_CARD`              : `MASTER_CARD` * `MASTER_CARD`              : `MAESTRO` * `MASTER_CARD`              : `POSTEPAY_MASTERCARD` * `SOLO`                     : `SOLO` * `SWITCH`                   : `SWITCH` * `MAESTRO`                  : `MAESTRO` * `CHINA_UNION_PAY`          : `CHINA_UNION_PAY` * `VISA`                     : `VISA` * `VISA`                     : `VISA_DELTA` * `VISA`                     : `VISA_ELECTRON` * `VISA`                     : `CARTA_SI` * `VISA`                     : `CARTE_BLEUE` * `VISA`                     : `VISA_DANKORT` * `VISA`                     : `POSTEPAY_VISA_ELECTRON`
         card_number(constr(max_length=200)): All the digits (unencrypted) of the credit card number associated with the payment.
         expiry_date(Optional[datetime], optional): Expiration date of the credit card used for payment, in ISO-8061 date and time format `yyyy-MM-ddTHH:mm:ss.SSSZ`.
         electronic_commerce_indicator(Optional[constr(max_length=200)], optional): Electronic Commerce Indicator, a two or three digit number usually returned by a 3rd party payment processor in regards to the authentication used when gathering the cardholder's payment credentials.
         virtual_credit_card_flag(Optional[bool], optional): A flag to indicate that the bank card being used for the charge is a virtual credit card.
         wallet_type(Optional[constr(max_length=200)], optional): If a virtual/digital form of payment was used, the type of digital wallet should be specified here. Possible `wallet_type`'s include: `Google` or `ApplePay`.
-        card_avs_response(constr(max_length=50)): A field used to confirm if the address provided at the time of purchase matches what the bank has on file for the Credit Card.
-        card_cvv_response(constr(max_length=20)): A field used to confirm the Card Verification Value on the Credit Card matches the Credit Card used at the time of purchase.
-        telephones(List[Telephone]): Telephone(s) associated with card holder and credit card.
+        card_avs_response(Optional[constr(max_length=50)], optional): A field used to confirm if the address provided at the time of purchase matches what the bank has on file for the Credit Card.
+        card_cvv_response(Optional[constr(max_length=20)], optional): A field used to confirm the Card Verification Value on the Credit Card matches the Credit Card used at the time of purchase.
+        telephones(Optional[List[Telephone]], optional): Telephone(s) associated with card holder and credit card.
         merchant_order_code(Optional[constr(max_length=200)], optional): Reference code passed to acquiring bank at the time of payment. This code is the key ID that ties back to payments data at the payment level.
         card_authentication_failure_count(Optional[int], optional): Total authentication failure count for given card.
         method(Literal['CREDIT_CARD']): --
 
     """
     card_type: CardType = None
     """
@@ -1887,23 +2074,23 @@
     """
     A flag to indicate that the bank card being used for the charge is a virtual credit card.
     """
     wallet_type: Optional[constr(max_length=200)] = None
     """
     If a virtual/digital form of payment was used, the type of digital wallet should be specified here. Possible `wallet_type`'s include: `Google` or `ApplePay`.
     """
-    card_avs_response: constr(max_length=50) = None
+    card_avs_response: Optional[constr(max_length=50)] = None
     """
     A field used to confirm if the address provided at the time of purchase matches what the bank has on file for the Credit Card.
     """
-    card_cvv_response: constr(max_length=20) = None
+    card_cvv_response: Optional[constr(max_length=20)] = None
     """
     A field used to confirm the Card Verification Value on the Credit Card matches the Credit Card used at the time of purchase.
     """
-    telephones: List[Telephone] = Field(..., maxItems=20, minItems=1)
+    telephones: Optional[List[Telephone]] = Field(None, maxItems=20, minItems=1)
     """
     Telephone(s) associated with card holder and credit card.
     """
     merchant_order_code: Optional[constr(max_length=200)] = None
     """
     Reference code passed to acquiring bank at the time of payment. This code is the key ID that ties back to payments data at the payment level.
     """
@@ -2033,15 +2220,15 @@
     transaction: Optional[OrderPurchaseTransaction] = None
 
 
 RefundUpdate = Union[IssuedRefundUpdate, SettledRefundUpdate, RefundUpdateGeneric]
 
 OrderPurchaseUpdateRequest = Union[OrderUpdate, ChargebackFeedback, InsultFeedback, RefundUpdate, PaymentUpdate, OrderPurchaseUpdateRequestGeneric]
 
-TravelProduct = Union[Air, Cruise, Car, Hotel, Insurance, TravelProductGeneric]
+TravelProduct = Union[Rail, Air, Cruise, Car, Hotel, Insurance, TravelProductGeneric]
 
 Payment = Union[CreditCard, PayPal, Points, PaymentGeneric]
 
 
 Error.update_forward_refs()
 
 
@@ -2095,14 +2282,20 @@
 
 Address.update_forward_refs()
 
 
 TravelersReference.update_forward_refs()
 
 
+OperatingCompany.update_forward_refs()
+
+
+RailwayStationDetails.update_forward_refs()
+
+
 AirSegment.update_forward_refs()
 
 
 HotelAddress.update_forward_refs()
 
 
 PaymentThreeDSCriteria.update_forward_refs()
@@ -2134,14 +2327,17 @@
 
 ChargebackDetail.update_forward_refs()
 
 
 OrderPurchaseScreenResponse.update_forward_refs()
 
 
+RailSegments.update_forward_refs()
+
+
 Air.update_forward_refs()
 
 
 Cruise.update_forward_refs()
 
 
 Car.update_forward_refs()
@@ -2170,14 +2366,17 @@
 
 CustomerAccount.update_forward_refs()
 
 
 Traveler.update_forward_refs()
 
 
+Rail.update_forward_refs()
+
+
 PaymentOperation.update_forward_refs()
 
 
 Verify.update_forward_refs()
 
 
 Authorize.update_forward_refs()
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.1.0/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO` & `openworld-sdk-python-fraudpreventionv2-1.2.0/openworld_sdk_python_fraudpreventionv2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openworld-sdk-python-fraudpreventionv2
-Version: 1.1.0
+Version: 1.2.0
 Summary: Open World fraudPreventionV2 SDK for Python
 Home-page: https://github.com/ExpediaGroup/openworld-sdk-python
 Author: Expedia Group
 Author-email: oss@expediagroup.com
 License: Apache License, Version 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
```

### Comparing `openworld-sdk-python-fraudpreventionv2-1.1.0/setup.py` & `openworld-sdk-python-fraudpreventionv2-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 
 from setuptools import setup
 
 setup(
     name='openworld-sdk-python-fraudpreventionv2',
-    version='1.1.0',
+    version='1.2.0',
     packages=['openworld.sdk.fraudpreventionv2'],
     package_dir={'openworld-sdk-python-fraudpreventionv2': '.'},
     license='Apache License, Version 2.0',
     author='Expedia Group',
     author_email='oss@expediagroup.com',
     url='https://github.com/ExpediaGroup/openworld-sdk-python',
     classifiers=[
```

