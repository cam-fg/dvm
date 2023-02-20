<!-- Header Area begin --->
<p align="center">
  <img align="center" padding="50px" src="../../resources/addix.svg" width="20%" />
  <img align="center" src="../../resources/lhind.png" width="20%" />
  <img align="center" src="../../resources/fh-kiel.png" width="20%" />
  <img align="center" src="../../resources/fh-westkueste.svg" width="20%" />
</p>
<!-- Header Area end --->

# OccupancySeries

A series of occupancy values for a given time period. Could be used to describe the flow or absolute occupancy of a certain entity (e.g. a parking lot, beach).

|Property|Expected Type|Description|Cardinality|
|---|---|---|---|
|id|[Text](https://schema.org/Text)|**From Vocabulary**: The identifier property represents any kind of identifier for any kind of [Thing](https://schema.org/Thing), such as ISBNs, GTIN codes, UUIDs etc. Schema.org provides dedicated properties for representing many of these, either as textual strings or as URL (URI) links. See [background notes](http://schema.org/docs/datamodel.html#identifierBg) for more details.|1|
|dateCreated|[DateTime](https://schema.org/DateTime)|The date on which the Entity was created. This will usually be allocated by the storage platform.|0..1|
|dateModified|[DateTime](https://schema.org/DateTime)|The date on which the Entity was most recently modified. This will usually be allocated by the storage platform.|0..1|
|source|[URL](https://schema.org/URL)|URL of the source of this entity.|0..1|
|name|[Text](https://schema.org/Text)|The name of the entity.|0..1|
|alternateName|[Text](https://schema.org/Text)|If available, an alternative name for the entity.|0..1|
|description|[Text](https://schema.org/Text)|A description of the entity.|0..1|
|dataProvider|[Text](https://schema.org/Text)|Name of the company, person or organisation providing this entity.|0..1|
|owner|[Text](https://schema.org/Text)|Identifier of the owner of this entity.|0..N|
|seeAlso|[Text](https://schema.org/Text)|List of additional resources about the entity.|0..N|
|location|[GeoCoordinates](https://schema.org/GeoCoordinates)|The geo coordinates of this entity.|1|
|address|[PostalAddress](https://schema.org/PostalAddress)|Physical address of the entity.|0..1|
|areaServed|[Text](https://schema.org/Text)|The geographic area where a service or offered item is provided.|0..1|
|index|[DateTime](https://schema.org/DateTime)|All date times that are linked to the values of the series.|0..N|
|refBasis|[Text](https://schema.org/Text)|Identifier this occupancy is referring to.|0..1|
|relativeValue|[Number](https://schema.org/Number)|Relative values of the occupancy series, each value in relation to the maximum capacity of the entity.|0..N|
|type|[Text](https://schema.org/Text)|NGSI Entity type. It has to be OccupancySeries|1|
|validFrom|[DateTime](https://schema.org/DateTime)|Date and time from which the entity is valid.|0..N|
|validTo|[DateTime](https://schema.org/DateTime)|Date and time until the entity is valid.|0..N|
|value|[Integer](https://schema.org/Integer)|The numeric values of the occupancy series.|0..N|