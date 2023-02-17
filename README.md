<!-- Header Area begin --->
<p align="center">
  <img align="center" padding="50px" src="resources/addix.svg" width="20%" />
  <img align="center" src="resources/lhind.png" width="20%" />
  <img align="center" src="resources/fh-kiel.png" width="20%" />
  <img align="center" src="resources/fh-westkueste.svg" width="20%" />
</p>
<!-- Header Area end --->

# Landesweites Digitales Besuchermanagement Tourismus in Schleswig-Holstein (LAB-TOUR SH)
(*engl.: State-wide Digital Visitor Management Tourism in Schleswig-Holstein*)

## Data Models

Within the LAB-TOUR-SH project, different data models were developed, which are listed in the following table. The data models are adapted to the needs identified in this project and meet the compatibility requirements of the different systems used in the LAB-TOUR-SH project. This mainly concerns the FIWARE platform, which is the basis for contextual information.

|Data Model|Description|
|---|---|
|[Occupancy](https://github.com/cam-fg/lab-tour-sh-doc/tree/main/models/Occupancy)|An atomic occupancy value. Can be used to describe the occupancy of a single point in time. This occupancy could be taken from a sensor or predicted by a model.|
|[OccupancySeries](https://github.com/cam-fg/lab-tour-sh-doc/tree/main/models/OccupancySeries)|A series of occupancy values for a given time period. Could be used to describe the flow or absolute occupancy of a certain entity (e.g. a parking lot, beach).|
|[TriggerRecommendation](https://github.com/cam-fg/lab-tour-sh-doc/tree/main/models/TriggerRecommendation)|Data model for triggering the creation of a recommendation. This is a request to the recommendation engine to create a recommendation for a given context.|
|[TouristRecommendation](https://github.com/cam-fg/lab-tour-sh-doc/tree/main/models/TouristRecommendation)|A recommendation that has been generated for a given location. The recommendation, which is based on a point of interest, includes a list of recommended points of interest and a list of recommended parking lots.|

## Smart Data Models

The models are based on the FIWARE Smart Data Models ([SmartDataModels.org](https://smartdatamodels.org/)) and hence there are some naming conventions that are used in the models. The following table shows the naming conventions used in the models.

|Name|Description|
|---|---|
|id|The unique identifier of the entity. (In Schema.org: [identifier](https://schema.org/identifier))|
|type|The type of the NGSI entity.|
|ref*|The reference to another entity.|
|seeAlso|URI to additional resources.|