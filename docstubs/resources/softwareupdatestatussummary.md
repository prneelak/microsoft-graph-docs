---
title: "softwareUpdateStatusSummary resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# softwareUpdateStatusSummary resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get softwareUpdateStatusSummary](../api/softwareupdatestatussummary-get.md)|[softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md)|Read properties and relationships of the [softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md) object.|
|[Update softwareUpdateStatusSummary](../api/softwareupdatestatussummary-update.md)|[softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md)|Update the properties of a [softwareUpdateStatusSummary](../resources/softwareupdatestatussummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantDeviceCount|Int32|Number of compliant devices.|
|compliantUserCount|Int32|Number of compliant users.|
|conflictDeviceCount|Int32|Number of conflict devices.|
|conflictUserCount|Int32|Number of conflict users.|
|displayName|String|The name of the policy.|
|errorDeviceCount|Int32|Number of devices had error.|
|errorUserCount|Int32|Number of users had error.|
|id|String| Inherited from [entity](../resources/entity.md)|
|nonCompliantDeviceCount|Int32|Number of non compliant devices.|
|nonCompliantUserCount|Int32|Number of non compliant users.|
|notApplicableDeviceCount|Int32|Number of not applicable devices.|
|notApplicableUserCount|Int32|Number of not applicable users.|
|remediatedDeviceCount|Int32|Number of remediated devices.|
|remediatedUserCount|Int32|Number of remediated users.|
|unknownDeviceCount|Int32|Number of unknown devices.|
|unknownUserCount|Int32|Number of unknown users.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.softwareUpdateStatusSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.softwareUpdateStatusSummary",
  "id": "String (identifier)",
  "displayName": "String",
  "compliantDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "unknownDeviceCount": 1024,
  "conflictDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "errorUserCount": 1024,
  "unknownUserCount": 1024,
  "conflictUserCount": 1024,
  "notApplicableUserCount": 1024
}
```

