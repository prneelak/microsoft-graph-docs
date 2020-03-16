---
title: "managedDeviceMobileAppConfiguration resource type"
description: "An abstract class for Mobile app configuration for enrolled devices."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# managedDeviceMobileAppConfiguration resource type


Namespace: microsoft.graph

An abstract class for Mobile app configuration for enrolled devices.


Inherits from [entity](../resources/entity.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[Get managedDeviceMobileAppConfiguration](../api/manageddevicemobileappconfiguration-get.md)|[managedDeviceMobileAppConfiguration](../resources/manageddevicemobileappconfiguration.md)|Read properties and relationships of the [managedDeviceMobileAppConfiguration](../resources/manageddevicemobileappconfiguration.md) object.|
|[assign](../api/manageddevicemobileappconfiguration-assign.md)|None||
|[List assignments](../api/manageddevicemobileappconfiguration-list-assignments.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/manageddevicemobileappconfigurationassignment.md) collection|Get the managedDeviceMobileAppConfigurationAssignments from the assignments navigation property.|
|[Add assignments](../api/manageddevicemobileappconfiguration-post-assignments.md)|[managedDeviceMobileAppConfigurationAssignment](../resources/manageddevicemobileappconfigurationassignment.md)|Add assignments by posting to the assignments collection.|
|[List deviceStatuses](../api/manageddevicemobileappconfiguration-list-devicestatuses.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md) collection|Get the managedDeviceMobileAppConfigurationDeviceStatuses from the deviceStatuses navigation property.|
|[Add deviceStatuses](../api/manageddevicemobileappconfiguration-post-devicestatuses.md)|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md)|Add deviceStatuses by posting to the deviceStatuses collection.|
|[List userStatuses](../api/manageddevicemobileappconfiguration-list-userstatuses.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/manageddevicemobileappconfigurationuserstatus.md) collection|Get the managedDeviceMobileAppConfigurationUserStatuses from the userStatuses navigation property.|
|[Add userStatuses](../api/manageddevicemobileappconfiguration-post-userstatuses.md)|[managedDeviceMobileAppConfigurationUserStatus](../resources/manageddevicemobileappconfigurationuserstatus.md)|Add userStatuses by posting to the userStatuses collection.|
|[Get managedDeviceMobileAppConfigurationDeviceSummary](../api/manageddevicemobileappconfigurationdevicesummary-get.md)|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/manageddevicemobileappconfigurationdevicesummary.md)|Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceSummary](../resources/manageddevicemobileappconfigurationdevicesummary.md) object.|
|[Get managedDeviceMobileAppConfigurationUserSummary](../api/manageddevicemobileappconfigurationusersummary-get.md)|[managedDeviceMobileAppConfigurationUserSummary](../resources/manageddevicemobileappconfigurationusersummary.md)|Read properties and relationships of the [managedDeviceMobileAppConfigurationUserSummary](../resources/manageddevicemobileappconfigurationusersummary.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|createdDateTime|DateTimeOffset|DateTime the object was created.|
|description|String|Admin provided description of the Device Configuration.|
|displayName|String|Admin provided name of the device configuration.|
|id|String| Inherited from [entity](../resources/entity.md)|
|lastModifiedDateTime|DateTimeOffset|DateTime the object was last modified.|
|targetedMobileApps|String collection|the associated app.|
|version|Int32|Version of the device configuration.|

## Relationships
|Relationship|Type|Description|
|:---|:---|:---|
|assignments|[managedDeviceMobileAppConfigurationAssignment](../resources/manageddevicemobileappconfigurationassignment.md) collection|The list of group assignemenets for app configration.|
|deviceStatuses|[managedDeviceMobileAppConfigurationDeviceStatus](../resources/manageddevicemobileappconfigurationdevicestatus.md) collection|List of ManagedDeviceMobileAppConfigurationDeviceStatus.|
|deviceStatusSummary|[managedDeviceMobileAppConfigurationDeviceSummary](../resources/manageddevicemobileappconfigurationdevicesummary.md)|App configuration device status summary.|
|userStatuses|[managedDeviceMobileAppConfigurationUserStatus](../resources/manageddevicemobileappconfigurationuserstatus.md) collection|List of ManagedDeviceMobileAppConfigurationUserStatus.|
|userStatusSummary|[managedDeviceMobileAppConfigurationUserSummary](../resources/manageddevicemobileappconfigurationusersummary.md)|App configuration user status summary.|

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedDeviceMobileAppConfiguration",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfiguration",
  "id": "String (identifier)",
  "targetedMobileApps": [
    "String"
  ],
  "createdDateTime": "String (timestamp)",
  "description": "String",
  "lastModifiedDateTime": "String (timestamp)",
  "displayName": "String",
  "version": 1024
}
```

