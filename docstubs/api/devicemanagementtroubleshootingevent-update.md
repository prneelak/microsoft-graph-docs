---
title: "Update deviceManagementTroubleshootingEvent"
description: "Update the properties of a deviceManagementTroubleshootingEvent object."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Update deviceManagementTroubleshootingEvent

Namespace: microsoft.graph

Update the properties of a [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) object.

## Permissions
One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).

|Permission type|Permissions (from most to least privileged)|
|:---|:---|
|Delegated (work or school account)|**TODO: Determine scopes **|
|Delegated (personal Microsoft account)|Not supported.|
|Application|**TODO: Determine AppOnly scopes **|

## HTTP request
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) object.

The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|eventDateTime|DateTimeOffset|Time when the event occurred .|
|correlationId|String|Id used for tracing the failure in the service.|



## Response
If successful, this method returns a `200 OK` response code and an updated [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "update_devicemanagementtroubleshootingevent"
}
-->
``` http
PATCH https://graph.microsoft.com/localtest/deviceManagement/troubleshootingEvents/{deviceManagementTroubleshootingEventId}
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2017-01-01T00:00:04.8508562+03:00",
  "correlationId": "Correlation Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "abbb3345-3345-abbb-4533-bbab4533bbab",
  "eventDateTime": "2017-01-01T00:00:04.8508562+03:00",
  "correlationId": "Correlation Id value"
}
```

