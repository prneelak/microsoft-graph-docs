---
title: "location resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# location resource type


Namespace: microsoft.graph



## Properties
|Property|Type|Description|
|:---|:---|:---|
|address|[physicalAddress](../resources/physicaladdress.md)||
|coordinates|[outlookGeoCoordinates](../resources/outlookgeocoordinates.md)||
|displayName|String||
|locationEmailAddress|String||
|locationType|Enumeration|. Possible values are: `default`, `conferenceRoom`, `homeAddress`, `businessAddress`, `geoCoordinates`, `streetAddress`, `hotel`, `restaurant`, `localBusiness`, `postalAddress`.|
|locationUri|String||
|uniqueId|String||
|uniqueIdType|Enumeration|. Possible values are: `unknown`, `locationStore`, `directory`, `private`, `bing`.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.location"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.location",
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
  "uniqueIdType": "String"
}
```

