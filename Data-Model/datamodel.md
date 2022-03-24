# Client

Identifies a clinet
-  `id`: Client Identifier
   -  Attribute type: **Property**. 
   -  Required
-  `clientTypeInstitution`: Type of client -> True identifies an institutional client. False identifies a singular client
   -  Attribute type: **Property**. 
   -  Required
-  `legalName`: Institution legal name
   -  Attribute type: **Property**. [legalName](https://schema.org/legalName)
   -  Optional
-  `givenName`: Client first name
   -  Attribute type: **Property**. [Person](https://schema.org/Person)
   -  Optional
-  `familyName`: Client last name
   -  Attribute type: **Property**. [Person](https://schema.org/Person)
   -  Optional
-  `taxId`: Client/Institution Tax ID
   -  Attribute type: **Property**. [Person](https://schema.org/Person)
   -  Required
-  `address`: The client's address
   -  Attribute type: **Property**. [address](https://schema.org/address)
   -  Required
-  `email`: Contact email address
   -  Attribute type: **Property**. [email](https://schema.org/email)
   -  Required
-  `telephone`: Mobile or telephone contact
   -  Attribute type: **Property**. [telephone](https://schema.org/telephone)
   -  Required



# MeasurementStation

Describes a given measurement station
-  `id`: Measurement station identifier
   -  Attribute type: **Property**. 
   -  Required
-  `name`: Measurement station name
   -  Attribute type: **Property**. [name](https://schema.org/name)
   -  Required
-  `location`: Geojson reference to the item. It can be Point, LineString, Polygon, MultiPoint, MultiLineString or MultiPolygon
   -  Attribute type: **GeoProperty**. 
   -  Required
-  `belongsTo`: Identification of the owner of the station.
   -  Attribute type: **Relationship**. [URL](https://schema.org/URL)
   -  Optional



# Sensor

Sensor's description and physical variables
-  `id`: Sensor identifier
   -  Attribute type: **Property**. 
   -  Required
-  `measurementVariable`: Defines the variable that the sensor can measure * `PM2.5` - PM2 measurement * `PM10` - PM10 measurement * `CO2` - CO2 measurement * `NO2` - NO2 measurement * `O3` - O3 measurement * `Sound` - Sound measurement. One of : `PM2.5`, `PM10`, `CO2`, `O3`, `NO2`, `Sound`.
   -  Attribute type: **Property**. 
   -  Required
-  `measurementValue`: Measured variable quantity consumed by a given asset, within a process
   -  Attribute type: **Property**. 
   -  Required
-  `belongsTo`: Identification of the Measurement station the sensor is attached in.
   -  Attribute type: **Relationship**. [URL](https://schema.org/URL)
   -  Required



## Examples

### OK


