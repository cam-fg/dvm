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
|[ReqRecommendation](https://github.com/cam-fg/lab-tour-sh-doc/tree/main/models/ReqRecommendation)|A request for a recommendation for a given location. Note: This is just the request, not the recommendation itself. The recommendation is provided by the recommendation service.|
|[TouristRecommendation](https://github.com/cam-fg/lab-tour-sh-doc/tree/main/models/TouristRecommendation)|A recommendation that has been generated for a given location. The recommendation, which is based on a point of interest, includes a list of recommended points of interest and a list of recommended parking lots.|