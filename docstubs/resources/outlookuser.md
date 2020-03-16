---
title: "outlookUser resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# outlookUser resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get outlookUser](../api/outlookuser-get.md)|[outlookUser](../resources/outlookuser.md)|Read properties and relationships of the [outlookUser](../resources/outlookuser.md) object.|
|[Update outlookUser](../api/outlookuser-update.md)|[outlookUser](../resources/outlookuser.md)|Update the properties of a [outlookUser](../resources/outlookuser.md) object.|
|[supportedLanguages](../api/outlookuser-supportedlanguages.md)|[localeInfo](../resources/localeinfo.md) collection||
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md)|[timeZoneInformation](../resources/timezoneinformation.md) collection||
|[supportedTimeZones](../api/outlookuser-supportedtimezones.md)|[timeZoneInformation](../resources/timezoneinformation.md) collection||
|[List masterCategories](../api/outlookuser-list-mastercategories.md)|[outlookCategory](../resources/outlookcategory.md) collection|Get the outlookCategories from the masterCategories navigation property.|
|[Add masterCategories](../api/outlookuser-post-mastercategories.md)|[outlookCategory](../resources/outlookcategory.md)|Add masterCategories by posting to the masterCategories collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|masterCategories|[outlookCategory](../resources/outlookcategory.md) collection||

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.outlookUser",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.outlookUser",
  "id": "String (identifier)"
}
```

