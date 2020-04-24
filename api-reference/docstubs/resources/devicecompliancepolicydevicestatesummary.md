---
title: "deviceCompliancePolicyDeviceStateSummary resource type"
description: "**TODO: Add Description**"
author: "**TODO: Provide Github Name. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
localization_priority: Normal
ms.prod: "**TODO: Add MS prod. See [topic-level metadata reference](https://msgo.azurewebsites.net/add/document/guidelines/metadata.html#topic-level-metadata)**"
doc_type: resourcePageType
---

# deviceCompliancePolicyDeviceStateSummary resource type


Namespace: microsoft.graph

**TODO: Add Description**


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get deviceCompliancePolicyDeviceStateSummary](../api/devicecompliancepolicydevicestatesummary-get.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/devicecompliancepolicydevicestatesummary.md)|Read the properties and relationships of a [deviceCompliancePolicyDeviceStateSummary](../resources/devicecompliancepolicydevicestatesummary.md) object.|
|[Update deviceCompliancePolicyDeviceStateSummary](../api/devicecompliancepolicydevicestatesummary-update.md)|[deviceCompliancePolicyDeviceStateSummary](../resources/devicecompliancepolicydevicestatesummary.md)|Update the properties of a [deviceCompliancePolicyDeviceStateSummary](../resources/devicecompliancepolicydevicestatesummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|compliantDeviceCount|Int32|Number of compliant devices|
|configManagerCount|Int32|Number of devices that have compliance managed by System Center Configuration Manager|
|conflictDeviceCount|Int32|Number of conflict devices|
|errorDeviceCount|Int32|Number of error devices|
|id|String|**TODO: Add Description** Inherited from [entity](../resources/entity.md)|
|inGracePeriodCount|Int32|Number of devices that are in grace period|
|nonCompliantDeviceCount|Int32|Number of NonCompliant devices|
|notApplicableDeviceCount|Int32|Number of not applicable devices|
|remediatedDeviceCount|Int32|Number of remediated devices|
|unknownDeviceCount|Int32|Number of unknown devices|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCompliancePolicyDeviceStateSummary",
  "id": "String (identifier)",
  "inGracePeriodCount": 1024,
  "configManagerCount": 1024,
  "unknownDeviceCount": 1024,
  "notApplicableDeviceCount": 1024,
  "compliantDeviceCount": 1024,
  "remediatedDeviceCount": 1024,
  "nonCompliantDeviceCount": 1024,
  "errorDeviceCount": 1024,
  "conflictDeviceCount": 1024
}
```

