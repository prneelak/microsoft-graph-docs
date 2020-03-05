---
title: "enrollmentTroubleshootingEvent resource type"
description: "Event representing an enrollment failure."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: resourcePageType
---

# enrollmentTroubleshootingEvent resource type


Namespace: microsoft.graph

Event representing an enrollment failure.


Inherits from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)

## Methods
|Method|Return Type|Description|
|:---|:---|:---|
|[List enrollmentTroubleshootingEvents](../api/enrollmenttroubleshootingevent-list.md)|[enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md) collection|List properties and relationships of the [enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md) objects.|
|[Get enrollmentTroubleshootingEvent](../api/enrollmenttroubleshootingevent-get.md)|[enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md)|Read properties and relationships of the [enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md) object.|
|[Create enrollmentTroubleshootingEvent](../api/enrollmenttroubleshootingevent-create.md)|[enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md)|Create a new [enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md) object.|
|[Delete enrollmentTroubleshootingEvent](../api/enrollmenttroubleshootingevent-delete.md)|None|Deletes a [enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md).|
|[Update enrollmentTroubleshootingEvent](../api/enrollmenttroubleshootingevent-update.md)|[enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md)|Update the properties of a [enrollmentTroubleshootingEvent](../resources/enrollmenttroubleshootingevent.md) object.|

## Properties
|Property|Type|Description|
|:---|:---|:---|
|correlationId|String|Id used for tracing the failure in the service. Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|deviceId|String|Azure AD device identifier.|
|enrollmentType|Enumeration|Type of the enrollment. Possible values are: `unknown`, `userEnrollment`, `deviceEnrollmentManager`, `appleBulkWithUser`, `appleBulkWithoutUser`, `windowsAzureADJoin`, `windowsBulkUserless`, `windowsAutoEnrollment`, `windowsBulkAzureDomainJoin`, `windowsCoManagement`.|
|eventDateTime|DateTimeOffset|Time when the event occurred . Inherited from [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md)|
|failureCategory|Enumeration|Highlevel failure category. Possible values are: `unknown`, `authentication`, `authorization`, `accountValidation`, `userValidation`, `deviceNotSupported`, `inMaintenance`, `badRequest`, `featureNotSupported`, `enrollmentRestrictionsEnforced`, `clientDisconnected`, `userAbandonment`.|
|failureReason|String|Detailed failure reason.|
|id|String| Inherited from [entity](../resources/entity.md)|
|managedDeviceIdentifier|String|Device identifier created or collected by Intune.|
|operatingSystem|String|Operating System.|
|osVersion|String|OS Version.|
|userId|String|Identifier for the user that tried to enroll the device.|

## Relationships
None

## JSON representation
Here is a JSON representation of the resource.
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.enrollmentTroubleshootingEvent",
  "baseType": "microsoft.graph.deviceManagementTroubleshootingEvent",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.enrollmentTroubleshootingEvent",
  "id": "String (identifier)",
  "eventDateTime": "String (timestamp)",
  "correlationId": "String",
  "managedDeviceIdentifier": "String",
  "operatingSystem": "String",
  "osVersion": "String",
  "userId": "String",
  "deviceId": "String",
  "enrollmentType": "String",
  "failureCategory": "String",
  "failureReason": "String"
}
```

