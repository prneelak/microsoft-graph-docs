---
title: "deviceComplianceUserStatus resource type"
description: ""
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# deviceComplianceUserStatus resource type


Namespace: microsoft.graph




Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceComplianceUserStatus](../api/devicecomplianceuserstatus-get.md)|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md)|Read properties and relationships of the [deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md) object.|
|[Update deviceComplianceUserStatus](../api/devicecomplianceuserstatus-update.md)|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md)|Update the properties of a [deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md) object.|
|[List userStatuses](../api/devicecompliancepolicy-list-userstatuses.md)|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md) collection|Get the deviceComplianceUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/devicecompliancepolicy-post-userstatuses.md)|[deviceComplianceUserStatus](../resources/devicecomplianceuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|devicesCount|Int32|Devices count for that user.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastReportedDateTime|DateTimeOffset|Last modified date time of the policy report.|
|status|Enumeration|Compliance status of the policy report. Possible values are: `unknown`, `notApplicable`, `compliant`, `remediated`, `nonCompliant`, `error`, `conflict`, `notAssigned`.|
|userDisplayName|String|User name of the DevicePolicyStatus.|
|userPrincipalName|String|UserPrincipalName.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceUserStatus",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceUserStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "devicesCount": 1024,
  "status": "String",
  "lastReportedDateTime": "String (timestamp)",
  "userPrincipalName": "String"
}
```

