---
title: "Add deviceManagementTroubleshootingEvents"
description: "Add deviceManagementTroubleshootingEvents by posting to the deviceManagementTroubleshootingEvents collection."
author: ""
localization_priority: Normal
ms.prod: ""
doc_type: apiPageType
---

# Add deviceManagementTroubleshootingEvents

Namespace: microsoft.graph

Add deviceManagementTroubleshootingEvents by posting to the deviceManagementTroubleshootingEvents collection.

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
POST /me/deviceManagementTroubleshootingEvents/$ref
POST /users/{usersId}/deviceManagementTroubleshootingEvents/$ref
```

## Request headers
|Header|Value|
|:---|:---|
|Authorization|Bearer {token}.Required|
|Content-Type|application/json.Required|

## Request body
In the request body, supply a JSON representation for the [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) object.

The following table shows the properties that are required when you create the [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md).

|Property|Type|Description|
|:---|:---|:---|
|id|String| Inherited from [entity](../resources/entity.md)|
|eventDateTime|DateTimeOffset|Time when the event occurred .|
|correlationId|String|Id used for tracing the failure in the service.|



## Response
If successful, this method returns a `201 Created` response code and a [deviceManagementTroubleshootingEvent](../resources/devicemanagementtroubleshootingevent.md) object in the response body.

## Examples

### Request
Here is an example of the request.
<!-- {
  "blockType": "request",
  "name": "create_devicemanagementtroubleshootingevent_from_"
}
-->
``` http
POST https://graph.microsoft.com/localtest/me/deviceManagementTroubleshootingEvents
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "eventDateTime": "2017-01-01T00:01:31.6259689+03:00",
  "correlationId": "Correlation Id value"
}
```

### Response
Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.devicemanagementtroubleshootingevent"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.deviceManagementTroubleshootingEvent",
  "id": "3a171e3c-1e3c-3a17-3c1e-173a3c1e173a",
  "eventDateTime": "2017-01-01T00:01:31.6259689+03:00",
  "correlationId": "Correlation Id value"
}
```

