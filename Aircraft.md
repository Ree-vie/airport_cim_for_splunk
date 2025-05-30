### Aircraft CIM

The fields within this section of the CIM are all related to the specific aircraft of the flight leg. Use this in conjunction with the [Departures](./Departures.md) and [Arrivals](./Arrivals.md) sections of the CIM

| Dataset Name  | Field Name  | Data Type | Description | Examples |
|:--------------|:------------|:----------|:------------|:---------|
| Airfield      | lastUpdated | int(10)   | The time the record was last updated. This should be used as your _time field when indexing your AODB events | 0516469200 |
| Airfield      | flightUID   | String    |A unique identifier for the flight leg | 6300189 |
|Airfield|flightNumber|int(4)|The numerical flight number of the aircraft|1234|
|Airfield|serviceType|String(1)|The operational status of the flight. Refer to [serviceTypes](https://github.com/ktugwell/Splunk4Airports/blob/main/lookups/serviceTypes.csv) lookup. | J (Scheduled), C (Charter) |
|Airfield|airline|String|The IATA code for the operating airline|EZY, DY, AA|
|Airfield|airlineName|String|The name of the operating airline|EasyJet|
|Airfield|FQFC|String|Fully Qualified Flight Code|EZY1234|
|Airfield|departureOrArrival|String(1)|Is the aircraft departing or arriving|D, A|
|Airfield|aircraftParkingPosition|String|Gate or hard stand where the aircraft is located|A10|
|Airfield|passengerGate|String|The public gate which the passengers will use to board or disembark.|A10|
|Airfield|remoteOperationalGate|String|An additional location used to transfer passengers to or from a remote parking position.|A10|
|Airfield|runway|String|The runway in use for this aircraft movement|26L|
|Airfield|terminal|String|Terminal where the passengers will be processed.|North, 1, 2, 3|
|Airfield|paxBusInd|Boolean|If true, an airside bus will be used for the passengers.|True, false|
|Airfield|registration|String|The aircraft registration number as assigned by the aircraft manufacturer|G-XWBD|
|Airfield|agentInfo|String|Identification of the handling agent for the flight leg|MA, ALS|
|Airfield|paxCount|String|The actual count of passengers on the aircraft|100|
|Airfield|delay|int(10)|Flight Delay Time||
|Airfield|distance_km|int|Route distance calculated using base lat/lon and other airport lan/lon|425|
|Airfield|paxCapacity|int|Aircraft passenger capacity|72|
|Airfield|bagCount|int|10|
|Airfield|belt|String|Luggage Belt|3|
|Airfield|beltStart|int|Belt start datetime|epoch|
|Airfield|beltStop|int|Belt start datetime|epoch|
|Airfield|beltTerminal|int|Belt start datetime|epoch|
|Airlield|



[Contents](./contents.md)<br />
[Home](./)
