<!-- Header Area begin --->
<p align="center">
  <img align="center" padding="50px" src="../../resources/addix.svg" width="20%" />
  <img align="center" src="../../resources/lhind.png" width="20%" />
  <img align="center" src="../../resources/fh-kiel.png" width="20%" />
  <img align="center" src="../../resources/fh-westkueste.svg" width="20%" />
</p>
<!-- Header Area end --->

# Occupancy

An atomic occupancy value. Can be used to describe the occupancy of a single point in time. This occupancy could be taken from a sensor or predicted by a model.

|Property|Expected Type|Description|Cardinality|
|---|---|---|---|
|id|[Text](https://schema.org/Text)|**From Vocabulary**: The identifier property represents any kind of identifier for any kind of [Thing](https://schema.org/Thing), such as ISBNs, GTIN codes, UUIDs etc. Schema.org provides dedicated properties for representing many of these, either as textual strings or as URL (URI) links. See [background notes](http://schema.org/docs/datamodel.html#identifierBg) for more details.|1|
|[dateCreated](https://schema.org/dateCreated)|[DateTime](https://schema.org/DateTime)|The date on which the Entity was created. This will usually be allocated by the storage platform.|0..1|
|[dateModified](https://schema.org/dateModified)|[DateTime](https://schema.org/DateTime)|The date on which the Entity was most recently modified. This will usually be allocated by the storage platform.|0..1|
|source|[URL](https://schema.org/URL)|URL of the source of this entity.|0..1|
|[name](https://schema.org/name)|[Text](https://schema.org/Text)|The name of the entity.|0..1|
|[alternateName](https://schema.org/alternateName)|[Text](https://schema.org/Text)|If available, an alternative name for the entity.|0..1|
|[description](https://schema.org/description)|[Text](https://schema.org/Text)|A description of the entity.|0..1|
|dataProvider|[Text](https://schema.org/Text)|Name of the company, person or organisation providing this entity.|0..1|
|owner|[Text](https://schema.org/Text)|Identifier of the owner of this entity.|0..N|
|seeAlso|[Text](https://schema.org/Text)|List of additional resources about the entity.|0..N|
|[location](https://schema.org/location)|[GeoCoordinates](https://schema.org/GeoCoordinates)|The geo coordinates of this entity.|1|
|[address](https://schema.org/address)|[PostalAddress](https://schema.org/PostalAddress)|Physical address of the entity.|0..1|
|[areaServed](https://schema.org/areaServed)|[Text](https://schema.org/Text)|The geographic area where a service or offered item is provided.|0..1|
|period|[Text](https://schema.org/Text)|Period to which this occupancy is assigned. Encoded as a ISO8601 duration.|0..1|
|refBasis|[Text](https://schema.org/Text)|Identifier this occupancy is referring to.|0..1|
|relativeValue|[Number](https://schema.org/Number)|Relative value of the occupancy, in relation to the maximum capacity of the entity.|0..1|
|type|[Text](https://schema.org/Text)|NGSI Entity type. It has to be Occupancy|1|
|validFrom|[DateTime](https://schema.org/DateTime)|Date and time from which the entity is valid.|0..1|
|validTo|[DateTime](https://schema.org/DateTime)|Date and time until the entity is valid.|0..1|
|[value](https://schema.org/value)|[Integer](https://schema.org/Integer)|The numeric value of the occupancy.|0..1|