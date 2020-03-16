---
title: "locationConstraintItem resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# locationConstraintItem resource type


Namespace: microsoft.graph




Inherits from [location](../resources/location.md)

## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[physicalAddress](../resources/physicaladdress.md)| Inherited from [location](../resources/location.md)|
|coordinates|[outlookGeoCoordinates](../resources/outlookgeocoordinates.md)| Inherited from [location](../resources/location.md)|
|displayName|String| Inherited from [location](../resources/location.md)|
|locationEmailAddress|String| Inherited from [location](../resources/location.md)|
|locationType|Enumeration| Inherited from [location](../resources/location.md). Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`, `geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.|
|locationUri|String| Inherited from [location](../resources/location.md)|
|resolveAvailability|Boolean||
|uniqueId|String| Inherited from [location](../resources/location.md)|
|uniqueIdType|Enumeration| Inherited from [location](../resources/location.md). Possible values are: `unknown`, `locationStore`, `directory`, `private`, `bing`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.locationConstraintItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.locationConstraintItem",
  "displayName": "String",
  "locationEmailAddress": "String",
  "address": {
    "@odata.type": "microsoft.graph.physicalAddress",
    "street": "String",
    "city": "String",
    "state": "String",
    "countryOrRegion": "String",
    "postalCode": "String"
  },
  "locationUri": "String",
  "coordinates": {
    "@odata.type": "microsoft.graph.outlookGeoCoordinates",
    "latitude": "Double",
    "longitude": "Double",
    "accuracy": "Double",
    "altitude": "Double",
    "altitudeAccuracy": "Double"
  },
  "locationType": "String",
  "uniqueId": "String",
  "uniqueIdType": "String",
  "resolveAvailability": true
}
```

