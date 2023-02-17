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
|id|<a href="https://schema.org/Text" target="_blank">Text</a>|**From Vocabulary**: The identifier property represents any kind of identifier for any kind of <a href="https://schema.org/Thing" target="_blank">Thing</a>, such as ISBNs, GTIN codes, UUIDs etc. Schema.org provides dedicated properties for representing many of these, either as textual strings or as URL (URI) links. See <a href="http://schema.org/docs/datamodel.html#identifierBg" target="_blank">background notes</a> for more details.|1|
|dateCreated|<a href="https://schema.org/DateTime" target="_blank">DateTime</a>|The date on which the Entity was created. This will usually be allocated by the storage platform.|0..1|
|dateModified|<a href="https://schema.org/DateTime" target="_blank">DateTime</a>|The date on which the Entity was most recently modified. This will usually be allocated by the storage platform.|0..1|
|source|<a href="https://schema.org/URL" target="_blank">URL</a>|URL of the source of this entity.|0..1|
|name|<a href="https://schema.org/Text" target="_blank">Text</a>|The name of the entity.|0..1|
|alternateName|<a href="https://schema.org/Text" target="_blank">Text</a>|If available, an alternative name for the entity.|0..1|
|description|<a href="https://schema.org/Text" target="_blank">Text</a>|A description of the entity.|0..1|
|dataProvider|<a href="https://schema.org/Text" target="_blank">Text</a>|Name of the company, person or organisation providing this entity.|0..1|
|owner|<a href="https://schema.org/Text" target="_blank">Text</a>|Identifier of the owner of this entity.|0..N|
|seeAlso|<a href="https://schema.org/Text" target="_blank">Text</a>|List of additional resources about the entity.|0..N|
|location|<a href="https://schema.org/GeoCoordinates" target="_blank">GeoCoordinates</a>|The geo coordinates of this entity.|1|
|address|<a href="https://schema.org/address" target="_blank">PostalAddress</a>|Physical address of the entity.|0..1|
|areaServed|<a href="https://schema.org/Text" target="_blank">Text</a>|The geographic area where a service or offered item is provided.|0..1|
|index|<a href="https://schema.org/DateTime" target="_blank">DateTime</a>|All date times that are linked to the values of the series.|0..N|
|refBasis|<a href="https://schema.org/Text" target="_blank">Text</a>|Identifier this occupancy is referring to.|0..1|
|relativeValue|<a href="https://schema.org/Number" target="_blank">Number</a>|Relative values of the occupancy series, each value in relation to the maximum capacity of the entity.|0..N|
|type|<a href="https://schema.org/Text" target="_blank">Text</a>|NGSI Entity type. It has to be OccupancySeries|1|
|validFrom|<a href="https://schema.org/DateTime" target="_blank">DateTime</a>|Date and time from which the entity is valid.|0..N|
|validTo|<a href="https://schema.org/DateTime" target="_blank">DateTime</a>|Date and time until the entity is valid.|0..N|
|value|<a href="https://schema.org/Integer" target="_blank">Integer</a>|The numeric values of the occupancy series.|0..N|