<!-- Header Area begin --->
<p align="center">
  <img align="center" padding="50px" src="../../resources/addix.svg" width="20%" />
  <img align="center" src="../../resources/lhind.png" width="20%" />
  <img align="center" src="../../resources/fh-kiel.png" width="20%" />
  <img align="center" src="../../resources/fh-westkueste.svg" width="20%" />
</p>
<!-- Header Area end --->

# TriggerRecommendation

Data model for triggering the creation of a recommendation. This is a request to the recommendation engine to create a recommendation for a given context.

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
|maxDistance|[Number](https://schema.org/Number)|Maximum distance of the entities to be considered.|0..1|
|refBasis|[Text](https://schema.org/Text)|If known, identifier the recommendation will be based on.|0..1|
|type|[Text](https://schema.org/Text)|NGSI Entity type. It has to be TouristRecommendation|1|